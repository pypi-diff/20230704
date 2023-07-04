# Comparing `tmp/remotivelabs_broker-0.2.0b1.tar.gz` & `tmp/remotivelabs_broker-0.2.0b2.tar.gz`

## Comparing `remotivelabs_broker-0.2.0b1.tar` & `remotivelabs_broker-0.2.0b2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/.DS_Store
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/CHANGELOG.md
--rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/misc/build_doc.sh
--rwxr-xr-x   0        0        0      431 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/misc/build_proto.sh
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/misc/fix_import_statements.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/misc/theme/theme.css
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/__about__.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/.gitignore
--rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/common_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/common_pb2_grpc.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/diagnostics_api_pb2.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/diagnostics_api_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/functional_api_pb2.py
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/functional_api_pb2_grpc.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/network_api_pb2.py
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/network_api_pb2_grpc.py
--rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/system_api_pb2.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/system_api_pb2_grpc.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/traffic_api_pb2.py
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/sync/__init__.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/sync/helper.py
--rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/remotivelabs/broker/sync/signalcreator.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/tests/__init__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/tests/random.bin
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/tests/test_live.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/tests/test_proto_types.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/tests/test_sha256.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/tests/configuration_udp/interfaces.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/tests/configuration_udp/can/test.dbc
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/.gitignore
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/LICENSE.txt
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/README.md
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/pyproject.toml
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b1/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/.DS_Store
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/CHANGELOG.md
+-rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/misc/build_doc.sh
+-rwxr-xr-x   0        0        0      431 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/misc/build_proto.sh
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/misc/fix_import_statements.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/misc/theme/theme.css
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/__about__.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/__init__.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/.gitignore
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/common_pb2.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/common_pb2_grpc.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/diagnostics_api_pb2.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/diagnostics_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/functional_api_pb2.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/functional_api_pb2_grpc.py
+-rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/network_api_pb2.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/network_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/system_api_pb2.py
+-rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/system_api_pb2_grpc.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/traffic_api_pb2.py
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/sync/__init__.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/sync/helper.py
+-rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/remotivelabs/broker/sync/signalcreator.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/tests/__init__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/tests/random.bin
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/tests/test_live.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/tests/test_proto_types.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/tests/test_sha256.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/tests/configuration_udp/interfaces.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/tests/configuration_udp/can/test.dbc
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/.gitignore
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/LICENSE.txt
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/README.md
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b2/PKG-INFO
```

### Comparing `remotivelabs_broker-0.2.0b1/.DS_Store` & `remotivelabs_broker-0.2.0b2/.DS_Store`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/misc/fix_import_statements.py` & `remotivelabs_broker-0.2.0b2/misc/fix_import_statements.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/remotivelabs/broker/__init__.py` & `remotivelabs_broker-0.2.0b2/remotivelabs/broker/__init__.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/common_pb2.py` & `remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/common_pb2.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/diagnostics_api_pb2_grpc.py` & `remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/network_api_pb2_grpc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,152 +1,173 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from . import common_pb2 as common__pb2
-from . import diagnostics_api_pb2 as diagnostics__api__pb2
+from . import network_api_pb2 as network__api__pb2
 
 
-class DiagnosticsServiceStub(object):
-    """*
-    Read data by service identifier
-
-    Data identifiers:
-    - 0x22 read data by identinifier (Service id).
-    - 0x1f90 DID (Data identifier) for VIN number.
+class NetworkServiceStub(object):
+    """/ Signal publish, subscribe and read.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.SendDiagnosticsQuery = channel.unary_unary(
-                '/base.DiagnosticsService/SendDiagnosticsQuery',
-                request_serializer=diagnostics__api__pb2.DiagnosticsRequest.SerializeToString,
-                response_deserializer=diagnostics__api__pb2.DiagnosticsResponse.FromString,
+        self.SubscribeToSignals = channel.unary_stream(
+                '/base.NetworkService/SubscribeToSignals',
+                request_serializer=network__api__pb2.SubscriberConfig.SerializeToString,
+                response_deserializer=network__api__pb2.Signals.FromString,
+                )
+        self.SubscribeToSignalsWithMapping = channel.unary_stream(
+                '/base.NetworkService/SubscribeToSignalsWithMapping',
+                request_serializer=network__api__pb2.SubscriberWithMappingConfig.SerializeToString,
+                response_deserializer=network__api__pb2.Signals.FromString,
                 )
-        self.PublishMultiFrame = channel.unary_unary(
-                '/base.DiagnosticsService/PublishMultiFrame',
-                request_serializer=diagnostics__api__pb2.MultiFrame.SerializeToString,
+        self.PublishSignals = channel.unary_unary(
+                '/base.NetworkService/PublishSignals',
+                request_serializer=network__api__pb2.PublisherConfig.SerializeToString,
                 response_deserializer=common__pb2.Empty.FromString,
                 )
-        self.SubscribeMultiFrame = channel.unary_stream(
-                '/base.DiagnosticsService/SubscribeMultiFrame',
-                request_serializer=diagnostics__api__pb2.MultiFrame.SerializeToString,
-                response_deserializer=diagnostics__api__pb2.Payload.FromString,
+        self.ReadSignals = channel.unary_unary(
+                '/base.NetworkService/ReadSignals',
+                request_serializer=network__api__pb2.SignalIds.SerializeToString,
+                response_deserializer=network__api__pb2.Signals.FromString,
                 )
 
 
-class DiagnosticsServiceServicer(object):
-    """*
-    Read data by service identifier
-
-    Data identifiers:
-    - 0x22 read data by identinifier (Service id).
-    - 0x1f90 DID (Data identifier) for VIN number.
+class NetworkServiceServicer(object):
+    """/ Signal publish, subscribe and read.
     """
 
-    def SendDiagnosticsQuery(self, request, context):
-        """/ Send diagnostics request
+    def SubscribeToSignals(self, request, context):
+        """/ Subscribe to signals.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubscribeToSignalsWithMapping(self, request, context):
+        """/ Subscribe to signals with mapping
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def PublishMultiFrame(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def PublishSignals(self, request, context):
+        """/ Publish signals with values.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SubscribeMultiFrame(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def ReadSignals(self, request, context):
+        """/ Read signals from cache.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_DiagnosticsServiceServicer_to_server(servicer, server):
+def add_NetworkServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'SendDiagnosticsQuery': grpc.unary_unary_rpc_method_handler(
-                    servicer.SendDiagnosticsQuery,
-                    request_deserializer=diagnostics__api__pb2.DiagnosticsRequest.FromString,
-                    response_serializer=diagnostics__api__pb2.DiagnosticsResponse.SerializeToString,
+            'SubscribeToSignals': grpc.unary_stream_rpc_method_handler(
+                    servicer.SubscribeToSignals,
+                    request_deserializer=network__api__pb2.SubscriberConfig.FromString,
+                    response_serializer=network__api__pb2.Signals.SerializeToString,
             ),
-            'PublishMultiFrame': grpc.unary_unary_rpc_method_handler(
-                    servicer.PublishMultiFrame,
-                    request_deserializer=diagnostics__api__pb2.MultiFrame.FromString,
+            'SubscribeToSignalsWithMapping': grpc.unary_stream_rpc_method_handler(
+                    servicer.SubscribeToSignalsWithMapping,
+                    request_deserializer=network__api__pb2.SubscriberWithMappingConfig.FromString,
+                    response_serializer=network__api__pb2.Signals.SerializeToString,
+            ),
+            'PublishSignals': grpc.unary_unary_rpc_method_handler(
+                    servicer.PublishSignals,
+                    request_deserializer=network__api__pb2.PublisherConfig.FromString,
                     response_serializer=common__pb2.Empty.SerializeToString,
             ),
-            'SubscribeMultiFrame': grpc.unary_stream_rpc_method_handler(
-                    servicer.SubscribeMultiFrame,
-                    request_deserializer=diagnostics__api__pb2.MultiFrame.FromString,
-                    response_serializer=diagnostics__api__pb2.Payload.SerializeToString,
+            'ReadSignals': grpc.unary_unary_rpc_method_handler(
+                    servicer.ReadSignals,
+                    request_deserializer=network__api__pb2.SignalIds.FromString,
+                    response_serializer=network__api__pb2.Signals.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'base.DiagnosticsService', rpc_method_handlers)
+            'base.NetworkService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class DiagnosticsService(object):
-    """*
-    Read data by service identifier
-
-    Data identifiers:
-    - 0x22 read data by identinifier (Service id).
-    - 0x1f90 DID (Data identifier) for VIN number.
+class NetworkService(object):
+    """/ Signal publish, subscribe and read.
     """
 
     @staticmethod
-    def SendDiagnosticsQuery(request,
+    def SubscribeToSignals(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/base.NetworkService/SubscribeToSignals',
+            network__api__pb2.SubscriberConfig.SerializeToString,
+            network__api__pb2.Signals.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubscribeToSignalsWithMapping(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/base.DiagnosticsService/SendDiagnosticsQuery',
-            diagnostics__api__pb2.DiagnosticsRequest.SerializeToString,
-            diagnostics__api__pb2.DiagnosticsResponse.FromString,
+        return grpc.experimental.unary_stream(request, target, '/base.NetworkService/SubscribeToSignalsWithMapping',
+            network__api__pb2.SubscriberWithMappingConfig.SerializeToString,
+            network__api__pb2.Signals.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def PublishMultiFrame(request,
+    def PublishSignals(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/base.DiagnosticsService/PublishMultiFrame',
-            diagnostics__api__pb2.MultiFrame.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/base.NetworkService/PublishSignals',
+            network__api__pb2.PublisherConfig.SerializeToString,
             common__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SubscribeMultiFrame(request,
+    def ReadSignals(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/base.DiagnosticsService/SubscribeMultiFrame',
-            diagnostics__api__pb2.MultiFrame.SerializeToString,
-            diagnostics__api__pb2.Payload.FromString,
+        return grpc.experimental.unary_unary(request, target, '/base.NetworkService/ReadSignals',
+            network__api__pb2.SignalIds.SerializeToString,
+            network__api__pb2.Signals.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/functional_api_pb2.py` & `remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/functional_api_pb2.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/functional_api_pb2_grpc.py` & `remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/functional_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/network_api_pb2.py` & `remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/network_api_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,30 +11,38 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import common_pb2 as common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11network_api.proto\x12\x04\x62\x61se\x1a\x0c\x63ommon.proto\"h\n\x10SubscriberConfig\x12 \n\x08\x63lientId\x18\x01 \x01(\x0b\x32\x0e.base.ClientId\x12 \n\x07signals\x18\x02 \x01(\x0b\x32\x0f.base.SignalIds\x12\x10\n\x08onChange\x18\x03 \x01(\x08\"-\n\tSignalIds\x12 \n\x08signalId\x18\x01 \x03(\x0b\x32\x0e.base.SignalId\"\'\n\x07Signals\x12\x1c\n\x06signal\x18\x01 \x03(\x0b\x32\x0c.base.Signal\"f\n\x0fPublisherConfig\x12\x1e\n\x07signals\x18\x01 \x01(\x0b\x32\r.base.Signals\x12 \n\x08\x63lientId\x18\x02 \x01(\x0b\x32\x0e.base.ClientId\x12\x11\n\tfrequency\x18\x03 \x01(\x05\"\x9c\x01\n\x06Signal\x12\x1a\n\x02id\x18\x01 \x01(\x0b\x32\x0e.base.SignalId\x12\x11\n\x07integer\x18\x02 \x01(\x03H\x00\x12\x10\n\x06\x64ouble\x18\x03 \x01(\x01H\x00\x12\x15\n\x0b\x61rbitration\x18\x04 \x01(\x08H\x00\x12\x0f\n\x05\x65mpty\x18\x06 \x01(\x08H\x00\x12\x0b\n\x03raw\x18\x05 \x01(\x0c\x12\x11\n\ttimestamp\x18\x07 \x01(\x03\x42\t\n\x07payload2\xba\x01\n\x0eNetworkService\x12?\n\x12SubscribeToSignals\x12\x16.base.SubscriberConfig\x1a\r.base.Signals\"\x00\x30\x01\x12\x36\n\x0ePublishSignals\x12\x15.base.PublisherConfig\x1a\x0b.base.Empty\"\x00\x12/\n\x0bReadSignals\x12\x0f.base.SignalIds\x1a\r.base.Signals\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11network_api.proto\x12\x04\x62\x61se\x1a\x0c\x63ommon.proto\"h\n\x10SubscriberConfig\x12 \n\x08\x63lientId\x18\x01 \x01(\x0b\x32\x0e.base.ClientId\x12 \n\x07signals\x18\x02 \x01(\x0b\x32\x0f.base.SignalIds\x12\x10\n\x08onChange\x18\x03 \x01(\x08\"f\n\x1bSubscriberWithMappingConfig\x12 \n\x08\x63lientId\x18\x01 \x01(\x0b\x32\x0e.base.ClientId\x12\x13\n\x0bmappingCode\x18\x02 \x01(\t\x12\x10\n\x08onChange\x18\x03 \x01(\x08\"-\n\tSignalIds\x12 \n\x08signalId\x18\x01 \x03(\x0b\x32\x0e.base.SignalId\"\'\n\x07Signals\x12\x1c\n\x06signal\x18\x01 \x03(\x0b\x32\x0c.base.Signal\"f\n\x0fPublisherConfig\x12\x1e\n\x07signals\x18\x01 \x01(\x0b\x32\r.base.Signals\x12 \n\x08\x63lientId\x18\x02 \x01(\x0b\x32\x0e.base.ClientId\x12\x11\n\tfrequency\x18\x03 \x01(\x05\"\x9c\x01\n\x06Signal\x12\x1a\n\x02id\x18\x01 \x01(\x0b\x32\x0e.base.SignalId\x12\x11\n\x07integer\x18\x02 \x01(\x03H\x00\x12\x10\n\x06\x64ouble\x18\x03 \x01(\x01H\x00\x12\x15\n\x0b\x61rbitration\x18\x04 \x01(\x08H\x00\x12\x0f\n\x05\x65mpty\x18\x06 \x01(\x08H\x00\x12\x0b\n\x03raw\x18\x05 \x01(\x0c\x12\x11\n\ttimestamp\x18\x07 \x01(\x03\x42\t\n\x07payload2\x91\x02\n\x0eNetworkService\x12?\n\x12SubscribeToSignals\x12\x16.base.SubscriberConfig\x1a\r.base.Signals\"\x00\x30\x01\x12U\n\x1dSubscribeToSignalsWithMapping\x12!.base.SubscriberWithMappingConfig\x1a\r.base.Signals\"\x00\x30\x01\x12\x36\n\x0ePublishSignals\x12\x15.base.PublisherConfig\x1a\x0b.base.Empty\"\x00\x12/\n\x0bReadSignals\x12\x0f.base.SignalIds\x1a\r.base.Signals\"\x00\x62\x06proto3')
 
 
 
 _SUBSCRIBERCONFIG = DESCRIPTOR.message_types_by_name['SubscriberConfig']
+_SUBSCRIBERWITHMAPPINGCONFIG = DESCRIPTOR.message_types_by_name['SubscriberWithMappingConfig']
 _SIGNALIDS = DESCRIPTOR.message_types_by_name['SignalIds']
 _SIGNALS = DESCRIPTOR.message_types_by_name['Signals']
 _PUBLISHERCONFIG = DESCRIPTOR.message_types_by_name['PublisherConfig']
 _SIGNAL = DESCRIPTOR.message_types_by_name['Signal']
 SubscriberConfig = _reflection.GeneratedProtocolMessageType('SubscriberConfig', (_message.Message,), {
   'DESCRIPTOR' : _SUBSCRIBERCONFIG,
   '__module__' : 'network_api_pb2'
   # @@protoc_insertion_point(class_scope:base.SubscriberConfig)
   })
 _sym_db.RegisterMessage(SubscriberConfig)
 
+SubscriberWithMappingConfig = _reflection.GeneratedProtocolMessageType('SubscriberWithMappingConfig', (_message.Message,), {
+  'DESCRIPTOR' : _SUBSCRIBERWITHMAPPINGCONFIG,
+  '__module__' : 'network_api_pb2'
+  # @@protoc_insertion_point(class_scope:base.SubscriberWithMappingConfig)
+  })
+_sym_db.RegisterMessage(SubscriberWithMappingConfig)
+
 SignalIds = _reflection.GeneratedProtocolMessageType('SignalIds', (_message.Message,), {
   'DESCRIPTOR' : _SIGNALIDS,
   '__module__' : 'network_api_pb2'
   # @@protoc_insertion_point(class_scope:base.SignalIds)
   })
 _sym_db.RegisterMessage(SignalIds)
 
@@ -61,18 +69,20 @@
 
 _NETWORKSERVICE = DESCRIPTOR.services_by_name['NetworkService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _SUBSCRIBERCONFIG._serialized_start=41
   _SUBSCRIBERCONFIG._serialized_end=145
-  _SIGNALIDS._serialized_start=147
-  _SIGNALIDS._serialized_end=192
-  _SIGNALS._serialized_start=194
-  _SIGNALS._serialized_end=233
-  _PUBLISHERCONFIG._serialized_start=235
-  _PUBLISHERCONFIG._serialized_end=337
-  _SIGNAL._serialized_start=340
-  _SIGNAL._serialized_end=496
-  _NETWORKSERVICE._serialized_start=499
-  _NETWORKSERVICE._serialized_end=685
+  _SUBSCRIBERWITHMAPPINGCONFIG._serialized_start=147
+  _SUBSCRIBERWITHMAPPINGCONFIG._serialized_end=249
+  _SIGNALIDS._serialized_start=251
+  _SIGNALIDS._serialized_end=296
+  _SIGNALS._serialized_start=298
+  _SIGNALS._serialized_end=337
+  _PUBLISHERCONFIG._serialized_start=339
+  _PUBLISHERCONFIG._serialized_end=441
+  _SIGNAL._serialized_start=444
+  _SIGNAL._serialized_end=600
+  _NETWORKSERVICE._serialized_start=603
+  _NETWORKSERVICE._serialized_end=876
 # @@protoc_insertion_point(module_scope)
```

### Comparing `remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/system_api_pb2.py` & `remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/system_api_pb2.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/system_api_pb2_grpc.py` & `remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/system_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/traffic_api_pb2.py` & `remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/remotivelabs/broker/generated/sync/traffic_api_pb2_grpc.py` & `remotivelabs_broker-0.2.0b2/remotivelabs/broker/generated/sync/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/remotivelabs/broker/sync/__init__.py` & `remotivelabs_broker-0.2.0b2/remotivelabs/broker/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/remotivelabs/broker/sync/helper.py` & `remotivelabs_broker-0.2.0b2/remotivelabs/broker/sync/helper.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/remotivelabs/broker/sync/signalcreator.py` & `remotivelabs_broker-0.2.0b2/remotivelabs/broker/sync/signalcreator.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/tests/random.bin` & `remotivelabs_broker-0.2.0b2/tests/random.bin`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/tests/test_live.py` & `remotivelabs_broker-0.2.0b2/tests/test_live.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/tests/configuration_udp/interfaces.json` & `remotivelabs_broker-0.2.0b2/tests/configuration_udp/interfaces.json`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/tests/configuration_udp/can/test.dbc` & `remotivelabs_broker-0.2.0b2/tests/configuration_udp/can/test.dbc`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/LICENSE.txt` & `remotivelabs_broker-0.2.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/README.md` & `remotivelabs_broker-0.2.0b2/README.md`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/pyproject.toml` & `remotivelabs_broker-0.2.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b1/PKG-INFO` & `remotivelabs_broker-0.2.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotivelabs-broker
-Version: 0.2.0b1
+Version: 0.2.0b2
 Summary: RemotiveLabs Broker gRPC API
 Project-URL: Homepage, https://remotivelabs.com/
 Project-URL: Documentation, https://docs.remotivelabs.com/python/remotivelabs-broker/
 Project-URL: Issues, https://github.com/remotivelabs/remotivelabs-apis/issues
 Project-URL: Source, https://github.com/remotivelabs/remotivelabs-apis/tree/main/python/remotivelabs-broker
 Author-email: Support <support@remotivelabs.com>
 License-File: LICENSE.txt
```

