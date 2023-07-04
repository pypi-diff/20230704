# Comparing `tmp/doipclient-1.0.8.tar.gz` & `tmp/doipclient-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\doipclient-1.0.8.tar", last modified: Tue Sep 13 05:34:44 2022, max compression
+gzip compressed data, was "doipclient-1.0.9.tar", last modified: Tue Jul  4 21:32:24 2023, max compression
```

## Comparing `doipclient-1.0.8.tar` & `doipclient-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-09-13 05:34:44.000000 doipclient-1.0.8/
-drwxrwxrwx   0        0        0        0 2022-09-13 05:34:44.000000 doipclient-1.0.8/doipclient/
--rw-rw-rw-   0        0        0    32984 2022-09-13 05:33:08.000000 doipclient-1.0.8/doipclient/client.py
--rw-rw-rw-   0        0        0     1707 2021-09-11 19:55:51.000000 doipclient-1.0.8/doipclient/connectors.py
--rw-rw-rw-   0        0        0      597 2022-01-23 21:31:32.000000 doipclient-1.0.8/doipclient/constants.py
--rw-rw-rw-   0        0        0    33278 2022-06-17 04:16:27.000000 doipclient-1.0.8/doipclient/messages.py
--rw-rw-rw-   0        0        0       31 2020-12-29 19:04:44.000000 doipclient-1.0.8/doipclient/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-13 05:34:44.000000 doipclient-1.0.8/doipclient.egg-info/
--rw-rw-rw-   0        0        0        1 2022-09-13 05:34:42.000000 doipclient-1.0.8/doipclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     5448 2022-09-13 05:34:42.000000 doipclient-1.0.8/doipclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2022-09-13 05:34:42.000000 doipclient-1.0.8/doipclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2022-09-13 05:34:42.000000 doipclient-1.0.8/doipclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5448 2022-09-13 05:34:44.000000 doipclient-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3982 2022-06-17 04:16:27.000000 doipclient-1.0.8/README.rst
--rw-rw-rw-   0        0        0       64 2022-09-13 05:34:44.000000 doipclient-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      927 2022-09-13 05:34:07.000000 doipclient-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-13 05:34:44.000000 doipclient-1.0.8/tests/
--rw-rw-rw-   0        0        0    21774 2022-09-13 05:33:08.000000 doipclient-1.0.8/tests/test_client.py
--rw-rw-rw-   0        0        0        0 2020-12-29 18:42:18.000000 doipclient-1.0.8/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 21:32:24.449567 doipclient-1.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-06-30 04:57:22.000000 doipclient-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4555 2023-07-04 21:32:24.449069 doipclient-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3947 2023-06-30 04:57:22.000000 doipclient-1.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-04 21:32:24.444067 doipclient-1.0.9/doipclient/
+-rw-rw-rw-   0        0        0       32 2023-06-30 04:57:22.000000 doipclient-1.0.9/doipclient/__init__.py
+-rw-rw-rw-   0        0        0    33511 2023-07-04 21:25:05.000000 doipclient-1.0.9/doipclient/client.py
+-rw-rw-rw-   0        0        0     1707 2023-06-30 04:57:22.000000 doipclient-1.0.9/doipclient/connectors.py
+-rw-rw-rw-   0        0        0      598 2023-06-30 04:57:22.000000 doipclient-1.0.9/doipclient/constants.py
+-rw-rw-rw-   0        0        0    33278 2023-06-30 04:57:22.000000 doipclient-1.0.9/doipclient/messages.py
+drwxrwxrwx   0        0        0        0 2023-07-04 21:32:24.447069 doipclient-1.0.9/doipclient.egg-info/
+-rw-rw-rw-   0        0        0     4555 2023-07-04 21:32:24.000000 doipclient-1.0.9/doipclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-07-04 21:32:24.000000 doipclient-1.0.9/doipclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 21:32:24.000000 doipclient-1.0.9/doipclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-04 21:32:24.000000 doipclient-1.0.9/doipclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      101 2023-06-30 04:57:22.000000 doipclient-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 21:32:24.449567 doipclient-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      976 2023-07-04 21:30:26.000000 doipclient-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 21:32:24.448570 doipclient-1.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-30 04:57:22.000000 doipclient-1.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0    23458 2023-07-04 21:28:31.000000 doipclient-1.0.9/tests/test_client.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `doipclient-1.0.8/doipclient/client.py` & `doipclient-1.0.9/doipclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import logging
 import ipaddress
 import socket
 import struct
 import time
 import ssl
 from enum import IntEnum
-from .constants import TCP_DATA_UNSECURED, UDP_DISCOVERY, A_PROCESSING_TIME, LINK_LOCAL_MULTICAST_ADDRESS
+from typing import Union
+from .constants import (
+    TCP_DATA_UNSECURED,
+    UDP_DISCOVERY,
+    A_PROCESSING_TIME,
+    LINK_LOCAL_MULTICAST_ADDRESS,
+)
 from .messages import *
 
 logger = logging.getLogger("doipclient")
 
 
 class Parser:
     """Implements state machine for DoIP transport layer.
@@ -64,23 +70,23 @@
                     self._state = Parser.ParserState.READ_PAYLOAD_TYPE
 
         if self._state == Parser.ParserState.READ_PAYLOAD_TYPE:
             if len(self.rx_buffer) >= 2:
                 self.payload_type = self.rx_buffer.pop(0) << 8
                 self.payload_type |= self.rx_buffer.pop(0)
                 self._state = Parser.ParserState.READ_PAYLOAD_SIZE
-        
+
         if self._state == Parser.ParserState.READ_PAYLOAD_SIZE:
             if len(self.rx_buffer) >= 4:
                 self.payload_size = self.rx_buffer.pop(0) << 24
                 self.payload_size |= self.rx_buffer.pop(0) << 16
                 self.payload_size |= self.rx_buffer.pop(0) << 8
                 self.payload_size |= self.rx_buffer.pop(0)
                 self._state = Parser.ParserState.READ_PAYLOAD
-        
+
         if self._state == Parser.ParserState.READ_PAYLOAD:
             remaining_bytes = self.payload_size - len(self.payload)
             self.payload += self.rx_buffer[:remaining_bytes]
             self.rx_buffer = self.rx_buffer[remaining_bytes:]
             if len(self.payload) == self.payload_size:
                 self._state = Parser.ParserState.READ_PROTOCOL_VERSION
                 logger.debug(
@@ -130,16 +136,17 @@
     :param client_logical_address: The logical address that this DoIP client will use to identify itself. Per the spec,
         this should be 0x0E00 to 0x0FFF. Can typically be left as default.
     :type client_logical_address: int
     :param client_ip_address: If specified, attempts to bind to this IP as the source for both UDP and TCP communication.
         Useful if you have multiple network adapters. Can be an IPv4 or IPv6 address just like `ecu_ip_address`, though
         the type should match.
     :type client_ip_address: str, optional
-    :param use_secure: Enables TLS if True. Untested. Should be combined with changing tcp_port to 3496.
-    :type use_secure: bool
+    :param use_secure: Enables TLS. If set to True, a default SSL context is used. For more control, a preconfigured
+        SSL context can be passed directly. Untested. Should be combined with changing tcp_port to 3496.
+    :type use_secure: Union[bool,ssl.SSLContext]
     :param log_level: Logging level
     :type log_level: int
     :param auto_reconnect_tcp: Attempt to automatically reconnect TCP sockets that were closed by peer
     :type auto_reconnect_tcp: bool
 
     :raises ConnectionRefusedError: If the activation request fails
     :raises ValueError: If the IPAddress is neither an IPv4 nor an IPv6 address
@@ -216,47 +223,47 @@
         :param ipv6: Bool forcing IPV6 socket instead of IPV4 socket
         :type ipv6: bool, optional
         :return: IP Address of ECU and VehicleAnnouncementMessage object
         :rtype: tuple
         :param source_interface: Interface name (like "eth0") to bind to for use with IPv6. Defaults to None which
             will use the default interface (which may not be the one connected to the ECU). Does nothing for IPv4,
             which will bind to all interfaces uses INADDR_ANY.
-        :type source_interface: str, optional 
+        :type source_interface: str, optional
         :raises TimeoutError: If vehicle announcement not received in time
         """
         start_time = time.time()
 
         if ipv6:
             sock = socket.socket(socket.AF_INET6, socket.SOCK_DGRAM)
 
-            # IPv6 version always uses link-local scope multicast address (FF02 16 ::1) 
+            # IPv6 version always uses link-local scope multicast address (FF02 16 ::1)
             sock.bind((LINK_LOCAL_MULTICAST_ADDRESS, udp_port))
 
             if source_interface is None:
                 # 0 is the "default multicast interface" which is unlikely to be correct, but it will do
                 interface_index = 0
             else:
                 interface_index = socket.if_nametoindex(source_interface)
 
             # Join the group so that packets are delivered
             mc_addr = ipaddress.IPv6Address(LINK_LOCAL_MULTICAST_ADDRESS)
-            join_data = struct.pack('16sI', mc_addr.packed, interface_index)
+            join_data = struct.pack("16sI", mc_addr.packed, interface_index)
             # IPV6_JOIN_GROUP is also known as IPV6_ADD_MEMBERSHIP, though older Python for Windows doesn't have it
             # IPPROTO_IPV6 may be missing in older Windows builds
             try:
                 from socket import IPPROTO_IPV6
             except ImportError:
                 IPPROTO_IPV6 = 41
             sock.setsockopt(IPPROTO_IPV6, socket.IPV6_JOIN_GROUP, join_data)
         else:
             sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             # IPv4, use INADDR_ANY to listen to all interfaces for broadcasts (not multicast)
             sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
             sock.bind(("", udp_port))
-        
+
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         if timeout is not None:
             sock.settimeout(timeout)
 
         parser = Parser()
 
         while True:
@@ -373,15 +380,15 @@
                     logger.debug("TCP Connection closed by ECU, attempting to reset")
                     self._tcp_close_detected = True
                     break
                 else:
                     self._tcp_parser.push_bytes(data)
                 # Subsequent reads, go to 0 timeout
                 self._tcp_sock.settimeout(0)
-        except (BlockingIOError, socket.timeout):
+        except (BlockingIOError, socket.timeout, ssl.SSLError):
             pass
         except (ConnectionResetError, BrokenPipeError):
             logger.debug("TCP Connection broken, attempting to reset")
             self._tcp_close_detected = True
         finally:
             self._tcp_sock.settimeout(original_timeout)
 
@@ -689,15 +696,23 @@
         self._udp_sock = socket.socket(self._address_family, socket.SOCK_DGRAM)
         self._udp_sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self._udp_sock.settimeout(A_PROCESSING_TIME)
         if self._client_ip_address is not None:
             self._udp_sock.bind((self._client_ip_address, 0))
 
         if self._use_secure:
-            self._tcp_sock = ssl.wrap_socket(self._tcp_sock)
+            if isinstance(self._use_secure, type(ssl.SSLContext)):
+                ssl_context = self._use_secure
+            else:
+                ssl_context = ssl.create_default_context()
+            self._wrap_socket(ssl_context)
+
+    def _wrap_socket(self, ssl_context):
+        """Wrap the underlying socket in a SSL context."""
+        self._tcp_sock = ssl_context.wrap_socket(self._tcp_sock)
 
     def close(self):
         """Close the DoIP client"""
         self._tcp_sock.close()
         self._udp_sock.close()
 
     def reconnect(self, close_delay=A_PROCESSING_TIME):
```

### Comparing `doipclient-1.0.8/doipclient/connectors.py` & `doipclient-1.0.9/doipclient/connectors.py`

 * *Files identical despite different names*

### Comparing `doipclient-1.0.8/doipclient/constants.py` & `doipclient-1.0.9/doipclient/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 # Table 41 - UDP ports
 UDP_DISCOVERY = 13400
 
 # Table 39 - Supported TCP ports
 TCP_DATA_UNSECURED = 13400
 TCP_DATA_SECURED = 3496
 
-# link-local scope multicast address (FF02 16 ::1) 
-LINK_LOCAL_MULTICAST_ADDRESS = "ff02::1"
+# link-local scope multicast address (FF02 16 ::1)
+LINK_LOCAL_MULTICAST_ADDRESS = "ff02::1"
```

### Comparing `doipclient-1.0.8/doipclient/messages.py` & `doipclient-1.0.9/doipclient/messages.py`

 * *Files identical despite different names*

### Comparing `doipclient-1.0.8/doipclient.egg-info/PKG-INFO` & `doipclient-1.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,122 +1,121 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: doipclient
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Diagnostic over IP (DoIP) client implementing ISO-13400-2.
 Home-page: https://github.com/jacobschaer/python-doipclient
 Author: Jacob Schaer
-Author-email: UNKNOWN
-License: UNKNOWN
-Description: python-doipclient
-        #################
-        
-        .. image:: https://travis-ci.com/jacobschaer/python-doipclient.svg?branch=main
-            :target: https://travis-ci.com/jacobschaer/python-doipclient
-        
-        doipclient is a pure Python 3 Diagnostic over IP (DoIP) client which can be used
-        for communicating with modern ECU's over automotive ethernet. It implements the
-        majority of ISO-13400 (2019) from the perspective of a short-lived synchronous
-        client. The primary use case is to serve as a transport layer implementation for
-        the `udsoncan <https://github.com/pylessard/python-udsoncan>`_ library. The code
-        is published under MIT license on GitHub (jacobschaer/python-doipclient).
-        
-        Documentation
-        -------------
-        
-        The documentation is available here : https://python-doipclient.readthedocs.io/
-        
-        Requirements
-        ------------
-        
-         - Python 3.6+
-        
-        Installation
-        ------------
-        
-        using pip::
-        
-            pip install doipclient
-        
-        Running Tests from source
-        -------------------------
-        
-        using pytest::
-        
-            pip install pytest pytest-mock
-            pytest
-        
-        Example
-        -------
-        Updated version of udsoncan's example using `python_doip` instead of IsoTPSocketConnection
-        
-        .. code-block:: python
-        
-           import SomeLib.SomeCar.SomeModel as MyCar
-        
-           import udsoncan
-           from doipclient import DoIPClient
-           from doipclient.connectors import DoIPClientUDSConnector
-           from udsoncan.client import Client
-           from udsoncan.exceptions import *
-           from udsoncan.services import *
-           
-           udsoncan.setup_logging()
-           
-           ecu_ip = '127.0.0.1'
-           ecu_logical_address = 0x00E0
-           doip_client = DoIPClient(ecu_ip, ecu_logical_address)
-           conn = DoIPClientUDSConnector(doip_client)
-           with Client(conn, request_timeout=2, config=MyCar.config) as client:
-              try:
-                 client.change_session(DiagnosticSessionControl.Session.extendedDiagnosticSession)  # integer with value of 3
-                 client.unlock_security_access(MyCar.debug_level)                                   # Fictive security level. Integer coming from fictive lib, let's say its value is 5
-                 client.write_data_by_identifier(udsoncan.DataIdentifier.VIN, 'ABC123456789')       # Standard ID for VIN is 0xF190. Codec is set in the client configuration
-                 print('Vehicle Identification Number successfully changed.')
-                 client.ecu_reset(ECUReset.ResetType.hardReset)                                     # HardReset = 0x01
-              except NegativeResponseException as e:
-                 print('Server refused our request for service %s with code "%s" (0x%02x)' % (e.response.service.get_name(), e.response.code_name, e.response.code))
-              except (InvalidResponseException, UnexpectedResponseException) as e:
-                 print('Server sent an invalid payload : %s' % e.response.original_payload)
-        
-              # Because we reset our UDS server, we must also reconnect/reactivate the DoIP socket
-              # Alternatively, we could have used the auto_reconnect_tcp flag on the DoIPClient
-              # Note: ECU's do not restart instantly, so you may need a sleep() before moving on
-              doip_client.reconnect()
-              client.tester_present()
-        
-           # Cleanup the DoIP Socket when we're done. Alternatively, we could have used the
-           # close_connection flag on conn so that the udsoncan client would clean it up
-           doip_client.close()
-        
-        python-uds Support
-        ------------------
-        The `python-uds <https://github.com/richClubb/python-uds>`_ can also be used
-        but requires a fork until the owner merges this PR
-        `Doip #63 <https://github.com/richClubb/python-uds/pull/63>`_. For now, to use
-        the port:
-        
-        using pip::
-        
-            git clone https://github.com/jacobschaer/python-uds
-            git checkout doip
-            cd python-uds
-            pip install .
-        
-        Example:
-        
-        .. code-block:: python
-        
-           from uds import Uds
-        
-           ecu = Uds(transportProtocol="DoIP", ecu_ip="192.168.1.1", ecu_logical_address=1)
-           try:
-               response = ecu.send([0x3E, 0x00])
-               print(response)  # This should be [0x7E, 0x00]
-           except:
-               print("Send did not complete")
 Keywords: uds,14229,iso-14229,diagnostic,automotive,13400,iso-13400,doip
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+python-doipclient
+#################
+
+.. image:: https://github.com/jacobschaer/python-doipclient/actions/workflows/tests.yml/badge.svg?branch=main
+
+doipclient is a pure Python 3 Diagnostic over IP (DoIP) client which can be used
+for communicating with modern ECU's over automotive ethernet. It implements the
+majority of ISO-13400 (2019) from the perspective of a short-lived synchronous
+client. The primary use case is to serve as a transport layer implementation for
+the `udsoncan <https://github.com/pylessard/python-udsoncan>`_ library. The code
+is published under MIT license on GitHub (jacobschaer/python-doipclient).
+
+Documentation
+-------------
+
+The documentation is available here : https://python-doipclient.readthedocs.io/
+
+Requirements
+------------
+
+ - Python 3.6+
+
+Installation
+------------
+
+using pip::
+
+    pip install doipclient
+
+Running Tests from source
+-------------------------
+
+using pytest::
+
+    pip install pytest pytest-mock
+    pytest
+
+Example
+-------
+Updated version of udsoncan's example using `python_doip` instead of IsoTPSocketConnection
+
+.. code-block:: python
+
+   import SomeLib.SomeCar.SomeModel as MyCar
+
+   import udsoncan
+   from doipclient import DoIPClient
+   from doipclient.connectors import DoIPClientUDSConnector
+   from udsoncan.client import Client
+   from udsoncan.exceptions import *
+   from udsoncan.services import *
+   
+   udsoncan.setup_logging()
+   
+   ecu_ip = '127.0.0.1'
+   ecu_logical_address = 0x00E0
+   doip_client = DoIPClient(ecu_ip, ecu_logical_address)
+   conn = DoIPClientUDSConnector(doip_client)
+   with Client(conn, request_timeout=2, config=MyCar.config) as client:
+      try:
+         client.change_session(DiagnosticSessionControl.Session.extendedDiagnosticSession)  # integer with value of 3
+         client.unlock_security_access(MyCar.debug_level)                                   # Fictive security level. Integer coming from fictive lib, let's say its value is 5
+         client.write_data_by_identifier(udsoncan.DataIdentifier.VIN, 'ABC123456789')       # Standard ID for VIN is 0xF190. Codec is set in the client configuration
+         print('Vehicle Identification Number successfully changed.')
+         client.ecu_reset(ECUReset.ResetType.hardReset)                                     # HardReset = 0x01
+      except NegativeResponseException as e:
+         print('Server refused our request for service %s with code "%s" (0x%02x)' % (e.response.service.get_name(), e.response.code_name, e.response.code))
+      except (InvalidResponseException, UnexpectedResponseException) as e:
+         print('Server sent an invalid payload : %s' % e.response.original_payload)
+
+      # Because we reset our UDS server, we must also reconnect/reactivate the DoIP socket
+      # Alternatively, we could have used the auto_reconnect_tcp flag on the DoIPClient
+      # Note: ECU's do not restart instantly, so you may need a sleep() before moving on
+      doip_client.reconnect()
+      client.tester_present()
+
+   # Cleanup the DoIP Socket when we're done. Alternatively, we could have used the
+   # close_connection flag on conn so that the udsoncan client would clean it up
+   doip_client.close()
+
+python-uds Support
+------------------
+The `python-uds <https://github.com/richClubb/python-uds>`_ can also be used
+but requires a fork until the owner merges this PR
+`Doip #63 <https://github.com/richClubb/python-uds/pull/63>`_. For now, to use
+the port:
+
+using pip::
+
+    git clone https://github.com/jacobschaer/python-uds
+    git checkout doip
+    cd python-uds
+    pip install .
+
+Example:
+
+.. code-block:: python
+
+   from uds import Uds
+
+   ecu = Uds(transportProtocol="DoIP", ecu_ip="192.168.1.1", ecu_logical_address=1)
+   try:
+       response = ecu.send([0x3E, 0x00])
+       print(response)  # This should be [0x7E, 0x00]
+   except:
+       print("Send did not complete")
```

### Comparing `doipclient-1.0.8/PKG-INFO` & `doipclient-1.0.9/doipclient.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,122 +1,121 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: doipclient
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Diagnostic over IP (DoIP) client implementing ISO-13400-2.
 Home-page: https://github.com/jacobschaer/python-doipclient
 Author: Jacob Schaer
-Author-email: UNKNOWN
-License: UNKNOWN
-Description: python-doipclient
-        #################
-        
-        .. image:: https://travis-ci.com/jacobschaer/python-doipclient.svg?branch=main
-            :target: https://travis-ci.com/jacobschaer/python-doipclient
-        
-        doipclient is a pure Python 3 Diagnostic over IP (DoIP) client which can be used
-        for communicating with modern ECU's over automotive ethernet. It implements the
-        majority of ISO-13400 (2019) from the perspective of a short-lived synchronous
-        client. The primary use case is to serve as a transport layer implementation for
-        the `udsoncan <https://github.com/pylessard/python-udsoncan>`_ library. The code
-        is published under MIT license on GitHub (jacobschaer/python-doipclient).
-        
-        Documentation
-        -------------
-        
-        The documentation is available here : https://python-doipclient.readthedocs.io/
-        
-        Requirements
-        ------------
-        
-         - Python 3.6+
-        
-        Installation
-        ------------
-        
-        using pip::
-        
-            pip install doipclient
-        
-        Running Tests from source
-        -------------------------
-        
-        using pytest::
-        
-            pip install pytest pytest-mock
-            pytest
-        
-        Example
-        -------
-        Updated version of udsoncan's example using `python_doip` instead of IsoTPSocketConnection
-        
-        .. code-block:: python
-        
-           import SomeLib.SomeCar.SomeModel as MyCar
-        
-           import udsoncan
-           from doipclient import DoIPClient
-           from doipclient.connectors import DoIPClientUDSConnector
-           from udsoncan.client import Client
-           from udsoncan.exceptions import *
-           from udsoncan.services import *
-           
-           udsoncan.setup_logging()
-           
-           ecu_ip = '127.0.0.1'
-           ecu_logical_address = 0x00E0
-           doip_client = DoIPClient(ecu_ip, ecu_logical_address)
-           conn = DoIPClientUDSConnector(doip_client)
-           with Client(conn, request_timeout=2, config=MyCar.config) as client:
-              try:
-                 client.change_session(DiagnosticSessionControl.Session.extendedDiagnosticSession)  # integer with value of 3
-                 client.unlock_security_access(MyCar.debug_level)                                   # Fictive security level. Integer coming from fictive lib, let's say its value is 5
-                 client.write_data_by_identifier(udsoncan.DataIdentifier.VIN, 'ABC123456789')       # Standard ID for VIN is 0xF190. Codec is set in the client configuration
-                 print('Vehicle Identification Number successfully changed.')
-                 client.ecu_reset(ECUReset.ResetType.hardReset)                                     # HardReset = 0x01
-              except NegativeResponseException as e:
-                 print('Server refused our request for service %s with code "%s" (0x%02x)' % (e.response.service.get_name(), e.response.code_name, e.response.code))
-              except (InvalidResponseException, UnexpectedResponseException) as e:
-                 print('Server sent an invalid payload : %s' % e.response.original_payload)
-        
-              # Because we reset our UDS server, we must also reconnect/reactivate the DoIP socket
-              # Alternatively, we could have used the auto_reconnect_tcp flag on the DoIPClient
-              # Note: ECU's do not restart instantly, so you may need a sleep() before moving on
-              doip_client.reconnect()
-              client.tester_present()
-        
-           # Cleanup the DoIP Socket when we're done. Alternatively, we could have used the
-           # close_connection flag on conn so that the udsoncan client would clean it up
-           doip_client.close()
-        
-        python-uds Support
-        ------------------
-        The `python-uds <https://github.com/richClubb/python-uds>`_ can also be used
-        but requires a fork until the owner merges this PR
-        `Doip #63 <https://github.com/richClubb/python-uds/pull/63>`_. For now, to use
-        the port:
-        
-        using pip::
-        
-            git clone https://github.com/jacobschaer/python-uds
-            git checkout doip
-            cd python-uds
-            pip install .
-        
-        Example:
-        
-        .. code-block:: python
-        
-           from uds import Uds
-        
-           ecu = Uds(transportProtocol="DoIP", ecu_ip="192.168.1.1", ecu_logical_address=1)
-           try:
-               response = ecu.send([0x3E, 0x00])
-               print(response)  # This should be [0x7E, 0x00]
-           except:
-               print("Send did not complete")
 Keywords: uds,14229,iso-14229,diagnostic,automotive,13400,iso-13400,doip
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+python-doipclient
+#################
+
+.. image:: https://github.com/jacobschaer/python-doipclient/actions/workflows/tests.yml/badge.svg?branch=main
+
+doipclient is a pure Python 3 Diagnostic over IP (DoIP) client which can be used
+for communicating with modern ECU's over automotive ethernet. It implements the
+majority of ISO-13400 (2019) from the perspective of a short-lived synchronous
+client. The primary use case is to serve as a transport layer implementation for
+the `udsoncan <https://github.com/pylessard/python-udsoncan>`_ library. The code
+is published under MIT license on GitHub (jacobschaer/python-doipclient).
+
+Documentation
+-------------
+
+The documentation is available here : https://python-doipclient.readthedocs.io/
+
+Requirements
+------------
+
+ - Python 3.6+
+
+Installation
+------------
+
+using pip::
+
+    pip install doipclient
+
+Running Tests from source
+-------------------------
+
+using pytest::
+
+    pip install pytest pytest-mock
+    pytest
+
+Example
+-------
+Updated version of udsoncan's example using `python_doip` instead of IsoTPSocketConnection
+
+.. code-block:: python
+
+   import SomeLib.SomeCar.SomeModel as MyCar
+
+   import udsoncan
+   from doipclient import DoIPClient
+   from doipclient.connectors import DoIPClientUDSConnector
+   from udsoncan.client import Client
+   from udsoncan.exceptions import *
+   from udsoncan.services import *
+   
+   udsoncan.setup_logging()
+   
+   ecu_ip = '127.0.0.1'
+   ecu_logical_address = 0x00E0
+   doip_client = DoIPClient(ecu_ip, ecu_logical_address)
+   conn = DoIPClientUDSConnector(doip_client)
+   with Client(conn, request_timeout=2, config=MyCar.config) as client:
+      try:
+         client.change_session(DiagnosticSessionControl.Session.extendedDiagnosticSession)  # integer with value of 3
+         client.unlock_security_access(MyCar.debug_level)                                   # Fictive security level. Integer coming from fictive lib, let's say its value is 5
+         client.write_data_by_identifier(udsoncan.DataIdentifier.VIN, 'ABC123456789')       # Standard ID for VIN is 0xF190. Codec is set in the client configuration
+         print('Vehicle Identification Number successfully changed.')
+         client.ecu_reset(ECUReset.ResetType.hardReset)                                     # HardReset = 0x01
+      except NegativeResponseException as e:
+         print('Server refused our request for service %s with code "%s" (0x%02x)' % (e.response.service.get_name(), e.response.code_name, e.response.code))
+      except (InvalidResponseException, UnexpectedResponseException) as e:
+         print('Server sent an invalid payload : %s' % e.response.original_payload)
+
+      # Because we reset our UDS server, we must also reconnect/reactivate the DoIP socket
+      # Alternatively, we could have used the auto_reconnect_tcp flag on the DoIPClient
+      # Note: ECU's do not restart instantly, so you may need a sleep() before moving on
+      doip_client.reconnect()
+      client.tester_present()
+
+   # Cleanup the DoIP Socket when we're done. Alternatively, we could have used the
+   # close_connection flag on conn so that the udsoncan client would clean it up
+   doip_client.close()
+
+python-uds Support
+------------------
+The `python-uds <https://github.com/richClubb/python-uds>`_ can also be used
+but requires a fork until the owner merges this PR
+`Doip #63 <https://github.com/richClubb/python-uds/pull/63>`_. For now, to use
+the port:
+
+using pip::
+
+    git clone https://github.com/jacobschaer/python-uds
+    git checkout doip
+    cd python-uds
+    pip install .
+
+Example:
+
+.. code-block:: python
+
+   from uds import Uds
+
+   ecu = Uds(transportProtocol="DoIP", ecu_ip="192.168.1.1", ecu_logical_address=1)
+   try:
+       response = ecu.send([0x3E, 0x00])
+       print(response)  # This should be [0x7E, 0x00]
+   except:
+       print("Send did not complete")
```

### Comparing `doipclient-1.0.8/README.rst` & `doipclient-1.0.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 python-doipclient
 #################
 
-.. image:: https://travis-ci.com/jacobschaer/python-doipclient.svg?branch=main
-    :target: https://travis-ci.com/jacobschaer/python-doipclient
+.. image:: https://github.com/jacobschaer/python-doipclient/actions/workflows/tests.yml/badge.svg?branch=main
 
 doipclient is a pure Python 3 Diagnostic over IP (DoIP) client which can be used
 for communicating with modern ECU's over automotive ethernet. It implements the
 majority of ISO-13400 (2019) from the perspective of a short-lived synchronous
 client. The primary use case is to serve as a transport layer implementation for
 the `udsoncan <https://github.com/pylessard/python-udsoncan>`_ library. The code
 is published under MIT license on GitHub (jacobschaer/python-doipclient).
```

### Comparing `doipclient-1.0.8/setup.py` & `doipclient-1.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import setuptools
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="doipclient",
-    version="1.0.8",
+    version="1.0.9",
     description="A Diagnostic over IP (DoIP) client implementing ISO-13400-2.",
     long_description=long_description,
+    long_description_content_type='text/x-rst',
     author="Jacob Schaer",
     url="https://github.com/jacobschaer/python-doipclient",
     packages=setuptools.find_packages(),
     keywords=[
         "uds",
         "14229",
         "iso-14229",
```

### Comparing `doipclient-1.0.8/tests/test_client.py` & `doipclient-1.0.9/tests/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import socket
+import ssl
 import pytest
 import logging
 from doipclient import DoIPClient
 from doipclient.client import Parser
 from doipclient.messages import *
 
 try:
@@ -612,19 +613,21 @@
     try:
         DoIPClient.await_vehicle_announcement(
             udp_port=13400, timeout=0.1, ipv6=True, source_interface=None
         )
     except TimeoutError:
         pass
     assert mock_socket._network == socket.AF_INET6
-    assert mock_socket._bound_ip == 'ff02::1'
+    assert mock_socket._bound_ip == "ff02::1"
     assert mock_socket._bound_port == 13400
     assert mock_socket.opts == {
         socket.SOL_SOCKET: {socket.SO_REUSEADDR: True},
-        IPPROTO_IPV6: {socket.IPV6_JOIN_GROUP: b'\xff\x02\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00'},
+        IPPROTO_IPV6: {
+            socket.IPV6_JOIN_GROUP: b"\xff\x02\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00"
+        },
     }
 
 
 def test_await_ipv4(mock_socket):
     mock_socket.rx_queue.clear()
     try:
         DoIPClient.await_vehicle_announcement(
@@ -633,8 +636,45 @@
     except TimeoutError:
         pass
     assert mock_socket._network == socket.AF_INET
     assert mock_socket._bound_ip == ""
     assert mock_socket._bound_port == 13400
     assert mock_socket.opts == {
         socket.SOL_SOCKET: {socket.SO_REUSEADDR: True, socket.SO_BROADCAST: True},
-    }
+    }
+
+
+def test_exception_from_blocking_ssl_socket(mock_socket, mocker):
+    """SSL sockets behave slightly different than regular sockets in
+    non-blocking mode. They won't raise BlockingIOError but SSLWantWriteError
+    or SSLWantReadError instead.
+
+    See: https://docs.python.org/3/library/ssl.html#notes-on-non-blocking-sockets
+    """
+    sut = DoIPClient(test_ip, test_logical_address)
+
+    try:
+        sut._tcp_sock.recv = mocker.Mock(side_effect=ssl.SSLWantReadError)
+        sut._tcp_socket_check()
+        sut._tcp_sock.recv = mocker.Mock(side_effect=ssl.SSLWantWriteError)
+        sut._tcp_socket_check()
+    except (ssl.SSLWantReadError, ssl.SSLWantWriteError) as exc:
+        pytest.fail(f"Should not raise exception: {exc.__class__.__name__}")
+
+
+def test_use_secure_uses_default_ssl_context(mock_socket, mocker):
+    """Wrap socket with default SSL-context when use_secure=True"""
+    mocked_context = mocker.patch.object(ssl, "SSLContext", autospec=True)
+    sut = DoIPClient(
+        test_ip, test_logical_address, use_secure=True, activation_type=None
+    )
+    mocked_wrap_socket = mocked_context.return_value.wrap_socket
+    mocked_wrap_socket.assert_called_once_with(mock_socket)
+
+
+def test_use_secure_with_external_ssl_context(mock_socket, mocker):
+    """Wrap socket with user provided SSL-context when use_secure=ssl_context"""
+    mocked_context = mocker.patch.object(ssl, "SSLContext", autospec=True)
+    sut = DoIPClient(
+        test_ip, test_logical_address, use_secure=mocked_context, activation_type=None
+    )
+    mocked_context.wrap_socket.assert_called_once_with(mock_socket)
```

