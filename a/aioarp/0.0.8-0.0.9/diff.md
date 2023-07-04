# Comparing `tmp/aioarp-0.0.8.tar.gz` & `tmp/aioarp-0.0.9.tar.gz`

## Comparing `aioarp-0.0.8.tar` & `aioarp-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aioarp-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 aioarp-0.0.8/mkdocs.yml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aioarp-0.0.8/requirements.txt
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 aioarp-0.0.8/unasync.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aioarp-0.0.8/.github/workflows/main.yml
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 aioarp-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/__about__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/__init__.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_arp.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_async.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_cli.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_client.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_exceptions.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_mock.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_sync.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_utils.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/defaults.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_backends/__init__.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_backends/_async.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_backends/_base.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_backends/_mock.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 aioarp-0.0.8/aioarp/_backends/_sync.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 aioarp-0.0.8/docs/client.md
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 aioarp-0.0.8/docs/index.md
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 aioarp-0.0.8/scripts/check
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 aioarp-0.0.8/scripts/lint
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 aioarp-0.0.8/scripts/publish
--rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 aioarp-0.0.8/scripts/publish-docs
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 aioarp-0.0.8/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aioarp-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 aioarp-0.0.8/tests/conftest.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 aioarp-0.0.8/tests/test_async.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aioarp-0.0.8/tests/test_client.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 aioarp-0.0.8/tests/test_proto.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 aioarp-0.0.8/tests/test_sync.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aioarp-0.0.8/tests/test_utils.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aioarp-0.0.8/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aioarp-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 aioarp-0.0.8/README.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 aioarp-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aioarp-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 aioarp-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 aioarp-0.0.9/mkdocs.yml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aioarp-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aioarp-0.0.9/unasync.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aioarp-0.0.9/.github/workflows/main.yml
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 aioarp-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/__about__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/__init__.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/_arp.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/_async.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/_cli.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/_client.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/_exceptions.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/_mock.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/_sync.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/_utils.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/defaults.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/_backends/__init__.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/_backends/_async.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/_backends/_base.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/_backends/_mock.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 aioarp-0.0.9/aioarp/_backends/_sync.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 aioarp-0.0.9/docs/client.md
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 aioarp-0.0.9/docs/index.md
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 aioarp-0.0.9/scripts/check
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 aioarp-0.0.9/scripts/lint
+-rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 aioarp-0.0.9/scripts/publish
+-rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 aioarp-0.0.9/scripts/publish-docs
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 aioarp-0.0.9/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aioarp-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aioarp-0.0.9/tests/conftest.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 aioarp-0.0.9/tests/test_async.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 aioarp-0.0.9/tests/test_client.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 aioarp-0.0.9/tests/test_proto.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 aioarp-0.0.9/tests/test_sync.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 aioarp-0.0.9/tests/test_utils.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aioarp-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aioarp-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 aioarp-0.0.9/README.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aioarp-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 aioarp-0.0.9/PKG-INFO
```

### Comparing `aioarp-0.0.8/CHANGELOG.md` & `aioarp-0.0.9/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+# 0.0.9 (27/6/2023)
+
+- Make `interface` argument optional. (#23)
+- Move `Stream` creation from `request` to `sync_send_arp`. (#24)
+
 # 0.0.8 (21/6/2023) 
 
 - Add `wait_response` argument to `sync_send_arp` and `async_send_arp`. (#13)
 
 # 0.0.7 (16/6/2023)
 
 - Add basic API documentation. (#7)
```

### Comparing `aioarp-0.0.8/unasync.py` & `aioarp-0.0.9/unasync.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 SUBS = [
     ('async def async_send_arp', 'def sync_send_arp'),
     ('async def', 'def'),
     ('from .backends._async import AsyncStream', 'from .backends._sync import Stream'),
     ('AsyncStream', 'Stream'),
     ('await ', ''),
     ('async_send_arp', 'sync_send_arp'),
-    ('aioarp.arequest', 'aioarp.request')
+    ('aioarp.arequest', 'aioarp.request'),
+    ("async with", "with")
 ]
 
 COMPILED_SUBS = [
     (re.compile(r'(^|\b)' + regex + r'($|\b)'), replaced)
     for regex, replaced in SUBS
 ]
```

### Comparing `aioarp-0.0.8/.github/workflows/main.yml` & `aioarp-0.0.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.8/.github/workflows/publish.yml` & `aioarp-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.8/aioarp/_arp.py` & `aioarp-0.0.9/aioarp/_arp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import struct
 import typing
 from enum import Enum
 
-from aioarp._utils import enforce_ip, enforce_mac, parse_ip, parse_mac
+from aioarp._utils import enforce_ip
+from aioarp._utils import enforce_mac
+from aioarp._utils import parse_ip
+from aioarp._utils import parse_mac
 
 ETHERNET_HEADER_SIZE = 14
 ARP_HEADER_SIZE = 28
 
 __all__ = (
     'ETHERNET_HEADER_SIZE',
     'ARP_HEADER_SIZE',
```

### Comparing `aioarp-0.0.8/aioarp/_async.py` & `aioarp-0.0.9/aioarp/_sync.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,41 @@
+import socket
 import time
 import typing
 
 from aioarp import _exceptions as exc
-from aioarp._arp import ARP_HEADER_SIZE, ETHERNET_HEADER_SIZE, ArpPacket, EthPacket, Protocol
-from aioarp._backends import AsyncStream
+from aioarp._arp import ARP_HEADER_SIZE
+from aioarp._arp import ETHERNET_HEADER_SIZE
+from aioarp._arp import ArpPacket
+from aioarp._arp import EthPacket
+from aioarp._arp import Protocol
+from aioarp._backends import Stream
+from aioarp._backends._base import SocketInterface
+from aioarp._utils import get_default_interface
 from aioarp._utils import is_valid_ipv4
-from aioarp.defaults import DEFAULT_READ_TIMEOUT, DEFAULT_REPLY_MISSING_TIME, DEFAULT_WRITE_TIMEOUT
+from aioarp.defaults import DEFAULT_READ_TIMEOUT
+from aioarp.defaults import DEFAULT_REPLY_MISSING_TIME
+from aioarp.defaults import DEFAULT_WRITE_TIMEOUT
 
 __all__ = (
-    'async_send_arp',
+    'sync_send_arp',
 )
 
 
-async def receive_arp(sock: AsyncStream, timeout: float) -> ArpPacket:
+def receive_arp(sock: Stream, timeout: float) -> ArpPacket:
     start_time = time.time()
     while True:
 
         # Check if timeout was expired
         if time.time() - start_time > timeout:
             raise exc.NotFoundError()
 
         # Try to read frame
         try:
-            frame = await sock.receive_frame(timeout=DEFAULT_READ_TIMEOUT)
+            frame = sock.receive_frame(timeout=DEFAULT_READ_TIMEOUT)
         except Exception as e:  # pragma: no cover
             raise exc.NotFoundError() from e
 
         # Extract the ethernet header
         eth_header = frame[:ETHERNET_HEADER_SIZE]
 
         try:
@@ -39,26 +48,32 @@
             if is_valid_ipv4(arp_response.sender_ip):
                 return arp_response
         except BaseException:  # pragma: no cover
             # TODO: catch concrete errors
             ...
 
 
-async def async_send_arp(arp_packet: ArpPacket,
-                         stream: AsyncStream,
+def sync_send_arp(arp_packet: ArpPacket,
+                         sock: typing.Optional[SocketInterface] = None,
+                         interface: typing.Optional[str] = None,
                          timeout: typing.Optional[float] = None,
                          wait_response: bool = True) -> typing.Optional[ArpPacket]:
     ethernet_packet = EthPacket(
         target_mac=arp_packet.target_mac,
         sender_mac=arp_packet.sender_mac,
         proto=Protocol.arp
     )
-
-    try:
-        frame_to_send = ethernet_packet.build_frame() + arp_packet.build_frame()
-        await stream.write_frame(frame_to_send, timeout=DEFAULT_WRITE_TIMEOUT)
-    except exc.WriteTimeoutError as e:  # pragma: no cover
-        raise exc.NotFoundError from e
-    
-    if wait_response:
-        return await receive_arp(stream, timeout or DEFAULT_REPLY_MISSING_TIME)
-    return None  # pragma: no cover
+    if interface is None:  # pragma: no cover
+        interface = get_default_interface()
+    if not sock:  # pragma: no cover
+        sock = socket.socket(socket.PF_PACKET, socket.SOCK_RAW, socket.ntohs(0x0003))
+    with Stream(interface=interface,
+                    sock=sock) as stream:
+        try:
+            frame_to_send = ethernet_packet.build_frame() + arp_packet.build_frame()
+            stream.write_frame(frame_to_send, timeout=DEFAULT_WRITE_TIMEOUT)
+        except exc.WriteTimeoutError as e:  # pragma: no cover
+            raise exc.NotFoundError from e
+        
+        if wait_response:
+            return receive_arp(stream, timeout or DEFAULT_REPLY_MISSING_TIME)
+        return None  # pragma: no cover
```

### Comparing `aioarp-0.0.8/aioarp/_cli.py` & `aioarp-0.0.9/aioarp/_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,18 +30,20 @@
         try:
             response = aioarp.request(interface=interface,
                                       target_ip=target_ip,
                                       timeout=timeout)
         except PermissionError:
             text = "To send ARP requests, you must run a script with root privileges."
             print(text)
-            return
+            return typer.Exit()
         ans = response.sender_mac
         text = f"The mac address of IP '{target_ip}' is: {ans}"
         print(text)
+        return typer.Exit()
     except aioarp.NotFoundError:
         text = f"The IP address {target_ip}' did not respond to our ARP request."
         print(text)
+        return typer.Exit(1)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `aioarp-0.0.8/aioarp/_client.py` & `aioarp-0.0.9/aioarp/_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-import socket
 import typing
 
 import aioarp
-from aioarp._arp import ArpPacket, HardwareType, Protocol
-from aioarp._async import async_send_arp
-from aioarp._backends._async import AsyncStream
-from aioarp._backends._base import SocketInterface
-from aioarp._backends._sync import Stream
-from aioarp._sync import sync_send_arp
-from aioarp._utils import get_ip, get_mac, is_valid_ipv4
+
+from ._arp import ArpPacket
+from ._arp import HardwareType
+from ._arp import Protocol
+from ._async import async_send_arp
+from ._backends._base import SocketInterface
+from ._sync import sync_send_arp
+from ._utils import get_ip
+from ._utils import get_mac
+from ._utils import is_valid_ipv4
 
 __all__ = (
     'build_arp_packet',
     'request',
     'arequest'
 )
 
 
 def build_arp_packet(
+        target_ip: str,
         interface: str,
-        target_ip: str
 ) -> ArpPacket:
     if not is_valid_ipv4(target_ip):
         raise aioarp.InvalidIpError("Invalid IPv4 Address was received")
 
     hardware_type = HardwareType.ethernet
     protocol_type = Protocol.ip
 
@@ -40,36 +42,32 @@
         target_mac,
         target_ip,
     )
     return request_packet
 
 
 def request(
-        interface: str,
         target_ip: str,
-        timeout: typing.Optional[float] = None,
+        interface: typing.Optional[str] = None,
         sock: typing.Optional[SocketInterface] = None,
+        timeout: typing.Optional[float] = None,
         wait_response: bool = True
 ) -> typing.Optional[ArpPacket]:
-    if not sock:  # pragma: no cover
-        sock = socket.socket(socket.PF_PACKET, socket.SOCK_RAW, socket.ntohs(0x0003))
-    with Stream(interface=interface,
-                    sock=sock) as stream:
-        request_packet = build_arp_packet(interface, target_ip)
-        arp_response = sync_send_arp(request_packet, stream, timeout, wait_response)
-        return arp_response
+    if interface is None:  # pragma: no cover
+        interface = aioarp.get_default_interface()
+    request_packet = build_arp_packet(target_ip, interface)
+    arp_response = sync_send_arp(request_packet, sock, interface, timeout, wait_response)
+    return arp_response
 
 
 async def arequest(
-        interface: str,
         target_ip: str,
-        timeout: typing.Optional[float] = None,
+        interface: typing.Optional[str] = None,
         sock: typing.Optional[SocketInterface] = None,
+        timeout: typing.Optional[float] = None,
         wait_response: bool = True
 ) -> typing.Optional[ArpPacket]:
-    if not sock:  # pragma: no cover
-        sock = socket.socket(socket.PF_PACKET, socket.SOCK_RAW, socket.ntohs(0x0003))
-    with AsyncStream(interface=interface,
-                    sock=sock) as stream:
-        request_packet = build_arp_packet(interface, target_ip)
-        arp_response = await async_send_arp(request_packet, stream, timeout, wait_response)
-        return arp_response
+    if interface is None:  # pragma: no cover
+        interface = aioarp.get_default_interface()
+    request_packet = build_arp_packet(target_ip, interface)
+    arp_response = await async_send_arp(request_packet, sock, interface, timeout, wait_response)
+    return arp_response
```

### Comparing `aioarp-0.0.8/aioarp/_sync.py` & `aioarp-0.0.9/aioarp/_async.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,41 @@
+import socket
 import time
 import typing
 
 from aioarp import _exceptions as exc
-from aioarp._arp import ARP_HEADER_SIZE, ETHERNET_HEADER_SIZE, ArpPacket, EthPacket, Protocol
-from aioarp._backends import Stream
+from aioarp._arp import ARP_HEADER_SIZE
+from aioarp._arp import ETHERNET_HEADER_SIZE
+from aioarp._arp import ArpPacket
+from aioarp._arp import EthPacket
+from aioarp._arp import Protocol
+from aioarp._backends import AsyncStream
+from aioarp._backends._base import SocketInterface
+from aioarp._utils import get_default_interface
 from aioarp._utils import is_valid_ipv4
-from aioarp.defaults import DEFAULT_READ_TIMEOUT, DEFAULT_REPLY_MISSING_TIME, DEFAULT_WRITE_TIMEOUT
+from aioarp.defaults import DEFAULT_READ_TIMEOUT
+from aioarp.defaults import DEFAULT_REPLY_MISSING_TIME
+from aioarp.defaults import DEFAULT_WRITE_TIMEOUT
 
 __all__ = (
-    'sync_send_arp',
+    'async_send_arp',
 )
 
 
-def receive_arp(sock: Stream, timeout: float) -> ArpPacket:
+async def receive_arp(sock: AsyncStream, timeout: float) -> ArpPacket:
     start_time = time.time()
     while True:
 
         # Check if timeout was expired
         if time.time() - start_time > timeout:
             raise exc.NotFoundError()
 
         # Try to read frame
         try:
-            frame = sock.receive_frame(timeout=DEFAULT_READ_TIMEOUT)
+            frame = await sock.receive_frame(timeout=DEFAULT_READ_TIMEOUT)
         except Exception as e:  # pragma: no cover
             raise exc.NotFoundError() from e
 
         # Extract the ethernet header
         eth_header = frame[:ETHERNET_HEADER_SIZE]
 
         try:
@@ -39,26 +48,32 @@
             if is_valid_ipv4(arp_response.sender_ip):
                 return arp_response
         except BaseException:  # pragma: no cover
             # TODO: catch concrete errors
             ...
 
 
-def sync_send_arp(arp_packet: ArpPacket,
-                         stream: Stream,
+async def async_send_arp(arp_packet: ArpPacket,
+                         sock: typing.Optional[SocketInterface] = None,
+                         interface: typing.Optional[str] = None,
                          timeout: typing.Optional[float] = None,
                          wait_response: bool = True) -> typing.Optional[ArpPacket]:
     ethernet_packet = EthPacket(
         target_mac=arp_packet.target_mac,
         sender_mac=arp_packet.sender_mac,
         proto=Protocol.arp
     )
-
-    try:
-        frame_to_send = ethernet_packet.build_frame() + arp_packet.build_frame()
-        stream.write_frame(frame_to_send, timeout=DEFAULT_WRITE_TIMEOUT)
-    except exc.WriteTimeoutError as e:  # pragma: no cover
-        raise exc.NotFoundError from e
-    
-    if wait_response:
-        return receive_arp(stream, timeout or DEFAULT_REPLY_MISSING_TIME)
-    return None  # pragma: no cover
+    if interface is None:  # pragma: no cover
+        interface = get_default_interface()
+    if not sock:  # pragma: no cover
+        sock = socket.socket(socket.PF_PACKET, socket.SOCK_RAW, socket.ntohs(0x0003))
+    async with AsyncStream(interface=interface,
+                    sock=sock) as stream:
+        try:
+            frame_to_send = ethernet_packet.build_frame() + arp_packet.build_frame()
+            await stream.write_frame(frame_to_send, timeout=DEFAULT_WRITE_TIMEOUT)
+        except exc.WriteTimeoutError as e:  # pragma: no cover
+            raise exc.NotFoundError from e
+        
+        if wait_response:
+            return await receive_arp(stream, timeout or DEFAULT_REPLY_MISSING_TIME)
+        return None  # pragma: no cover
```

### Comparing `aioarp-0.0.8/aioarp/_utils.py` & `aioarp-0.0.9/aioarp/_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import fcntl
 import ipaddress
 import socket
 import struct
+import subprocess
 import typing
 
 __all__ = (
     'is_valid_ipv4',
     'get_mac',
     'get_ip',
+    'get_default_interface',
     'enforce_mac',
     'enforce_ip',
     'parse_mac',
     'parse_ip'
 )
 
 OUR_MAC = None
 OUR_IP = None
+OUR_INTERFACE = None
 
 
 def is_valid_ipv4(ip: str) -> bool:
     try:
         ipaddress.IPv4Address(ip)
         return True
     except ipaddress.AddressValueError:
@@ -58,14 +61,25 @@
 def enforce_ip(ip: str) -> bytes:
     ip_bytes = []
     for b in ip.split('.'):
         ip_bytes.append(int(b))
     return bytes(ip_bytes)
 
 
+def get_default_interface() -> str:  # pragma: no cover
+    global OUR_INTERFACE
+    if OUR_INTERFACE:
+        return OUR_INTERFACE
+    output = subprocess.check_output(['ip', 'route', 'list']).decode().split()
+    for ind, word in enumerate(output):
+        if word == 'dev':
+            OUR_INTERFACE = output[ind + 1]
+            return OUR_INTERFACE
+    raise RuntimeError('Could not find default interface')    
+        
 def parse_mac(mac: bytes) -> str:
     mac_parts = []
     for b in mac:
         hex = f'{b:x}'
         if len(hex) == 1:
             hex = '0' + hex
         mac_parts.append(hex)
```

### Comparing `aioarp-0.0.8/aioarp/_backends/_async.py` & `aioarp-0.0.9/aioarp/_backends/_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,12 +49,18 @@
                 await anyio.sleep(0)
         if frame:  # pragma: no cover
             raise exc.WriteTimeoutError()
 
     def close(self) -> None:
         self.sock.close()
 
-    def __enter__(self) -> "AsyncStream":
+    def __enter__(self) -> "AsyncStream":  # pragma: no cover
+        return self
+    
+    def __exit__(self) -> None:  # pragma: no cover
+        self.close()
+
+    async def __aenter__(self) -> "AsyncStream":
         return self
 
-    def __exit__(self, exc_type: typing.Any, exc_val: typing.Any, exc_tb: typing.Any) -> None:
+    async def __aexit__(self, exc_type: typing.Any, exc_val: typing.Any, exc_tb: typing.Any) -> None:
         self.close()
```

### Comparing `aioarp-0.0.8/aioarp/_backends/_mock.py` & `aioarp-0.0.9/aioarp/_backends/_mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,17 @@
     def sendall(self, data: bytes) -> None:
         self._file.write(data)
 
     def recv(self, max_bytes: typing.Optional[int] = None) -> bytes:
         return self._to_receive
 
     def bind(self, address: typing.Union[_Address, bytes]) -> None: ...
-    def settimeout(self, value: typing.Union[float, None]) -> None: ...
 
+    def settimeout(self, value: typing.Union[float, None]) -> None: ...
+    
     def fileno(self) -> int:
         return self._file.fileno()
 
     def close(self) -> None:
         self._file.close()
 
     def __enter__(self):
```

### Comparing `aioarp-0.0.8/aioarp/_backends/_sync.py` & `aioarp-0.0.9/aioarp/_backends/_sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,12 +31,24 @@
     def write_frame(self, frame: bytes, timeout: float) -> None:
         self.sock.settimeout(timeout)
         try:
             self.sock.sendall(frame)
         except socket.timeout:  # pragma: no cover
             raise exc.WriteTimeoutError()
 
-    def __enter__(self) -> 'Stream':
-        return self
+    def close(self) -> None:
+        self.sock.close()
 
+    def __enter__(self) -> "Stream":
+        return self
+    
     def __exit__(self, exc_type: typing.Any, exc_val: typing.Any, exc_tb: typing.Any) -> None:
-        self.sock.close()
+        self.close()
+
+    async def __aenter__(self) -> "Stream":  # pragma: no cover
+        return self
+
+    async def __aexit__(self, 
+                        exc_type: typing.Any, 
+                        exc_val: typing.Any, 
+                        exc_tb: typing.Any) -> None:  # pragma: no cover
+        self.close()
```

### Comparing `aioarp-0.0.8/docs/client.md` & `aioarp-0.0.9/docs/client.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 # Requests
 
 ## Sending requests
 
 ```py title="request"
 import aioarp
 
-aioarp.request("enp0s3", "10.0.2.2")
+aioarp.request("10.0.2.2", "enp0s3")
 ```
 
 This is simply sending the arp packet that searches the network for a mac address of the `10.0.2.2` ip using the interface that you provided.
 You can also use a `timeout` to ensure that waiting for a response does not go on indefinitely.
 
 ```py title="timeout request"
-aioarp.request("enp0s3", "10.0.2.2", timeout=0.5)
+aioarp.request("10.0.2.2", "enp0s3", timeout=0.5)
 ```
 
+This function accepts the network interface that will be used to send the ARP request as the second argument.
+However, interface is an optional parameter that can be ignored. if it is not passed, aioarp will look up your system's default interface and use it.
+
+Example:
+
+```py title="without specifying interface"
+aioarp.request("10.0.2.2")
+```
+
+!!! note
+
+    If the default network interface is not specified, Aioarp will use the `ip` command to find it.
+
 You can also use the `wait_response` parameter to tell aioarp whether you need the response or not.
 ```py title="without waiting for a response"
-aioarp.request("enp0s3", "10.0.2.2", wait_response=False)
+aioarp.request("10.0.2.2", "enp0s3", wait_response=False)
 ```
 
 !!! note
 
     When the `wait_response` argument is false, the `timeout` argument has no effect.
 
-
 This method can also take the `sock` argument, which is a socket connection that will be used for IO operations. (useful for mocking)
 
 ## Asynchronous requests
 
 It is very simple to switch from synchronous to asynchronous aioarp; simply use the await keyword and change request to arequest.
 
 ```py title="async request"
-await arequest("enp0s3", "10.0.2.2")
+await arequest("10.0.2.2", "enp0s3")
 ```
 
 Because the synchronous and asynchronous interfaces shared the same function signatures, all synchronous features worked as expected in asynchronous.
 
 ## Building requests
 
 You may need to build your own ARP packet and set each ARP header to whatever you want; aioarp supports that behavior, and you can pass not only the target ip, but also the source ip, source mac, desctination mac, and so on.
@@ -50,19 +62,19 @@
          target_mac='11:11:11:11:11:11',
          target_ip='127.0.0.1')
 ```
 
 Now that you have your arp packet with all of the required headers, you can ask `aioarp` to send that request.
 
 ```py
-aioarp.sync_send_arp(arp_packet, Stream("enp0s3"))
+aioarp.sync_send_arp(arp_packet, "enp0s3")
 ```
 
 If the `ArpPacket` is too complicated for you, you can use the `build_arp_packet` function to generate an `ArpPacket` for you, which you can then modify.
 
 ```py title="build_arp_packet"
-arp_packet = build_arp_packet('enp0s3', '10.0.2.2')
+arp_packet = build_arp_packet('10.0.2.2', 'enp0s3')
 arp_packet.sender_ip
 '10.0.2.2' 
 ```
 
 `build_arp_packet` accepts only two arguments: interface and target IP address.
```

### Comparing `aioarp-0.0.8/docs/index.md` & `aioarp-0.0.9/docs/index.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 pip install aioarp
 ```
 
 ## How to send ARP requests
 
 ```py title="Sync" linenums="1" 
 import aioarp
-response = aioarp.request('enp0s3', '10.0.2.2')
+response = aioarp.request('10.0.2.2', 'enp0s3')
 print(response.sender_mac)
 ee:xx:aa:mm:pp:le  # mac address
 ```
 
 ```py title="trio" linenums="1"
 import trio
 import aioarp
-response = trio.run(aioarp.arequest, 'enp0s3', '10.0.2.2')
+response = trio.run(aioarp.arequest, '10.0.2.2', 'enp0s3')
 ```
 
 ```py title="asyncio" linenums="1"
 import asyncio
 import aioarp
-response = asyncio.run(aioarp.arequest('enp0s3', '10.0.2.2'))
+response = asyncio.run(aioarp.arequest('10.0.2.2', 'enp0s3'))
 ```
 
 This is the packet that was sent over the network.
 ```
 Ethernet II, Src: PcsCompu (YOUR MAC), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
     Destination: Broadcast (ff:ff:ff:ff:ff:ff)
     Source: PcsCompu (YOUR MAC)
@@ -69,15 +69,15 @@
     hardware_type=aioarp.HardwareType.ethernet,
     protocol_type=aioarp.Protocol.ip,
     sender_mac='11:11:11:11:11:11',
     sender_ip='127.0.0.1',
     target_mac='11:11:11:11:11:11',
     target_ip='127.0.0.1')
 
-response = aioarp.sync_send_arp(arp_packet, aioarp.Stream('enp0s3'))
+response = aioarp.sync_send_arp(arp_packet)
 ```
 
 This sends the same ARP request as your `ArpPacket` instance.
 
 !!! note
 
     The **Hardware Size** and **Protocol Size** headers are automatically set depending on the hardware type and protocol used.
@@ -101,15 +101,15 @@
 
 ## ARP response
 
 Let's try again with another arp request and see what we can do with the respone object.
 
 ```py linenums="1"
 import aioarp
-response = aioarp.request('enp0s3', '10.0.2.2')
+response = aioarp.request('10.0.2.2', 'enp0s3')
 # The `sender_mac` header for arp responses, as we know, 
 # indicates the actual answer to our question "Who has 10.0.2.2?" 
 # That is the protocol implementation; 
 # the other computer that responds should 
 # set the sender_mac to the computer's mac address that we are looking for.
 print(response.sender_mac)
 # ee:xx:aa:mm:pp:le  # mac address of 10.0.2.2
@@ -128,13 +128,13 @@
 ## Failed Responses
 
 If the response is not received, aioarp should throw a `aioarp.NotFoundError` exception. 
 
 This occurs when the default arp request `timeout expires`. The timeout is set to 5 by default, but it can be changed by passing the `timeout` argument to the `request` function.
 
 ```py title="Without timeout" linenums="1"
-response = aioarp.request('enp0s3', '10.0.2.25')
+response = aioarp.request('10.0.2.25', 'enp0s3')
 ```
 
 ```py title="With timeout" linenums="1"
-response = aioarp.request('enp0s3', '10.0.2.25', timeout=0.5)
+response = aioarp.request('10.0.2.25', 'enp0s3', timeout=0.5)
 ```
```

### Comparing `aioarp-0.0.8/tests/test_async.py` & `aioarp-0.0.9/tests/test_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     b"\x7f\x00\x00\x01"
 )
 
 
 @pytest.mark.anyio
 async def test_async_send_arp():
     msocket = MockSocket(eth_header_arp + arp_header)
-    response = await aioarp.arequest('null', '100.100.100.100', sock=msocket)
+    response = await aioarp.arequest('100.100.100.100', 'null', sock=msocket)
     assert response
     assert response.sender_mac == '11:11:11:11:11:11'
 
 
 @pytest.mark.anyio
 async def test_async_send_arp_timeout():
     with MockSocket(eth_header_no_arp + arp_header) as msocket:
         with pytest.raises(aioarp.NotFoundError):
-            await aioarp.arequest('null', '100.100.100.100', sock=msocket, timeout=0.5)
+            await aioarp.arequest('100.100.100.100', 'null',  sock=msocket, timeout=0.5)
```

### Comparing `aioarp-0.0.8/tests/test_client.py` & `aioarp-0.0.9/tests/test_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 
 import pytest
 
 import aioarp
-from aioarp import HardwareType, Protocol, build_arp_packet
-
+from aioarp import HardwareType
+from aioarp import Protocol
+from aioarp import build_arp_packet
 
 def test_invalid_ip():
     with pytest.raises(aioarp.InvalidIpError):
-        aioarp.build_arp_packet('test', '10.10.10.10.10')
+        aioarp.build_arp_packet('10.10.10.10.10', 'test')
 
 
 def test_build_packet(monkeypatch):
-    packet = build_arp_packet('test', '192.168.0.85')
+    packet = build_arp_packet('192.168.0.85', 'test')
 
     assert packet.sender_mac == '11:11:11:11:11:11'
     assert packet.sender_ip == '127.0.0.1'
     assert packet.hardware_type == HardwareType.ethernet
     assert packet.protocol_type == Protocol.ip
     assert packet.target_mac == 'ff:ff:ff:ff:ff:ff'
     assert packet.target_ip == '192.168.0.85'
```

### Comparing `aioarp-0.0.8/tests/test_proto.py` & `aioarp-0.0.9/tests/test_proto.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-from aioarp import ArpPacket, EthPacket, HardwareType, Opcode, Protocol
-
+from aioarp import ArpPacket
+from aioarp import EthPacket
+from aioarp import HardwareType
+from aioarp import Opcode
+from aioarp import Protocol
 
 class TestEth:
 
     def test_eth_parse(self):
         eth_header = (
             b"\x11\x11\x11\x11\x11\x11\x11"
             b"\x11\x11\x11\x11\x11\x08\x06"
```

### Comparing `aioarp-0.0.8/tests/test_sync.py` & `aioarp-0.0.9/tests/test_sync.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     b"\x7f\x00\x00\x01"
 )
 
 
 @pytest.mark.anyio
 def test_async_send_arp():
     msocket = MockSocket(eth_header_arp + arp_header)
-    response = aioarp.request('null', '100.100.100.100', sock=msocket)
+    response = aioarp.request('100.100.100.100', 'null', sock=msocket)
     assert response
     assert response.sender_mac == '11:11:11:11:11:11'
 
 
 @pytest.mark.anyio
 def test_async_send_arp_timeout():
     with MockSocket(eth_header_no_arp + arp_header) as msocket:
         with pytest.raises(aioarp.NotFoundError):
-            aioarp.request('null', '100.100.100.100', sock=msocket, timeout=0.5)
+            aioarp.request('100.100.100.100', 'null',  sock=msocket, timeout=0.5)
```

### Comparing `aioarp-0.0.8/.gitignore` & `aioarp-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.8/LICENSE.txt` & `aioarp-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.8/README.md` & `aioarp-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,29 +24,35 @@
 [Click here](https://karosis88.github.io/aioarp/)
 
 ## How to send ARP requests
 
 ### Sync
 ```py
 import aioarp
-response = aioarp.request('enp0s3', '10.0.2.2')
+response = aioarp.request('10.0.2.2', 'enp0s3')
 print(response.sender_mac)
 # ee:xx:aa:mm:pp:le mac address
 ```
 
 ### Async [trio or asyncio]
 ```py
 import trio
 import aioarp
-response = trio.run(aioarp.arequest, 'enp0s3', '10.0.2.2')
+response = trio.run(aioarp.arequest, '10.0.2.2', 'enp0s3')
 ```
 
 ```py
 import asyncio
 import aioarp
-response = asyncio.run(aioarp.arequest('enp0s3', '10.0.2.2'))
+response = asyncio.run(aioarp.arequest('10.0.2.2', 'enp0s3'))
+```
+
+Or without specifying an interface parameter
+
+```
+response = aioarp.request('10.0.2.2')
 ```
 
 ## License
 
 `aioarp` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `aioarp-0.0.8/pyproject.toml` & `aioarp-0.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -35,28 +35,31 @@
   "typer==0.9.0"
 ]
 
 [project.scripts]
 aioarp = "aioarp._cli:app"
 
 [project.urls]
-Documentation = "https://github.com/karosis88/aioarp#readme"
-Issues = "https://github.com/karosis88/aioarp/issues"
 Source = "https://github.com/karosis88/aioarp"
+Documentation = "https://karosis88.github.io/aioarp/"
+Changelog = "https://github.com/karosis88/aioarp/blob/master/CHANGELOG.md"
+Issues = "https://github.com/karosis88/aioarp/issues"
 
 [tool.hatch.version]
 path = "aioarp/__about__.py"
 
 [tool.ruff]
 select = ["E", "F", "I", "B", "PIE"]
 ignore = ["B904", "B028", "F403"]
 line-length = 120
 
 [tool.ruff.isort]
 combine-as-imports = true
+lines-after-imports = 1
+force-single-line = true
 
 [tool.mypy]
 ignore_missing_imports = true
 strict = true
 exclude = ["unasync.py", "_mock.py", "aioarp/_cli.py"]
 
 [[tool.mypy.overrides]]
```

### Comparing `aioarp-0.0.8/PKG-INFO` & `aioarp-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: aioarp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Aioarp is a ARP protocol implementation that provides synchronous and asynchronous interfaces and gives you complete control over how ARP packets are sent.
-Project-URL: Documentation, https://github.com/karosis88/aioarp#readme
-Project-URL: Issues, https://github.com/karosis88/aioarp/issues
 Project-URL: Source, https://github.com/karosis88/aioarp
+Project-URL: Documentation, https://karosis88.github.io/aioarp/
+Project-URL: Changelog, https://github.com/karosis88/aioarp/blob/master/CHANGELOG.md
+Project-URL: Issues, https://github.com/karosis88/aioarp/issues
 Author-email: Karen Petrosyan <kar.petrosyanpy@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -50,29 +51,35 @@
 [Click here](https://karosis88.github.io/aioarp/)
 
 ## How to send ARP requests
 
 ### Sync
 ```py
 import aioarp
-response = aioarp.request('enp0s3', '10.0.2.2')
+response = aioarp.request('10.0.2.2', 'enp0s3')
 print(response.sender_mac)
 # ee:xx:aa:mm:pp:le mac address
 ```
 
 ### Async [trio or asyncio]
 ```py
 import trio
 import aioarp
-response = trio.run(aioarp.arequest, 'enp0s3', '10.0.2.2')
+response = trio.run(aioarp.arequest, '10.0.2.2', 'enp0s3')
 ```
 
 ```py
 import asyncio
 import aioarp
-response = asyncio.run(aioarp.arequest('enp0s3', '10.0.2.2'))
+response = asyncio.run(aioarp.arequest('10.0.2.2', 'enp0s3'))
+```
+
+Or without specifying an interface parameter
+
+```
+response = aioarp.request('10.0.2.2')
 ```
 
 ## License
 
 `aioarp` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

