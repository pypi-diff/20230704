# Comparing `tmp/uniswap-universal-router-decoder-0.8.0.tar.gz` & `tmp/uniswap-universal-router-decoder-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniswap-universal-router-decoder-0.8.0.tar", last modified: Sat Mar 18 13:00:07 2023, max compression
+gzip compressed data, was "uniswap-universal-router-decoder-0.9.0.tar", last modified: Tue Jul  4 17:21:02 2023, max compression
```

## Comparing `uniswap-universal-router-decoder-0.8.0.tar` & `uniswap-universal-router-decoder-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-03-18 13:00:07.203271 uniswap-universal-router-decoder-0.8.0/
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1064 2023-02-10 14:36:58.000000 uniswap-universal-router-decoder-0.8.0/LICENSE
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    16148 2023-03-18 13:00:07.203271 uniswap-universal-router-decoder-0.8.0/PKG-INFO
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    15062 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.8.0/README.md
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1255 2023-03-18 12:58:33.000000 uniswap-universal-router-decoder-0.8.0/pyproject.toml
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)       38 2023-03-18 13:00:07.203271 uniswap-universal-router-decoder-0.8.0/setup.cfg
-drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-03-18 13:00:07.203271 uniswap-universal-router-decoder-0.8.0/tests/
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1311 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.8.0/tests/test_abi_builder.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     4750 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.8.0/tests/test_decoder.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    16662 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.8.0/tests/test_encoder.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)      347 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.8.0/tests/test_router_codec.py
-drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-03-18 13:00:07.203271 uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder/
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)      189 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder/__init__.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     5517 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder/_abi_builder.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     7003 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder/_constants.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     4273 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder/_decoder.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    17595 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder/_encoder.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1013 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder/_enums.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     4309 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder/router_codec.py
-drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-03-18 13:00:07.203271 uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder.egg-info/
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    16148 2023-03-18 13:00:07.000000 uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder.egg-info/PKG-INFO
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)      731 2023-03-18 13:00:07.000000 uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder.egg-info/SOURCES.txt
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)        1 2023-03-18 13:00:07.000000 uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder.egg-info/dependency_links.txt
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)       15 2023-03-18 13:00:07.000000 uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder.egg-info/requires.txt
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)       33 2023-03-18 13:00:07.000000 uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder.egg-info/top_level.txt
+drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-07-04 17:21:02.951264 uniswap-universal-router-decoder-0.9.0/
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1064 2023-02-10 14:36:58.000000 uniswap-universal-router-decoder-0.9.0/LICENSE
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    15747 2023-07-04 17:21:02.951264 uniswap-universal-router-decoder-0.9.0/PKG-INFO
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    14647 2023-07-04 17:12:01.000000 uniswap-universal-router-decoder-0.9.0/README.md
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1279 2023-07-04 17:12:21.000000 uniswap-universal-router-decoder-0.9.0/pyproject.toml
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)       38 2023-07-04 17:21:02.951264 uniswap-universal-router-decoder-0.9.0/setup.cfg
+drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-07-04 17:21:02.951264 uniswap-universal-router-decoder-0.9.0/tests/
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1311 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/tests/test_abi_builder.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     4750 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/tests/test_decoder.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    20784 2023-07-04 17:12:01.000000 uniswap-universal-router-decoder-0.9.0/tests/test_encoder.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)      347 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/tests/test_router_codec.py
+drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-07-04 17:21:02.951264 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)      189 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/__init__.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     5517 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_abi_builder.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     7003 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_constants.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     4273 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_decoder.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    22088 2023-07-04 17:12:01.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_encoder.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1073 2023-07-04 17:12:01.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_enums.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     4309 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/router_codec.py
+drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-07-04 17:21:02.951264 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    15747 2023-07-04 17:21:02.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/PKG-INFO
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)      731 2023-07-04 17:21:02.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/SOURCES.txt
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)        1 2023-07-04 17:21:02.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/dependency_links.txt
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)       19 2023-07-04 17:21:02.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/requires.txt
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)       33 2023-07-04 17:21:02.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/top_level.txt
```

### Comparing `uniswap-universal-router-decoder-0.8.0/LICENSE` & `uniswap-universal-router-decoder-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uniswap-universal-router-decoder-0.8.0/PKG-INFO` & `uniswap-universal-router-decoder-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,8 @@
-Metadata-Version: 2.1
-Name: uniswap-universal-router-decoder
-Version: 0.8.0
-Summary: Decode & Encode transaction data sent to Uniswap universal router
-Author-email: Elnaril <elnaril_dev@caramail.com>
-License: MIT License
-Project-URL: Homepage, https://github.com/Elnaril/uniswap-universal-router-decoder
-Project-URL: Bug Tracker, https://github.com/Elnaril/uniswap-universal-router-decoder/issues
-Project-URL: Fiverr, https://www.fiverr.com/elnaril
-Keywords: blockchain,ethereum,uniswap,universal router,decoder,encoder
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Uniswap Universal Router Decoder & Encoder v0.8.0
-⚠ This version introduces breaking changes compared to v0.7 !
+# Uniswap Universal Router Decoder & Encoder v0.9.0
 
 ---
 
 #### Project Information
 [![Tests & Lint](https://github.com/Elnaril/uniswap-universal-router-decoder/actions/workflows/tests.yml/badge.svg)](https://github.com/Elnaril/uniswap-universal-router-decoder/actions/workflows/tests.yml)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/uniswap-universal-router-decoder)](https://pypi.org/project/uniswap-universal-router-decoder/)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/Elnaril/uniswap-universal-router-decoder)](https://github.com/Elnaril/uniswap-universal-router-decoder/releases)
@@ -40,54 +15,44 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Type Checker: mypy](https://img.shields.io/badge/%20type%20checker-mypy-%231674b1?style=flat&labelColor=ef8336)](https://mypy-lang.org/)
 [![Linter: flake8](https://img.shields.io/badge/%20linter-flake8-%231674b1?style=flat&labelColor=ef8336)](https://flake8.pycqa.org/en/latest/)
 
 ---
 
 ## Release Notes
+### V0.9.0
+ - Add support for UNWRAP_WETH encoding
+ - Add v2_swap_exact_in_from_balance() and v3_swap_exact_in_from_balance(): 2 convenient methods which are used when the exact in_amount is not known when the transaction is built, typically chained after a V*_SWAP_EXACT_IN.
 ### V0.8.0
  - Breaking changes because of refactoring
  - Command chaining extension: all supported UR functions can now be chained in a single transaction
-### V0.7.1
- -  Fix issue [#1](https://github.com/Elnaril/uniswap-universal-router-decoder/issues/1) - v3 path decoding fails for some paths 
-### V0.7.0
- - Add support for encoding V2_SWAP_EXACT_OUT
- - Add support for encoding V3_SWAP_EXACT_OUT
- - Fix V3_SWAP_EXACT_OUT ABI
- - Fix typos in README
-### V0.6.0
- - Breaking changes: use Web3.py v6 i/o v5
- - Add support for the PERMIT2_PERMIT function
- - Add support for chaining PERMIT2_PERMIT and V2_SWAP_EXACT_IN in the same transaction
 
 ---
 
 ## Overview and Points of Attention
 
 The object of this library is to decode & encode the transaction input sent to the Uniswap universal router (UR)
-(address [`0xEf1c6E67703c7BD7107eed8303Fbe6EC2554BF6B`](https://etherscan.io/address/0xEf1c6E67703c7BD7107eed8303Fbe6EC2554BF6B) 
+(address [`0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD`](https://etherscan.io/address/0xEf1c6E67703c7BD7107eed8303Fbe6EC2554BF6B) 
 on Ethereum Mainnet). It is based on, and is intended to be used with [web3.py](https://github.com/ethereum/web3.py)
 
 ⚠ This library has not been audited, so use at your own risk !
 
-⚠ At this stage, there is no guarantee of compatibility between 2 versions: consider forcing the version in your dependency requirements.
-
 ⚠ This project is a work in progress so not all commands are decoded yet. Below the list of the already implemented ones.
 
 | Command Id | Function Name | Decode | Encode
 | ---------- | ------------- |:------:|:------:
 | 0x00 | V3_SWAP_EXACT_IN | ✅ | ✅
 | 0x01 | V3_SWAP_EXACT_OUT | ✅ | ✅
 | 0x02 - 0x06 |  | ❌ | ❌
 | 0x07 | placeholder  | N/A | N/A
 | 0x08 | V2_SWAP_EXACT_IN | ✅ | ✅
 | 0x09 | V2_SWAP_EXACT_OUT | ✅ | ✅
 | 0x0a | PERMIT2_PERMIT | ✅ | ✅
 | 0x0b | WRAP_ETH | ✅ | ✅
-| 0x0c | UNWRAP_WETH | ✅ | ❌
+| 0x0c | UNWRAP_WETH | ✅ | ✅
 | 0x0d | PERMIT2_TRANSFER_FROM_BATCH | ❌ | ❌
 | 0x0e - 0x0f | placeholders | N/A | N/A
 | 0x10 - 0x1d |  | ❌ | ❌
 | 0x1e - 0x3f | placeholders | N/A | N/A
 
 ---
 
@@ -221,15 +186,14 @@
 
 # then in your transaction dict:
 transaction["data"] = encoded_data
 
 # you can now sign and send the transaction to the UR
 ```
 
-
 ### How to encode a call to the function V2_SWAP_EXACT_IN
 This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before using sending such transaction.
 ```python
 from uniswap_universal_router_decoder import FunctionRecipient, RouterCodec
 
 codec = RouterCodec()
 encoded_data = codec.encode.chain().v2_swap_exact_in(
```

### Comparing `uniswap-universal-router-decoder-0.8.0/README.md` & `uniswap-universal-router-decoder-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,32 @@
-# Uniswap Universal Router Decoder & Encoder v0.8.0
-⚠ This version introduces breaking changes compared to v0.7 !
+Metadata-Version: 2.1
+Name: uniswap-universal-router-decoder
+Version: 0.9.0
+Summary: Decode & Encode transaction data sent to Uniswap Universal Router
+Author-email: Elnaril <elnaril_dev@caramail.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/Elnaril/uniswap-universal-router-decoder
+Project-URL: Bug Tracker, https://github.com/Elnaril/uniswap-universal-router-decoder/issues
+Project-URL: Fiverr, https://www.fiverr.com/elnaril
+Keywords: blockchain,ethereum,uniswap,universal router,decoder,encoder,codec,wrapper
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Uniswap Universal Router Decoder & Encoder v0.9.0
 
 ---
 
 #### Project Information
 [![Tests & Lint](https://github.com/Elnaril/uniswap-universal-router-decoder/actions/workflows/tests.yml/badge.svg)](https://github.com/Elnaril/uniswap-universal-router-decoder/actions/workflows/tests.yml)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/uniswap-universal-router-decoder)](https://pypi.org/project/uniswap-universal-router-decoder/)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/Elnaril/uniswap-universal-router-decoder)](https://github.com/Elnaril/uniswap-universal-router-decoder/releases)
@@ -16,54 +39,44 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Type Checker: mypy](https://img.shields.io/badge/%20type%20checker-mypy-%231674b1?style=flat&labelColor=ef8336)](https://mypy-lang.org/)
 [![Linter: flake8](https://img.shields.io/badge/%20linter-flake8-%231674b1?style=flat&labelColor=ef8336)](https://flake8.pycqa.org/en/latest/)
 
 ---
 
 ## Release Notes
+### V0.9.0
+ - Add support for UNWRAP_WETH encoding
+ - Add v2_swap_exact_in_from_balance() and v3_swap_exact_in_from_balance(): 2 convenient methods which are used when the exact in_amount is not known when the transaction is built, typically chained after a V*_SWAP_EXACT_IN.
 ### V0.8.0
  - Breaking changes because of refactoring
  - Command chaining extension: all supported UR functions can now be chained in a single transaction
-### V0.7.1
- -  Fix issue [#1](https://github.com/Elnaril/uniswap-universal-router-decoder/issues/1) - v3 path decoding fails for some paths 
-### V0.7.0
- - Add support for encoding V2_SWAP_EXACT_OUT
- - Add support for encoding V3_SWAP_EXACT_OUT
- - Fix V3_SWAP_EXACT_OUT ABI
- - Fix typos in README
-### V0.6.0
- - Breaking changes: use Web3.py v6 i/o v5
- - Add support for the PERMIT2_PERMIT function
- - Add support for chaining PERMIT2_PERMIT and V2_SWAP_EXACT_IN in the same transaction
 
 ---
 
 ## Overview and Points of Attention
 
 The object of this library is to decode & encode the transaction input sent to the Uniswap universal router (UR)
-(address [`0xEf1c6E67703c7BD7107eed8303Fbe6EC2554BF6B`](https://etherscan.io/address/0xEf1c6E67703c7BD7107eed8303Fbe6EC2554BF6B) 
+(address [`0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD`](https://etherscan.io/address/0xEf1c6E67703c7BD7107eed8303Fbe6EC2554BF6B) 
 on Ethereum Mainnet). It is based on, and is intended to be used with [web3.py](https://github.com/ethereum/web3.py)
 
 ⚠ This library has not been audited, so use at your own risk !
 
-⚠ At this stage, there is no guarantee of compatibility between 2 versions: consider forcing the version in your dependency requirements.
-
 ⚠ This project is a work in progress so not all commands are decoded yet. Below the list of the already implemented ones.
 
 | Command Id | Function Name | Decode | Encode
 | ---------- | ------------- |:------:|:------:
 | 0x00 | V3_SWAP_EXACT_IN | ✅ | ✅
 | 0x01 | V3_SWAP_EXACT_OUT | ✅ | ✅
 | 0x02 - 0x06 |  | ❌ | ❌
 | 0x07 | placeholder  | N/A | N/A
 | 0x08 | V2_SWAP_EXACT_IN | ✅ | ✅
 | 0x09 | V2_SWAP_EXACT_OUT | ✅ | ✅
 | 0x0a | PERMIT2_PERMIT | ✅ | ✅
 | 0x0b | WRAP_ETH | ✅ | ✅
-| 0x0c | UNWRAP_WETH | ✅ | ❌
+| 0x0c | UNWRAP_WETH | ✅ | ✅
 | 0x0d | PERMIT2_TRANSFER_FROM_BATCH | ❌ | ❌
 | 0x0e - 0x0f | placeholders | N/A | N/A
 | 0x10 - 0x1d |  | ❌ | ❌
 | 0x1e - 0x3f | placeholders | N/A | N/A
 
 ---
 
@@ -197,15 +210,14 @@
 
 # then in your transaction dict:
 transaction["data"] = encoded_data
 
 # you can now sign and send the transaction to the UR
 ```
 
-
 ### How to encode a call to the function V2_SWAP_EXACT_IN
 This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before using sending such transaction.
 ```python
 from uniswap_universal_router_decoder import FunctionRecipient, RouterCodec
 
 codec = RouterCodec()
 encoded_data = codec.encode.chain().v2_swap_exact_in(
```

### Comparing `uniswap-universal-router-decoder-0.8.0/pyproject.toml` & `uniswap-universal-router-decoder-0.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uniswap-universal-router-decoder"
-version = "0.8.0"
+version = "0.9.0"
 authors = [
   { name="Elnaril", email="elnaril_dev@caramail.com" },
 ]
-description = "Decode & Encode transaction data sent to Uniswap universal router"
+description = "Decode & Encode transaction data sent to Uniswap Universal Router"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
@@ -21,17 +21,17 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
 license = {text = "MIT License"}
 dependencies = [
-  "web3>=6.0.0b11",
+  "web3>=6.0.0,<7.0.0",
 ]
-keywords = ["blockchain", "ethereum", "uniswap", "universal router", "decoder", "encoder"]
+keywords = ["blockchain", "ethereum", "uniswap", "universal router", "decoder", "encoder", "codec", "wrapper"]
 
 [tool.setuptools]
 packages = ["uniswap_universal_router_decoder"]
 
 [project.urls]
 "Homepage" = "https://github.com/Elnaril/uniswap-universal-router-decoder"
 "Bug Tracker" = "https://github.com/Elnaril/uniswap-universal-router-decoder/issues"
```

### Comparing `uniswap-universal-router-decoder-0.8.0/tests/test_abi_builder.py` & `uniswap-universal-router-decoder-0.9.0/tests/test_abi_builder.py`

 * *Files identical despite different names*

### Comparing `uniswap-universal-router-decoder-0.8.0/tests/test_decoder.py` & `uniswap-universal-router-decoder-0.9.0/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `uniswap-universal-router-decoder-0.8.0/tests/test_encoder.py` & `uniswap-universal-router-decoder-0.9.0/tests/test_encoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,76 +16,94 @@
 
 
 @pytest.mark.parametrize(
     "function_recipient, custom_recipient, expected_recipient, expected_exception",
     (
         (FunctionRecipient.SENDER, None, Web3.to_checksum_address("0x0000000000000000000000000000000000000001"), None),
         (FunctionRecipient.ROUTER, None, Web3.to_checksum_address("0x0000000000000000000000000000000000000002"), None),
-        (FunctionRecipient.CUSTOM, Web3.to_checksum_address("0xB4FBF271143F4FBf7B91A5ded31805e42b2208d6"), Web3.to_checksum_address("0xB4FBF271143F4FBf7B91A5ded31805e42b2208d6"), None),  # noqa
+        (FunctionRecipient.CUSTOM, Web3.to_checksum_address("0xB4FBF271143F4FBf7B91A5ded31805e42b2208d6"), Web3.to_checksum_address("0xB4FBF271143F4FBf7B91A5ded31805e42b2208d6"), None),  # noqa E501
         (FunctionRecipient.CUSTOM, None, None, ValueError),
         (FunctionRecipient.CUSTOM, "moo", None, ValueError),
     )
 )
 def test_get_recipient(function_recipient, custom_recipient, expected_recipient, expected_exception):
     if expected_exception:
         with pytest.raises(expected_exception):
             _ChainedFunctionBuilder._get_recipient(function_recipient, custom_recipient)
     else:
         assert expected_recipient == _ChainedFunctionBuilder._get_recipient(function_recipient, custom_recipient)
 
 
 def test_chain_wrap_eth(codec):
     encoded_input = codec.encode.chain().wrap_eth(FunctionRecipient.SENDER, Wei(10**17), None).build(1676825611)
-    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063f2540b00000000000000000000000000000000000000000000000000000000000000010b000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000000400000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000016345785d8a0000")  # noqa
+    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063f2540b00000000000000000000000000000000000000000000000000000000000000010b000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000000400000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000016345785d8a0000")  # noqa E501
+
+
+def test_chain_unwrap_weth(codec):
+    encoded_input = codec.encode.chain().unwrap_weth(FunctionRecipient.SENDER, Wei(10**17), None).build(1676825611)
+    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063f2540b00000000000000000000000000000000000000000000000000000000000000010c000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000000400000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000016345785d8a0000")  # noqa E501
 
 
 def test_chain_v2_swap_exact_in(codec):
     encoded_input = codec.encode.chain().v2_swap_exact_in(
         FunctionRecipient.SENDER,
         Wei(10**17),
         Wei(0),
         [
             Web3.to_checksum_address("0xB4FBF271143F4FBf7B91A5ded31805e42b2208d6"),
             Web3.to_checksum_address("0x326C977E6efc84E512bB9C30f76E30c160eD06FB"),
         ],
         payer_is_sender=True,
     ).build(1676919287)
-    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063f3c1f7000000000000000000000000000000000000000000000000000000000000000108000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000016345785d8a0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000002000000000000000000000000b4fbf271143f4fbf7b91a5ded31805e42b2208d6000000000000000000000000326c977e6efc84e512bb9c30f76e30c160ed06fb")  # noqa
+    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063f3c1f7000000000000000000000000000000000000000000000000000000000000000108000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000016345785d8a0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000002000000000000000000000000b4fbf271143f4fbf7b91a5ded31805e42b2208d6000000000000000000000000326c977e6efc84e512bb9c30f76e30c160ed06fb")  # noqa E501
+
+
+def test_chain_v2_swap_exact_in_from_balance(codec):
+    encoded_input = codec.encode.chain().v2_swap_exact_in_from_balance(
+        FunctionRecipient.SENDER,
+        Wei(0),
+        [
+            Web3.to_checksum_address("0xB4FBF271143F4FBf7B91A5ded31805e42b2208d6"),
+            Web3.to_checksum_address("0x326C977E6efc84E512bB9C30f76E30c160eD06FB"),
+        ],
+        payer_is_sender=True,
+    ).build(1676919287)
+    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063f3c1f70000000000000000000000000000000000000000000000000000000000000001080000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000000018000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000002000000000000000000000000b4fbf271143f4fbf7b91a5ded31805e42b2208d6000000000000000000000000326c977e6efc84e512bb9c30f76e30c160ed06fb")  # noqa E501
 
 
 def test_chain_v2_swap_exact_out(codec):
     # https://etherscan.io/tx/0xd3abc2fe01376ebaff699a944ae3fb94b00ab899e8ed845a5e22ae120e83cb9e
     encoded_input = codec.encode.chain().v2_swap_exact_out(
         FunctionRecipient.SENDER,
         Wei(5000000000000000000000000),
         Wei(1364343969533288399),
         [
             Web3.to_checksum_address("0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2"),
             Web3.to_checksum_address("0xC74B43cC61b627667a608c3F650c2558F88028a1"),
         ],
         payer_is_sender=True,
     ).build(1678369883)
-    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a0000000000000000000000000000000000000000000000000000000006409e45b0000000000000000000000000000000000000000000000000000000000000001090000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000422ca8b0a00a42500000000000000000000000000000000000000000000000000000012ef1f9c977a5fcf00000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000002000000000000000000000000c02aaa39b223fe8d0a0e5c4f27ead9083c756cc2000000000000000000000000c74b43cc61b627667a608c3f650c2558f88028a1")  # noqa
+    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a0000000000000000000000000000000000000000000000000000000006409e45b0000000000000000000000000000000000000000000000000000000000000001090000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000422ca8b0a00a42500000000000000000000000000000000000000000000000000000012ef1f9c977a5fcf00000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000002000000000000000000000000c02aaa39b223fe8d0a0e5c4f27ead9083c756cc2000000000000000000000000c74b43cc61b627667a608c3f650c2558f88028a1")  # noqa E501
 
 
 path_seq_1 = (
     Web3.to_checksum_address("0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2"),
     3000,
     Web3.to_checksum_address("0xf3dcbc6D72a4E1892f7917b7C43b74131Df8480e"),
 )
-expected_v3_path_1 = Web3.to_bytes(hexstr=HexStr("0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2000bb8f3dcbc6D72a4E1892f7917b7C43b74131Df8480e"))  # noqa
+expected_v3_path_1 = Web3.to_bytes(hexstr=HexStr("0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2000bb8f3dcbc6D72a4E1892f7917b7C43b74131Df8480e"))  # noqa E501
 
 path_seq_2 = (
     Web3.to_checksum_address("0xdAC17F958D2ee523a2206206994597C13D831ec7"),
     500,
     Web3.to_checksum_address("0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2"),
     3000,
     Web3.to_checksum_address("0xABe580E7ee158dA464b51ee1a83Ac0289622e6be"),
 )
-expected_v3_path_2 = Web3.to_bytes(hexstr=HexStr("0xABe580E7ee158dA464b51ee1a83Ac0289622e6be000bb8C02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc20001F4dAC17F958D2ee523a2206206994597C13D831ec7"))  # noqa
+expected_v3_path_2 = Web3.to_bytes(hexstr=HexStr("0xABe580E7ee158dA464b51ee1a83Ac0289622e6be000bb8C02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc20001F4dAC17F958D2ee523a2206206994597C13D831ec7"))  # noqa E501
 
 
 @pytest.mark.parametrize(
     "fn_name, path_seq, expected_v3_path, expected_exception",
     (
         ("V3_SWAP_EXACT_IN", path_seq_1, expected_v3_path_1, None),
         ("V2_SWAP_EXACT_OUT", path_seq_1, expected_v3_path_1, ValueError),
@@ -112,15 +130,31 @@
             500,
             Web3.to_checksum_address("0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2"),
             500,
             Web3.to_checksum_address("0x2260FAC5E5542a773Aa44fBCfeDf7C193bc2C599"),
         ],
         payer_is_sender=True,
     ).build(1677080627)
-    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063f638330000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000012000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000003562e057c400000000000000000000000000000000000000000000000000000000383747ae00000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000042a0b86991c6218b36c1d19d4a2e9eb0ce3606eb480001f4c02aaa39b223fe8d0a0e5c4f27ead9083c756cc20001f42260fac5e5542a773aa44fbcfedf7c193bc2c599000000000000000000000000000000000000000000000000000000000000")  # noqa
+    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063f638330000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000012000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000003562e057c400000000000000000000000000000000000000000000000000000000383747ae00000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000042a0b86991c6218b36c1d19d4a2e9eb0ce3606eb480001f4c02aaa39b223fe8d0a0e5c4f27ead9083c756cc20001f42260fac5e5542a773aa44fbcfedf7c193bc2c599000000000000000000000000000000000000000000000000000000000000")  # noqa E501
+
+
+def test_chain_v3_swap_exact_in_from_balance(codec):
+    encoded_input = codec.encode.chain().v3_swap_exact_in_from_balance(
+        FunctionRecipient.SENDER,
+        Wei(943146926),
+        [
+            Web3.to_checksum_address("0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48"),
+            500,
+            Web3.to_checksum_address("0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2"),
+            500,
+            Web3.to_checksum_address("0x2260FAC5E5542a773Aa44fBCfeDf7C193bc2C599"),
+        ],
+        payer_is_sender=True,
+    ).build(1677080627)
+    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063f63833000000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000001200000000000000000000000000000000000000000000000000000000000000001800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000383747ae00000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000042a0b86991c6218b36c1d19d4a2e9eb0ce3606eb480001f4c02aaa39b223fe8d0a0e5c4f27ead9083c756cc20001f42260fac5e5542a773aa44fbcfedf7c193bc2c599000000000000000000000000000000000000000000000000000000000000")  # noqa E501
 
 
 def test_chain_v3_swap_exact_out(codec):
     # https://etherscan.io/tx/0x6aa16d2af66a8d960ce459abdd0a9018e35b2338cd3d2eb52b1280cc5a5f93ff
     encoded_input = codec.encode.chain().v3_swap_exact_out(
         FunctionRecipient.SENDER,
         Wei(40_000 * 10**18),
@@ -128,15 +162,15 @@
         [
             Web3.to_checksum_address("0x0a5E677a6A24b2F1A2Bf4F3bFfC443231d2fDEc8"),
             3000,
             Web3.to_checksum_address("0x431ad2ff6a9C365805eBaD47Ee021148d6f7DBe0"),
         ],
         payer_is_sender=True,
     ).build(1678369559)
-    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a0000000000000000000000000000000000000000000000000000000006409e317000000000000000000000000000000000000000000000000000000000000000101000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000878678326eac900000000000000000000000000000000000000000000000000007c29f86b56545f0ac800000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000002b431ad2ff6a9c365805ebad47ee021148d6f7dbe0000bb80a5e677a6a24b2f1a2bf4f3bffc443231d2fdec8000000000000000000000000000000000000000000")  # noqa
+    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a0000000000000000000000000000000000000000000000000000000006409e317000000000000000000000000000000000000000000000000000000000000000101000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000878678326eac900000000000000000000000000000000000000000000000000007c29f86b56545f0ac800000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000002b431ad2ff6a9c365805ebad47ee021148d6f7dbe0000bb80a5e677a6a24b2f1a2bf4f3bffc443231d2fdec8000000000000000000000000000000000000000000")  # noqa E501
 
 
 expected_permit_parameters = {
     "details": {
         "token": Web3.to_checksum_address("0x4Fabb145d64652a948d72533023f6E7A623C7C53"),
         "amount": Wei(1461501637330902918203684832716283019655932542975),
         "expiration": 1679922321,
@@ -152,23 +186,23 @@
         *expected_permit_parameters["details"].values(),
         expected_permit_parameters["spender"],
         expected_permit_parameters["sigDeadline"],
     ]
     permit_parameters, signable_message = codec.create_permit2_signable_message(*params)
     assert permit_parameters == expected_permit_parameters
     assert signable_message.version == b'\x01'
-    assert signable_message.header == b'\x86jZ\xba!\x96j\xf9]lz\xb7\x8e\xb2\xb2\xfc\x919\x15\xc2\x8b\xe3\xb9\xaa\x07\xcc\x04\xff\x90>?('  # noqa
-    assert signable_message.body == b'\x92U\x83n\x15\x87\x9ay\xcb\xcez\xc2B\xb6Z\xd2\xe4>\xd2n\x8b\xa8\xedl\xa9\x16\x8f\xcco\x88\xb3\xe0'  # noqa
+    assert signable_message.header == b'\x86jZ\xba!\x96j\xf9]lz\xb7\x8e\xb2\xb2\xfc\x919\x15\xc2\x8b\xe3\xb9\xaa\x07\xcc\x04\xff\x90>?('  # noqa E501
+    assert signable_message.body == b'\x92U\x83n\x15\x87\x9ay\xcb\xcez\xc2B\xb6Z\xd2\xe4>\xd2n\x8b\xa8\xedl\xa9\x16\x8f\xcco\x88\xb3\xe0'  # noqa E501
 
     account: LocalAccount = Account.from_key(keccak(text="moo"))
     signed_message: SignedMessage = account.sign_message(signable_message)
-    assert signed_message.signature == HexBytes('0xc18b2a09e7d03f38102824a401a765fe05a40753a2188520250e7ffb825f41960dd8703c82a9683c0a7a8eafb2b930aa29b3edc018cad7afc6e29781420a8ec51b')  # noqa
+    assert signed_message.signature == HexBytes('0xc18b2a09e7d03f38102824a401a765fe05a40753a2188520250e7ffb825f41960dd8703c82a9683c0a7a8eafb2b930aa29b3edc018cad7afc6e29781420a8ec51b')  # noqa E501
 
     encoded_input = codec.encode.chain().permit2_permit(permit_parameters, signed_message).build(1677332121)
-    assert encoded_input == HexStr('0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063fa0e9900000000000000000000000000000000000000000000000000000000000000010a000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000001600000000000000000000000004fabb145d64652a948d72533023f6e7a623c7c53000000000000000000000000ffffffffffffffffffffffffffffffffffffffff00000000000000000000000000000000000000000000000000000000642194910000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ef1c6e67703c7bd7107eed8303fbe6ec2554bf6b0000000000000000000000000000000000000000000000000000000063fa0e9900000000000000000000000000000000000000000000000000000000000000e00000000000000000000000000000000000000000000000000000000000000041c18b2a09e7d03f38102824a401a765fe05a40753a2188520250e7ffb825f41960dd8703c82a9683c0a7a8eafb2b930aa29b3edc018cad7afc6e29781420a8ec51b00000000000000000000000000000000000000000000000000000000000000')  # noqa
+    assert encoded_input == HexStr('0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063fa0e9900000000000000000000000000000000000000000000000000000000000000010a000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000001600000000000000000000000004fabb145d64652a948d72533023f6e7a623c7c53000000000000000000000000ffffffffffffffffffffffffffffffffffffffff00000000000000000000000000000000000000000000000000000000642194910000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ef1c6e67703c7bd7107eed8303fbe6ec2554bf6b0000000000000000000000000000000000000000000000000000000063fa0e9900000000000000000000000000000000000000000000000000000000000000e00000000000000000000000000000000000000000000000000000000000000041c18b2a09e7d03f38102824a401a765fe05a40753a2188520250e7ffb825f41960dd8703c82a9683c0a7a8eafb2b930aa29b3edc018cad7afc6e29781420a8ec51b00000000000000000000000000000000000000000000000000000000000000')  # noqa E501
 
 
 @pytest.mark.parametrize(
     "router_functions, expected_command",
     (
         ((), ""),
         ((_RouterFunction.PERMIT2_PERMIT, ), "0a"),
@@ -201,8 +235,8 @@
         .encode
         .chain()
         .permit2_permit(permit_parameters, signed_message)
         .v2_swap_exact_in(FunctionRecipient.SENDER, Wei(10**18), Wei(0), path, payer_is_sender=True)
         .build(1677332121)
     )
 
-    assert encoded_input == HexStr('0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063fa0e9900000000000000000000000000000000000000000000000000000000000000020a080000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000004000000000000000000000000000000000000000000000000000000000000001c000000000000000000000000000000000000000000000000000000000000001600000000000000000000000004fabb145d64652a948d72533023f6e7a623c7c53000000000000000000000000ffffffffffffffffffffffffffffffffffffffff00000000000000000000000000000000000000000000000000000000642194910000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ef1c6e67703c7bd7107eed8303fbe6ec2554bf6b0000000000000000000000000000000000000000000000000000000063fa0e9900000000000000000000000000000000000000000000000000000000000000e00000000000000000000000000000000000000000000000000000000000000041c18b2a09e7d03f38102824a401a765fe05a40753a2188520250e7ffb825f41960dd8703c82a9683c0a7a8eafb2b930aa29b3edc018cad7afc6e29781420a8ec51b00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000de0b6b3a7640000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a0000000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000000000020000000000000000000000004fabb145d64652a948d72533023f6e7a623c7c53000000000000000000000000c02aaa39b223fe8d0a0e5c4f27ead9083c756cc2')  # noqa
+    assert encoded_input == HexStr('0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063fa0e9900000000000000000000000000000000000000000000000000000000000000020a080000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000004000000000000000000000000000000000000000000000000000000000000001c000000000000000000000000000000000000000000000000000000000000001600000000000000000000000004fabb145d64652a948d72533023f6e7a623c7c53000000000000000000000000ffffffffffffffffffffffffffffffffffffffff00000000000000000000000000000000000000000000000000000000642194910000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ef1c6e67703c7bd7107eed8303fbe6ec2554bf6b0000000000000000000000000000000000000000000000000000000063fa0e9900000000000000000000000000000000000000000000000000000000000000e00000000000000000000000000000000000000000000000000000000000000041c18b2a09e7d03f38102824a401a765fe05a40753a2188520250e7ffb825f41960dd8703c82a9683c0a7a8eafb2b930aa29b3edc018cad7afc6e29781420a8ec51b00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000de0b6b3a7640000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a0000000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000000000020000000000000000000000004fabb145d64652a948d72533023f6e7a623c7c53000000000000000000000000c02aaa39b223fe8d0a0e5c4f27ead9083c756cc2')  # noqa E501
```

### Comparing `uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder/_abi_builder.py` & `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_abi_builder.py`

 * *Files identical despite different names*

### Comparing `uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder/_constants.py` & `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_constants.py`

 * *Files identical despite different names*

### Comparing `uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder/_decoder.py` & `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_decoder.py`

 * *Files identical despite different names*

### Comparing `uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder/_encoder.py` & `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_encoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -133,14 +133,38 @@
         :return: The chain link corresponding to this function call.
         """
         recipient = self._get_recipient(function_recipient, custom_recipient)
         self.commands.append(_RouterFunction.WRAP_ETH)
         self.arguments.append(Web3.to_bytes(hexstr=self._encode_wrap_eth_sub_contract(recipient, amount)))
         return self
 
+    def _encode_unwrap_weth_sub_contract(self, recipient: ChecksumAddress, amount_min: Wei) -> HexStr:
+        abi_mapping = self._abi_map[_RouterFunction.UNWRAP_WETH]
+        sub_contract = self._w3.eth.contract(abi=abi_mapping.fct_abi.get_full_abi())
+        contract_function: ContractFunction = sub_contract.functions.UNWRAP_WETH(recipient, amount_min)
+        return remove_0x_prefix(encode_abi(self._w3, contract_function.abi, [recipient, amount_min]))
+
+    def unwrap_weth(
+            self,
+            function_recipient: FunctionRecipient,
+            amount: Wei,
+            custom_recipient: Optional[ChecksumAddress] = None) -> _ChainedFunctionBuilder:
+        """
+        Encode the call to the function UNWRAP_WETH which convert WETH to ETH through the UR
+
+        :param function_recipient: A FunctionRecipient which defines the recipient of this function output.
+        :param amount: The amount of sent WETH in WEI.
+        :param custom_recipient: If function_recipient is CUSTOM, must be the actual recipient, otherwise None.
+        :return: The chain link corresponding to this function call.
+        """
+        recipient = self._get_recipient(function_recipient, custom_recipient)
+        self.commands.append(_RouterFunction.UNWRAP_WETH)
+        self.arguments.append(Web3.to_bytes(hexstr=self._encode_unwrap_weth_sub_contract(recipient, amount)))
+        return self
+
     def _encode_v2_swap_exact_in_sub_contract(
             self,
             recipient: ChecksumAddress,
             amount_in: Wei,
             amount_out_min: Wei,
             path: Sequence[ChecksumAddress],
             payer_is_user: bool) -> HexStr:
@@ -181,14 +205,43 @@
                     path,
                     payer_is_sender,
                 )
             )
         )
         return self
 
+    def v2_swap_exact_in_from_balance(
+            self,
+            function_recipient: FunctionRecipient,
+            amount_out_min: Wei,
+            path: Sequence[ChecksumAddress],
+            custom_recipient: Optional[ChecksumAddress] = None,
+            payer_is_sender: bool = True) -> _ChainedFunctionBuilder:
+        """
+        Encode the call to the function V2_SWAP_EXACT_IN, using the router balance as amount_in,
+        which swaps tokens on Uniswap V2.
+        Typically used when the amount_in is unknown because it comes from a V*_SWAP_EXACT_IN output.
+        Correct allowances must have been set before sending such transaction.
+
+        :param function_recipient: A FunctionRecipient which defines the recipient of this function output.
+        :param amount_out_min: The minimum accepted bought token (token_out)
+        :param path: The V2 path: a list of 2 or 3 tokens where the first is token_in and the last is token_out
+        :param custom_recipient: If function_recipient is CUSTOM, must be the actual recipient, otherwise None.
+        :param payer_is_sender: True if the in tokens come from the sender, False if they already are in the router
+        :return: The chain link corresponding to this function call.
+        """
+        return self.v2_swap_exact_in(
+            function_recipient,
+            _RouterConstant.ROUTER_BALANCE.value,
+            amount_out_min,
+            path,
+            custom_recipient,
+            payer_is_sender,
+        )
+
     def _encode_v2_swap_exact_out_sub_contract(
             self,
             recipient: ChecksumAddress,
             amount_out: Wei,
             amount_in_max: Wei,
             path: Sequence[ChecksumAddress],
             payer_is_user: bool) -> HexStr:
@@ -279,14 +332,44 @@
                     path,
                     payer_is_sender,
                 )
             )
         )
         return self
 
+    def v3_swap_exact_in_from_balance(
+            self,
+            function_recipient: FunctionRecipient,
+            amount_out_min: Wei,
+            path: Sequence[Union[int, ChecksumAddress]],
+            custom_recipient: Optional[ChecksumAddress] = None,
+            payer_is_sender: bool = True) -> _ChainedFunctionBuilder:
+        """
+        Encode the call to the function V3_SWAP_EXACT_IN, using the router balance as amount_in,
+        which swaps tokens on Uniswap V3.
+        Typically used when the amount_in is unknown because it comes from a V*_SWAP_EXACT_IN output.
+        Correct allowances must have been set before sending such transaction.
+
+        :param function_recipient: A FunctionRecipient which defines the recipient of this function output.
+        :param amount_out_min: The minimum accepted bought token (token_out) in Wei
+        :param path: The V3 path: a list of tokens where the first is the token_in, the last one is the token_out, and
+        with the pool fee between each token in basis points (ex: 3000 for 0.3%)
+        :param custom_recipient: If function_recipient is CUSTOM, must be the actual recipient, otherwise None.
+        :param payer_is_sender: True if the in tokens come from the sender, False if they already are in the router
+        :return: The chain link corresponding to this function call.
+        """
+        return self.v3_swap_exact_in(
+            function_recipient,
+            _RouterConstant.ROUTER_BALANCE.value,
+            amount_out_min,
+            path,
+            custom_recipient,
+            payer_is_sender,
+        )
+
     def _encode_v3_swap_exact_out_sub_contract(
             self,
             recipient: ChecksumAddress,
             amount_out: Wei,
             amount_in_max: Wei,
             path: Sequence[Union[int, ChecksumAddress]],
             payer_is_user: bool) -> HexStr:
```

### Comparing `uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder/_enums.py` & `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 * Doc: https://github.com/Elnaril/uniswap-universal-router-decoder
 """
 
 
 from enum import Enum
 
 from web3 import Web3
+from web3.types import Wei
 
 
 class _RouterFunction(Enum):
     # https://docs.uniswap.org/contracts/universal-router/technical-reference#command
     V3_SWAP_EXACT_IN = 0
     V3_SWAP_EXACT_OUT = 1
     V2_SWAP_EXACT_IN = 8
@@ -29,7 +30,8 @@
     CUSTOM = "recipient is custom"
 
 
 class _RouterConstant(Enum):
     # https://github.com/Uniswap/universal-router/blob/main/contracts/libraries/Constants.sol
     MSG_SENDER = Web3.to_checksum_address("0x0000000000000000000000000000000000000001")
     ADDRESS_THIS = Web3.to_checksum_address("0x0000000000000000000000000000000000000002")
+    ROUTER_BALANCE = Wei(2**255)
```

### Comparing `uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder/router_codec.py` & `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/router_codec.py`

 * *Files identical despite different names*

### Comparing `uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder.egg-info/PKG-INFO` & `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: uniswap-universal-router-decoder
-Version: 0.8.0
-Summary: Decode & Encode transaction data sent to Uniswap universal router
+Version: 0.9.0
+Summary: Decode & Encode transaction data sent to Uniswap Universal Router
 Author-email: Elnaril <elnaril_dev@caramail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Elnaril/uniswap-universal-router-decoder
 Project-URL: Bug Tracker, https://github.com/Elnaril/uniswap-universal-router-decoder/issues
 Project-URL: Fiverr, https://www.fiverr.com/elnaril
-Keywords: blockchain,ethereum,uniswap,universal router,decoder,encoder
+Keywords: blockchain,ethereum,uniswap,universal router,decoder,encoder,codec,wrapper
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Uniswap Universal Router Decoder & Encoder v0.8.0
-⚠ This version introduces breaking changes compared to v0.7 !
+# Uniswap Universal Router Decoder & Encoder v0.9.0
 
 ---
 
 #### Project Information
 [![Tests & Lint](https://github.com/Elnaril/uniswap-universal-router-decoder/actions/workflows/tests.yml/badge.svg)](https://github.com/Elnaril/uniswap-universal-router-decoder/actions/workflows/tests.yml)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/uniswap-universal-router-decoder)](https://pypi.org/project/uniswap-universal-router-decoder/)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/Elnaril/uniswap-universal-router-decoder)](https://github.com/Elnaril/uniswap-universal-router-decoder/releases)
@@ -40,54 +39,44 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Type Checker: mypy](https://img.shields.io/badge/%20type%20checker-mypy-%231674b1?style=flat&labelColor=ef8336)](https://mypy-lang.org/)
 [![Linter: flake8](https://img.shields.io/badge/%20linter-flake8-%231674b1?style=flat&labelColor=ef8336)](https://flake8.pycqa.org/en/latest/)
 
 ---
 
 ## Release Notes
+### V0.9.0
+ - Add support for UNWRAP_WETH encoding
+ - Add v2_swap_exact_in_from_balance() and v3_swap_exact_in_from_balance(): 2 convenient methods which are used when the exact in_amount is not known when the transaction is built, typically chained after a V*_SWAP_EXACT_IN.
 ### V0.8.0
  - Breaking changes because of refactoring
  - Command chaining extension: all supported UR functions can now be chained in a single transaction
-### V0.7.1
- -  Fix issue [#1](https://github.com/Elnaril/uniswap-universal-router-decoder/issues/1) - v3 path decoding fails for some paths 
-### V0.7.0
- - Add support for encoding V2_SWAP_EXACT_OUT
- - Add support for encoding V3_SWAP_EXACT_OUT
- - Fix V3_SWAP_EXACT_OUT ABI
- - Fix typos in README
-### V0.6.0
- - Breaking changes: use Web3.py v6 i/o v5
- - Add support for the PERMIT2_PERMIT function
- - Add support for chaining PERMIT2_PERMIT and V2_SWAP_EXACT_IN in the same transaction
 
 ---
 
 ## Overview and Points of Attention
 
 The object of this library is to decode & encode the transaction input sent to the Uniswap universal router (UR)
-(address [`0xEf1c6E67703c7BD7107eed8303Fbe6EC2554BF6B`](https://etherscan.io/address/0xEf1c6E67703c7BD7107eed8303Fbe6EC2554BF6B) 
+(address [`0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD`](https://etherscan.io/address/0xEf1c6E67703c7BD7107eed8303Fbe6EC2554BF6B) 
 on Ethereum Mainnet). It is based on, and is intended to be used with [web3.py](https://github.com/ethereum/web3.py)
 
 ⚠ This library has not been audited, so use at your own risk !
 
-⚠ At this stage, there is no guarantee of compatibility between 2 versions: consider forcing the version in your dependency requirements.
-
 ⚠ This project is a work in progress so not all commands are decoded yet. Below the list of the already implemented ones.
 
 | Command Id | Function Name | Decode | Encode
 | ---------- | ------------- |:------:|:------:
 | 0x00 | V3_SWAP_EXACT_IN | ✅ | ✅
 | 0x01 | V3_SWAP_EXACT_OUT | ✅ | ✅
 | 0x02 - 0x06 |  | ❌ | ❌
 | 0x07 | placeholder  | N/A | N/A
 | 0x08 | V2_SWAP_EXACT_IN | ✅ | ✅
 | 0x09 | V2_SWAP_EXACT_OUT | ✅ | ✅
 | 0x0a | PERMIT2_PERMIT | ✅ | ✅
 | 0x0b | WRAP_ETH | ✅ | ✅
-| 0x0c | UNWRAP_WETH | ✅ | ❌
+| 0x0c | UNWRAP_WETH | ✅ | ✅
 | 0x0d | PERMIT2_TRANSFER_FROM_BATCH | ❌ | ❌
 | 0x0e - 0x0f | placeholders | N/A | N/A
 | 0x10 - 0x1d |  | ❌ | ❌
 | 0x1e - 0x3f | placeholders | N/A | N/A
 
 ---
 
@@ -221,15 +210,14 @@
 
 # then in your transaction dict:
 transaction["data"] = encoded_data
 
 # you can now sign and send the transaction to the UR
 ```
 
-
 ### How to encode a call to the function V2_SWAP_EXACT_IN
 This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before using sending such transaction.
 ```python
 from uniswap_universal_router_decoder import FunctionRecipient, RouterCodec
 
 codec = RouterCodec()
 encoded_data = codec.encode.chain().v2_swap_exact_in(
```

### Comparing `uniswap-universal-router-decoder-0.8.0/uniswap_universal_router_decoder.egg-info/SOURCES.txt` & `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

