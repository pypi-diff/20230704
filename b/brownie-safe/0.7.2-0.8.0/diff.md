# Comparing `tmp/brownie_safe-0.7.2.tar.gz` & `tmp/brownie_safe-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brownie_safe-0.7.2.tar", max compression
+gzip compressed data, was "brownie_safe-0.8.0.tar", max compression
```

## Comparing `brownie_safe-0.7.2.tar` & `brownie_safe-0.8.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    16748 2023-06-28 15:46:23.877988 brownie_safe-0.7.2/brownie_safe.py
--rw-r--r--   0        0        0      539 2023-06-28 15:45:42.147713 brownie_safe-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      910 2023-06-28 15:50:55.502434 brownie_safe-0.7.2/readme.md
--rw-r--r--   0        0        0     1634 1970-01-01 00:00:00.000000 brownie_safe-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    17686 2023-07-04 18:56:06.394943 brownie_safe-0.8.0/brownie_safe.py
+-rw-r--r--   0        0        0      539 2023-07-04 18:57:17.353280 brownie_safe-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      910 2023-06-28 16:20:48.160418 brownie_safe-0.8.0/readme.md
+-rw-r--r--   0        0        0     1634 1970-01-01 00:00:00.000000 brownie_safe-0.8.0/PKG-INFO
```

### Comparing `brownie_safe-0.7.2/brownie_safe.py` & `brownie_safe-0.8.0/brownie_safe.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from gnosis.eth import EthereumClient, EthereumNetwork
 from web3 import Web3  # don't move below brownie import
 from brownie import Contract, accounts, chain, history, web3
 from brownie.convert.datatypes import EthAddress
 from brownie.network.account import LocalAccount
 from brownie.network.transaction import TransactionReceipt
 from eth_abi import encode_abi
-from eth_utils import is_address, to_checksum_address
+from eth_utils import is_address, to_checksum_address, encode_hex, keccak
 from gnosis.safe import Safe, SafeOperation
 from gnosis.safe.multi_send import MultiSend, MultiSendOperation, MultiSendTx
 from gnosis.safe.safe_tx import SafeTx
 from gnosis.safe.signatures import signature_split, signature_to_bytes
 from gnosis.safe.api import TransactionServiceApi
 from hexbytes import HexBytes
 from trezorlib import ethereum, tools, ui
@@ -93,14 +93,16 @@
         Create an BrownieSafe from an address or a ENS name and use a default connection.
         """
         address = to_checksum_address(address) if is_address(address) else web3.ens.resolve(address)
         ethereum_client = EthereumClient(web3.provider.endpoint_uri)
         self.transaction_service = TransactionServiceBackport(ethereum_client.get_network(), ethereum_client, base_url)
         self.multisend = multisend or multisends.get(chain.id, MULTISEND_CALL_ONLY)
         super().__init__(address, ethereum_client)
+        if web3.clientVersion.startswith('anvil'):
+            web3.manager.request_blocking('anvil_setNextBlockBaseFeePerGas', ['0x0'])
 
     def __str__(self):
         return EthAddress(self.address)
 
     def __repr__(self):
         return f'BrownieSafe("{self.address}")'
 
@@ -302,31 +304,45 @@
 
     def estimate_gas(self, safe_tx: SafeTx) -> int:
         """
         Estimate gas limit for successful execution.
         """
         return self.estimate_tx_gas(safe_tx.to, safe_tx.value, safe_tx.data, safe_tx.operation)
 
+    def set_storage(self, account: str, slot: int, value: int):
+        params = [account, hex(slot), encode_hex(encode_abi(['uint'], [value]))]
+
+        if web3.clientVersion.startswith('anvil'):
+            web3.manager.request_blocking('anvil_setStorageAt', params)
+        elif web3.clientVersion.startswith('Hardhat'):
+            web3.manager.request_blocking('hardhat_setStorageAt', params)
+        else:
+            raise NotImplementedError(f'setting storage is not supported for {web3.clientVersion}')
+
     def preview_tx(self, safe_tx: SafeTx, events=True, call_trace=False) -> TransactionReceipt:
         tx = copy(safe_tx)
         safe = Contract.from_abi('Gnosis Safe', self.address, self.get_contract().abi)
         # Replace pending nonce with the subsequent nonce, this could change the safe_tx_hash
         tx.safe_nonce = safe.nonce()
         # Forge signatures from the needed amount of owners, skip the one which submits the tx
         # Owners must be sorted numerically, sorting as checksum addresses may yield wrong order
         threshold = safe.getThreshold()
         sorted_owners = sorted(safe.getOwners(), key=lambda x: int(x, 16))
         owners = [accounts.at(owner, force=True) for owner in sorted_owners[:threshold]]
-        for owner in owners:
-            safe.approveHash(tx.safe_tx_hash, {'from': owner})
-
         # Signautres are encoded as [bytes32 r, bytes32 s, bytes8 v]
         # Pre-validated signatures are encoded as r=owner, s unused and v=1.
         # https://docs.gnosis.io/safe/docs/contracts_signatures/#pre-validated-signatures
         tx.signatures = b''.join([encode_abi(['address', 'uint'], [str(owner), 0]) + b'\x01' for owner in owners])
+
+        # approvedHashes are in slot 8 and have type of mapping(address => mapping(bytes32 => uint256))
+        for owner in owners[:threshold]:
+            outer_key = keccak(encode_abi(['address', 'uint'], [str(owner), 8]))
+            slot = int.from_bytes(keccak(tx.safe_tx_hash + outer_key), 'big')
+            self.set_storage(tx.safe_address, slot, 1)
+
         payload = tx.w3_tx.buildTransaction()
         receipt = owners[0].transfer(payload['to'], payload['value'], gas_limit=payload['gas'], data=payload['data'])
 
         if 'ExecutionSuccess' not in receipt.events:
             receipt.info()
             receipt.call_trace(True)
             raise ExecutionFailure()
```

### Comparing `brownie_safe-0.7.2/pyproject.toml` & `brownie_safe-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brownie-safe"
-version = "0.7.2"
+version = "0.8.0"
 description = "Build complex Gnosis Safe transactions and safely preview them in a forked environment."
 authors = ["banteg"]
 license = "MIT"
 repository = "https://github.com/banteg/brownie-safe"
 readme = "readme.md"
 
 [tool.poetry.dependencies]
```

### Comparing `brownie_safe-0.7.2/readme.md` & `brownie_safe-0.8.0/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Brownie Safe: Gnosis Safe tx builder
 
 [Read Documentation](https://safe.ape.tax/)
 
 Brownie Safe allows you to iteratively build complex multi-step Gnosis Safe transactions and safely preview their side effects from the convenience of a locally forked mainnet environment.
 
-*Previously known as Ape Safe`
+*Previously known as Ape Safe*
 
 ## Installation
 
 ```
 pip install -U brownie-safe
 ```
```

### Comparing `brownie_safe-0.7.2/PKG-INFO` & `brownie_safe-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brownie-safe
-Version: 0.7.2
+Version: 0.8.0
 Summary: Build complex Gnosis Safe transactions and safely preview them in a forked environment.
 Home-page: https://github.com/banteg/brownie-safe
 License: MIT
 Author: banteg
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 
 # Brownie Safe: Gnosis Safe tx builder
 
 [Read Documentation](https://safe.ape.tax/)
 
 Brownie Safe allows you to iteratively build complex multi-step Gnosis Safe transactions and safely preview their side effects from the convenience of a locally forked mainnet environment.
 
-*Previously known as Ape Safe`
+*Previously known as Ape Safe*
 
 ## Installation
 
 ```
 pip install -U brownie-safe
 ```
```

