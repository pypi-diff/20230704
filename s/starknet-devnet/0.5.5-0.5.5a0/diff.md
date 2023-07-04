# Comparing `tmp/starknet_devnet-0.5.5.tar.gz` & `tmp/starknet_devnet-0.5.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starknet_devnet-0.5.5.tar", max compression
+gzip compressed data, was "starknet_devnet-0.5.5a0.tar", max compression
```

## Comparing `starknet_devnet-0.5.5.tar` & `starknet_devnet-0.5.5a0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1067 2023-07-04 13:41:12.919190 starknet_devnet-0.5.5/LICENSE
--rw-r--r--   0        0        0     1054 2023-07-04 13:41:12.919190 starknet_devnet-0.5.5/README.md
--rw-r--r--   0        0        0     1818 2023-07-04 13:41:12.931190 starknet_devnet-0.5.5/pyproject.toml
--rw-r--r--   0        0        0   208485 2023-07-04 13:41:12.935190 starknet_devnet-0.5.5/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json
--rw-r--r--   0        0        0    32739 2023-07-04 13:41:12.935190 starknet_devnet-0.5.5/starknet_devnet/MockStarknetMessaging.json
--rw-r--r--   0        0        0    35645 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/UDC_OZ_0.5.0.json
--rw-r--r--   0        0        0     2958 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/__init__.py
--rw-r--r--   0        0        0     2779 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/account.py
--rw-r--r--   0        0        0     4161 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/account_util.py
--rw-r--r--   0        0        0     2511 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/accounts.py
--rw-r--r--   0        0        0   118818 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json
--rw-r--r--   0        0        0     1784 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json
--rw-r--r--   0        0        0     1866 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/block_info_generator.py
--rw-r--r--   0        0        0    12483 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blocks.py
--rw-r--r--   0        0        0        0 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/__init__.py
--rw-r--r--   0        0        0     7585 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/base.py
--rw-r--r--   0        0        0    14072 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/feeder_gateway.py
--rw-r--r--   0        0        0     2256 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/gateway.py
--rw-r--r--   0        0        0     3959 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/postman.py
--rw-r--r--   0        0        0        0 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/__init__.py
--rw-r--r--   0        0        0     2138 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/blocks.py
--rw-r--r--   0        0        0     2120 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/call.py
--rw-r--r--   0        0        0     2195 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/classes.py
--rw-r--r--   0        0        0     6257 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/misc.py
--rw-r--r--   0        0        0     4953 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/routes.py
--rw-r--r--   0        0        0   116673 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/rpc_spec.py
--rw-r--r--   0        0        0     6049 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/rpc_spec_write.py
--rw-r--r--   0        0        0    16310 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/rpc_trace_spec.py
--rw-r--r--   0        0        0     7135 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/schema.py
--rw-r--r--   0        0        0     1144 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/state.py
--rw-r--r--   0        0        0      929 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/storage.py
--rw-r--r--   0        0        0        0 2023-07-04 13:41:12.939190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/structures/__init__.py
--rw-r--r--   0        0        0    32879 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/structures/payloads.py
--rw-r--r--   0        0        0     6494 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/structures/responses.py
--rw-r--r--   0        0        0     3457 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/structures/types.py
--rw-r--r--   0        0        0     8789 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/transactions.py
--rw-r--r--   0        0        0     3542 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/utils.py
--rw-r--r--   0        0        0      899 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/blueprints/shared.py
--rw-r--r--   0        0        0    24763 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/cairo_rs_py_patch.py
--rw-r--r--   0        0        0     1038 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/chargeable_account.py
--rw-r--r--   0        0        0     5310 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/compiler.py
--rw-r--r--   0        0        0     1239 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/constants.py
--rw-r--r--   0        0        0      646 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/contract_class_wrapper.py
--rw-r--r--   0        0        0    16332 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/devnet_config.py
--rw-r--r--   0        0        0      784 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/dump.py
--rw-r--r--   0        0        0     6558 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/fee_token.py
--rw-r--r--   0        0        0     8332 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/forked_state.py
--rw-r--r--   0        0        0     1680 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/general_config.py
--rw-r--r--   0        0        0     9005 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/origin.py
--rw-r--r--   0        0        0    10015 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/postman_wrapper.py
--rw-r--r--   0        0        0     2237 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/predeployed_contract_wrapper.py
--rw-r--r--   0        0        0     4353 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/server.py
--rw-r--r--   0        0        0    41451 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/starknet_wrapper.py
--rw-r--r--   0        0        0     1988 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/state.py
--rw-r--r--   0        0        0     2573 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/state_archive.py
--rw-r--r--   0        0        0    11947 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/transactions.py
--rw-r--r--   0        0        0     1822 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/udc.py
--rw-r--r--   0        0        0    11174 2023-07-04 13:41:12.943190 starknet_devnet-0.5.5/starknet_devnet/util.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 starknet_devnet-0.5.5/setup.py
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 starknet_devnet-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-03 11:45:14.809619 starknet_devnet-0.5.5a0/LICENSE
+-rw-r--r--   0        0        0     1054 2023-07-03 11:45:14.809619 starknet_devnet-0.5.5a0/README.md
+-rw-r--r--   0        0        0     1822 2023-07-03 11:45:14.821619 starknet_devnet-0.5.5a0/pyproject.toml
+-rw-r--r--   0        0        0   208485 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json
+-rw-r--r--   0        0        0    32739 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/MockStarknetMessaging.json
+-rw-r--r--   0        0        0    35645 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/UDC_OZ_0.5.0.json
+-rw-r--r--   0        0        0     2960 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/__init__.py
+-rw-r--r--   0        0        0     2779 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/account.py
+-rw-r--r--   0        0        0     4161 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/account_util.py
+-rw-r--r--   0        0        0     2511 2023-07-03 11:45:14.825619 starknet_devnet-0.5.5a0/starknet_devnet/accounts.py
+-rw-r--r--   0        0        0   118818 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json
+-rw-r--r--   0        0        0     1784 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json
+-rw-r--r--   0        0        0     1866 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/block_info_generator.py
+-rw-r--r--   0        0        0    12483 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blocks.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/__init__.py
+-rw-r--r--   0        0        0     7585 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/base.py
+-rw-r--r--   0        0        0    14072 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/feeder_gateway.py
+-rw-r--r--   0        0        0     2256 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/gateway.py
+-rw-r--r--   0        0        0     3959 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/postman.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/__init__.py
+-rw-r--r--   0        0        0     2138 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/blocks.py
+-rw-r--r--   0        0        0     2120 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/call.py
+-rw-r--r--   0        0        0     2195 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/classes.py
+-rw-r--r--   0        0        0     6257 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/misc.py
+-rw-r--r--   0        0        0     4953 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/routes.py
+-rw-r--r--   0        0        0   116673 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_spec.py
+-rw-r--r--   0        0        0     6049 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_spec_write.py
+-rw-r--r--   0        0        0    16310 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_trace_spec.py
+-rw-r--r--   0        0        0     7135 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/schema.py
+-rw-r--r--   0        0        0     1144 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/state.py
+-rw-r--r--   0        0        0      929 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/storage.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/__init__.py
+-rw-r--r--   0        0        0    32879 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/payloads.py
+-rw-r--r--   0        0        0     6494 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/responses.py
+-rw-r--r--   0        0        0     3457 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/types.py
+-rw-r--r--   0        0        0     8789 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/transactions.py
+-rw-r--r--   0        0        0     3542 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/utils.py
+-rw-r--r--   0        0        0      899 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/blueprints/shared.py
+-rw-r--r--   0        0        0    24763 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/cairo_rs_py_patch.py
+-rw-r--r--   0        0        0     1038 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/chargeable_account.py
+-rw-r--r--   0        0        0     5310 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/compiler.py
+-rw-r--r--   0        0        0     1239 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/constants.py
+-rw-r--r--   0        0        0      646 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/contract_class_wrapper.py
+-rw-r--r--   0        0        0    16332 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/devnet_config.py
+-rw-r--r--   0        0        0      784 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/dump.py
+-rw-r--r--   0        0        0     6558 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/fee_token.py
+-rw-r--r--   0        0        0     8332 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/forked_state.py
+-rw-r--r--   0        0        0     1640 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/general_config.py
+-rw-r--r--   0        0        0     9005 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/origin.py
+-rw-r--r--   0        0        0    10015 2023-07-03 11:45:14.829619 starknet_devnet-0.5.5a0/starknet_devnet/postman_wrapper.py
+-rw-r--r--   0        0        0     2237 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/predeployed_contract_wrapper.py
+-rw-r--r--   0        0        0     4353 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/server.py
+-rw-r--r--   0        0        0    41451 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/starknet_wrapper.py
+-rw-r--r--   0        0        0     1988 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/state.py
+-rw-r--r--   0        0        0     2573 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/state_archive.py
+-rw-r--r--   0        0        0    11947 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/transactions.py
+-rw-r--r--   0        0        0     1822 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/udc.py
+-rw-r--r--   0        0        0    11174 2023-07-03 11:45:14.833619 starknet_devnet-0.5.5a0/starknet_devnet/util.py
+-rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 starknet_devnet-0.5.5a0/setup.py
+-rw-r--r--   0        0        0     2193 1970-01-01 00:00:00.000000 starknet_devnet-0.5.5a0/PKG-INFO
```

### Comparing `starknet_devnet-0.5.5/LICENSE` & `starknet_devnet-0.5.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/README.md` & `starknet_devnet-0.5.5a0/README.md`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/pyproject.toml` & `starknet_devnet-0.5.5a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "starknet_devnet"
-version = "0.5.5"
+version = "0.5.5a0"
 description = "A local testnet for Starknet"
 authors = ["FabijanC <fabijan.corak@gmail.com>"]
 license = "MIT"
 
 readme = "README.md"
 repository = "https://github.com/0xSpaceShard/starknet-devnet"
 homepage = "https://github.com/0xSpaceShard/starknet-devnet"
 keywords = ["starknet", "cairo", "testnet", "local", "server"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.10"
 Flask = {extras = ["async"], version = "~2.0.3"}
 flask-cors = "~3.0.10"
-cairo-lang = "0.12.0"
+cairo-lang = "0.12.0a0"
 Werkzeug = "~2.0.3"
 cloudpickle = "~2.1.0"
 crypto-cpp-py = "~1.4.0"
 marshmallow = "~3.17.0"
 typing-extensions = "~4.3.0"
 gunicorn = "~20.1.0"
 marshmallow-dataclass = "~8.4"
```

### Comparing `starknet_devnet-0.5.5/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json` & `starknet_devnet-0.5.5a0/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/MockStarknetMessaging.json` & `starknet_devnet-0.5.5a0/starknet_devnet/MockStarknetMessaging.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/UDC_OZ_0.5.0.json` & `starknet_devnet-0.5.5a0/starknet_devnet/UDC_OZ_0.5.0.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/__init__.py` & `starknet_devnet-0.5.5a0/starknet_devnet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # pylint: disable=unused-import
 # pylint: disable=import-outside-toplevel
 
 import os
 import sys
 
-__version__ = "0.5.5"
+__version__ = "0.5.5a0"
 
 
 def _patch_pedersen_hash():
     """
     Improves performance by substituting the default Python implementation of Pedersen hash
     with Software Mansion's Python wrapper of C++ implementation.
     """
```

### Comparing `starknet_devnet-0.5.5/starknet_devnet/account.py` & `starknet_devnet-0.5.5a0/starknet_devnet/account.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/account_util.py` & `starknet_devnet-0.5.5a0/starknet_devnet/account_util.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/accounts.py` & `starknet_devnet-0.5.5a0/starknet_devnet/accounts.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json` & `starknet_devnet-0.5.5a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json` & `starknet_devnet-0.5.5a0/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/block_info_generator.py` & `starknet_devnet-0.5.5a0/starknet_devnet/block_info_generator.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blocks.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blocks.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/base.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/base.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/feeder_gateway.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/feeder_gateway.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/gateway.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/gateway.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/postman.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/postman.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/blocks.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/blocks.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/call.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/call.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/classes.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/classes.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/misc.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/misc.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/routes.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/routes.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/rpc_spec.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_spec.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/rpc_spec_write.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_spec_write.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/rpc_trace_spec.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/rpc_trace_spec.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/schema.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/schema.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/state.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/storage.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/storage.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/structures/payloads.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/payloads.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/structures/responses.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/responses.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/structures/types.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/structures/types.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/transactions.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/transactions.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/rpc/utils.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/blueprints/shared.py` & `starknet_devnet-0.5.5a0/starknet_devnet/blueprints/shared.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/cairo_rs_py_patch.py` & `starknet_devnet-0.5.5a0/starknet_devnet/cairo_rs_py_patch.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/chargeable_account.py` & `starknet_devnet-0.5.5a0/starknet_devnet/chargeable_account.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/compiler.py` & `starknet_devnet-0.5.5a0/starknet_devnet/compiler.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/constants.py` & `starknet_devnet-0.5.5a0/starknet_devnet/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 OLD_SUPPORTED_VERSIONS = [0]
 
 # account used by Starknet CLI; calculated using
 # poetry run python scripts/compute_compiled_class_hash.py \
 #   ~/.cache/pypoetry/virtualenvs/<YOUR_VENV>/lib/python3.9/site-packages/starkware/starknet/third_party/open_zeppelin/account.json
 STARKNET_CLI_ACCOUNT_CLASS_HASH = (
-    0x646A72E2AAB2FCA75D713FBE4A58F2D12CBD64105621B89DC9CE7045B5BF02B
+    0x2AF01407D426B1FFF03A6982813EA9F3E9467B2B19EDCC9FB612C3B5B6FFCEB
 )
 
 # starkware.starknet.public.abi.get_selector_from_name("replace_class")
 REPLACE_CLASS_SELECTOR = (
     0x217DF192877EED2921E241046523F8D8DA7981F0A3DDAFE0E7517F6523276D2
 )
```

### Comparing `starknet_devnet-0.5.5/starknet_devnet/contract_class_wrapper.py` & `starknet_devnet-0.5.5a0/starknet_devnet/contract_class_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/devnet_config.py` & `starknet_devnet-0.5.5a0/starknet_devnet/devnet_config.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/dump.py` & `starknet_devnet-0.5.5a0/starknet_devnet/dump.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/fee_token.py` & `starknet_devnet-0.5.5a0/starknet_devnet/fee_token.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/forked_state.py` & `starknet_devnet-0.5.5a0/starknet_devnet/forked_state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/general_config.py` & `starknet_devnet-0.5.5a0/starknet_devnet/general_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
             "compiled_class_hash_commitment_tree_height": constants.COMPILED_CLASS_HASH_COMMITMENT_TREE_HEIGHT,
             "contract_storage_commitment_tree_height": constants.CONTRACT_STATES_COMMITMENT_TREE_HEIGHT,
             "enforce_l1_handler_fee": True,
             "event_commitment_tree_height": constants.EVENT_COMMITMENT_TREE_HEIGHT,
             "global_state_commitment_tree_height": constants.CONTRACT_ADDRESS_BITS,
             "invoke_tx_max_n_steps": DEFAULT_MAX_STEPS,
             "min_gas_price": DEFAULT_GAS_PRICE,
-            "constant_gas_price": True,
             "sequencer_address": hex(DEFAULT_SEQUENCER_ADDRESS),
             "starknet_os_config": {
                 "chain_id": chain_id.value,
                 "fee_token_address": hex(FeeToken.ADDRESS),
             },
             "tx_commitment_tree_height": constants.TRANSACTION_COMMITMENT_TREE_HEIGHT,
             "validate_max_n_steps": DEFAULT_VALIDATE_MAX_STEPS,
```

### Comparing `starknet_devnet-0.5.5/starknet_devnet/origin.py` & `starknet_devnet-0.5.5a0/starknet_devnet/origin.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/postman_wrapper.py` & `starknet_devnet-0.5.5a0/starknet_devnet/postman_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/predeployed_contract_wrapper.py` & `starknet_devnet-0.5.5a0/starknet_devnet/predeployed_contract_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/server.py` & `starknet_devnet-0.5.5a0/starknet_devnet/server.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/starknet_wrapper.py` & `starknet_devnet-0.5.5a0/starknet_devnet/starknet_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/state.py` & `starknet_devnet-0.5.5a0/starknet_devnet/state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/state_archive.py` & `starknet_devnet-0.5.5a0/starknet_devnet/state_archive.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/transactions.py` & `starknet_devnet-0.5.5a0/starknet_devnet/transactions.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/udc.py` & `starknet_devnet-0.5.5a0/starknet_devnet/udc.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/starknet_devnet/util.py` & `starknet_devnet-0.5.5a0/starknet_devnet/util.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.5/setup.py` & `starknet_devnet-0.5.5a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 package_data = \
 {'': ['*'],
  'starknet_devnet': ['accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/*']}
 
 install_requires = \
 ['Flask[async]>=2.0.3,<2.1.0',
  'Werkzeug>=2.0.3,<2.1.0',
- 'cairo-lang==0.12.0',
+ 'cairo-lang==0.12.0a0',
  'cloudpickle>=2.1.0,<2.2.0',
  'crypto-cpp-py>=1.4.0,<1.5.0',
  'flask-cors>=3.0.10,<3.1.0',
  'gunicorn>=20.1.0,<20.2.0',
  'jsonschema>=4.17.0,<4.18.0',
  'marshmallow-dataclass>=8.4,<8.5',
  'marshmallow>=3.17.0,<3.18.0',
@@ -27,15 +27,15 @@
  'web3>=6.0.0,<6.1.0']
 
 entry_points = \
 {'console_scripts': ['starknet-devnet = starknet_devnet.server:main']}
 
 setup_kwargs = {
     'name': 'starknet-devnet',
-    'version': '0.5.5',
+    'version': '0.5.5a0',
     'description': 'A local testnet for Starknet',
     'long_description': '<!-- logo / title -->\n<p align="center" style="margin-bottom: 0px !important">\n  <img width="200" src="https://user-images.githubusercontent.com/2848732/193076972-da6fa36e-11f7-4cb3-aa29-673224f8576d.png" alt="Devnet" align="center">\n</p>\n<h1 align="center" style="margin-top: 0px !important">Starknet Devnet</h1>\n\nA Flask wrapper of Starknet state. Similar in purpose to Ganache.\n\nAims to mimic Starknet\'s Alpha testnet, but with simplified functionality.\n\n## 🌐 Docs\n\nOn the following links you can find the documentation of:\n\n- [the latest official release](https://0xspaceshard.github.io/starknet-devnet/)\n- [the latest master commit (not officially released)](https://github.com/0xSpaceShard/starknet-devnet/tree/master/page/docs)\n\n## ✏️ Contributing\n\nWe ❤️ and encourage all contributions!\n\n[Click here](https://0xspaceshard.github.io/starknet-devnet/docs/guide/development) for the development guide.\n\n## 🙌 Special Thanks\n\nSpecial thanks to all the [contributors](https://github.com/0xSpaceShard/starknet-devnet/graphs/contributors)!\n',
     'author': 'FabijanC',
     'author_email': 'fabijan.corak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xSpaceShard/starknet-devnet',
```

### Comparing `starknet_devnet-0.5.5/PKG-INFO` & `starknet_devnet-0.5.5a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: starknet-devnet
-Version: 0.5.5
+Version: 0.5.5a0
 Summary: A local testnet for Starknet
 Home-page: https://github.com/0xSpaceShard/starknet-devnet
 License: MIT
 Keywords: starknet,cairo,testnet,local,server
 Author: FabijanC
 Author-email: fabijan.corak@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask[async] (>=2.0.3,<2.1.0)
 Requires-Dist: Werkzeug (>=2.0.3,<2.1.0)
-Requires-Dist: cairo-lang (==0.12.0)
+Requires-Dist: cairo-lang (==0.12.0a0)
 Requires-Dist: cloudpickle (>=2.1.0,<2.2.0)
 Requires-Dist: crypto-cpp-py (>=1.4.0,<1.5.0)
 Requires-Dist: flask-cors (>=3.0.10,<3.1.0)
 Requires-Dist: gunicorn (>=20.1.0,<20.2.0)
 Requires-Dist: jsonschema (>=4.17.0,<4.18.0)
 Requires-Dist: marshmallow (>=3.17.0,<3.18.0)
 Requires-Dist: marshmallow-dataclass (>=8.4,<8.5)
```

