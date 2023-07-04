# Comparing `tmp/rubi-2.0.6.tar.gz` & `tmp/rubi-2.0.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.0.6.tar", max compression
+gzip compressed data, was "rubi-2.0.7b1.tar", max compression
```

## Comparing `rubi-2.0.6.tar` & `rubi-2.0.7b1.tar`

### file list

```diff
@@ -1,52 +1,38 @@
--rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.6/LICENSE
--rw-r--r--   0        0        0     2757 2023-06-01 22:20:20.359716 rubi-2.0.6/README.md
--rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.0.6/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.0.6/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.0.6/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.0.6/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      633 2023-06-30 02:50:06.551418 rubi-2.0.6/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.0.6/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.0.6/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      651 2023-06-30 02:50:06.551545 rubi-2.0.6/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.0.6/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.0.6/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      560 2023-06-30 22:38:54.821457 rubi-2.0.6/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.0.6/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.0.6/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      619 2023-06-30 02:50:06.551793 rubi-2.0.6/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0      898 2023-06-30 22:38:54.823155 rubi-2.0.6/pyproject.toml
--rw-r--r--   0        0        0      104 2023-06-30 02:50:06.553692 rubi-2.0.6/rubi/__init__.py
--rw-r--r--   0        0        0    26255 2023-06-30 22:38:54.823356 rubi-2.0.6/rubi/client.py
--rw-r--r--   0        0        0      163 2023-06-30 02:50:06.554484 rubi-2.0.6/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.6/rubi/contracts/aid.py
--rw-r--r--   0        0        0    11860 2023-06-30 22:38:54.823525 rubi-2.0.6/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0       74 2023-06-30 22:38:54.823906 rubi-2.0.6/rubi/contracts/contract_types/__init__.py
--rw-r--r--   0        0        0    15968 2023-06-30 02:50:06.555210 rubi-2.0.6/rubi/contracts/contract_types/events.py
--rw-r--r--   0        0        0     2708 2023-06-30 22:38:54.824073 rubi-2.0.6/rubi/contracts/contract_types/transaction_reciept.py
--rw-r--r--   0        0        0    17101 2023-06-30 22:38:54.824447 rubi-2.0.6/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24668 2023-06-30 22:38:54.824645 rubi-2.0.6/rubi/contracts/market.py
--rw-r--r--   0        0        0    14847 2023-06-30 02:50:06.556060 rubi-2.0.6/rubi/contracts/router.py
--rw-r--r--   0        0        0      257 2023-06-30 02:50:03.540922 rubi-2.0.6/rubi/data/README.md
--rw-r--r--   0        0        0       33 2023-06-30 02:50:03.541036 rubi-2.0.6/rubi/data/__init__.py
--rw-r--r--   0        0        0     3968 2023-06-30 02:50:03.541150 rubi-2.0.6/rubi/data/data.py
--rw-r--r--   0        0        0     1198 2023-06-30 02:50:03.541258 rubi-2.0.6/rubi/data/processing/README.md
--rw-r--r--   0        0        0       64 2023-06-30 02:50:03.541320 rubi-2.0.6/rubi/data/processing/__init__.py
--rw-r--r--   0        0        0    20226 2023-06-30 02:50:03.541646 rubi-2.0.6/rubi/data/processing/aid.py
--rw-r--r--   0        0        0       31 2023-06-30 02:50:03.541785 rubi-2.0.6/rubi/data/processing/helper/__init__.py
--rw-r--r--   0        0        0     2292 2023-06-30 02:50:03.541878 rubi-2.0.6/rubi/data/processing/helper/processing.py
--rw-r--r--   0        0        0    10226 2023-06-30 02:50:03.541970 rubi-2.0.6/rubi/data/processing/user.py
--rw-r--r--   0        0        0       69 2023-06-30 02:50:03.542086 rubi-2.0.6/rubi/data/sources/__init__.py
--rw-r--r--   0        0        0    21161 2023-06-30 02:50:03.542477 rubi-2.0.6/rubi/data/sources/aid.py
--rw-r--r--   0        0        0     1194 2023-06-30 02:50:03.542594 rubi-2.0.6/rubi/data/sources/helper/README.md
--rw-r--r--   0        0        0       76 2023-06-30 02:50:03.542657 rubi-2.0.6/rubi/data/sources/helper/__init__.py
--rw-r--r--   0        0        0    12589 2023-06-30 02:50:03.542925 rubi-2.0.6/rubi/data/sources/helper/gas.py
--rw-r--r--   0        0        0    15373 2023-06-30 02:50:03.543041 rubi-2.0.6/rubi/data/sources/helper/price.py
--rw-r--r--   0        0        0     7319 2023-06-30 02:50:03.543148 rubi-2.0.6/rubi/data/sources/helper/rolodex.py
--rw-r--r--   0        0        0    22425 2023-06-30 02:50:03.543454 rubi-2.0.6/rubi/data/sources/market.py
--rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.6/rubi/network/__init__.py
--rw-r--r--   0        0        0     7596 2023-06-30 02:50:06.556325 rubi-2.0.6/rubi/network/network.py
--rw-r--r--   0        0        0       66 2023-06-30 02:50:06.556396 rubi-2.0.6/rubi/rubicon_types/__init__.py
--rw-r--r--   0        0        0    15554 2023-06-30 22:38:54.825030 rubi-2.0.6/rubi/rubicon_types/order.py
--rw-r--r--   0        0        0     6305 2023-06-30 22:38:54.825201 rubi-2.0.6/rubi/rubicon_types/orderbook.py
--rw-r--r--   0        0        0     2776 2023-06-30 02:50:06.556913 rubi-2.0.6/rubi/rubicon_types/pair.py
--rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 rubi-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.7b1/LICENSE
+-rw-r--r--   0        0        0     2757 2023-06-01 22:20:20.359716 rubi-2.0.7b1/README.md
+-rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.0.7b1/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.0.7b1/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.0.7b1/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.0.7b1/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      721 2023-07-04 04:06:44.820395 rubi-2.0.7b1/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.0.7b1/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.0.7b1/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      745 2023-07-04 04:06:44.820830 rubi-2.0.7b1/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.0.7b1/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.0.7b1/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      648 2023-07-04 04:07:12.026104 rubi-2.0.7b1/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.0.7b1/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.0.7b1/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      721 2023-07-04 04:06:44.821665 rubi-2.0.7b1/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0      900 2023-07-04 04:09:57.055232 rubi-2.0.7b1/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-04 04:06:44.824417 rubi-2.0.7b1/rubi/__init__.py
+-rw-r--r--   0        0        0    27431 2023-07-04 04:06:47.229455 rubi-2.0.7b1/rubi/client.py
+-rw-r--r--   0        0        0      163 2023-06-30 02:50:06.554484 rubi-2.0.7b1/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.7b1/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    11860 2023-07-04 04:06:47.229669 rubi-2.0.7b1/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0       74 2023-07-04 04:06:47.229802 rubi-2.0.7b1/rubi/contracts/contract_types/__init__.py
+-rw-r--r--   0        0        0    15968 2023-06-30 02:50:06.555210 rubi-2.0.7b1/rubi/contracts/contract_types/events.py
+-rw-r--r--   0        0        0     2708 2023-07-04 04:06:47.229945 rubi-2.0.7b1/rubi/contracts/contract_types/transaction_reciept.py
+-rw-r--r--   0        0        0    18474 2023-07-04 04:06:47.230142 rubi-2.0.7b1/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24668 2023-07-04 04:06:47.230369 rubi-2.0.7b1/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14847 2023-06-30 02:50:06.556060 rubi-2.0.7b1/rubi/contracts/router.py
+-rw-r--r--   0        0        0       77 2023-07-04 04:06:44.826720 rubi-2.0.7b1/rubi/data/README.md
+-rw-r--r--   0        0        0       31 2023-07-04 04:06:44.827064 rubi-2.0.7b1/rubi/data/__init__.py
+-rw-r--r--   0        0        0    19848 2023-07-04 04:06:44.827426 rubi-2.0.7b1/rubi/data/market.py
+-rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.7b1/rubi/network/__init__.py
+-rw-r--r--   0        0        0     8052 2023-07-04 04:06:44.827822 rubi-2.0.7b1/rubi/network/network.py
+-rw-r--r--   0        0        0       66 2023-06-30 02:50:06.556396 rubi-2.0.7b1/rubi/rubicon_types/__init__.py
+-rw-r--r--   0        0        0    15554 2023-07-04 04:06:47.230559 rubi-2.0.7b1/rubi/rubicon_types/order.py
+-rw-r--r--   0        0        0     6305 2023-07-04 04:06:47.230678 rubi-2.0.7b1/rubi/rubicon_types/orderbook.py
+-rw-r--r--   0        0        0     2776 2023-06-30 02:50:06.556913 rubi-2.0.7b1/rubi/rubicon_types/pair.py
+-rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 rubi-2.0.7b1/PKG-INFO
```

### Comparing `rubi-2.0.6/LICENSE` & `rubi-2.0.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/README.md` & `rubi-2.0.7b1/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/network_config/ERC20.json` & `rubi-2.0.7b1/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/network_config/README.md` & `rubi-2.0.7b1/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/network_config/abitrum_goerli/abis/market.json` & `rubi-2.0.7b1/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/network_config/abitrum_goerli/abis/router.json` & `rubi-2.0.7b1/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/network_config/abitrum_goerli/network.yaml` & `rubi-2.0.7b1/network_config/abitrum_goerli/network.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 name: "Arbitrum Goerli"
 chain_id: 421613
 currency: "ETH"
 rpc_url: "https://goerli-rollup.arbitrum.io/rpc"
 explorer_url: "https://goerli-rollup-explorer.arbitrum.io"
+market_data_url: "https://api.rubicon.finance/subgraphs/name/RubiconV2_Arbitrum_Goerli"
 
 rubicon:
  market:
   address: "0x506407f25B746C39807c03A96DD595a6BE223211"
  router:
   address: "0x3AbA34a8C9616eA927225C045EEa5d5b51a7a6FC"
```

### Comparing `rubi-2.0.6/network_config/optimism/abis/market.json` & `rubi-2.0.7b1/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/network_config/optimism/abis/router.json` & `rubi-2.0.7b1/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/network_config/optimism/network.yaml` & `rubi-2.0.7b1/network_config/optimism/network.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 name: "Optimism"
 chain_id: 10
 currency: "ETH"
 rpc_url: "https://mainnet.optimism.io"
 explorer_url: "https://optimistic.etherscan.io/"
+market_data_url: "https://api.rubicon.finance/subgraphs/name/RubiconV2_Optimism_Mainnet_Dev"
 
 rubicon:
  market:
   address: "0x7a512d3609211e719737e82c7bb7271ec05da70d"
  router:
   address: "0x7Af14ADc8Aea70f063c7eA3B2C1AD0D7A59C4bFf"
 
 token_addresses:
  ETH: "0xDeadDeAddeAddEAddeadDEaDDEAdDeaDDeAD0000"
  WETH: "0x4200000000000000000000000000000000000006"
  WBTC: "0x68f180fcCe6836688e9084f035309E29Bf0A2095"
  OP: "0x4200000000000000000000000000000000000042"
  USDC: "0x7F5c764cBc14f9669B88837ca1490cCa17c31607"
  DAI: "0xDA10009cBd5D07dd0CeCc66161FC93D7c9000da1"
- USDT: "0x94b008aA00579c1307B0EF2c499aD98a8ce58e58"
+ USDT: "0x94b008aA00579c1307B0EF2c499aD98a8ce58e58"
```

### Comparing `rubi-2.0.6/network_config/optimism_goerli/abis/market.json` & `rubi-2.0.7b1/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/network_config/optimism_goerli/abis/router.json` & `rubi-2.0.7b1/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/network_config/optimism_goerli/network.yaml` & `rubi-2.0.7b1/network_config/optimism_goerli/network.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 name: "Optimism Goerli"
 chain_id: 420
 currency: "ETH"
 rpc_url: "https://goerli.optimism.io"
 explorer_url: "https://goerli-explorer.optimism.io/"
+market_data_url: "https://api.rubicon.finance/subgraphs/name/RubiconV2_Optimism_Goerli"
 
 rubicon:
  market:
   address: "0x9d0D6c259566d8161a1b2c513af0463992db38bc"
  router:
   address: "0x0a0795d7015aB52BcDd987975474bD73062B5494"
```

### Comparing `rubi-2.0.6/network_config/polygon_mumbai/abis/market.json` & `rubi-2.0.7b1/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/network_config/polygon_mumbai/abis/router.json` & `rubi-2.0.7b1/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/network_config/polygon_mumbai/network.yaml` & `rubi-2.0.7b1/network_config/polygon_mumbai/network.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 name: "Polygon Mumbai"
 chain_id: 80001
 currency: "MATIC"
 rpc_url: "https://rpc-mumbai.maticvigil.com/"
 explorer_url: "https://mumbai.polygonscan.com/"
+market_data_url: "https://api.thegraph.com/subgraphs/name/denverbaumgartner/rubiconv2-polygon-mumbai"
 
 rubicon:
  market:
   address: "0x10418D9e730fa659b0Baf0b640ee41FcF4EA2aaE"
  router:
   address: "0xbA81dF0251A017C2fB687e5469a897529442f008"
```

### Comparing `rubi-2.0.6/pyproject.toml` & `rubi-2.0.7b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.0.6"
+version = "2.0.7b1"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `rubi-2.0.6/rubi/client.py` & `rubi-2.0.7b1/rubi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     OrderEvent,
     Transaction,
     BaseNewOrder,
     NewCancelOrder,
     UpdateLimitOrder
 )
 
+from rubi.data import (
+    MarketData
+)
+
 
 class Client:
     """This class is a client for Rubicon. It aims to provide a simple and understandable interface when interacting
     with the Rubicon protocol. If not instantiated with a wallet and key then all the methods that require signing
     will throw an error.
 
     :param network: A Network instance
@@ -66,14 +70,16 @@
         self.market = RubiconMarket.from_network(network=self.network, wallet=self.wallet, key=self.key)
         self.router = RubiconRouter.from_network(network=self.network, wallet=self.wallet, key=self.key)
 
         self._pairs: Dict[str, Pair] = {}
 
         self.message_queue = message_queue  # type: Queue | None
 
+        self.market_data = MarketData.from_network(network=self.network)
+
     @classmethod
     def from_http_node_url(
         cls,
         http_node_url: str,
         custom_token_addresses_file: Optional[str] = None,
         message_queue: Optional[Queue] = None,
         wallet: Optional[Union[ChecksumAddress, str]] = None,
@@ -593,14 +599,38 @@
 
             order_ids.append(order.order_id)
 
         return self.market.batch_cancel(
             ids=order_ids,
             **transaction.args()
         )
+    
+    ######################################################################
+    # data methods (raw data) TODO: once we have cleanly formatted data functions, we can switch to only exposing those
+    ######################################################################
+
+    def get_offers(
+        self, 
+        maker: Optional[str] = None,
+        from_address: Optional[str] = None,
+        pair_name: Optional[str] = None,
+        book_side: Optional[OrderSide] = None,
+        pay_gem: Optional[str] = None,
+        buy_gem: Optional[str] = None,
+        open: Optional[bool] = None,
+        start_time: Optional[int] = None,
+        end_time: Optional[int] = None,
+        first: Optional[int] = 1000,
+        order_by: Optional[str] = 'timestamp',
+        order_direction: Optional[str] = 'desc',
+        formatted: Optional[bool] = True
+    ):
+        
+        df = self.market_data.get_offers(maker, from_address, pair_name, book_side, pay_gem, buy_gem, open, start_time, end_time, first, order_by, order_direction, formatted)
+        return df
 
     ######################################################################
     # helper methods
     ######################################################################
 
     # TODO: revisit as the safer thing is to set approval to 0 and then set approval to new_allowance
     #  or use increaseAllowance and decreaseAllowance but the current abi does not support these methods
```

### Comparing `rubi-2.0.6/rubi/contracts/aid.py` & `rubi-2.0.7b1/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/rubi/contracts/base_contract.py` & `rubi-2.0.7b1/rubi/contracts/base_contract.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/rubi/contracts/contract_types/events.py` & `rubi-2.0.7b1/rubi/contracts/contract_types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/rubi/contracts/contract_types/transaction_reciept.py` & `rubi-2.0.7b1/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/rubi/contracts/erc20.py` & `rubi-2.0.7b1/rubi/contracts/erc20.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,56 @@
         return cls.from_address_and_abi(
             w3=network.w3,
             address=network.token_addresses[name],
             contract_abi=abi,
             wallet=wallet,
             key=key
         )
+    
+    @classmethod
+    def from_address(
+        cls,
+        w3: Web3,
+        address: ChecksumAddress,
+        wallet: Optional[ChecksumAddress] = None,
+        key: Optional[str] = None
+    ) -> "ERC20":
+        """Create an ERC20 instance based on an address and a network connection.
+        
+        :param w3: Web3 instance.
+        :type w3: Web3
+        :param address: The address of the contract.
+        :type address: ChecksumAddress
+        :param wallet: Optional wallet address to use for interacting with the contract (optional, default is None).
+        :type wallet: Optional[ChecksumAddress]
+        :param key: Optional private key for the wallet (optional, default is None).
+        :type key: Optional[str]
+        :return: An ERC20 instance based on the address and network connection.
+        :rtype: ERC20
+        """
+
+        abi: ABI
+
+        try:
+            path = f"{os.path.dirname(os.path.abspath(__file__))}/../../network_config/ERC20.json"
+
+            with open(path) as f:
+                abi = json.load(f)
+
+        except FileNotFoundError:
+            raise Exception("ERC20.json abi not found. this file should in the network_config folder")
+        
+        return cls.from_address_and_abi(
+            w3=w3,
+            address=address,
+            contract_abi=abi,
+            wallet=wallet,
+            key=key
+        )
+
 
     ######################################################################
     # read calls
     ######################################################################
 
     # allowance(owner (address), spender (address)) -> uint256
     def allowance(self, owner: ChecksumAddress, spender: ChecksumAddress) -> int:
```

### Comparing `rubi-2.0.6/rubi/contracts/market.py` & `rubi-2.0.7b1/rubi/contracts/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/rubi/contracts/router.py` & `rubi-2.0.7b1/rubi/contracts/router.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/rubi/data/sources/aid.py` & `rubi-2.0.7b1/rubi/data/market.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,459 +1,426 @@
-#from helper import Gas
 import pandas as pd
-from .helper import Gas
+import logging as log
+from datetime import datetime
 from subgrounds import Subgrounds
+from subgrounds.subgraph import SyntheticField
 from subgrounds.pagination import ShallowStrategy
+from typing import Union, List, Optional, Dict, Type, Any, Callable
 
-from rubi.data.sources.helper import networks
-
-class AidData: 
-    """this class acts as the main access point to a variety of data and tooling for MarketAid.sol contracts.
-    the MarketAid.sol contracts are meant to be a hub for extended functionality for automated traders on the Rubicon protocol.
-    the end goal of this class, and this SDK by extension, is to act as a collaborative platform for the advancement of shared data tooling and analysis.
+from rubi.rubicon_types.order import (
+    OrderSide,
+)
+
+from rubi.network import (
+    Network,
+)
+
+from rubi.contracts import (
+    ERC20,
+)
+
+class MarketData: 
+    """This class represents the RubiconV2 Subgraph, which contains data primarily related to the RubiconMarket.sol contract.
+    If a Network object is not passed in instantiation then this class will only be used to query data related to the subgraph.
+    
+    :param subgrounds: a Subgrounds instance 
+    :type subgrounds: Subgrounds
+    param subgraph_url: a RubiconV2 Subgraph url endpoint that should be utilized for this class
+    :type subgraph_url: str
+    :param network: a Network object, native to the package
+    :type network: Network
     """
 
-    def __init__(self, subgrounds, chain_id):
-        """constructor method
-
-        :param subgrounds: the subgrounds object
-        :type subgrounds: subgrounds.Subgrounds
-        :param chain_id: the chain id of the network that is of interest
-        :type chain_id: int
-        """
-        self.network = networks[chain_id]()
-        self.subgrounds = subgrounds
-        self.market_aid = self.subgrounds.load_subgraph(self.network.market_aid)
+    def __init__(
+        self, 
+        subgrounds: Subgrounds,
+        subgraph_url: str,
+        network: Optional[Network] = None # we could just require a web3 connection, but this is more convenient 
+    ): 
+        """constructor method"""
+        self.sg = subgrounds
+        self.subgraph_url = subgraph_url
+        self.network = network # type: Network | None
+
+        # TODO: we probably won't do this here, but we should figure out where to store the token's for the class
+        self.tokens = self.get_network_tokens(self.network) if self.network else None
+
+        # create a token map that maps the token address (lowercase) to the token object
+        self.token_map = {token.address.lower(): token for token in self.tokens} if self.tokens else None
+
+        # initialize the subgraph 
+        try: 
+            self.data = self.sg.load_subgraph(self.subgraph_url)
+            # TODO: we should add a check here to guarantee the schema matches what we expect to be receiving
+        except: 
+            # TODO: not sure exactly what error we should be throwing here, this is if the url does not work 
+            raise ValueError(f"subgraph_url: {subgraph_url} failed when attempting to load.")
+        
+    @classmethod
+    def from_network(
+        cls,
+        network: Network
+    ) -> "MarketData": 
+        
+        """Initialize a MarketData object using a Network object."""
+        return cls(
+            subgrounds=network.subgrounds,
+            subgraph_url=network.market_data_url,
+            network=network
+        )
     
-    def get_aid_history(self, aid=None, asset=None, start_time=None, end_time=None, bin_size=60, first=1000000000):
-        """this method is used to get all of the asset history for a given aid. it tracks any change in asset balance on the market aid due to a transaction. currently, this is all supported through the event emittals on the market aid contract. any activity not recorded by a covered event will be missed...
+    #####################################
+    # General Helper Methods             # TODO: we will want to move this somewhere else most likely
+    #####################################
+
+    # TODO: FIGURE OUT WHERE THIS GOES, i think we probably want all of the token addresses initialized as a class object somewhere, but i also 
+    # think that when people start building extremely long token lists that we may not want to do this by default
+    # maybe it goes on the network object? or the client?
+
+    def get_network_tokens(
+            self, 
+            network: Optional[Network] = None 
+    ) -> List[ERC20] : # TODO: determine what type to return here, probably a list of ERC20 objects
         
-        :param aid: the address of the market aid that is of interest
-        :type aid: str
-        :param bin_size: the size of the time bins that are of interest, defaults to 60. this is actually not really used at the moment, so reach out if you have a use case for it
-        :type bin_size: int, optional
-        :param first: the number of transactions to return, defaults to 1000000000
-        :type first: int, optional
-        """
-        # TODO: we are going to need to extned the information we collect from the subgraph, and possibly modify the subgraph itself, in order to make sure we can account for deposits / withdrawals in any pnl calculation
-
-        AidToken = self.market_aid.AidToken
-        AidTokenHistory = self.market_aid.AidTokenHistory
-
-        AidTokenHistory.time_bin = (AidTokenHistory.timestamp // bin_size) * bin_size
-        AidTokenHistory.balance_formatted = AidTokenHistory.balance / 10 ** AidTokenHistory.aid_token.token.decimals
-        AidTokenHistory.balance_change_formatted = AidTokenHistory.balance_change / 10 ** AidTokenHistory.aid_token.token.decimals
-
-        where = {}
-        if aid: 
-            where['aid'] = aid.lower()
-        if asset:
-            where['aid_token_'] = {'token' : asset.lower()}
-        if start_time:
-            where['timestamp_gte'] = start_time
-        if end_time:
-            where['timestamp_lte'] = end_time
-
-        #histories = self.market_aid.Query.aidTokenHistories(first = first, where = [AidToken.aid == aid.lower()])
-        if where:
-            histories = self.market_aid.Query.aidTokenHistories(first = first, where = where)
-        else:
-            histories = self.market_aid.Query.aidTokenHistories(first = first)
-
-        field_paths = [
-            histories.timestamp,
-            histories.time_bin,
-            histories.aid_token.token.symbol,
-            histories.balance_formatted,
-            histories.balance_change_formatted,
-            histories.transaction.id,
-            histories.transaction.block,
-            histories.transaction.index,
-            histories.index,
-            histories.balance,
-            histories.balance_change,
-            histories.book_update
-        ]
-
-        df = self.subgrounds.query_df(field_paths, pagination_strategy=ShallowStrategy)
-
-        # rename the columns if the dataframe is not empty, else return an empty dataframe with the correct columns
-        column_name_mapping = {
-            'aidTokenHistories_timestamp' : 'timestamp',
-            'aidTokenHistories_time_bin' : 'time_bin',
-            'aidTokenHistories_aid_token_token_symbol' : 'asset',
-            'aidTokenHistories_balance_formatted' : 'balance',
-            'aidTokenHistories_balance_change_formatted' : 'balance_change',
-            'aidTokenHistories_transaction_id' : 'txn',
-            'aidTokenHistories_transaction_block' : 'block',
-            'aidTokenHistories_transaction_index' : 'block_index',
-            'aidTokenHistories_index' : 'index',
-            'aidTokenHistories_balance' : 'balance_raw',
-            'aidTokenHistories_balance_change' : 'balance_change_raw',
-            'aidTokenHistories_book_update' : 'book_update'
-        }
-
-        if df.empty:
-            return pd.DataFrame(columns=column_name_mapping.values())
+        """Returns a list of ERC20 objects for all tokens on the network."""
+        if network: 
+            token_addresses = network.token_addresses
+        elif self.network:
+            token_addresses = self.network.token_addresses
         else:
-            df = df.rename(columns=column_name_mapping)
-            df = df.sort_values(['block', 'block_index', 'index']).reset_index(drop=True)
-
-            #TODO: this should most likely be moved to a synthetic field going forward 
-            df['credits_debits'] = 0
-            df['credits_debits_raw'] = 0
-            mask = df['book_update'] == True
-            df.loc[mask, 'credits_debits'] = df.loc[mask, 'balance_change']
-            df.loc[mask, 'credits_debits_raw'] = df.loc[mask, 'balance_change_raw']
-            return df
-
-    # TODO: issue #19 dealing with filtering nested entities, that or modify the subgraph so that we can filter by timestamp
-    def get_aid_offers(self, aid=None, pair=None, pay_gem=None, buy_gem=None, start_time=None, end_time=None, first=1000000000):
-        # TODO: figure out if we want to filter by token symbol or token address, or both
-        # address is going to be network specific, but if we are losing the ability to use the symbol through the subgraph then we will need to change several things in the SDK :( 
-        """this method is used to get all of the offers for a given aid that have been tracked through the market aid subgraph. https://github.com/RubiconDeFi/rubi-subgraphs
-
-        # relevant issue: need to add filtering for pay_gem, buy_gem, start_time, end_time either through added functionality in subgrounds for nested filtering or through the underlying subgraph 
-        # i am currently hesistant to do much with expected changes that will occur to the subgraph schema that will necessitate changes here as well
-        # if you are reading this, we are moving to event only based subgraphs x0
-
-        :param aid: the address of the market aid that is of interest
-        :type aid: str
-        :param pay_gem: the address of the pay gem that is of interest
-        :type pay_gem: str
-        :param buy_gem: the address of the buy gem that is of interest
-        :type buy_gem: str
-        :param start_time: the start time of the time range that is of interest, defaults to None
-        :type start_time: int, optional
-        :param end_time: the end time of the time range that is of interest, defaults to None
-        :type end_time: int, optional
-        :param first: the number of offers to return, defaults to 1000000000
-        :type first: int, optional
-        """
+            raise ValueError("No network object passed and no network object initialized on the class.")
+        
+        tokens = [ERC20.from_network(name=address, network=self.network) for address in token_addresses]
 
-        Offer = self.market_aid.Offer
-        Offer.pay_amt_formatted = Offer.pay_amt / 10 ** Offer.pay_gem.decimals
-        Offer.buy_amt_formatted = Offer.buy_amt / 10 ** Offer.buy_gem.decimals
-        Offer.paid_amt_formatted = Offer.paid_amt / 10 ** Offer.pay_gem.decimals
-        Offer.bought_amt_formatted = Offer.bought_amt / 10 ** Offer.buy_gem.decimals
+        return tokens
     
-        where = {}
-        if aid:
-            where['maker'] = aid.lower()
-        if pay_gem:
-            where['pay_gem'] = pay_gem.lower()
-        if buy_gem:
-            where['buy_gem'] = buy_gem.lower()
-        if start_time:
-            where['transaction'] = {'timestamp_gte': start_time}
-        if end_time:
-            where['transaction'] = {'timestamp_lte': end_time}
+    def get_token(
+            self,
+            token_address: str
+    ) -> ERC20:
+        """Returns an ERC20 object for the token address passed from the token_map if it exists or add it to the token_map if it does not exist."""
+
+        if not self.network:
+            raise ValueError("No network object initialized on the class.")
+        else: 
+
+            try: 
+                token_address = self.network.w3.to_checksum_address(token_address)
+                token_address = token_address.lower()
+
+                if token_address not in self.token_map:
+                    self.token_map[token_address] = ERC20.from_network(address=token_address, network=self.network)
+                
+                return self.token_map[token_address]
 
-        if where:
-            offers = self.market_aid.Query.offers(first = first, where = where)
-        else:
-            offers = self.market_aid.Query.offers(first = first)
+            except:
+                raise ValueError(f"Token address: {token_address} is invalid.")
+    
+    #####################################
+    # Query Helper Methods              # # TODO: we will want to move these to their own class most likely
+    #####################################
+
+    # TODO: we will probably actually want to move this to the class constructor if it behaves as expected
+    def offer_entity(
+        self,  
+    ): # TODO: return a typed object (see subgrounds documentation for more info)
         
-        field_paths = [
-            offers.id,
-            offers.transaction.timestamp,
-            offers.removed_timestamp,
-            offers.pay_gem.symbol,
-            offers.pay_amt_formatted,
-            offers.paid_amt_formatted,
-            offers.buy_gem.symbol,
-            offers.buy_amt_formatted,
-            offers.bought_amt_formatted,
-            offers.pay_gem.id,
-            offers.buy_gem.id,
-            offers.live
-        ]
+        Offer = self.data.Offer
 
-        df = self.subgrounds.query_df(field_paths, pagination_strategy=ShallowStrategy)
+        # if we have a network object we can get all the token information we need
+        if self.network: 
 
-        return df
-
-    def get_aid_txns(self, aid=None, start_time=None, end_time=None, first=1000000000): 
-        """this method is used to get all of the transactions for a given aid that have been tracked through the market aid subgraph. https://github.com/RubiconDeFi/rubi-subgraphs
+            Offer.pay_amt_formatted = SyntheticField(
+                f=lambda pay_amt, pay_gem: self.get_token(pay_gem).to_decimal(pay_amt),
+                type_=SyntheticField.FLOAT,
+                deps=[Offer.pay_amt, Offer.pay_gem],
+            )
+
+            Offer.buy_amt_formatted = SyntheticField(
+                f=lambda buy_amt, buy_gem: self.get_token(buy_gem).to_decimal(buy_amt),
+                type_=SyntheticField.FLOAT,
+                deps=[Offer.buy_amt, Offer.buy_gem],
+            )
+
+            Offer.paid_amt_formatted = SyntheticField(
+                f=lambda paid_amt, pay_gem: self.get_token(pay_gem).to_decimal(paid_amt),
+                type_=SyntheticField.FLOAT,
+                deps=[Offer.paid_amt, Offer.pay_gem],
+            )
+
+            Offer.bought_amt_formatted = SyntheticField(
+                f=lambda bought_amt, buy_gem: self.get_token(buy_gem).to_decimal(bought_amt),
+                type_=SyntheticField.FLOAT,
+                deps=[Offer.bought_amt, Offer.buy_gem],
+            )
+
+            Offer.pay_gem_symbol = SyntheticField(
+                f=lambda pay_gem: self.get_token(pay_gem).symbol,
+                type_=SyntheticField.STRING,
+                deps=[Offer.pay_gem],
+            )
+
+            Offer.buy_gem_symbol = SyntheticField(
+                f=lambda buy_gem: self.get_token(buy_gem).symbol,
+                type_=SyntheticField.STRING,
+                deps=[Offer.buy_gem],
+            )
+
+            Offer.datetime = SyntheticField(
+                f=lambda timestamp: str(datetime.fromtimestamp(timestamp)),
+                type_=SyntheticField.STRING,
+                deps=[Offer.timestamp],
+            )
         
-        :param aid: the address of the market aid that is of interest, defaults to None
-        :type aid: str, optional
-        :param start_time: the start time of the time range that is of interest, defaults to None
-        :type start_time: int, optional
-        :param end_time: the end time of the time range that is of interest, defaults to None
-        :type end_time: int, optional
-        :param first: the number of transactions to return, defaults to 1000000000
-        :type first: int, optional
-        """
-
-        Transaction = self.market_aid.Transaction
-
-        where = []
-        if aid:
-            where.append(Transaction.aid == aid)
-        if start_time:
-            where.append(Transaction.timestamp >= start_time)
-        if end_time:
-            where.append(Transaction.timestamp <= end_time)
-
-        if where == []:
-            txns = self.market_aid.Query.transactions(first=first)
-        else:
-            txns = self.market_aid.Query.transactions(first=first, where=where)
-
-        field_paths = [
-            txns.id,
-            txns.timestamp,
-            txns.aid.id
-        ]
+        return Offer
 
-        df = self.subgrounds.query_df(field_paths, pagination_strategy=ShallowStrategy)
-
-        return df
-
-    def get_book_updates(self, aid=None, asset=None, start_time=None, end_time=None, first=1000000000):
-        """this method is used to get all of the book updates for a given aid that have been tracked through the market aid subgraph.
+    def offers_query(
+        self,
+        offer, # TODO: determine what type this should be (subgrounds may have types that we can utilize here)
+        order_by: str, 
+        order_direction: str,
+        first: int,
+        maker: Optional[str] = None,
+        from_address: Optional[str] = None,
+        pay_gem: Optional[str] = None, 
+        buy_gem: Optional[str] = None, 
+        open: Optional[bool] = None,
+        start_time: Optional[int] = None,
+        end_time: Optional[int] = None,
+        # TODO: there is definitely a clear way to pass these parameters in a more concise way, prolly **kargs   
+    ): # TODO: return a typed object (see subgrounds documentation for more info)
         
-        :param aid: the address of the market aid that is of interest, defaults to None
-        :type aid: str, optional
-        :param asset: the address of the asset that is of interest, defaults to None
-        :type asset: str, optional
-        :param start_time: the start time of the time range that is of interest, defaults to None
-        :type start_time: int, optional
-        :param end_time: the end time of the time range that is of interest, defaults to None
-        :type end_time: int, optional
-        :param first: the number of book updates to return, defaults to 1000000000
-        :type first: int, optional
-        :return: a dataframe containing the book updates
-        :rtype: pandas.DataFrame
-        """
-
-        BookUpdate = self.market_aid.BookUpdate
-        BookUpdate.amount_formatted = BookUpdate.amount / 10 ** BookUpdate.aid_token.token.decimals
-
-        where = []
-        if aid:
-            where.append(BookUpdate.aid == aid.lower())
-        #if asset:
-        #    where.append(BookUpdate.asset == asset)
-        if start_time:
-            where.append(BookUpdate.timestamp >= start_time)
-        if end_time:
-            where.append(BookUpdate.timestamp <= end_time)
-
-        if where == []:
-            book_updates = self.market_aid.Query.bookUpdates(first=first)
-        else:
-            book_updates = self.market_aid.Query.bookUpdates(first=first, where=where)
-
-        field_paths = [
-            book_updates.timestamp,
-            book_updates.aid.id,
-            book_updates.aid_token.token.symbol,
-            book_updates.amount,
-            book_updates.amount_formatted,
-            book_updates.transaction.id,
-            book_updates.transaction.block,
-            book_updates.transaction.index,
-            book_updates.index
-        ]
-
-        df = self.subgrounds.query_df(field_paths, pagination_strategy=ShallowStrategy)
+        # determine that the parameters are valid
+        error_messages = []
 
-        # rename the columns: timestamp, aid, asset, txn, amount, amount_formatted
-        column_name_mapping = {
-            'bookUpdates_timestamp': 'timestamp',
-            'bookUpdates_aid_id': 'aid',
-            'bookUpdates_aid_token_token_symbol': 'asset',
-            'bookUpdates_amount': 'amount',
-            'bookUpdates_amount_formatted': 'amount_formatted',
-            'bookUpdates_transaction_id': 'txn',
-            'bookUpdates_transaction_block': 'block',
-            'bookUpdates_transaction_index': 'block_index',
-            'bookUpdates_index': 'index'
-        }
-
-        if df.empty:
-            df = pd.DataFrame(columns=column_name_mapping.values())
+        # check the order_by parameter
+        if order_by.lower() not in ('timestamp', 'price'):
+            error_messages.append("Invalid order_by, must be 'timestamp' or 'price' (default: timestamp)")
+        elif order_by.lower() == 'timestamp':
+            order_by = offer.timestamp
+        elif order_by.lower() == 'price':
+            order_by = offer.price
+        
+        # check the order_direction parameter
+        if order_direction.lower() not in ('asc', 'desc'):
+            error_messages.append("Invalid order_direction, must be 'asc' or 'desc' (default: desc)")
         else:
-            df = df.rename(columns=column_name_mapping)
-            df = df.sort_values(by=['timestamp', 'index']).reset_index(drop=True)
-
-        return df
+            order_direction = order_direction.lower()
 
-    def get_aid_balances(self, aid=None, asset=None, first=1000000000):
-        """ a function to query the subgraph and get the most recent balances for a given aid and the tokens it trades with. 
+        # check the first parameter
+        if first < 1:
+            error_messages.append("Invalid first, must be greater than 0 (default: 1000)")
+        if not isinstance(first, int):
+            error_messages.append("Invalid first, must be an integer (default: 1000)")
         
-        :param aid: the address of the market aid that is of interest, defaults to None
-        :type aid: str, optional
-        :param first: the number of balances to return, defaults to 1000000000
-        :type first: int, optional
-        :return: a dataframe containing the balances
-        :rtype: pandas.DataFrame
-        """
-
-        aidToken = self.market_aid.AidToken
-        aidToken.balance_formatted = aidToken.balance / 10 ** aidToken.token.decimals
-
-        where = []
-        if aid:
-            where.append(aidToken.aid == aid.lower())
-        #if asset:
-        #    where.append(aidToken.token == asset)
-
-        if where == []:
-            aid_tokens = self.market_aid.Query.aidTokens(first=first)
-        else:
-            aid_tokens = self.market_aid.Query.aidTokens(first=first, where=where)
+        # raise an error if there are any
+        if error_messages:
+            raise ValueError('\n'.join(error_messages))
         
-        field_paths = [
-            aid_tokens.token.symbol,
-            aid_tokens.balance,
-            aid_tokens.balance_formatted,
+        # build the list of where conditions
+        where = [
+            offer.maker == maker.lower() if maker else None,
+            offer.from_address == from_address.lower() if from_address else None,
+            offer.pay_gem == pay_gem.lower() if pay_gem else None,
+            offer.buy_gem == buy_gem.lower() if buy_gem else None,
+            offer.open == open if open is not None else None,
+            offer.timestamp >= start_time if start_time else None,
+            offer.timestamp <= end_time if end_time else None
         ]
+        where = [condition for condition in where if condition is not None]
+    
+        """Helper method to build a query for the offers subgraph entity."""
+        offers = self.data.Query.offers(
+            orderBy = order_by,
+            orderDirection = order_direction,
+            first=first,
+            where = where if where else {}
+        )
 
-        df = self.subgrounds.query_df(field_paths, pagination_strategy=ShallowStrategy)
-
-        # rename the columns: asset, balance, balance_formatted
-        column_name_mapping = {
-            'aidTokens_token_symbol': 'asset',
-            'aidTokens_balance': 'balance',
-            'aidTokens_balance_formatted': 'balance_formatted'
-        }
-
-        df = df.rename(columns=column_name_mapping)
-
-        return df
+        return offers
     
-    def get_aid_arbs(self, aid=None, asset=None, quote=None, start_time=None, end_time=None, first=1000000000):
-        """ this method is intended to query arbitrage trades that occured on the market aid subgraph 
-        
-        :param aid: the address of the market aid that is of interest, defaults to None
-        :type aid: str, optional
-        :param asset: the address of the asset that is of interest, defaults to None
-        :type asset: str, optional
-        :param quote: the address of the quote asset that is of interest, defaults to None
-        :type quote: str, optional
-        :param start_time: the start time of the time range that is of interest, defaults to None
-        :type start_time: int, optional
-        :param end_time: the end time of the time range that is of interest, defaults to None
-        :type end_time: int, optional
-        :param first: the number of arbs to return, defaults to 1000000000
-        :type first: int, optional
-        :return: a dataframe containing the arbs
-        :rtype: pandas.DataFrame
+    def offers_fields(
+        self,
+        offers: Any, # TODO: check that this is the correct type (subgrounds may have types that we can utilize here)
+        formatted: bool = False
+    ): # TODO: return a typed object (see subgrounds documentation for more info)
         
-        """
-
-        Arb = self.market_aid.Arb
-        #Arb.amount_formatted = Arb.amount / 10 ** Arb.asset.decimals
-        Arb.profit_formatted = Arb.profit / 10 ** Arb.asset.decimals
-
-        where = []
-        if aid:
-            where.append(Arb.aid == aid.lower())
-        if asset:
-            where.append(Arb.asset == asset.lower())
-        if quote:
-            where.append(Arb.quote == quote.lower())
-        if start_time:
-            where.append(Arb.timestamp >= start_time)
-        if end_time:
-            where.append(Arb.timestamp <= end_time)
-
-        if where == []:
-            arbs = self.market_aid.Query.arbs(first=first)
-        else:
-            arbs = self.market_aid.Query.arbs(first=first, where=where)
-
-        field_paths = [
-            arbs.timestamp,
-            arbs.aid.id,
-            arbs.asset.symbol,
-            arbs.quote.symbol,
-            arbs.amount,
-            arbs.profit,
-            arbs.profit_formatted
+        """Helper method to build a list of fields for the offers subgraph entity."""
+        fields = [
+            offers.id,
+            offers.timestamp,
+            offers.index,
+            offers.maker.id,
+            offers.from_address.id,
+            offers.pay_gem,
+            offers.buy_gem,
+            offers.pay_amt,
+            offers.buy_amt,
+            offers.paid_amt,
+            offers.bought_amt,
+            offers.price,
+            offers.open,
+            offers.removed_timestamp,
+            offers.removed_block,
+            offers.transaction.id,
+            offers.transaction.block_number,
+            offers.transaction.block_index
         ]
 
-        df = self.subgrounds.query_df(field_paths, pagination_strategy=ShallowStrategy)
-
-        # if the dataframe is empty, return an empty dataframe with the correct column names
-        if df.empty:
-            df = pd.DataFrame(columns=['timestamp', 'aid', 'asset', 'quote', 'amount', 'profit', 'profit_formatted'])
-            return df
+        if formatted:
+            fields.append(offers.pay_amt_formatted)
+            fields.append(offers.buy_amt_formatted)
+            fields.append(offers.paid_amt_formatted)
+            fields.append(offers.bought_amt_formatted)
+            fields.append(offers.pay_gem_symbol)
+            fields.append(offers.buy_gem_symbol)
+            fields.append(offers.datetime)
 
-        # rename the columns: timestamp, aid, asset, quote, amount, profit, profit_formatted
-        column_name_mapping = {
-            'arbs_timestamp': 'timestamp',
-            'arbs_aid_id': 'aid',
-            'arbs_asset_symbol': 'asset',
-            'arbs_quote_symbol': 'quote',
-            'arbs_amount': 'amount',
-            'arbs_profit': 'profit',
-            'arbs_profit_formatted': 'profit_formatted'
-        }
-
-        df = df.rename(columns=column_name_mapping)
-
-        return df
-
-    #def get_external_swaps()
-
-class SuperAidData(AidData): 
-    """this class acts as an extension of the AidData class and has some additional functionality that is enabled by a node connection. 
-    """
-
-    def __init__(self, w3, subgrounds, chain_id):
-        """a super class of the AidData class that has additional functionality enabled by a node connection.
-
-        :param w3: a web3 object
-        :type w3: web3.main.Web3
-        :param subgrounds: the subgrounds object
-        :type subgrounds: subgrounds.Subgrounds
-        :param chain_id: the chain id of the network that is of interest
-        :type chain_id: int
-        """
-        super().__init__(subgrounds, chain_id)
-
-        # set class variables
-        self.w3 = w3
-        self.gas = Gas(self.w3)
+        return fields
     
-    def get_aid_txns_gas_data(self, aid=None, start_time=None, end_time=None, total_fee_eth=True, total_fee_usd=True, l2_gas_price=None, l2_gas_used=None, l1_gas_used=None, 
-        l1_gas_price=None, l1_fee_scalar=None, l1_fee=None, l2_fee=None, total_fee=None, l1_fee_eth=None, l2_fee_eth=None, eth_price=None, l1_fee_usd=None, l2_fee_usd=None, first=1000000000):
-
-        # get the transactions for the market aid contract
-        txns = self.get_aid_txns(aid, start_time, end_time, first)
+    def query_offers(
+            self,
+            fields: List, 
+            formatted: bool = False,
+            # TOOD: maybe we give the user the option to define a custom pagination strategy?
+    ): # TODO: return a typed object (see subgrounds documentation for more info)
+        """Helper method to query the offers subgraph entity."""
+        df =  self.sg.query_df(
+            fields,
+            pagination_strategy=ShallowStrategy
+        ) 
+
+        # if the dataframe is empty, return an empty dataframe with the correct columns
+        if df.empty and not formatted:
+            cols = ['id', 'timestamp', 'index', 'maker', 'from_address', 'pay_gem',
+                'buy_gem', 'pay_amt', 'buy_amt', 'paid_amt', 'bought_amt', 'price',
+                'open', 'removed_timestamp', 'removed_block', 'transaction', 
+                'transaction_block_number', 'transaction_block_index']
+            df = pd.DataFrame(columns=cols)
+
+        elif df.empty and formatted:
+            cols = ['id', 'maker', 'from_address', 'pay_gem', 'buy_gem', 'pay_amt', 'buy_amt', 'paid_amt', 'bought_amt']
+            df = pd.DataFrame(columns=cols)
+        
+        else: 
+            df.columns = [col.replace('offers_', '') for col in df.columns]
+            df.columns = [col.replace('_id', '') for col in df.columns]
+            
+            # convert the id to an integer
+            df['id'] = df['id'].apply(lambda x: int(x, 16)) # TODO: i don't love the lambda (cc pickling, but it appears we are forced to use them in sythetic fields regardless)
+
+            # TODO: decide whether we should return the unformatted fields or not
+            if formatted:
+                print('the formmatkalkakdklj')
+                df = df.drop(columns=['pay_amt', 'buy_amt', 'paid_amt', 'bought_amt', 'pay_gem', 'buy_gem', 'timestamp', 'index', 'price', 'removed_timestamp', 'removed_block', 'transaction_block_number', 'transaction_block_index'])
+                df = df.rename(columns={'pay_amt_formatted': 'pay_amt', 'buy_amt_formatted': 'buy_amt', 'paid_amt_formatted': 'paid_amt', 'bought_amt_formatted': 'bought_amt', 'pay_gem_symbol': 'pay_gem', 'buy_gem_symbol': 'buy_gem', 'datetime': 'timestamp'})
+                # TODO: we could also get smart with displaying price dependent upon the pair_name and direction of the order
+            
+        # TODO: apply any data type conversions to the dataframe - possibly converting unformatted values to integers   
+        return df
     
-        # update the dataframe to contain the relevant gas data
-        df = self.gas.txn_dataframe_update(txns, 'transactions_id', 'transactions_timestamp', total_fee_eth = total_fee_eth, total_fee_usd = total_fee_usd, l2_gas_price = l2_gas_price, l2_gas_used = l2_gas_used, l1_gas_used = l1_gas_used, l1_gas_price = l1_gas_price, l1_fee_scalar = l1_fee_scalar, l1_fee = l1_fee, l2_fee = l2_fee, total_fee = total_fee, l1_fee_eth = l1_fee_eth, l2_fee_eth = l2_fee_eth, eth_price = eth_price, l1_fee_usd = l1_fee_usd, l2_fee_usd = l2_fee_usd)
-
-        return df 
-
-    def get_aid_gas_spend_binned(self, aid=None, start_time=None, end_time=None, granularity=60, type = 'USD', total_fee_eth=True, total_fee_usd=True, l2_gas_price=None, l2_gas_used=None, l1_gas_used=None, 
-        l1_gas_price=None, l1_fee_scalar=None, l1_fee=None, l2_fee=None, total_fee=None, l1_fee_eth=None, l2_fee_eth=None, eth_price=None, l1_fee_usd=None, l2_fee_usd=None, first=1000000000):
-        """this function takes in a market aid address, start time, end time, and granularity in order to return a dictionary of the gas spend dictionary that is binned by the granularity.
-        this dictionary is a key-pair mapping of the time bin (start of a minute, hour, day, etc) to the gas spend of the contract during that period.
+    #####################################
+    # Subgraph Query Methods (raw data) #
+    #####################################
+
+    # TODO: refractor using a decorator to handle the parameter validation
+    def get_offers(
+        self, 
+        maker: Optional[str] = None,
+        from_address: Optional[str] = None,
+        pair_name: Optional[str] = None,
+        book_side: Optional[OrderSide] = None,
+        pay_gem: Optional[str] = None, # TODO: maybe we should allow the user to pass in an address here?
+        buy_gem: Optional[str] = None, # TODO: maybe we should allow the user to pass in an address here?
+        open: Optional[bool] = None,
+        start_time: Optional[int] = None,
+        end_time: Optional[int] = None,
+        first: Optional[int] = 1000,
+        order_by: Optional[str] = 'timestamp',
+        order_direction: Optional[str] = 'desc',
+        formatted: Optional[bool] = False
+        ) -> pd.DataFrame: 
+        """Returns a dataframe of offers placed on the market contract, with the option to pass in filters.
+
+        :param maker: the address of the maker of the offer
+        :type maker: str
+        :param from_address: the address that originated the transaction that created the offer
+        :type from_address: str
+        :param pay_gem: the address of the token that the maker is offering (will override pair_name if both are passed)
+        :type pay_gem: str
+        :param buy_gem: the address of the token that the maker is requesting (will override pair_name if both are passed)
+        :type buy_gem: str
+        :param open: whether or not the offer is still active
+        :type open: bool
+        :param start_time: the timestamp of the earliest offer to return
+        :type start_time: int
+        :param end_time: the timestamp of the latest offer to return
+        :type end_time: int
+        :param first: the number of offers to return
+        :type first: int
+        :param order_by: the field to order the offers by (default: timestamp, options: timestamp, price) TODO: expand this list
+        :type order_by: str
+        :param order_direction: the direction to order the offers by (default: desc, options: asc, desc)
+        :type order_direction: str
+        :param formatted: whether or not to return the formatted fields (default: False, requires a network object to be passed)
+        :return: a dataframe of offers placed on the market contract
+        :rtype: pd.DataFrame 
         """
 
-        if start_time: 
-            start_time = int(start_time)
-        if end_time:
-            end_time = int(end_time)
-
-        gas_spend = self.get_aid_txns_gas_data(aid, start_time, end_time, total_fee_eth, total_fee_usd, l2_gas_price, l2_gas_used, l1_gas_used, l1_gas_price, l1_fee_scalar, l1_fee, l2_fee, total_fee, l1_fee_eth, l2_fee_eth, eth_price, l1_fee_usd, l2_fee_usd, first)
+        # set the offer entity 
+        Offer = self.offer_entity()
 
-        # bin the data
-        gas_spend['time_bin'] = gas_spend['transactions_timestamp'].apply(lambda x: (x // granularity) * granularity)
-
-        # group by time_bin and get the aggregate gas spend during the period represented as a dictionary with time_bin as the key and the gas spend as the value
-        grouped = gas_spend.groupby(['time_bin'])
-
-        if type == 'USD':
-            gas_spend = grouped['total_fee_usd'].sum().to_dict()
-
-        if type == 'ETH':
-            gas_spend = grouped['total_fee_eth'].sum().to_dict()
-
-        return gas_spend
+        # if we want formatted fields, make sure we have a network object
+        # TODO: we could pass this to the offers_query method and handle it there - if we start to utilize something like **kargs lets do that
+        if formatted and not self.network:
+            raise ValueError("Cannot return formatted fields without a network object initialized on the class.")
+
+        # handle the pair_name parameter
+        if pair_name:
+            base, quote = pair_name.split("/")
+            base_asset = ERC20.from_network(name=base, network=self.network)
+            quote_asset = ERC20.from_network(name=quote, network=self.network)
+
+        # handle the book_side parameter
+        if book_side and pair_name:
+            
+            match book_side:
+                case OrderSide.BUY:
+                    buy_query = self.offers_query(Offer, order_by, order_direction, first, maker, from_address, pay_gem = quote_asset.address, buy_gem = base_asset.address, open = open, start_time = start_time, end_time = end_time)
+                    buy_fields = self.offers_fields(buy_query, formatted)
+                    buy_df = self.query_offers(buy_fields, formatted)
+                    buy_df['side'] = 'buy' # TODO: we could also pass this data to the offers_query method and handle it there, could help with price
+
+                    return buy_df
+
+                case OrderSide.SELL:
+                    sell_query = self.offers_query(Offer, order_by, order_direction, first, maker, from_address, pay_gem = base_asset.address, buy_gem = quote_asset.address, open = open, start_time = start_time, end_time = end_time)
+                    sell_fields = self.offers_fields(sell_query, formatted)
+                    sell_df = self.query_offers(sell_fields, formatted)
+                    sell_df['side'] = 'sell' # TODO: we could also pass this data to the offers_query method and handle it there, could help with price
+
+                    return sell_df
+
+                case OrderSide.NEUTRAL:
+                    buy_query = self.offers_query(Offer, order_by, order_direction, first, maker, from_address, pay_gem = quote_asset.address, buy_gem = base_asset.address, open = open, start_time = start_time, end_time = end_time)
+                    buy_fields = self.offers_fields(buy_query, formatted)
+                    buy_df = self.query_offers(buy_fields, formatted)
+                    buy_df['side'] = 'buy' # TODO: we could also pass this data to the offers_query method and handle it there, could help with price
+
+                    sell_query = self.offers_query(Offer, order_by, order_direction, first, maker, from_address, pay_gem = base_asset.address, buy_gem = quote_asset.address, open = open, start_time = start_time, end_time = end_time)
+                    sell_fields = self.offers_fields(sell_query, formatted)
+                    sell_df = self.query_offers(sell_fields, formatted)
+                    sell_df['side'] = 'sell' # TODO: we could also pass this data to the offers_query method and handle it there, could help with price
+
+                    # TODO: decide what we want to do here, maybe we just return both dataframes?
+
+                    # reset the index  # need to pass a somewhat more complicated ordering here to comply with what happened in the same block time
+                    return pd.concat([buy_df, sell_df]).reset_index(drop=True)
+
+        # handle the pay_gem and buy_gem parameters
+        elif pay_gem and buy_gem:
+
+            query = self.offers_query(Offer, order_by, order_direction, first, maker, from_address, pay_gem = pay_gem, buy_gem = buy_gem, open = open, start_time = start_time, end_time = end_time)
+            fields = self.offers_fields(query)
+            df = self.query_offers(fields)
 
+            return df
```

### Comparing `rubi-2.0.6/rubi/network/network.py` & `rubi-2.0.7b1/rubi/network/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 from enum import Enum
 from typing import Optional
 
 import yaml
 from eth_typing import ChecksumAddress
 from web3 import Web3
+from subgrounds import Subgrounds
 
 
 class NetworkId(Enum):
     # MAINNET
     OPTIMISM = 10
 
     # TESTNET
@@ -23,20 +24,22 @@
     provides and easy way to configure a client or contracts.
     """
 
     def __init__(
         self,
         path: str,
         w3: Web3,
+        subgrounds: Subgrounds, 
         # The below all come from network_config/{network_name}/network.yaml
         name: str,
         chain_id: int,
         currency: str,
         rpc_url: str,
         explorer_url: str,
+        market_data_url: str,
         rubicon: dict,
         token_addresses: dict,
         # optional custom token config file from the user
         custom_token_addresses_file: Optional[str] = None
     ):
         """Initializes a Network instance.
 
@@ -50,30 +53,34 @@
         :type chain_id: int
         :param currency: The base currency of the network.
         :type currency: str
         :param rpc_url: The RPC URL of the network.
         :type rpc_url: str
         :param explorer_url: The URL of the network explorer.
         :type explorer_url: str
+        :param market_data_url: the URL of the market data subgraph (RubiconV2)
         :param rubicon: Dictionary containing Rubicon contract parameters.
         :type rubicon: dict
         :param token_addresses: Dictionary containing token addresses on the network.
         :type token_addresses: dict
         :param custom_token_addresses_file: The name of a yaml file (relative to the current working directory) with
             custom token addresses. Overwrites the token config found in network_config/{chain}/network.yaml.
             (optional, default is None).
         :type custom_token_addresses_file: Optional[str]
         """
         self.name = name
         self.chain_id = chain_id
         self.w3 = w3
+        self.subgrounds = subgrounds
 
         self.currency = currency
         self.rpc_url = rpc_url
         self.explorer_url = explorer_url
+        # TODO: currently we are utilizing just a single url, we should switch to a dictionary as the number of subgraphs we support grows
+        self.market_data_url = market_data_url
         self.rubicon = RubiconContracts(path=path, w3=self.w3, **rubicon)
 
         checksummed_token_addresses: dict[str, ChecksumAddress] = {}
         for k, v in token_addresses.items():
             checksummed_token_addresses[k] = self.w3.to_checksum_address(v)
 
         if custom_token_addresses_file:
@@ -108,23 +115,24 @@
             (optional, default is None).
         :type custom_token_addresses_file: Optional[str]
         :return: A Network instance based on the network configuration.
         :rtype: Network
         :raises Exception: If no network configuration file is found for the specified network name.
         """
         w3 = Web3(Web3.HTTPProvider(http_node_url))
+        subgrounds = Subgrounds()
 
         network_name = NetworkId(w3.eth.chain_id).name.lower()
 
         try:
             path = f"{os.path.dirname(os.path.abspath(__file__))}/../../network_config/{network_name}"
 
             with open(f"{path}/network.yaml") as f:
                 network_data = yaml.safe_load(f)
-                return cls(path=path, w3=w3, custom_token_addresses_file=custom_token_addresses_file, **network_data)
+                return cls(path=path, w3=w3, subgrounds=subgrounds,custom_token_addresses_file=custom_token_addresses_file, **network_data)
         except FileNotFoundError:
             raise Exception(f"no network config found for {network_name}, there should be a corresponding folder in "
                             f"the network_config directory")
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
```

### Comparing `rubi-2.0.6/rubi/rubicon_types/order.py` & `rubi-2.0.7b1/rubi/rubicon_types/order.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/rubi/rubicon_types/orderbook.py` & `rubi-2.0.7b1/rubi/rubicon_types/orderbook.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/rubi/rubicon_types/pair.py` & `rubi-2.0.7b1/rubi/rubicon_types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.6/PKG-INFO` & `rubi-2.0.7b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.0.6
+Version: 2.0.7b1
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

