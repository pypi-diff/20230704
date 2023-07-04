# Comparing `tmp/gl_client-0.1.8.tar.gz` & `tmp/gl_client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gl_client-0.1.8.tar", max compression
+gzip compressed data, was "gl_client-0.1.9.tar", max compression
```

## Comparing `gl_client-0.1.8.tar` & `gl_client-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0    16437 2023-06-06 13:01:54.714300 gl_client-0.1.8/glclient/__init__.py
--rw-r--r--   0        0        0     1102 2023-06-06 13:01:54.714300 gl_client-0.1.8/glclient/glclient.pyi
--rw-r--r--   0        0        0    41334 2023-06-06 13:01:54.714300 gl_client-0.1.8/glclient/greenlight_pb2.py
--rw-r--r--   0        0        0    53249 2023-06-06 13:01:54.714300 gl_client-0.1.8/glclient/greenlight_pb2.pyi
--rw-r--r--   0        0        0    36771 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/greenlight_pb2_grpc.py
--rw-r--r--   0        0        0    14152 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/greenlight_pb2_grpc.pyi
--rw-r--r--   0        0        0   132174 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/node_pb2.py
--rw-r--r--   0        0        0    70118 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/node_pb2_grpc.py
--rw-r--r--   0        0        0    25418 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/rpc.py
--rw-r--r--   0        0        0    11865 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/scheduler_pb2.py
--rw-r--r--   0        0        0    10996 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/scheduler_pb2.pyi
--rw-r--r--   0        0        0    22459 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/scheduler_pb2_grpc.py
--rw-r--r--   0        0        0     1520 2023-06-06 13:01:54.718300 gl_client-0.1.8/glclient/tls.py
--rw-r--r--   0        0        0      719 2023-06-06 13:01:54.718300 gl_client-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 gl_client-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    17276 2023-07-04 12:58:26.638913 gl_client-0.1.9/glclient/__init__.py
+-rw-r--r--   0        0        0     1102 2023-07-04 12:58:26.638913 gl_client-0.1.9/glclient/glclient.pyi
+-rw-r--r--   0        0        0    44301 2023-07-04 12:58:26.638913 gl_client-0.1.9/glclient/greenlight_pb2.py
+-rw-r--r--   0        0        0    53249 2023-07-04 12:58:26.638913 gl_client-0.1.9/glclient/greenlight_pb2.pyi
+-rw-r--r--   0        0        0    38876 2023-07-04 12:58:26.638913 gl_client-0.1.9/glclient/greenlight_pb2_grpc.py
+-rw-r--r--   0        0        0    14152 2023-07-04 12:58:26.638913 gl_client-0.1.9/glclient/greenlight_pb2_grpc.pyi
+-rw-r--r--   0        0        0    25726 2023-07-04 12:58:26.638913 gl_client-0.1.9/glclient/rpc.py
+-rw-r--r--   0        0        0    11865 2023-07-04 12:58:26.642913 gl_client-0.1.9/glclient/scheduler_pb2.py
+-rw-r--r--   0        0        0    10996 2023-07-04 12:58:26.642913 gl_client-0.1.9/glclient/scheduler_pb2.pyi
+-rw-r--r--   0        0        0    22459 2023-07-04 12:58:26.642913 gl_client-0.1.9/glclient/scheduler_pb2_grpc.py
+-rw-r--r--   0        0        0     1520 2023-07-04 12:58:26.642913 gl_client-0.1.9/glclient/tls.py
+-rw-r--r--   0        0        0      681 2023-07-04 12:58:26.642913 gl_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 gl_client-0.1.9/PKG-INFO
```

### Comparing `gl_client-0.1.8/glclient/__init__.py` & `gl_client-0.1.9/glclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from . import scheduler_pb2 as schedpb
 from . import greenlight_pb2 as nodepb
-from . import node_pb2 as clnpb  # type: ignore
+from pyln import grpc as clnpb  # type: ignore
 from . import glclient as native
 from .tls import TlsConfig
 from .glclient import backup_decrypt_with_seed
 from google.protobuf.message import Message as PbMessage
 from .greenlight_pb2 import Amount
 from binascii import hexlify, unhexlify
 from typing import Optional, List, Union, Iterable, SupportsIndex, Type, TypeVar
@@ -157,15 +157,24 @@
         req = nodepb.ListPeersRequest().SerializeToString()
         res = nodepb.ListPeersResponse
 
         return res.FromString(
             bytes(self.inner.call(uri, bytes(req)))
         )
 
-    def listpays(self) -> clnpb.ListpaysResponse:    
+    def list_closed_channels(self) -> clnpb.ListclosedchannelsResponse:
+        uri = "/cln.Node/ListClosedChannels"
+        req = clnpb.ListclosedchannelsRequest().SerializeToString()
+        res = clnpb.ListclosedchannelsResponse
+
+        return res.FromString(
+            bytes(self.inner.call(uri, bytes(req)))
+        )
+
+    def listpays(self) -> clnpb.ListpaysResponse:
         uri = "/cln.Node/ListPays"
         req = clnpb.ListpaysRequest().SerializeToString()
         res = clnpb.ListpaysResponse
 
         return res.FromString(
             bytes(self.inner.call(uri, req))
         )
@@ -337,39 +346,37 @@
             self,
             amount_msat: clnpb.AmountOrAny,
             label: str,
             description: str,
             expiry: Optional[int]=None,
             fallbacks: Optional[List[str]]=None,
             preimage: Optional[bytes]=None,
-            exposeprivatechannels: Optional[bool]=None,
             cltv: Optional[int]=None,
             deschashonly: Optional[bool]=None
     ) -> clnpb.InvoiceResponse:
         if preimage and len(preimage) != 32:
             raise ValueError("Preimage must be 32 bytes in length")
-        
+
         uri = "/cln.Node/Invoice"
         res = clnpb.InvoiceResponse
         req = clnpb.InvoiceRequest(
             amount_msat=amount_msat,
             label=label,
             description=description,
             preimage=preimage,
             expiry=expiry,
             fallbacks=fallbacks,
-            exposeprivatechannels=exposeprivatechannels,
             cltv=cltv,
             deschashonly=deschashonly,
         ).SerializeToString()
 
         return res.FromString(
             bytes(self.inner.call(uri, bytes(req)))
         )
-    
+
     def create_invoice(
             self,
             label: str,
             amount=None,
             description: Optional[str]=None,
             preimage: Optional[Union[str,bytes]]=None
     ) -> nodepb.Invoice:
@@ -454,14 +461,34 @@
         stream = self.inner.stream_incoming(b"")
         while True:
             n = stream.next()
             if n is None:
                 break
             yield nodepb.IncomingPayment.FromString(bytes(n))
 
+    def stream_custommsg(self):
+        stream = self.inner.stream_custommsg(b"")
+        while True:
+            n = stream.next()
+            if n is None:
+                break
+            yield nodepb.Custommsg.FromString(bytes(n))
+
+    def send_custommsg(self, node_id: str, msg: bytes) -> clnpb.SendcustommsgResponse:
+        uri = "/cln.Node/SendCustomMsg"
+        res = clnpb.SendcustommsgResponse
+        req = clnpb.SendcustommsgRequest(
+            node_id=normalize_node_id(node_id),
+            msg=msg,
+        ).SerializeToString()
+
+        return res.FromString(
+            bytes(self.inner.call(uri, bytes(req)))
+        )
+
     def datastore(
             self,
             key,
             string=None,
             hex=None,
             mode=None,
             generation=None
```

### Comparing `gl_client-0.1.8/glclient/glclient.pyi` & `gl_client-0.1.9/glclient/glclient.pyi`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.8/glclient/greenlight_pb2.py` & `gl_client-0.1.9/glclient/greenlight_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10greenlight.proto\x12\ngreenlight\"H\n\x11HsmRequestContext\x12\x0f\n\x07node_id\x18\x01 \x01(\x0c\x12\x0c\n\x04\x64\x62id\x18\x02 \x01(\x04\x12\x14\n\x0c\x63\x61pabilities\x18\x03 \x01(\x04\"b\n\x0bHsmResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\r\x12\x0b\n\x03raw\x18\x02 \x01(\x0c\x12\x32\n\x0csigner_state\x18\x05 \x03(\x0b\x32\x1c.greenlight.SignerStateEntry\"\xbf\x01\n\nHsmRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\r\x12.\n\x07\x63ontext\x18\x02 \x01(\x0b\x32\x1d.greenlight.HsmRequestContext\x12\x0b\n\x03raw\x18\x03 \x01(\x0c\x12\x32\n\x0csigner_state\x18\x04 \x03(\x0b\x32\x1c.greenlight.SignerStateEntry\x12,\n\x08requests\x18\x05 \x03(\x0b\x32\x1a.greenlight.PendingRequest\"\x07\n\x05\x45mpty\"O\n\x07\x41\x64\x64ress\x12(\n\x04type\x18\x01 \x01(\x0e\x32\x1a.greenlight.NetAddressType\x12\x0c\n\x04\x61\x64\x64r\x18\x02 \x01(\t\x12\x0c\n\x04port\x18\x03 \x01(\r\"\x10\n\x0eGetInfoRequest\"\xb2\x01\n\x0fGetInfoResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\x0c\x12\r\n\x05\x61lias\x18\x02 \x01(\t\x12\r\n\x05\x63olor\x18\x03 \x01(\x0c\x12\x11\n\tnum_peers\x18\x04 \x01(\r\x12&\n\taddresses\x18\x05 \x03(\x0b\x32\x13.greenlight.Address\x12\x0f\n\x07version\x18\x06 \x01(\t\x12\x13\n\x0b\x62lockheight\x18\x07 \x01(\r\x12\x0f\n\x07network\x18\x08 \x01(\t\"\r\n\x0bStopRequest\"\x0e\n\x0cStopResponse\"/\n\x0e\x43onnectRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04\x61\x64\x64r\x18\x02 \x01(\t\"4\n\x0f\x43onnectResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x10\n\x08\x66\x65\x61tures\x18\x02 \x01(\t\"#\n\x10ListPeersRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\"\x81\x01\n\x04Htlc\x12\x11\n\tdirection\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x04\x12\x0e\n\x06\x61mount\x18\x03 \x01(\t\x12\x0e\n\x06\x65xpiry\x18\x04 \x01(\x04\x12\x14\n\x0cpayment_hash\x18\x05 \x01(\t\x12\r\n\x05state\x18\x06 \x01(\t\x12\x15\n\rlocal_trimmed\x18\x07 \x01(\x08\"(\n\x07\x41liases\x12\r\n\x05local\x18\x01 \x01(\t\x12\x0e\n\x06remote\x18\x02 \x01(\t\"\x8f\x03\n\x07\x43hannel\x12\r\n\x05state\x18\x01 \x01(\t\x12\r\n\x05owner\x18\x02 \x01(\t\x12\"\n\x05\x61lias\x18\x12 \x01(\x0b\x32\x13.greenlight.Aliases\x12\x18\n\x10short_channel_id\x18\x03 \x01(\t\x12\x11\n\tdirection\x18\x04 \x01(\r\x12\x12\n\nchannel_id\x18\x05 \x01(\t\x12\x14\n\x0c\x66unding_txid\x18\x06 \x01(\t\x12\x15\n\rclose_to_addr\x18\x07 \x01(\t\x12\x10\n\x08\x63lose_to\x18\x08 \x01(\t\x12\x0f\n\x07private\x18\t \x01(\x08\x12\r\n\x05total\x18\n \x01(\t\x12\x12\n\ndust_limit\x18\x0b \x01(\t\x12\x11\n\tspendable\x18\x0c \x01(\t\x12\x12\n\nreceivable\x18\r \x01(\t\x12\x1b\n\x13their_to_self_delay\x18\x0e \x01(\r\x12\x19\n\x11our_to_self_delay\x18\x0f \x01(\r\x12\x0e\n\x06status\x18\x10 \x03(\t\x12\x1f\n\x05htlcs\x18\x11 \x03(\x0b\x32\x10.greenlight.Htlc\"\x86\x01\n\x04Peer\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x11\n\tconnected\x18\x02 \x01(\x08\x12&\n\taddresses\x18\x03 \x03(\x0b\x32\x13.greenlight.Address\x12\x10\n\x08\x66\x65\x61tures\x18\x04 \x01(\t\x12%\n\x08\x63hannels\x18\x05 \x03(\x0b\x32\x13.greenlight.Channel\"4\n\x11ListPeersResponse\x12\x1f\n\x05peers\x18\x01 \x03(\x0b\x32\x10.greenlight.Peer\"3\n\x11\x44isconnectRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\x14\n\x12\x44isconnectResponse\"B\n\x0eNewAddrRequest\x12\x30\n\x0c\x61\x64\x64ress_type\x18\x01 \x01(\x0e\x32\x1a.greenlight.BtcAddressType\"T\n\x0fNewAddrResponse\x12\x30\n\x0c\x61\x64\x64ress_type\x18\x01 \x01(\x0e\x32\x1a.greenlight.BtcAddressType\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\"=\n\x10ListFundsRequest\x12)\n\x07minconf\x18\x01 \x01(\x0b\x32\x18.greenlight.Confirmation\"\xc3\x01\n\x0fListFundsOutput\x12$\n\x06output\x18\x01 \x01(\x0b\x32\x14.greenlight.Outpoint\x12\"\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x12.greenlight.Amount\x12\x0f\n\x07\x61\x64\x64ress\x18\x04 \x01(\t\x12(\n\x06status\x18\x05 \x01(\x0e\x32\x18.greenlight.OutputStatus\x12\x10\n\x08reserved\x18\x06 \x01(\x08\x12\x19\n\x11reserved_to_block\x18\x07 \x01(\r\"\xac\x01\n\x10ListFundsChannel\x12\x0f\n\x07peer_id\x18\x01 \x01(\x0c\x12\x11\n\tconnected\x18\x02 \x01(\x08\x12\x18\n\x10short_channel_id\x18\x03 \x01(\x04\x12\x17\n\x0four_amount_msat\x18\x04 \x01(\x04\x12\x13\n\x0b\x61mount_msat\x18\x05 \x01(\x04\x12\x14\n\x0c\x66unding_txid\x18\x06 \x01(\x0c\x12\x16\n\x0e\x66unding_output\x18\x07 \x01(\r\"q\n\x11ListFundsResponse\x12,\n\x07outputs\x18\x01 \x03(\x0b\x32\x1b.greenlight.ListFundsOutput\x12.\n\x08\x63hannels\x18\x02 \x03(\x0b\x32\x1c.greenlight.ListFundsChannel\"a\n\x07\x46\x65\x65rate\x12+\n\x06preset\x18\x01 \x01(\x0e\x32\x19.greenlight.FeeratePresetH\x00\x12\x0f\n\x05perkw\x18\x05 \x01(\x04H\x00\x12\x0f\n\x05perkb\x18\x06 \x01(\x04H\x00\x42\x07\n\x05value\"\x1e\n\x0c\x43onfirmation\x12\x0e\n\x06\x62locks\x18\x01 \x01(\r\"\xc0\x01\n\x0fWithdrawRequest\x12\x13\n\x0b\x64\x65stination\x18\x01 \x01(\t\x12\"\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x12.greenlight.Amount\x12$\n\x07\x66\x65\x65rate\x18\x03 \x01(\x0b\x32\x13.greenlight.Feerate\x12)\n\x07minconf\x18\x07 \x01(\x0b\x32\x18.greenlight.Confirmation\x12#\n\x05utxos\x18\x08 \x03(\x0b\x32\x14.greenlight.Outpoint\",\n\x10WithdrawResponse\x12\n\n\x02tx\x18\x01 \x01(\x0c\x12\x0c\n\x04txid\x18\x02 \x01(\x0c\"\xbe\x01\n\x12\x46undChannelRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\x0c\x12\"\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x12.greenlight.Amount\x12$\n\x07\x66\x65\x65rate\x18\x03 \x01(\x0b\x32\x13.greenlight.Feerate\x12\x10\n\x08\x61nnounce\x18\x07 \x01(\x08\x12)\n\x07minconf\x18\x08 \x01(\x0b\x32\x18.greenlight.Confirmation\x12\x10\n\x08\x63lose_to\x18\n \x01(\t\"(\n\x08Outpoint\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\x12\x0e\n\x06outnum\x18\x02 \x01(\r\"o\n\x13\x46undChannelResponse\x12\n\n\x02tx\x18\x01 \x01(\x0c\x12&\n\x08outpoint\x18\x02 \x01(\x0b\x32\x14.greenlight.Outpoint\x12\x12\n\nchannel_id\x18\x03 \x01(\x0c\x12\x10\n\x08\x63lose_to\x18\x04 \x01(\t\"\x1a\n\x07Timeout\x12\x0f\n\x07seconds\x18\x01 \x01(\r\"!\n\x0e\x42itcoinAddress\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\"\x87\x01\n\x13\x43loseChannelRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\x0c\x12.\n\x11unilateraltimeout\x18\x02 \x01(\x0b\x32\x13.greenlight.Timeout\x12/\n\x0b\x64\x65stination\x18\x03 \x01(\x0b\x32\x1a.greenlight.BitcoinAddress\"b\n\x14\x43loseChannelResponse\x12\x30\n\nclose_type\x18\x01 \x01(\x0e\x32\x1c.greenlight.CloseChannelType\x12\n\n\x02tx\x18\x02 \x01(\x0c\x12\x0c\n\x04txid\x18\x03 \x01(\x0c\"l\n\x06\x41mount\x12\x16\n\x0cmillisatoshi\x18\x01 \x01(\x04H\x00\x12\x11\n\x07satoshi\x18\x02 \x01(\x04H\x00\x12\x11\n\x07\x62itcoin\x18\x03 \x01(\x04H\x00\x12\r\n\x03\x61ll\x18\x04 \x01(\x08H\x00\x12\r\n\x03\x61ny\x18\x05 \x01(\x08H\x00\x42\x06\n\x04unit\"j\n\x0eInvoiceRequest\x12\"\n\x06\x61mount\x18\x01 \x01(\x0b\x32\x12.greenlight.Amount\x12\r\n\x05label\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x10\n\x08preimage\x18\x04 \x01(\x0c\"\x8d\x02\n\x07Invoice\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\"\n\x06\x61mount\x18\x03 \x01(\x0b\x32\x12.greenlight.Amount\x12$\n\x08received\x18\x04 \x01(\x0b\x32\x12.greenlight.Amount\x12)\n\x06status\x18\x05 \x01(\x0e\x32\x19.greenlight.InvoiceStatus\x12\x14\n\x0cpayment_time\x18\x06 \x01(\r\x12\x13\n\x0b\x65xpiry_time\x18\x07 \x01(\r\x12\x0e\n\x06\x62olt11\x18\x08 \x01(\t\x12\x14\n\x0cpayment_hash\x18\t \x01(\x0c\x12\x18\n\x10payment_preimage\x18\n \x01(\x0c\"\x8c\x01\n\nPayRequest\x12\x0e\n\x06\x62olt11\x18\x01 \x01(\t\x12\"\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x12.greenlight.Amount\x12\x0f\n\x07timeout\x18\x03 \x01(\r\x12\x15\n\rmaxfeepercent\x18\x04 \x01(\x01\x12\"\n\x06maxfee\x18\x05 \x01(\x0b\x32\x12.greenlight.Amount\"\xfc\x01\n\x07Payment\x12\x13\n\x0b\x64\x65stination\x18\x01 \x01(\x0c\x12\x14\n\x0cpayment_hash\x18\x02 \x01(\x0c\x12\x18\n\x10payment_preimage\x18\x03 \x01(\x0c\x12%\n\x06status\x18\x04 \x01(\x0e\x32\x15.greenlight.PayStatus\x12\"\n\x06\x61mount\x18\x05 \x01(\x0b\x32\x12.greenlight.Amount\x12\'\n\x0b\x61mount_sent\x18\x06 \x01(\x0b\x32\x12.greenlight.Amount\x12\x0e\n\x06\x62olt11\x18\x07 \x01(\t\x12\x12\n\ncreated_at\x18\x08 \x01(\x01\x12\x14\n\x0c\x63ompleted_at\x18\t \x01(\x04\"C\n\x11PaymentIdentifier\x12\x10\n\x06\x62olt11\x18\x01 \x01(\tH\x00\x12\x16\n\x0cpayment_hash\x18\x02 \x01(\x0cH\x00\x42\x04\n\x02id\"H\n\x13ListPaymentsRequest\x12\x31\n\nidentifier\x18\x01 \x01(\x0b\x32\x1d.greenlight.PaymentIdentifier\"=\n\x14ListPaymentsResponse\x12%\n\x08payments\x18\x01 \x03(\x0b\x32\x13.greenlight.Payment\"W\n\x11InvoiceIdentifier\x12\x0f\n\x05label\x18\x01 \x01(\tH\x00\x12\x13\n\tinvstring\x18\x02 \x01(\tH\x00\x12\x16\n\x0cpayment_hash\x18\x03 \x01(\x0cH\x00\x42\x04\n\x02id\"H\n\x13ListInvoicesRequest\x12\x31\n\nidentifier\x18\x01 \x01(\x0b\x32\x1d.greenlight.InvoiceIdentifier\"\x16\n\x14StreamIncomingFilter\"=\n\x14ListInvoicesResponse\x12%\n\x08invoices\x18\x01 \x03(\x0b\x32\x13.greenlight.Invoice\"\'\n\x08TlvField\x12\x0c\n\x04type\x18\x01 \x01(\x04\x12\r\n\x05value\x18\x02 \x01(\x0c\"\xa5\x01\n\x0fOffChainPayment\x12\r\n\x05label\x18\x01 \x01(\t\x12\x10\n\x08preimage\x18\x02 \x01(\x0c\x12\"\n\x06\x61mount\x18\x03 \x01(\x0b\x32\x12.greenlight.Amount\x12\'\n\textratlvs\x18\x04 \x03(\x0b\x32\x14.greenlight.TlvField\x12\x14\n\x0cpayment_hash\x18\x05 \x01(\x0c\x12\x0e\n\x06\x62olt11\x18\x06 \x01(\t\"M\n\x0fIncomingPayment\x12/\n\x08offchain\x18\x01 \x01(\x0b\x32\x1b.greenlight.OffChainPaymentH\x00\x42\t\n\x07\x64\x65tails\"x\n\x0cRoutehintHop\x12\x0f\n\x07node_id\x18\x01 \x01(\x0c\x12\x18\n\x10short_channel_id\x18\x02 \x01(\t\x12\x10\n\x08\x66\x65\x65_base\x18\x03 \x01(\x04\x12\x10\n\x08\x66\x65\x65_prop\x18\x04 \x01(\r\x12\x19\n\x11\x63ltv_expiry_delta\x18\x05 \x01(\r\"3\n\tRoutehint\x12&\n\x04hops\x18\x01 \x03(\x0b\x32\x18.greenlight.RoutehintHop\"\xa8\x01\n\x0eKeysendRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\x0c\x12\"\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x12.greenlight.Amount\x12\r\n\x05label\x18\x03 \x01(\t\x12)\n\nroutehints\x18\x04 \x03(\x0b\x32\x15.greenlight.Routehint\x12\'\n\textratlvs\x18\x05 \x03(\x0b\x32\x14.greenlight.TlvField\"\x12\n\x10StreamLogRequest\"\x18\n\x08LogEntry\x12\x0c\n\x04line\x18\x01 \x01(\t\"?\n\x10SignerStateEntry\x12\x0f\n\x07version\x18\x01 \x01(\x04\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x0c\"Q\n\x0ePendingRequest\x12\x0f\n\x07request\x18\x01 \x01(\x0c\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x11\n\tsignature\x18\x03 \x01(\x0c\x12\x0e\n\x06pubkey\x18\x04 \x01(\x0c\"=\n\nNodeConfig\x12/\n\x0bstartupmsgs\x18\x01 \x03(\x0b\x32\x1a.greenlight.StartupMessage\"3\n\x0eStartupMessage\x12\x0f\n\x07request\x18\x01 \x01(\x0c\x12\x10\n\x08response\x18\x02 \x01(\x0c*:\n\x0eNetAddressType\x12\x08\n\x04Ipv4\x10\x00\x12\x08\n\x04Ipv6\x10\x01\x12\t\n\x05TorV2\x10\x02\x12\t\n\x05TorV3\x10\x03*-\n\x0e\x42tcAddressType\x12\n\n\x06\x42\x45\x43H32\x10\x00\x12\x0f\n\x0bP2SH_SEGWIT\x10\x01*.\n\x0cOutputStatus\x12\r\n\tCONFIRMED\x10\x00\x12\x0f\n\x0bUNCONFIRMED\x10\x01*1\n\rFeeratePreset\x12\n\n\x06NORMAL\x10\x00\x12\x08\n\x04SLOW\x10\x01\x12\n\n\x06URGENT\x10\x02*.\n\x10\x43loseChannelType\x12\n\n\x06MUTUAL\x10\x00\x12\x0e\n\nUNILATERAL\x10\x01*2\n\rInvoiceStatus\x12\n\n\x06UNPAID\x10\x00\x12\x08\n\x04PAID\x10\x01\x12\x0b\n\x07\x45XPIRED\x10\x02*2\n\tPayStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x43OMPLETE\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\x32\xf3\n\n\x04Node\x12\x44\n\x07GetInfo\x12\x1a.greenlight.GetInfoRequest\x1a\x1b.greenlight.GetInfoResponse\"\x00\x12;\n\x04Stop\x12\x17.greenlight.StopRequest\x1a\x18.greenlight.StopResponse\"\x00\x12H\n\x0b\x43onnectPeer\x12\x1a.greenlight.ConnectRequest\x1a\x1b.greenlight.ConnectResponse\"\x00\x12J\n\tListPeers\x12\x1c.greenlight.ListPeersRequest\x1a\x1d.greenlight.ListPeersResponse\"\x00\x12M\n\nDisconnect\x12\x1d.greenlight.DisconnectRequest\x1a\x1e.greenlight.DisconnectResponse\"\x00\x12\x44\n\x07NewAddr\x12\x1a.greenlight.NewAddrRequest\x1a\x1b.greenlight.NewAddrResponse\"\x00\x12J\n\tListFunds\x12\x1c.greenlight.ListFundsRequest\x1a\x1d.greenlight.ListFundsResponse\"\x00\x12G\n\x08Withdraw\x12\x1b.greenlight.WithdrawRequest\x1a\x1c.greenlight.WithdrawResponse\"\x00\x12P\n\x0b\x46undChannel\x12\x1e.greenlight.FundChannelRequest\x1a\x1f.greenlight.FundChannelResponse\"\x00\x12S\n\x0c\x43loseChannel\x12\x1f.greenlight.CloseChannelRequest\x1a .greenlight.CloseChannelResponse\"\x00\x12\x42\n\rCreateInvoice\x12\x1a.greenlight.InvoiceRequest\x1a\x13.greenlight.Invoice\"\x00\x12\x34\n\x03Pay\x12\x16.greenlight.PayRequest\x1a\x13.greenlight.Payment\"\x00\x12<\n\x07Keysend\x12\x1a.greenlight.KeysendRequest\x1a\x13.greenlight.Payment\"\x00\x12S\n\x0cListPayments\x12\x1f.greenlight.ListPaymentsRequest\x1a .greenlight.ListPaymentsResponse\"\x00\x12S\n\x0cListInvoices\x12\x1f.greenlight.ListInvoicesRequest\x1a .greenlight.ListInvoicesResponse\"\x00\x12S\n\x0eStreamIncoming\x12 .greenlight.StreamIncomingFilter\x1a\x1b.greenlight.IncomingPayment\"\x00\x30\x01\x12\x43\n\tStreamLog\x12\x1c.greenlight.StreamLogRequest\x1a\x14.greenlight.LogEntry\"\x00\x30\x01\x12\x42\n\x11StreamHsmRequests\x12\x11.greenlight.Empty\x1a\x16.greenlight.HsmRequest\"\x00\x30\x01\x12\x41\n\x11RespondHsmRequest\x12\x17.greenlight.HsmResponse\x1a\x11.greenlight.Empty\"\x00\x32s\n\x03Hsm\x12<\n\x07Request\x12\x16.greenlight.HsmRequest\x1a\x17.greenlight.HsmResponse\"\x00\x12.\n\x04Ping\x12\x11.greenlight.Empty\x1a\x11.greenlight.Empty\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10greenlight.proto\x12\ngreenlight\"H\n\x11HsmRequestContext\x12\x0f\n\x07node_id\x18\x01 \x01(\x0c\x12\x0c\n\x04\x64\x62id\x18\x02 \x01(\x04\x12\x14\n\x0c\x63\x61pabilities\x18\x03 \x01(\x04\"b\n\x0bHsmResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\r\x12\x0b\n\x03raw\x18\x02 \x01(\x0c\x12\x32\n\x0csigner_state\x18\x05 \x03(\x0b\x32\x1c.greenlight.SignerStateEntry\"\xbf\x01\n\nHsmRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\r\x12.\n\x07\x63ontext\x18\x02 \x01(\x0b\x32\x1d.greenlight.HsmRequestContext\x12\x0b\n\x03raw\x18\x03 \x01(\x0c\x12\x32\n\x0csigner_state\x18\x04 \x03(\x0b\x32\x1c.greenlight.SignerStateEntry\x12,\n\x08requests\x18\x05 \x03(\x0b\x32\x1a.greenlight.PendingRequest\"\x07\n\x05\x45mpty\"O\n\x07\x41\x64\x64ress\x12(\n\x04type\x18\x01 \x01(\x0e\x32\x1a.greenlight.NetAddressType\x12\x0c\n\x04\x61\x64\x64r\x18\x02 \x01(\t\x12\x0c\n\x04port\x18\x03 \x01(\r\"\x10\n\x0eGetInfoRequest\"\xb2\x01\n\x0fGetInfoResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\x0c\x12\r\n\x05\x61lias\x18\x02 \x01(\t\x12\r\n\x05\x63olor\x18\x03 \x01(\x0c\x12\x11\n\tnum_peers\x18\x04 \x01(\r\x12&\n\taddresses\x18\x05 \x03(\x0b\x32\x13.greenlight.Address\x12\x0f\n\x07version\x18\x06 \x01(\t\x12\x13\n\x0b\x62lockheight\x18\x07 \x01(\r\x12\x0f\n\x07network\x18\x08 \x01(\t\"\r\n\x0bStopRequest\"\x0e\n\x0cStopResponse\"/\n\x0e\x43onnectRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x0c\n\x04\x61\x64\x64r\x18\x02 \x01(\t\"4\n\x0f\x43onnectResponse\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\x10\n\x08\x66\x65\x61tures\x18\x02 \x01(\t\"#\n\x10ListPeersRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\"\x81\x01\n\x04Htlc\x12\x11\n\tdirection\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x04\x12\x0e\n\x06\x61mount\x18\x03 \x01(\t\x12\x0e\n\x06\x65xpiry\x18\x04 \x01(\x04\x12\x14\n\x0cpayment_hash\x18\x05 \x01(\t\x12\r\n\x05state\x18\x06 \x01(\t\x12\x15\n\rlocal_trimmed\x18\x07 \x01(\x08\"(\n\x07\x41liases\x12\r\n\x05local\x18\x01 \x01(\t\x12\x0e\n\x06remote\x18\x02 \x01(\t\"\x8f\x03\n\x07\x43hannel\x12\r\n\x05state\x18\x01 \x01(\t\x12\r\n\x05owner\x18\x02 \x01(\t\x12\"\n\x05\x61lias\x18\x12 \x01(\x0b\x32\x13.greenlight.Aliases\x12\x18\n\x10short_channel_id\x18\x03 \x01(\t\x12\x11\n\tdirection\x18\x04 \x01(\r\x12\x12\n\nchannel_id\x18\x05 \x01(\t\x12\x14\n\x0c\x66unding_txid\x18\x06 \x01(\t\x12\x15\n\rclose_to_addr\x18\x07 \x01(\t\x12\x10\n\x08\x63lose_to\x18\x08 \x01(\t\x12\x0f\n\x07private\x18\t \x01(\x08\x12\r\n\x05total\x18\n \x01(\t\x12\x12\n\ndust_limit\x18\x0b \x01(\t\x12\x11\n\tspendable\x18\x0c \x01(\t\x12\x12\n\nreceivable\x18\r \x01(\t\x12\x1b\n\x13their_to_self_delay\x18\x0e \x01(\r\x12\x19\n\x11our_to_self_delay\x18\x0f \x01(\r\x12\x0e\n\x06status\x18\x10 \x03(\t\x12\x1f\n\x05htlcs\x18\x11 \x03(\x0b\x32\x10.greenlight.Htlc\"\x86\x01\n\x04Peer\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x11\n\tconnected\x18\x02 \x01(\x08\x12&\n\taddresses\x18\x03 \x03(\x0b\x32\x13.greenlight.Address\x12\x10\n\x08\x66\x65\x61tures\x18\x04 \x01(\t\x12%\n\x08\x63hannels\x18\x05 \x03(\x0b\x32\x13.greenlight.Channel\"4\n\x11ListPeersResponse\x12\x1f\n\x05peers\x18\x01 \x03(\x0b\x32\x10.greenlight.Peer\"3\n\x11\x44isconnectRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\x14\n\x12\x44isconnectResponse\"B\n\x0eNewAddrRequest\x12\x30\n\x0c\x61\x64\x64ress_type\x18\x01 \x01(\x0e\x32\x1a.greenlight.BtcAddressType\"T\n\x0fNewAddrResponse\x12\x30\n\x0c\x61\x64\x64ress_type\x18\x01 \x01(\x0e\x32\x1a.greenlight.BtcAddressType\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\"=\n\x10ListFundsRequest\x12)\n\x07minconf\x18\x01 \x01(\x0b\x32\x18.greenlight.Confirmation\"\xc3\x01\n\x0fListFundsOutput\x12$\n\x06output\x18\x01 \x01(\x0b\x32\x14.greenlight.Outpoint\x12\"\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x12.greenlight.Amount\x12\x0f\n\x07\x61\x64\x64ress\x18\x04 \x01(\t\x12(\n\x06status\x18\x05 \x01(\x0e\x32\x18.greenlight.OutputStatus\x12\x10\n\x08reserved\x18\x06 \x01(\x08\x12\x19\n\x11reserved_to_block\x18\x07 \x01(\r\"\xac\x01\n\x10ListFundsChannel\x12\x0f\n\x07peer_id\x18\x01 \x01(\x0c\x12\x11\n\tconnected\x18\x02 \x01(\x08\x12\x18\n\x10short_channel_id\x18\x03 \x01(\x04\x12\x17\n\x0four_amount_msat\x18\x04 \x01(\x04\x12\x13\n\x0b\x61mount_msat\x18\x05 \x01(\x04\x12\x14\n\x0c\x66unding_txid\x18\x06 \x01(\x0c\x12\x16\n\x0e\x66unding_output\x18\x07 \x01(\r\"q\n\x11ListFundsResponse\x12,\n\x07outputs\x18\x01 \x03(\x0b\x32\x1b.greenlight.ListFundsOutput\x12.\n\x08\x63hannels\x18\x02 \x03(\x0b\x32\x1c.greenlight.ListFundsChannel\"a\n\x07\x46\x65\x65rate\x12+\n\x06preset\x18\x01 \x01(\x0e\x32\x19.greenlight.FeeratePresetH\x00\x12\x0f\n\x05perkw\x18\x05 \x01(\x04H\x00\x12\x0f\n\x05perkb\x18\x06 \x01(\x04H\x00\x42\x07\n\x05value\"\x1e\n\x0c\x43onfirmation\x12\x0e\n\x06\x62locks\x18\x01 \x01(\r\"\xc0\x01\n\x0fWithdrawRequest\x12\x13\n\x0b\x64\x65stination\x18\x01 \x01(\t\x12\"\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x12.greenlight.Amount\x12$\n\x07\x66\x65\x65rate\x18\x03 \x01(\x0b\x32\x13.greenlight.Feerate\x12)\n\x07minconf\x18\x07 \x01(\x0b\x32\x18.greenlight.Confirmation\x12#\n\x05utxos\x18\x08 \x03(\x0b\x32\x14.greenlight.Outpoint\",\n\x10WithdrawResponse\x12\n\n\x02tx\x18\x01 \x01(\x0c\x12\x0c\n\x04txid\x18\x02 \x01(\x0c\"\xbe\x01\n\x12\x46undChannelRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\x0c\x12\"\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x12.greenlight.Amount\x12$\n\x07\x66\x65\x65rate\x18\x03 \x01(\x0b\x32\x13.greenlight.Feerate\x12\x10\n\x08\x61nnounce\x18\x07 \x01(\x08\x12)\n\x07minconf\x18\x08 \x01(\x0b\x32\x18.greenlight.Confirmation\x12\x10\n\x08\x63lose_to\x18\n \x01(\t\"(\n\x08Outpoint\x12\x0c\n\x04txid\x18\x01 \x01(\x0c\x12\x0e\n\x06outnum\x18\x02 \x01(\r\"o\n\x13\x46undChannelResponse\x12\n\n\x02tx\x18\x01 \x01(\x0c\x12&\n\x08outpoint\x18\x02 \x01(\x0b\x32\x14.greenlight.Outpoint\x12\x12\n\nchannel_id\x18\x03 \x01(\x0c\x12\x10\n\x08\x63lose_to\x18\x04 \x01(\t\"\x1a\n\x07Timeout\x12\x0f\n\x07seconds\x18\x01 \x01(\r\"!\n\x0e\x42itcoinAddress\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\"\x87\x01\n\x13\x43loseChannelRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\x0c\x12.\n\x11unilateraltimeout\x18\x02 \x01(\x0b\x32\x13.greenlight.Timeout\x12/\n\x0b\x64\x65stination\x18\x03 \x01(\x0b\x32\x1a.greenlight.BitcoinAddress\"b\n\x14\x43loseChannelResponse\x12\x30\n\nclose_type\x18\x01 \x01(\x0e\x32\x1c.greenlight.CloseChannelType\x12\n\n\x02tx\x18\x02 \x01(\x0c\x12\x0c\n\x04txid\x18\x03 \x01(\x0c\"l\n\x06\x41mount\x12\x16\n\x0cmillisatoshi\x18\x01 \x01(\x04H\x00\x12\x11\n\x07satoshi\x18\x02 \x01(\x04H\x00\x12\x11\n\x07\x62itcoin\x18\x03 \x01(\x04H\x00\x12\r\n\x03\x61ll\x18\x04 \x01(\x08H\x00\x12\r\n\x03\x61ny\x18\x05 \x01(\x08H\x00\x42\x06\n\x04unit\"j\n\x0eInvoiceRequest\x12\"\n\x06\x61mount\x18\x01 \x01(\x0b\x32\x12.greenlight.Amount\x12\r\n\x05label\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x10\n\x08preimage\x18\x04 \x01(\x0c\"\x8d\x02\n\x07Invoice\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\"\n\x06\x61mount\x18\x03 \x01(\x0b\x32\x12.greenlight.Amount\x12$\n\x08received\x18\x04 \x01(\x0b\x32\x12.greenlight.Amount\x12)\n\x06status\x18\x05 \x01(\x0e\x32\x19.greenlight.InvoiceStatus\x12\x14\n\x0cpayment_time\x18\x06 \x01(\r\x12\x13\n\x0b\x65xpiry_time\x18\x07 \x01(\r\x12\x0e\n\x06\x62olt11\x18\x08 \x01(\t\x12\x14\n\x0cpayment_hash\x18\t \x01(\x0c\x12\x18\n\x10payment_preimage\x18\n \x01(\x0c\"\x8c\x01\n\nPayRequest\x12\x0e\n\x06\x62olt11\x18\x01 \x01(\t\x12\"\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x12.greenlight.Amount\x12\x0f\n\x07timeout\x18\x03 \x01(\r\x12\x15\n\rmaxfeepercent\x18\x04 \x01(\x01\x12\"\n\x06maxfee\x18\x05 \x01(\x0b\x32\x12.greenlight.Amount\"\xfc\x01\n\x07Payment\x12\x13\n\x0b\x64\x65stination\x18\x01 \x01(\x0c\x12\x14\n\x0cpayment_hash\x18\x02 \x01(\x0c\x12\x18\n\x10payment_preimage\x18\x03 \x01(\x0c\x12%\n\x06status\x18\x04 \x01(\x0e\x32\x15.greenlight.PayStatus\x12\"\n\x06\x61mount\x18\x05 \x01(\x0b\x32\x12.greenlight.Amount\x12\'\n\x0b\x61mount_sent\x18\x06 \x01(\x0b\x32\x12.greenlight.Amount\x12\x0e\n\x06\x62olt11\x18\x07 \x01(\t\x12\x12\n\ncreated_at\x18\x08 \x01(\x01\x12\x14\n\x0c\x63ompleted_at\x18\t \x01(\x04\"C\n\x11PaymentIdentifier\x12\x10\n\x06\x62olt11\x18\x01 \x01(\tH\x00\x12\x16\n\x0cpayment_hash\x18\x02 \x01(\x0cH\x00\x42\x04\n\x02id\"H\n\x13ListPaymentsRequest\x12\x31\n\nidentifier\x18\x01 \x01(\x0b\x32\x1d.greenlight.PaymentIdentifier\"=\n\x14ListPaymentsResponse\x12%\n\x08payments\x18\x01 \x03(\x0b\x32\x13.greenlight.Payment\"W\n\x11InvoiceIdentifier\x12\x0f\n\x05label\x18\x01 \x01(\tH\x00\x12\x13\n\tinvstring\x18\x02 \x01(\tH\x00\x12\x16\n\x0cpayment_hash\x18\x03 \x01(\x0cH\x00\x42\x04\n\x02id\"H\n\x13ListInvoicesRequest\x12\x31\n\nidentifier\x18\x01 \x01(\x0b\x32\x1d.greenlight.InvoiceIdentifier\"\x16\n\x14StreamIncomingFilter\"=\n\x14ListInvoicesResponse\x12%\n\x08invoices\x18\x01 \x03(\x0b\x32\x13.greenlight.Invoice\"\'\n\x08TlvField\x12\x0c\n\x04type\x18\x01 \x01(\x04\x12\r\n\x05value\x18\x02 \x01(\x0c\"\xa5\x01\n\x0fOffChainPayment\x12\r\n\x05label\x18\x01 \x01(\t\x12\x10\n\x08preimage\x18\x02 \x01(\x0c\x12\"\n\x06\x61mount\x18\x03 \x01(\x0b\x32\x12.greenlight.Amount\x12\'\n\textratlvs\x18\x04 \x03(\x0b\x32\x14.greenlight.TlvField\x12\x14\n\x0cpayment_hash\x18\x05 \x01(\x0c\x12\x0e\n\x06\x62olt11\x18\x06 \x01(\t\"M\n\x0fIncomingPayment\x12/\n\x08offchain\x18\x01 \x01(\x0b\x32\x1b.greenlight.OffChainPaymentH\x00\x42\t\n\x07\x64\x65tails\"x\n\x0cRoutehintHop\x12\x0f\n\x07node_id\x18\x01 \x01(\x0c\x12\x18\n\x10short_channel_id\x18\x02 \x01(\t\x12\x10\n\x08\x66\x65\x65_base\x18\x03 \x01(\x04\x12\x10\n\x08\x66\x65\x65_prop\x18\x04 \x01(\r\x12\x19\n\x11\x63ltv_expiry_delta\x18\x05 \x01(\r\"3\n\tRoutehint\x12&\n\x04hops\x18\x01 \x03(\x0b\x32\x18.greenlight.RoutehintHop\"\xa8\x01\n\x0eKeysendRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\x0c\x12\"\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x12.greenlight.Amount\x12\r\n\x05label\x18\x03 \x01(\t\x12)\n\nroutehints\x18\x04 \x03(\x0b\x32\x15.greenlight.Routehint\x12\'\n\textratlvs\x18\x05 \x03(\x0b\x32\x14.greenlight.TlvField\"\x12\n\x10StreamLogRequest\"\x18\n\x08LogEntry\x12\x0c\n\x04line\x18\x01 \x01(\t\"?\n\x10SignerStateEntry\x12\x0f\n\x07version\x18\x01 \x01(\x04\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x0c\"d\n\x0ePendingRequest\x12\x0f\n\x07request\x18\x01 \x01(\x0c\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x11\n\tsignature\x18\x03 \x01(\x0c\x12\x0e\n\x06pubkey\x18\x04 \x01(\x0c\x12\x11\n\ttimestamp\x18\x05 \x01(\x04\"=\n\nNodeConfig\x12/\n\x0bstartupmsgs\x18\x01 \x03(\x0b\x32\x1a.greenlight.StartupMessage\"3\n\x0eStartupMessage\x12\x0f\n\x07request\x18\x01 \x01(\x0c\x12\x10\n\x08response\x18\x02 \x01(\x0c\"\x18\n\x16StreamCustommsgRequest\"-\n\tCustommsg\x12\x0f\n\x07peer_id\x18\x01 \x01(\x0c\x12\x0f\n\x07payload\x18\x02 \x01(\x0c*:\n\x0eNetAddressType\x12\x08\n\x04Ipv4\x10\x00\x12\x08\n\x04Ipv6\x10\x01\x12\t\n\x05TorV2\x10\x02\x12\t\n\x05TorV3\x10\x03*-\n\x0e\x42tcAddressType\x12\n\n\x06\x42\x45\x43H32\x10\x00\x12\x0f\n\x0bP2SH_SEGWIT\x10\x01*.\n\x0cOutputStatus\x12\r\n\tCONFIRMED\x10\x00\x12\x0f\n\x0bUNCONFIRMED\x10\x01*1\n\rFeeratePreset\x12\n\n\x06NORMAL\x10\x00\x12\x08\n\x04SLOW\x10\x01\x12\n\n\x06URGENT\x10\x02*.\n\x10\x43loseChannelType\x12\n\n\x06MUTUAL\x10\x00\x12\x0e\n\nUNILATERAL\x10\x01*2\n\rInvoiceStatus\x12\n\n\x06UNPAID\x10\x00\x12\x08\n\x04PAID\x10\x01\x12\x0b\n\x07\x45XPIRED\x10\x02*2\n\tPayStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x43OMPLETE\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\x32\xec\x0b\n\x04Node\x12G\n\x07GetInfo\x12\x1a.greenlight.GetInfoRequest\x1a\x1b.greenlight.GetInfoResponse\"\x03\x88\x02\x01\x12>\n\x04Stop\x12\x17.greenlight.StopRequest\x1a\x18.greenlight.StopResponse\"\x03\x88\x02\x01\x12K\n\x0b\x43onnectPeer\x12\x1a.greenlight.ConnectRequest\x1a\x1b.greenlight.ConnectResponse\"\x03\x88\x02\x01\x12M\n\tListPeers\x12\x1c.greenlight.ListPeersRequest\x1a\x1d.greenlight.ListPeersResponse\"\x03\x88\x02\x01\x12P\n\nDisconnect\x12\x1d.greenlight.DisconnectRequest\x1a\x1e.greenlight.DisconnectResponse\"\x03\x88\x02\x01\x12G\n\x07NewAddr\x12\x1a.greenlight.NewAddrRequest\x1a\x1b.greenlight.NewAddrResponse\"\x03\x88\x02\x01\x12M\n\tListFunds\x12\x1c.greenlight.ListFundsRequest\x1a\x1d.greenlight.ListFundsResponse\"\x03\x88\x02\x01\x12J\n\x08Withdraw\x12\x1b.greenlight.WithdrawRequest\x1a\x1c.greenlight.WithdrawResponse\"\x03\x88\x02\x01\x12S\n\x0b\x46undChannel\x12\x1e.greenlight.FundChannelRequest\x1a\x1f.greenlight.FundChannelResponse\"\x03\x88\x02\x01\x12V\n\x0c\x43loseChannel\x12\x1f.greenlight.CloseChannelRequest\x1a .greenlight.CloseChannelResponse\"\x03\x88\x02\x01\x12\x45\n\rCreateInvoice\x12\x1a.greenlight.InvoiceRequest\x1a\x13.greenlight.Invoice\"\x03\x88\x02\x01\x12\x37\n\x03Pay\x12\x16.greenlight.PayRequest\x1a\x13.greenlight.Payment\"\x03\x88\x02\x01\x12?\n\x07Keysend\x12\x1a.greenlight.KeysendRequest\x1a\x13.greenlight.Payment\"\x03\x88\x02\x01\x12S\n\x0cListPayments\x12\x1f.greenlight.ListPaymentsRequest\x1a .greenlight.ListPaymentsResponse\"\x00\x12S\n\x0cListInvoices\x12\x1f.greenlight.ListInvoicesRequest\x1a .greenlight.ListInvoicesResponse\"\x00\x12S\n\x0eStreamIncoming\x12 .greenlight.StreamIncomingFilter\x1a\x1b.greenlight.IncomingPayment\"\x00\x30\x01\x12\x43\n\tStreamLog\x12\x1c.greenlight.StreamLogRequest\x1a\x14.greenlight.LogEntry\"\x00\x30\x01\x12P\n\x0fStreamCustommsg\x12\".greenlight.StreamCustommsgRequest\x1a\x15.greenlight.Custommsg\"\x00\x30\x01\x12\x42\n\x11StreamHsmRequests\x12\x11.greenlight.Empty\x1a\x16.greenlight.HsmRequest\"\x00\x30\x01\x12\x41\n\x11RespondHsmRequest\x12\x17.greenlight.HsmResponse\x1a\x11.greenlight.Empty\"\x00\x32s\n\x03Hsm\x12<\n\x07Request\x12\x16.greenlight.HsmRequest\x1a\x17.greenlight.HsmResponse\"\x00\x12.\n\x04Ping\x12\x11.greenlight.Empty\x1a\x11.greenlight.Empty\"\x00\x62\x06proto3')
 
 _NETADDRESSTYPE = DESCRIPTOR.enum_types_by_name['NetAddressType']
 NetAddressType = enum_type_wrapper.EnumTypeWrapper(_NETADDRESSTYPE)
 _BTCADDRESSTYPE = DESCRIPTOR.enum_types_by_name['BtcAddressType']
 BtcAddressType = enum_type_wrapper.EnumTypeWrapper(_BTCADDRESSTYPE)
 _OUTPUTSTATUS = DESCRIPTOR.enum_types_by_name['OutputStatus']
 OutputStatus = enum_type_wrapper.EnumTypeWrapper(_OUTPUTSTATUS)
@@ -108,14 +108,16 @@
 _KEYSENDREQUEST = DESCRIPTOR.message_types_by_name['KeysendRequest']
 _STREAMLOGREQUEST = DESCRIPTOR.message_types_by_name['StreamLogRequest']
 _LOGENTRY = DESCRIPTOR.message_types_by_name['LogEntry']
 _SIGNERSTATEENTRY = DESCRIPTOR.message_types_by_name['SignerStateEntry']
 _PENDINGREQUEST = DESCRIPTOR.message_types_by_name['PendingRequest']
 _NODECONFIG = DESCRIPTOR.message_types_by_name['NodeConfig']
 _STARTUPMESSAGE = DESCRIPTOR.message_types_by_name['StartupMessage']
+_STREAMCUSTOMMSGREQUEST = DESCRIPTOR.message_types_by_name['StreamCustommsgRequest']
+_CUSTOMMSG = DESCRIPTOR.message_types_by_name['Custommsg']
 HsmRequestContext = _reflection.GeneratedProtocolMessageType('HsmRequestContext', (_message.Message,), {
   'DESCRIPTOR' : _HSMREQUESTCONTEXT,
   '__module__' : 'greenlight_pb2'
   # @@protoc_insertion_point(class_scope:greenlight.HsmRequestContext)
   })
 _sym_db.RegisterMessage(HsmRequestContext)
 
@@ -528,33 +530,73 @@
 StartupMessage = _reflection.GeneratedProtocolMessageType('StartupMessage', (_message.Message,), {
   'DESCRIPTOR' : _STARTUPMESSAGE,
   '__module__' : 'greenlight_pb2'
   # @@protoc_insertion_point(class_scope:greenlight.StartupMessage)
   })
 _sym_db.RegisterMessage(StartupMessage)
 
+StreamCustommsgRequest = _reflection.GeneratedProtocolMessageType('StreamCustommsgRequest', (_message.Message,), {
+  'DESCRIPTOR' : _STREAMCUSTOMMSGREQUEST,
+  '__module__' : 'greenlight_pb2'
+  # @@protoc_insertion_point(class_scope:greenlight.StreamCustommsgRequest)
+  })
+_sym_db.RegisterMessage(StreamCustommsgRequest)
+
+Custommsg = _reflection.GeneratedProtocolMessageType('Custommsg', (_message.Message,), {
+  'DESCRIPTOR' : _CUSTOMMSG,
+  '__module__' : 'greenlight_pb2'
+  # @@protoc_insertion_point(class_scope:greenlight.Custommsg)
+  })
+_sym_db.RegisterMessage(Custommsg)
+
 _NODE = DESCRIPTOR.services_by_name['Node']
 _HSM = DESCRIPTOR.services_by_name['Hsm']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _NETADDRESSTYPE._serialized_start=5716
-  _NETADDRESSTYPE._serialized_end=5774
-  _BTCADDRESSTYPE._serialized_start=5776
-  _BTCADDRESSTYPE._serialized_end=5821
-  _OUTPUTSTATUS._serialized_start=5823
-  _OUTPUTSTATUS._serialized_end=5869
-  _FEERATEPRESET._serialized_start=5871
-  _FEERATEPRESET._serialized_end=5920
-  _CLOSECHANNELTYPE._serialized_start=5922
-  _CLOSECHANNELTYPE._serialized_end=5968
-  _INVOICESTATUS._serialized_start=5970
-  _INVOICESTATUS._serialized_end=6020
-  _PAYSTATUS._serialized_start=6022
-  _PAYSTATUS._serialized_end=6072
+  _NODE.methods_by_name['GetInfo']._options = None
+  _NODE.methods_by_name['GetInfo']._serialized_options = b'\210\002\001'
+  _NODE.methods_by_name['Stop']._options = None
+  _NODE.methods_by_name['Stop']._serialized_options = b'\210\002\001'
+  _NODE.methods_by_name['ConnectPeer']._options = None
+  _NODE.methods_by_name['ConnectPeer']._serialized_options = b'\210\002\001'
+  _NODE.methods_by_name['ListPeers']._options = None
+  _NODE.methods_by_name['ListPeers']._serialized_options = b'\210\002\001'
+  _NODE.methods_by_name['Disconnect']._options = None
+  _NODE.methods_by_name['Disconnect']._serialized_options = b'\210\002\001'
+  _NODE.methods_by_name['NewAddr']._options = None
+  _NODE.methods_by_name['NewAddr']._serialized_options = b'\210\002\001'
+  _NODE.methods_by_name['ListFunds']._options = None
+  _NODE.methods_by_name['ListFunds']._serialized_options = b'\210\002\001'
+  _NODE.methods_by_name['Withdraw']._options = None
+  _NODE.methods_by_name['Withdraw']._serialized_options = b'\210\002\001'
+  _NODE.methods_by_name['FundChannel']._options = None
+  _NODE.methods_by_name['FundChannel']._serialized_options = b'\210\002\001'
+  _NODE.methods_by_name['CloseChannel']._options = None
+  _NODE.methods_by_name['CloseChannel']._serialized_options = b'\210\002\001'
+  _NODE.methods_by_name['CreateInvoice']._options = None
+  _NODE.methods_by_name['CreateInvoice']._serialized_options = b'\210\002\001'
+  _NODE.methods_by_name['Pay']._options = None
+  _NODE.methods_by_name['Pay']._serialized_options = b'\210\002\001'
+  _NODE.methods_by_name['Keysend']._options = None
+  _NODE.methods_by_name['Keysend']._serialized_options = b'\210\002\001'
+  _NETADDRESSTYPE._serialized_start=5808
+  _NETADDRESSTYPE._serialized_end=5866
+  _BTCADDRESSTYPE._serialized_start=5868
+  _BTCADDRESSTYPE._serialized_end=5913
+  _OUTPUTSTATUS._serialized_start=5915
+  _OUTPUTSTATUS._serialized_end=5961
+  _FEERATEPRESET._serialized_start=5963
+  _FEERATEPRESET._serialized_end=6012
+  _CLOSECHANNELTYPE._serialized_start=6014
+  _CLOSECHANNELTYPE._serialized_end=6060
+  _INVOICESTATUS._serialized_start=6062
+  _INVOICESTATUS._serialized_end=6112
+  _PAYSTATUS._serialized_start=6114
+  _PAYSTATUS._serialized_end=6164
   _HSMREQUESTCONTEXT._serialized_start=32
   _HSMREQUESTCONTEXT._serialized_end=104
   _HSMRESPONSE._serialized_start=106
   _HSMRESPONSE._serialized_end=204
   _HSMREQUEST._serialized_start=207
   _HSMREQUEST._serialized_end=398
   _EMPTY._serialized_start=400
@@ -662,17 +704,21 @@
   _STREAMLOGREQUEST._serialized_start=5406
   _STREAMLOGREQUEST._serialized_end=5424
   _LOGENTRY._serialized_start=5426
   _LOGENTRY._serialized_end=5450
   _SIGNERSTATEENTRY._serialized_start=5452
   _SIGNERSTATEENTRY._serialized_end=5515
   _PENDINGREQUEST._serialized_start=5517
-  _PENDINGREQUEST._serialized_end=5598
-  _NODECONFIG._serialized_start=5600
-  _NODECONFIG._serialized_end=5661
-  _STARTUPMESSAGE._serialized_start=5663
-  _STARTUPMESSAGE._serialized_end=5714
-  _NODE._serialized_start=6075
-  _NODE._serialized_end=7470
-  _HSM._serialized_start=7472
-  _HSM._serialized_end=7587
+  _PENDINGREQUEST._serialized_end=5617
+  _NODECONFIG._serialized_start=5619
+  _NODECONFIG._serialized_end=5680
+  _STARTUPMESSAGE._serialized_start=5682
+  _STARTUPMESSAGE._serialized_end=5733
+  _STREAMCUSTOMMSGREQUEST._serialized_start=5735
+  _STREAMCUSTOMMSGREQUEST._serialized_end=5759
+  _CUSTOMMSG._serialized_start=5761
+  _CUSTOMMSG._serialized_end=5806
+  _NODE._serialized_start=6167
+  _NODE._serialized_end=7683
+  _HSM._serialized_start=7685
+  _HSM._serialized_end=7800
 # @@protoc_insertion_point(module_scope)
```

### Comparing `gl_client-0.1.8/glclient/greenlight_pb2.pyi` & `gl_client-0.1.9/glclient/greenlight_pb2.pyi`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.8/glclient/greenlight_pb2_grpc.py` & `gl_client-0.1.9/glclient/greenlight_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     `Scheduler.Schedule()` RPC call.
 
     Notice that in order to connect to the node the caller must use the
     node-specific mTLS keypair returned by `Scheduler.Register()` or
     `Scheduler.Recover()`. In particular the anonymous mTLS keypair is
     rejected by the node.
 
+    Deprecated methods are being replaced by the standardized and
+    automatically managed cln-grpc protocol you can find in
+    `node.proto`
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -106,14 +109,19 @@
                 response_deserializer=greenlight__pb2.IncomingPayment.FromString,
                 )
         self.StreamLog = channel.unary_stream(
                 '/greenlight.Node/StreamLog',
                 request_serializer=greenlight__pb2.StreamLogRequest.SerializeToString,
                 response_deserializer=greenlight__pb2.LogEntry.FromString,
                 )
+        self.StreamCustommsg = channel.unary_stream(
+                '/greenlight.Node/StreamCustommsg',
+                request_serializer=greenlight__pb2.StreamCustommsgRequest.SerializeToString,
+                response_deserializer=greenlight__pb2.Custommsg.FromString,
+                )
         self.StreamHsmRequests = channel.unary_stream(
                 '/greenlight.Node/StreamHsmRequests',
                 request_serializer=greenlight__pb2.Empty.SerializeToString,
                 response_deserializer=greenlight__pb2.HsmRequest.FromString,
                 )
         self.RespondHsmRequest = channel.unary_unary(
                 '/greenlight.Node/RespondHsmRequest',
@@ -130,14 +138,17 @@
     `Scheduler.Schedule()` RPC call.
 
     Notice that in order to connect to the node the caller must use the
     node-specific mTLS keypair returned by `Scheduler.Register()` or
     `Scheduler.Recover()`. In particular the anonymous mTLS keypair is
     rejected by the node.
 
+    Deprecated methods are being replaced by the standardized and
+    automatically managed cln-grpc protocol you can find in
+    `node.proto`
     """
 
     def GetInfo(self, request, context):
         """Retrieve general information about the node.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
@@ -282,14 +293,24 @@
         be rather large, and should not be streamed onto
         resource-constrained devices.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def StreamCustommsg(self, request, context):
+        """Listen for incoming `custommsg` messages from peers.
+
+        The messages are forwarded as they come in, and will not be
+        replayed if the stream is interrupted.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def StreamHsmRequests(self, request, context):
         """////////////////////////////// HSM Messages ////////////////////////
 
         The following messages are related to communicating HSM
         requests back and forth. Chances are you won't need to
         interact with these at all, unless you want to embed the
         hsmd into your client. We recommend using a standalone hsmd
@@ -392,14 +413,19 @@
                     response_serializer=greenlight__pb2.IncomingPayment.SerializeToString,
             ),
             'StreamLog': grpc.unary_stream_rpc_method_handler(
                     servicer.StreamLog,
                     request_deserializer=greenlight__pb2.StreamLogRequest.FromString,
                     response_serializer=greenlight__pb2.LogEntry.SerializeToString,
             ),
+            'StreamCustommsg': grpc.unary_stream_rpc_method_handler(
+                    servicer.StreamCustommsg,
+                    request_deserializer=greenlight__pb2.StreamCustommsgRequest.FromString,
+                    response_serializer=greenlight__pb2.Custommsg.SerializeToString,
+            ),
             'StreamHsmRequests': grpc.unary_stream_rpc_method_handler(
                     servicer.StreamHsmRequests,
                     request_deserializer=greenlight__pb2.Empty.FromString,
                     response_serializer=greenlight__pb2.HsmRequest.SerializeToString,
             ),
             'RespondHsmRequest': grpc.unary_unary_rpc_method_handler(
                     servicer.RespondHsmRequest,
@@ -421,14 +447,17 @@
     `Scheduler.Schedule()` RPC call.
 
     Notice that in order to connect to the node the caller must use the
     node-specific mTLS keypair returned by `Scheduler.Register()` or
     `Scheduler.Recover()`. In particular the anonymous mTLS keypair is
     rejected by the node.
 
+    Deprecated methods are being replaced by the standardized and
+    automatically managed cln-grpc protocol you can find in
+    `node.proto`
     """
 
     @staticmethod
     def GetInfo(request,
             target,
             options=(),
             channel_credentials=None,
@@ -713,14 +742,31 @@
         return grpc.experimental.unary_stream(request, target, '/greenlight.Node/StreamLog',
             greenlight__pb2.StreamLogRequest.SerializeToString,
             greenlight__pb2.LogEntry.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def StreamCustommsg(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/greenlight.Node/StreamCustommsg',
+            greenlight__pb2.StreamCustommsgRequest.SerializeToString,
+            greenlight__pb2.Custommsg.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def StreamHsmRequests(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `gl_client-0.1.8/glclient/greenlight_pb2_grpc.pyi` & `gl_client-0.1.9/glclient/greenlight_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.8/glclient/rpc.py` & `gl_client-0.1.9/glclient/rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # This file was generated by `genrpcstubs` from the CLN JSON-Schema.
 # Do not edit this file.
 from .tls import TlsConfig
 from . import glclient as native
 import logging
-from .node_pb2 import *  # noqa: F401,F403
-from . import node_pb2 as clnpb
+from pyln import grpc as clnpb
 
 
 class Node(object):
     def __init__(
             self,
             node_id: bytes,
             network: str,
@@ -108,14 +107,27 @@
             destination=destination
         ).SerializeToString()
         res = clnpb.ListchannelsResponse
         return res.FromString(
             bytes(self.inner.call(uri, bytes(req)))
         )
 
+    def list_closed_channels(
+            self,
+            id=None,
+    ):
+        uri = "/cln.Node/ListClosedChannels"
+        req = clnpb.ListchannelsRequest(
+            id=id,
+        ).SerializeToString()
+        res = clnpb.ListclosedchannelsResponse
+        return res.FromString(
+            bytes(self.inner.call(uri, bytes(req)))
+        )
+
     def add_gossip(
             self,
             message
     ):
         uri = "/cln.Node/AddGossip"
         req = clnpb.AddgossipRequest(
             message=message
```

### Comparing `gl_client-0.1.8/glclient/scheduler_pb2.py` & `gl_client-0.1.9/glclient/scheduler_pb2.py`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.8/glclient/scheduler_pb2.pyi` & `gl_client-0.1.9/glclient/scheduler_pb2.pyi`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.8/glclient/scheduler_pb2_grpc.py` & `gl_client-0.1.9/glclient/scheduler_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `gl_client-0.1.8/glclient/tls.py` & `gl_client-0.1.9/glclient/tls.py`

 * *Files identical despite different names*

