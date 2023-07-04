# Comparing `tmp/kade_drive-0.1.0.tar.gz` & `tmp/kade_drive-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kade_drive-0.1.0.tar", max compression
+gzip compressed data, was "kade_drive-0.2.0.tar", max compression
```

## Comparing `kade_drive-0.1.0.tar` & `kade_drive-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1069 2023-05-31 00:41:16.838542 kade_drive-0.1.0/LICENSE
--rw-r--r--   0        0        0      220 2023-07-04 03:13:39.414643 kade_drive-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-04 03:33:26.660364 kade_drive-0.1.0/kade_drive/__init__.py
--rw-r--r--   0        0        0     1574 2023-07-04 03:36:54.317172 kade_drive-0.1.0/kade_drive/cli.py
--rw-r--r--   0        0        0     6111 2023-07-04 03:36:23.347903 kade_drive-0.1.0/kade_drive/client.py
--rw-r--r--   0        0        0        1 2023-07-04 03:13:39.414643 kade_drive-0.1.0/kade_drive/core/__init__.py
--rw-r--r--   0        0        0     9109 2023-07-04 03:13:39.414643 kade_drive-0.1.0/kade_drive/core/crawling.py
--rw-r--r--   0        0        0    18361 2023-07-04 03:13:39.414643 kade_drive-0.1.0/kade_drive/core/network.py
--rw-r--r--   0        0        0     3994 2023-07-04 03:13:39.414643 kade_drive-0.1.0/kade_drive/core/node.py
--rw-r--r--   0        0        0     7886 2023-07-04 03:13:39.414643 kade_drive-0.1.0/kade_drive/core/protocol.py
--rw-r--r--   0        0        0     8614 2023-07-04 03:13:39.414643 kade_drive-0.1.0/kade_drive/core/routing.py
--rw-r--r--   0        0        0     9169 2023-07-04 03:13:39.414643 kade_drive-0.1.0/kade_drive/core/storage.py
--rw-r--r--   0        0        0     1340 2023-07-04 03:13:39.414643 kade_drive-0.1.0/kade_drive/core/utils.py
--rw-r--r--   0        0        0      209 2023-06-21 14:46:22.196979 kade_drive-0.1.0/kade_drive/main_recv.py
--rw-r--r--   0        0        0      248 2023-06-22 16:03:58.821886 kade_drive-0.1.0/kade_drive/main_send.py
--rw-r--r--   0        0        0        0 2023-07-04 03:13:39.414643 kade_drive-0.1.0/kade_drive/message_system/__init__.py
--rw-r--r--   0        0        0     6954 2023-07-04 03:13:39.414643 kade_drive-0.1.0/kade_drive/message_system/message_system.py
--rw-r--r--   0        0        0     2244 2023-07-04 03:13:39.415643 kade_drive-0.1.0/kade_drive/server.py
--rw-r--r--   0        0        0       25 2023-06-27 22:54:55.421483 kade_drive-0.1.0/kade_drive/tests/__init__.py
--rw-r--r--   0        0        0     1598 2023-07-04 03:13:39.415643 kade_drive-0.1.0/kade_drive/tests/conftest.py
--rw-r--r--   0        0        0     3100 2023-06-27 22:54:55.421483 kade_drive-0.1.0/kade_drive/tests/data_to_split.txt
--rw-r--r--   0        0        0     1785 2023-07-04 03:13:39.415643 kade_drive-0.1.0/kade_drive/tests/test_node.py
--rw-r--r--   0        0        0     4520 2023-07-04 03:13:39.415643 kade_drive-0.1.0/kade_drive/tests/test_routing.py
--rw-r--r--   0        0        0        1 2023-07-04 03:13:39.415643 kade_drive-0.1.0/kade_drive/tests/test_server.py
--rw-r--r--   0        0        0      841 2023-07-04 03:39:24.651482 kade_drive-0.1.0/kade_drive/tests/test_splitdata.py
--rw-r--r--   0        0        0     1458 2023-06-27 22:54:55.421483 kade_drive-0.1.0/kade_drive/tests/test_storage.py
--rw-r--r--   0        0        0      678 2023-07-04 03:39:29.194521 kade_drive-0.1.0/kade_drive/tests/test_store_file.py
--rw-r--r--   0        0        0      717 2023-07-04 03:13:39.415643 kade_drive-0.1.0/kade_drive/tests/test_utils.py
--rw-r--r--   0        0        0      508 2023-07-04 04:30:43.691648 kade_drive-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 kade_drive-0.1.0/setup.py
--rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 kade_drive-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-31 00:41:16.838542 kade_drive-0.2.0/LICENSE
+-rw-r--r--   0        0        0      220 2023-07-04 03:13:39.414643 kade_drive-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-04 16:17:23.029053 kade_drive-0.2.0/kade_drive/__init__.py
+-rw-r--r--   0        0        0     1574 2023-07-04 16:17:23.029053 kade_drive-0.2.0/kade_drive/cli.py
+-rw-r--r--   0        0        0     6752 2023-07-04 16:41:46.747892 kade_drive-0.2.0/kade_drive/client.py
+-rw-r--r--   0        0        0        1 2023-07-04 16:17:23.029053 kade_drive-0.2.0/kade_drive/core/__init__.py
+-rw-r--r--   0        0        0     9109 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/core/crawling.py
+-rw-r--r--   0        0        0    18449 2023-07-04 16:51:20.329071 kade_drive-0.2.0/kade_drive/core/network.py
+-rw-r--r--   0        0        0     3994 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/core/node.py
+-rw-r--r--   0        0        0     7886 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/core/protocol.py
+-rw-r--r--   0        0        0     8614 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/core/routing.py
+-rw-r--r--   0        0        0     9169 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/core/storage.py
+-rw-r--r--   0        0        0     1340 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/core/utils.py
+-rw-r--r--   0        0        0      209 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/main_recv.py
+-rw-r--r--   0        0        0      248 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/main_send.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/message_system/__init__.py
+-rw-r--r--   0        0        0     6954 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/message_system/message_system.py
+-rw-r--r--   0        0        0     2244 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/server.py
+-rw-r--r--   0        0        0       25 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/__init__.py
+-rw-r--r--   0        0        0     1598 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/conftest.py
+-rw-r--r--   0        0        0     3100 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/data_to_split.txt
+-rw-r--r--   0        0        0     1785 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/test_node.py
+-rw-r--r--   0        0        0     4520 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/test_routing.py
+-rw-r--r--   0        0        0        1 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/test_server.py
+-rw-r--r--   0        0        0      841 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/test_splitdata.py
+-rw-r--r--   0        0        0     1458 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/test_storage.py
+-rw-r--r--   0        0        0      678 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/test_store_file.py
+-rw-r--r--   0        0        0      717 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/test_utils.py
+-rw-r--r--   0        0        0      508 2023-07-04 19:15:12.893711 kade_drive-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 kade_drive-0.2.0/setup.py
+-rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 kade_drive-0.2.0/PKG-INFO
```

### Comparing `kade_drive-0.1.0/LICENSE` & `kade_drive-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/cli.py` & `kade_drive-0.2.0/kade_drive/cli.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/client.py` & `kade_drive-0.2.0/kade_drive/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,52 +68,68 @@
             print(
                 f"Connection to {ip} failed, removing from bootstrap nodes list.")
             nodes_to_try.pop(0)
             return nodes_to_try, total_attempts_to_reconnect
 
         return nodes_to_try, remaining_attempts_to_reconnect
 
-    def get(self, key):
-        metadata_list = self.connection.root.get(key)
+    def get(self, key, apply_hash_to_key=True):
+        logger = logging.getLogger(__name__)
+        if not self.connection:
+            logger.error(f'No connection stablished to do get')
+            return None
+        metadata_list = self.connection.root.get(key, apply_hash_to_key)
         logger = logging.getLogger(__name__)
 
         logger.debug(f'metadata_list received {str(len(metadata_list) > 0)}')
         data_received = []
+
+        if metadata_list is None or len(metadata_list) == 0:
+            logger.debug(f'No data with key {key}')
+            return None
+
         for chunk_key in metadata_list:
             # print('chunk key', chunk_key)
             locations: list[tuple[str, int]] = self.connection.root.get_file_chunk_location(
                 chunk_key)
             logger.debug(
                 f'locations for chunk_key {chunk_key} are {locations}')
             if self.bootstrap_nodes[0] in locations:
                 logger.debug('Using primary connection to get chunk')
                 data_received.append(
-                    self.connection.root.get_file_chunk_value(chunk_key))
+                    self.connection.root.rpc_get_file_chunk_value(chunk_key))
             else:
-                conn = self._ensure_connection(
+                conn, _ = self._ensure_connection(
                     locations, None, use_broadcast_if_needed=False, update_boostrap_nodes=False)
                 if conn:
                     data_received.append(
-                        conn.root.get_file_chunk_value(chunk_key))
+                        conn.root.rpc_get_file_chunk_value(chunk_key))
                 else:
                     logger.warning('No Servers to get chunk')
 
         # data_recv = bytearray()
         logger.debug('len data received', len(data_received))
         data_received = b''.join(data_received)
-        return pickle.loads(data_received)
-
+        try:
+            data_to_return = pickle.loads(data_received)
+            return data_to_return
+        except pickle.UnpicklingError as e:
+            logger.error(e)
+            return None
+        
     def put(self, key, value: bytes, apply_hash_to_key=True):
         logger = logging.getLogger(__name__)
-
         logger.debug(f'key: {key}, value: {value}')
         # print(self.connection.root.upload_file.)
-        self.connection.root.upload_file(key=key, data=value, apply_hash_to_key=apply_hash_to_key)
-        sleep(1)
-        logger.info(f'put > Success')
+        if self.connection:
+            self.connection.root.upload_file(key=key, data=value, apply_hash_to_key=apply_hash_to_key)
+            sleep(1)
+            logger.info(f'put > Success')
+        else: 
+            logger.error(f'No connection stablished to do put')
 
     def _update_bootstrap_nodes(self, connection: rpyc.Connection):
         logger = logging.getLogger(__name__)
 
         nodes_to_add = [node for node in connection.root.find_neighbors(
         ) if node not in self.bootstrap_nodes]
         self.bootstrap_nodes.extend(nodes_to_add)
```

### Comparing `kade_drive-0.1.0/kade_drive/core/crawling.py` & `kade_drive-0.2.0/kade_drive/core/crawling.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/core/network.py` & `kade_drive-0.2.0/kade_drive/core/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,29 +325,25 @@
         Args:
             sender : sender node
             nodeid (bytes): node to be probed
 
         Returns:
             bytes: node id if alive, None if not 
         """
-        
-
         logger.debug(f"rpc ping called from {nodeid}, {sender[0]}, {sender[1]}")
         source = Node(nodeid, sender[0], sender[1])
         # if a new node is sending the request, give all data it should contain
         address = (source.ip, source.port)
         with ServerSession(address[0], address[1]) as conn:
             FileSystemProtocol.welcome_if_new(conn, source)
         logger.debug("return ping")
         return FileSystemProtocol.source_node.id
 
     @rpyc.exposed
     def rpc_find_node(self, sender, nodeid: bytes, key: bytes):
-        
-
         logger.debug(
             f"finding neighbors of {int(nodeid.hex(), 16)} in local table")
 
         source = Node(nodeid, sender[0], sender[1])
 
         logger.debug(f'node id {nodeid}')
         # if a new node is sending the request, give all data it should contain
@@ -373,15 +369,15 @@
         address = (source.ip, source.port)
         with ServerSession(address[0], address[1]) as conn:
             FileSystemProtocol.welcome_if_new(conn, source)
         # get value from storage
         return FileSystemProtocol.storage.contains(key)
 
     @rpyc.exposed
-    def get_file_chunk_value(self, key):
+    def rpc_get_file_chunk_value(self, key):
         return Server.storage.get(key, metadata=False)
 
     @rpyc.exposed
     def bootstrappable_neighbors(self):
         """
         Get a :class:`list` of (ip, port) :class:`tuple` pairs suitable for
         use as an argument to the bootstrap method.
@@ -402,31 +398,33 @@
         Returns:
             :class:`None` if not found, the value otherwise.
         """
         
         logger.debug(f"Looking up key {key}")
         if apply_hash_to_key:
             key = digest(key)
-        # if this node has it, return it
-        if Server.storage.get(key, True) is not None:
-            return pickle.loads(Server.storage.get(key, True))
+        
         node = Node(key)
         nearest = FileSystemProtocol.router.find_neighbors(node)
         if not nearest:
-            logger.info(f"There are no known neighbors to get key {key}")
+            logger.debug(f"There are no known neighbors to get key {key}")
+            if Server.storage.contains(key) is not None:
+                logger.debug(f'Getting key from this same node')
+                return pickle.loads(Server.storage.get(key, True))
             return None
         spider = ValueSpiderCrawl(node, nearest,
                                   Server.ksize, Server.alpha)
-        metadata_list = pickle.loads(spider.find())
+        data = spider.find()
+        if data is None:
+            return None
+        metadata_list = pickle.loads(data)
         return metadata_list
 
     @rpyc.exposed
     def get_file_chunk_location(self, chunk_key):
-        
-
         logger.debug('looking file chunk location')
         node = Node(chunk_key)
         nearest = FileSystemProtocol.router.find_neighbors(node)
         if not nearest:
             logger.debug(
                 f"There are no known neighbors to get file chunk location {chunk_key}")
             if Server.storage.contains(chunk_key) is not None:
@@ -436,15 +434,15 @@
 
         logger.debug('Initiating ChunkLocationSpiderCrawl')
         spider = ChunkLocationSpiderCrawl(
             node, nearest, Server.ksize, Server.alpha)
         results = spider.find()
         logger.debug(f'results of ChunkLocationSpider {results}')
         return results
-
+    
     @rpyc.exposed
     def upload_file(self, key, data: bytes, apply_hash_to_key=True):
         chunks = Server.split_data(data, 1000)
         logger.debug(f'chunks {len(chunks)}, {chunks}')
         digested_chunks = [digest(c) for c in chunks]
         metadata_list = pickle.dumps(digested_chunks)
         processed_chunks = ((digest(c), c) for c in chunks)
```

### Comparing `kade_drive-0.1.0/kade_drive/core/node.py` & `kade_drive-0.2.0/kade_drive/core/node.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/core/protocol.py` & `kade_drive-0.2.0/kade_drive/core/protocol.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/core/routing.py` & `kade_drive-0.2.0/kade_drive/core/routing.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/core/storage.py` & `kade_drive-0.2.0/kade_drive/core/storage.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/core/utils.py` & `kade_drive-0.2.0/kade_drive/core/utils.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/message_system/message_system.py` & `kade_drive-0.2.0/kade_drive/message_system/message_system.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/server.py` & `kade_drive-0.2.0/kade_drive/server.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/tests/conftest.py` & `kade_drive-0.2.0/kade_drive/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/tests/data_to_split.txt` & `kade_drive-0.2.0/kade_drive/tests/data_to_split.txt`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/tests/test_node.py` & `kade_drive-0.2.0/kade_drive/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/tests/test_routing.py` & `kade_drive-0.2.0/kade_drive/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/tests/test_splitdata.py` & `kade_drive-0.2.0/kade_drive/tests/test_splitdata.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/tests/test_storage.py` & `kade_drive-0.2.0/kade_drive/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/tests/test_store_file.py` & `kade_drive-0.2.0/kade_drive/tests/test_store_file.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/kade_drive/tests/test_utils.py` & `kade_drive-0.2.0/kade_drive/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.1.0/setup.py` & `kade_drive-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['netifaces==0.11.0', 'rpyc==5.3.1', 'typer==0.9.0']
 
 setup_kwargs = {
     'name': 'kade-drive',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'distributed file system based on kademlia dht',
     'long_description': 'Sistema de ficheros distribuidos immplementado usando el codigo fuente de la implementacion de Kademlia en https://github.com/bmuller/kademlia \n\n### Tests\nPara Correr los tests se requiere un servidor levantado en la red',
     'author': 'DanielUH2019',
     'author_email': 'danielcardenascabrera2016@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kade_drive-0.1.0/PKG-INFO` & `kade_drive-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kade-drive
-Version: 0.1.0
+Version: 0.2.0
 Summary: distributed file system based on kademlia dht
 License: MIT
 Author: DanielUH2019
 Author-email: danielcardenascabrera2016@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

