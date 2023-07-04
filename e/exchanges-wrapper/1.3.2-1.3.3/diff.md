# Comparing `tmp/exchanges_wrapper-1.3.2.tar.gz` & `tmp/exchanges_wrapper-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchanges_wrapper-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "exchanges_wrapper-1.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `exchanges_wrapper-1.3.2.tar` & `exchanges_wrapper-1.3.3.tar`

### file list

```diff
@@ -1,22 +1,20 @@
--rw-r--r--   0        0        0     1114 2023-06-29 17:23:13.074875 exchanges_wrapper-1.3.2/LICENSE.md
--rw-r--r--   0        0        0     7142 2023-06-29 17:23:13.074875 exchanges_wrapper-1.3.2/README.md
--rw-r--r--   0        0        0     1317 2023-06-29 17:23:13.074875 exchanges_wrapper-1.3.2/exchanges_wrapper/__init__.py
--rw-r--r--   0        0        0    45215 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/api_pb2.py
--rw-r--r--   0        0        0    44445 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/api_pb2_grpc.py
--rw-r--r--   0        0        0    19618 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/bitfinex_parser.py
--rw-r--r--   0        0        0     6184 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/c_structures.py
--rw-r--r--   0        0        0    62117 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/client.py
--rw-r--r--   0        0        0     2768 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/definitions.py
--rw-r--r--   0        0        0      796 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/errors.py
--rw-r--r--   0        0        0    12494 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/events.py
--rwxr-xr-x   0        0        0    48580 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/exch_srv.py
--rw-r--r--   0        0        0     4429 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/exch_srv_cfg.toml.template
--rw-r--r--   0        0        0    10270 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/http_client.py
--rw-r--r--   0        0        0    15723 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/huobi_parser.py
--rw-r--r--   0        0        0    16098 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/okx_parser.py
--rw-r--r--   0        0        0    12097 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/proto/exchanges_wrapper/api.proto
--rw-r--r--   0        0        0    22397 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/web_sockets.py
--rw-r--r--   0        0        0      612 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/ws_api/__init__.py
--rw-r--r--   0        0        0     8315 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/exchanges_wrapper/ws_api/ws_session.py
--rw-r--r--   0        0        0     1147 2023-06-29 17:23:13.078875 exchanges_wrapper-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     8054 1970-01-01 00:00:00.000000 exchanges_wrapper-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1114 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/LICENSE.md
+-rw-r--r--   0        0        0     7142 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/README.md
+-rw-r--r--   0        0        0     1317 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/exchanges_wrapper/__init__.py
+-rw-r--r--   0        0        0    45215 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/exchanges_wrapper/api_pb2.py
+-rw-r--r--   0        0        0    44445 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/exchanges_wrapper/api_pb2_grpc.py
+-rw-r--r--   0        0        0    19609 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/exchanges_wrapper/bitfinex_parser.py
+-rw-r--r--   0        0        0     6184 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/exchanges_wrapper/c_structures.py
+-rw-r--r--   0        0        0    62056 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/exchanges_wrapper/client.py
+-rw-r--r--   0        0        0     2768 2023-07-04 16:51:46.630457 exchanges_wrapper-1.3.3/exchanges_wrapper/definitions.py
+-rw-r--r--   0        0        0      796 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/errors.py
+-rw-r--r--   0        0        0    12485 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/events.py
+-rwxr-xr-x   0        0        0    47721 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/exch_srv.py
+-rw-r--r--   0        0        0     4429 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/exch_srv_cfg.toml.template
+-rw-r--r--   0        0        0    10260 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/http_client.py
+-rw-r--r--   0        0        0    15714 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/huobi_parser.py
+-rw-r--r--   0        0        0    16089 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/okx_parser.py
+-rw-r--r--   0        0        0    12097 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/proto/exchanges_wrapper/api.proto
+-rw-r--r--   0        0        0    22397 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/exchanges_wrapper/web_sockets.py
+-rw-r--r--   0        0        0     1175 2023-07-04 16:51:46.634458 exchanges_wrapper-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     8090 1970-01-01 00:00:00.000000 exchanges_wrapper-1.3.3/PKG-INFO
```

### Comparing `exchanges_wrapper-1.3.2/LICENSE.md` & `exchanges_wrapper-1.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.2/README.md` & `exchanges_wrapper-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/__init__.py` & `exchanges_wrapper-1.3.3/exchanges_wrapper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 __authors__ = ["Th0rgal", "Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "1.3.2"
+__version__ = "1.3.3"
 
 from pathlib import Path
 import shutil
 
 WORK_PATH = Path(Path.home(), ".MartinBinance")
 CONFIG_PATH = Path(WORK_PATH, "config")
 CONFIG_FILE = Path(CONFIG_PATH, "exch_srv_cfg.toml")
```

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/api_pb2.py` & `exchanges_wrapper-1.3.3/exchanges_wrapper/api_pb2.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/api_pb2_grpc.py` & `exchanges_wrapper-1.3.3/exchanges_wrapper/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/bitfinex_parser.py` & `exchanges_wrapper-1.3.3/exchanges_wrapper/bitfinex_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Parser for convert Bitfinex REST API/WSS response to Binance like result
 """
 import time
 from decimal import Decimal
 import logging
 
-logger = logging.getLogger('exch_srv_logger')
+logger = logging.getLogger(__name__)
 
 
 class OrderBook:
     def __init__(self, _order_book, symbol) -> None:
         self.symbol = symbol[1:].replace(':', '').lower()
         self.last_update_id = 1
         self.asks = {}
```

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/c_structures.py` & `exchanges_wrapper-1.3.3/exchanges_wrapper/c_structures.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/client.py` & `exchanges_wrapper-1.3.3/exchanges_wrapper/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 from exchanges_wrapper.web_sockets import UserEventsDataStream,\
                                             MarketEventsDataStream,\
                                             BfxPrivateEventsDataStream,\
                                             HbpPrivateEventsDataStream,\
                                             OkxPrivateEventsDataStream
 from exchanges_wrapper.definitions import OrderType
 from exchanges_wrapper.events import Events
-from exchanges_wrapper.ws_api.ws_session import UserWSSession
 import exchanges_wrapper.bitfinex_parser as bfx
 import exchanges_wrapper.huobi_parser as hbp
 import exchanges_wrapper.okx_parser as okx
 
-logger = logging.getLogger('exch_srv_logger')
+from crypto_ws_api.ws_session import UserWSSession
+
+logger = logging.getLogger(__name__)
 
 STATUS_TIMEOUT = 5  # sec
 
 
 def truncate(f, n):
     return math.floor(f * 10 ** n) / 10 ** n
 
@@ -129,16 +130,15 @@
             self._events = Events()  # skipcq: PYL-W0201
         return self._events
 
     async def start_user_events_listener(self, _trade_id, symbol):
         logger.info(f"Start '{self.exchange}' user events listener for {_trade_id}")
         user_data_stream = None
         if self.exchange == 'binance':
-            if self.user_wss_session:
-                await self.user_wss_session.start(_trade_id)
+            await self.user_wss_session.start(_trade_id)
             user_data_stream = UserEventsDataStream(self, self.endpoint_ws_auth, self.exchange, _trade_id)
         elif self.exchange == 'bitfinex':
             user_data_stream = BfxPrivateEventsDataStream(self, self.endpoint_ws_auth, self.exchange, _trade_id)
         elif self.exchange == 'huobi':
             user_data_stream = HbpPrivateEventsDataStream(self, self.endpoint_ws_auth, self.exchange, _trade_id, symbol)
         elif self.exchange == 'okx':
             user_data_stream = OkxPrivateEventsDataStream(self,
```

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/definitions.py` & `exchanges_wrapper-1.3.3/exchanges_wrapper/definitions.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/errors.py` & `exchanges_wrapper-1.3.3/exchanges_wrapper/errors.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/events.py` & `exchanges_wrapper-1.3.3/exchanges_wrapper/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import functools
 from collections import defaultdict
 import logging
 
 from exchanges_wrapper.errors import UnknownEventType
 
-logger = logging.getLogger('exch_srv_logger')
+logger = logging.getLogger(__name__)
 
 
 # based on: https://stackoverflow.com/a/2022629/10144963
 class Handlers(list):
     async def __call__(self, *args, **kwargs):
         loop = asyncio.get_running_loop()
         trade_id = kwargs.pop('trade_id', None)
```

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/exch_srv.py` & `exchanges_wrapper-1.3.3/exchanges_wrapper/exch_srv.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,32 @@
 from exchanges_wrapper.client import Client
 from exchanges_wrapper.definitions import Side, OrderType, TimeInForce, ResponseType
 from exchanges_wrapper.c_structures import OrderUpdateEvent, OrderTradesEvent
 from exchanges_wrapper import WORK_PATH, CONFIG_FILE, LOG_FILE
 #
 HEARTBEAT = 1  # Sec
 MAX_QUEUE_SIZE = 50
-logger = logging.getLogger('exch_srv_logger')
+#
+logger = logging.getLogger(__name__)
+formatter = logging.Formatter(fmt="[%(asctime)s: %(levelname)s] %(message)s")
+#
+fh = logging.handlers.RotatingFileHandler(LOG_FILE, maxBytes=1000000, backupCount=10)
+fh.setFormatter(formatter)
+fh.setLevel(logging.DEBUG)
+# logger.addHandler(fh)
+#
+sh = logging.StreamHandler()
+sh.setFormatter(formatter)
+sh.setLevel(logging.INFO)
+# logger.addHandler(sh)
+#
+root_logger = logging.getLogger()
+root_logger.setLevel(min([fh.level, sh.level]))
+root_logger.addHandler(fh)
+root_logger.addHandler(sh)
 
 
 def get_account(_account_name: str) -> ():
     config = toml.load(str(CONFIG_FILE))
     accounts = config.get('accounts')
     res = ()
     for account in accounts:
@@ -198,29 +215,26 @@
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         # message list
         response = api_pb2.FetchOpenOrdersResponse()
         # Nested dict
         response_order = api_pb2.FetchOpenOrdersResponse.Order()
         try:
-            res = []
-            ws_status = bool(client.exchange == 'binance'
-                             and client.user_wss_session
-                             and client.user_wss_session.operational_status)
-            if ws_status:
+            res = None
+            if client.exchange == 'binance':
                 params = {
                     "symbol": request.symbol,
                 }
                 res = await client.user_wss_session.handle_request(
                     "openOrders.status",
                     params,
                     api_key=True,
                     signed=True
                 )
-            if not ws_status or res is None:
+            if res is None:
                 res = await client.fetch_open_orders(symbol=request.symbol, receive_window=None)
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error
         except (errors.RateLimitReached, errors.QueryCanceled) as ex:
             Martin.rate_limit_reached_time = time.time()
             logger.warning(f"FetchOpenOrders for {open_client.name}:{request.symbol} exception: {ex}")
             _context.set_details(f"{ex}")
@@ -261,30 +275,27 @@
     async def FetchOrder(self, request: api_pb2.FetchOrderRequest,
                          _context: grpc.aio.ServicerContext) -> api_pb2.FetchOrderResponse:
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         _queue = client.on_order_update_queues.get(request.trade_id)
         response = api_pb2.FetchOrderResponse()
         try:
-            res = {}
-            ws_status = bool(client.exchange == 'binance'
-                             and client.user_wss_session
-                             and client.user_wss_session.operational_status)
-            if ws_status:
+            res = None
+            if client.exchange == 'binance':
                 params = {
                     "symbol": request.symbol,
                     "orderId": request.order_id,
                 }
                 res = await client.user_wss_session.handle_request(
                     "order.status",
                     params,
                     api_key=True,
                     signed=True
                 )
-            if not ws_status or res is None:
+            if res is None:
                 res = await client.fetch_order(symbol=request.symbol,
                                                order_id=request.order_id,
                                                origin_client_order_id=None,
                                                receive_window=None)
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error
         except Exception as _ex:
@@ -315,29 +326,26 @@
 
     async def CancelAllOrders(self, request: api_pb2.MarketRequest,
                               _context: grpc.aio.ServicerContext) -> api_pb2.SimpleResponse():
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         response = api_pb2.SimpleResponse()
         try:
-            res = []
-            ws_status = bool(client.exchange == 'binance'
-                             and client.user_wss_session
-                             and client.user_wss_session.operational_status)
-            if ws_status:
+            res = None
+            if client.exchange == 'binance':
                 params = {
                     "symbol": request.symbol,
                 }
                 res = await client.user_wss_session.handle_request(
                     "openOrders.cancelAll",
                     params,
                     api_key=True,
                     signed=True
                 )
-            if not ws_status or res is None:
+            if res is None:
                 res = await client.cancel_all_orders(symbol=request.symbol, receive_window=None)
             # logger.info(f"CancelAllOrders: {res}")
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error
         except Exception as ex:
             logger.error(f"CancelAllOrder for {open_client.name}:{request.symbol} exception: {ex}")
             _context.set_details(f"{ex}")
@@ -407,25 +415,22 @@
     async def FetchAccountInformation(self, request: api_pb2.OpenClientConnectionId,
                                       _context: grpc.aio.ServicerContext
                                       ) -> api_pb2.FetchAccountBalanceResponse:
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         response = api_pb2.FetchAccountBalanceResponse()
         response_balance = api_pb2.FetchAccountBalanceResponse.Balances()
-        account_information = {}
-        ws_status = bool(client.exchange == 'binance'
-                         and client.user_wss_session
-                         and client.user_wss_session.operational_status)
-        if ws_status:
+        account_information = None
+        if client.exchange == 'binance':
             account_information = await client.user_wss_session.handle_request(
                 "account.status",
                 api_key=True,
                 signed=True
             )
-        if not ws_status or account_information is None:
+        if account_information is None:
             account_information = await client.fetch_account_information(receive_window=None)
         # Send only balances
         res = account_information.get('balances', [])
         # Create consolidated list of asset balances from SPOT and Funding wallets
         balances = []
         for i in res:
             _free = float(i.get('free'))
@@ -557,44 +562,49 @@
                           _event.kline_ignore
                           ]
                 response.candle = json.dumps(candle)
                 yield response
 
     async def FetchAccountTradeList(self, request: api_pb2.AccountTradeListRequest,
                                     _context: grpc.aio.ServicerContext) -> api_pb2.AccountTradeListResponse:
-        client = OpenClient.get_client(request.client_id).client
+        open_client = OpenClient.get_client(request.client_id)
+        client = open_client.client
         response = api_pb2.AccountTradeListResponse()
         response_trade = api_pb2.AccountTradeListResponse.Trade()
-        res = []
-        ws_status = bool(client.user_wss_session and client.user_wss_session.operational_status)
-        if ws_status:
-            params = {
-                "symbol": request.symbol,
-                "startTime": request.start_time,
-                "limit": request.limit,
-                "apiKey": 1,
-                "signature": 1,
-                "timestamp": 1
-            }
-            try:
-                res = await client.user_wss_session.handle_request("myTrades", params)
-            except TimeoutError:
-                ws_status = False
-        if not ws_status:
-            res = await client.fetch_account_trade_list(
-                symbol=request.symbol,
-                start_time=request.start_time,
-                end_time=None,
-                from_id=None,
-                limit=request.limit,
-                receive_window=None)
-        # logger.info(f"FetchAccountTradeList: {res}")
-        for trade in res:
-            trade_order = json_format.ParseDict(trade, response_trade)
-            response.items.append(trade_order)
+        try:
+            res = None
+            if client.exchange == 'binance':
+                params = {
+                    "symbol": request.symbol,
+                    "startTime": request.start_time,
+                    "limit": request.limit,
+                }
+                res = await client.user_wss_session.handle_request(
+                    "myTrades",
+                    params,
+                    api_key=True,
+                    signed=True
+                )
+            if res is None:
+                res = await client.fetch_account_trade_list(
+                    symbol=request.symbol,
+                    start_time=request.start_time,
+                    end_time=None,
+                    from_id=None,
+                    limit=request.limit,
+                    receive_window=None)
+        except asyncio.CancelledError:
+            pass  # Task cancellation should not be logged as an error
+        except Exception as _ex:
+            logger.error(f"FetchAccountTradeList for {open_client.name}: {request.symbol} exception: {_ex}")
+        else:
+            # logger.info(f"FetchAccountTradeList: {res}")
+            for trade in res:
+                trade_order = json_format.ParseDict(trade, response_trade)
+                response.items.append(trade_order)
         return response
 
     async def OnTickerUpdate(self, request: api_pb2.MarketRequest,
                              _context: grpc.aio.ServicerContext) -> api_pb2.OnTickerUpdateResponse:
         response = api_pb2.OnTickerUpdateResponse()
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
@@ -744,19 +754,16 @@
     async def CreateLimitOrder(self, request: api_pb2.CreateLimitOrderRequest,
                                _context: grpc.aio.ServicerContext) -> api_pb2.CreateLimitOrderResponse:
         response = api_pb2.CreateLimitOrderResponse()
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         # logger.info(f"CreateLimitOrder: quantity: {request.quantity}, price: {request.price}")
         try:
-            res = {}
-            ws_status = bool(client.exchange == 'binance'
-                             and client.user_wss_session
-                             and client.user_wss_session.operational_status)
-            if ws_status:
+            res = None
+            if client.exchange == 'binance':
                 params = {
                     "symbol": request.symbol,
                     "side": 'BUY' if request.buy_side else 'SELL',
                     "type": 'LIMIT',
                     "timeInForce": 'GTC',
                     "price": request.price,
                     "quantity": request.quantity,
@@ -765,15 +772,15 @@
                 }
                 res = await client.user_wss_session.handle_request(
                     "order.place",
                     params,
                     api_key=True,
                     signed=True
                 )
-            if not ws_status or res is None:
+            if res is None:
                 res = await client.create_order(
                     request.symbol,
                     Side.BUY if request.buy_side else Side.SELL,
                     order_type=OrderType.LIMIT,
                     time_in_force=TimeInForce.GTC,
                     quantity=request.quantity,
                     quote_order_quantity=None,
@@ -807,30 +814,27 @@
 
     async def CancelOrder(self, request: api_pb2.CancelOrderRequest,
                           _context: grpc.aio.ServicerContext) -> api_pb2.CancelOrderResponse:
         response = api_pb2.CancelOrderResponse()
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         try:
-            res = {}
-            ws_status = bool(client.exchange == 'binance'
-                             and client.user_wss_session
-                             and client.user_wss_session.operational_status)
-            if ws_status:
+            res = None
+            if client.exchange == 'binance':
                 params = {
                     "symbol": request.symbol,
                     "orderId": request.order_id,
                 }
                 res = await client.user_wss_session.handle_request(
                     "order.cancel",
                     params,
                     api_key=True,
                     signed=True
                 )
-            if not ws_status or res is None:
+            if res is None:
                 res = await client.cancel_order(
                     request.symbol,
                     order_id=request.order_id,
                     origin_client_order_id=None,
                     new_client_order_id=None,
                     receive_window=None)
         except asyncio.CancelledError:
@@ -899,19 +903,23 @@
         response = api_pb2.SimpleResponse()
         await stop_stream(client, request.trade_id)
         response.success = True
         return response
 
     async def CheckStream(self, request: api_pb2.MarketRequest,
                           _context: grpc.aio.ServicerContext) -> api_pb2.SimpleResponse:
-        open_client = OpenClient.get_client(request.client_id)
-        client = open_client.client
         response = api_pb2.SimpleResponse()
-        response.success = bool(client.data_streams.get(request.trade_id))
-        logger.debug(f"CheckStream request passed: {response.success} for {request.symbol} on {client.exchange}")
+        open_client = OpenClient.get_client(request.client_id)
+        if open_client:
+            client = open_client.client
+            response.success = bool(client.data_streams.get(request.trade_id))
+        else:
+            response.success = False
+        if not response.success:
+            logger.warning(f"CheckStream request filed for {request.symbol}")
         return response
 
 
 async def stop_stream(client, trade_id):
     await client.stop_events_listener(trade_id)
     client.events.unregister(client.exchange, trade_id)
     [await _queue.put(trade_id) for _queue in client.stream_queue.get(trade_id, [])]
@@ -947,28 +955,14 @@
     server.add_insecure_port(listen_addr)
     logger.info(f"Starting server on {listen_addr}")
     await server.start()
     await server.wait_for_termination()
 
 
 def main():
-    logger.setLevel(logging.DEBUG)
-    formatter = logging.Formatter(fmt="[%(asctime)s: %(levelname)s] %(message)s")
-    #
-    file_handler = logging.handlers.RotatingFileHandler(LOG_FILE, maxBytes=1000000, backupCount=10)
-    file_handler.setFormatter(formatter)
-    file_handler.setLevel(logging.DEBUG)
-    logger.addHandler(file_handler)
-    #
-    stream_handler = logging.StreamHandler()
-    stream_handler.setFormatter(formatter)
-    stream_handler.setLevel(logging.INFO)
-    # stream_handler.setLevel(logging.DEBUG)
-    logger.addHandler(stream_handler)
-    #
     loop = asyncio.new_event_loop()
     loop.create_task(serve())
     try:
         loop.run_forever()
     except KeyboardInterrupt:
         pass
     finally:
```

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/exch_srv_cfg.toml.template` & `exchanges_wrapper-1.3.3/exchanges_wrapper/exch_srv_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/http_client.py` & `exchanges_wrapper-1.3.3/exchanges_wrapper/http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     RateLimitReached,
     ExchangeError,
     WAFLimitViolated,
     IPAddressBanned,
     HTTPError,
     QueryCanceled,
 )
-
-logger = logging.getLogger('exch_srv_logger')
+logger = logging.getLogger(__name__)
 
 AJ = 'application/json'
 
 
 class HttpClient:
     def __init__(self, **kwargs):
         self.api_key = kwargs.get('api_key')
```

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/huobi_parser.py` & `exchanges_wrapper-1.3.3/exchanges_wrapper/huobi_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Parser for convert Huobi REST API/WSS response to Binance like result
 """
 import time
 from decimal import Decimal
 import logging
 
-logger = logging.getLogger('exch_srv_logger')
+logger = logging.getLogger(__name__)
 
 
 def on_balance_update(res: {}) -> {}:
     balance = {
         'e': 'balanceUpdate',
         'E': res.get('transactTime'),
         'a': res.get('currency').upper(),
```

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/okx_parser.py` & `exchanges_wrapper-1.3.3/exchanges_wrapper/okx_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Parser for convert OKX REST API/WSS response to Binance like result
 """
 import time
 from decimal import Decimal
 import logging
 
-logger = logging.getLogger('exch_srv_logger')
+logger = logging.getLogger(__name__)
 
 
 def fetch_server_time(res: []) -> {}:
     if res:
         return {'serverTime': int(res[0].get('ts'))}
```

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/proto/exchanges_wrapper/api.proto` & `exchanges_wrapper-1.3.3/exchanges_wrapper/proto/exchanges_wrapper/api.proto`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.2/exchanges_wrapper/web_sockets.py` & `exchanges_wrapper-1.3.3/exchanges_wrapper/web_sockets.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-1.3.2/pyproject.toml` & `exchanges_wrapper-1.3.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "grpcio==1.48.1",
     "grpcio-tools==1.48.1",
     "toml==0.10.2",
     "idna==3.4",
     "pyotp~=2.8.0",
     "simplejson==3.19.1",
     "shortuuid~=1.0.11",
+    "crypto_ws_api~=1.0.1",
 ]
 
 [tool.flit.module]
 name = "exchanges_wrapper"
 
 [project.urls]
 Source = "https://github.com/DogsTailFarmer/exchanges-wrapper"
```

### Comparing `exchanges_wrapper-1.3.2/PKG-INFO` & `exchanges_wrapper-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchanges-wrapper
-Version: 1.3.2
+Version: 1.3.3
 Summary: REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
 Author-email: Thomas Marchand <thomas.marchand@tuta.io>, Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,15 @@
 Requires-Dist: grpcio==1.48.1
 Requires-Dist: grpcio-tools==1.48.1
 Requires-Dist: toml==0.10.2
 Requires-Dist: idna==3.4
 Requires-Dist: pyotp~=2.8.0
 Requires-Dist: simplejson==3.19.1
 Requires-Dist: shortuuid~=1.0.11
+Requires-Dist: crypto_ws_api~=1.0.1
 Project-URL: Source, https://github.com/DogsTailFarmer/exchanges-wrapper
 
 
 <p align="center"><img src="https://raw.githubusercontent.com/gist/DogsTailFarmer/167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/Logo%202v3.svg" width="300"></p>
 
 ***
 <h1 align="center">Crypto exchanges API/WSS wrapper with grpc powered server</h1>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.2 Summary: REST API
+Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.3 Summary: REST API
 and WebSocket asyncio wrapper with grpc powered multiplexer server Author-
 email: Thomas Marchand
 marchand@tuta.io>, Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
 Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.48.1 Requires-Dist: grpcio-
 tools==1.48.1 Requires-Dist: toml==0.10.2 Requires-Dist: idna==3.4 Requires-
 Dist: pyotp~=2.8.0 Requires-Dist: simplejson==3.19.1 Requires-Dist:
-shortuuid~=1.0.11 Project-URL: Source, https://github.com/DogsTailFarmer/
-exchanges-wrapper
+shortuuid~=1.0.11 Requires-Dist: crypto_ws_api~=1.0.1 Project-URL: Source,
+https://github.com/DogsTailFarmer/exchanges-wrapper
             [https://raw.githubusercontent.com/gist/DogsTailFarmer/
 167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/
                                 Logo%202v3.svg]
 ***
     ****** Crypto exchanges API/WSS wrapper with grpc powered server ******
                   ***** Binance, Bitfinex, Huobi, OKX, *****
                           **** For SPOT markets ****
```

