# Comparing `tmp/ssdp-1.2.0.tar.gz` & `tmp/ssdp-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssdp-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ssdp-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ssdp-1.2.0.tar` & `ssdp-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2023-06-11 13:26:21.152245 ssdp-1.2.0/LICENSE
--rw-r--r--   0        0        0     5489 2023-06-11 13:26:21.152245 ssdp-1.2.0/README.md
--rw-r--r--   0        0        0     1929 2023-06-11 13:26:21.152245 ssdp-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      491 2023-06-11 13:26:21.152245 ssdp-1.2.0/ssdp/__init__.py
--rw-r--r--   0        0        0     2896 2023-06-11 13:26:21.152245 ssdp-1.2.0/ssdp/__main__.py
--rw-r--r--   0        0        0      160 2023-06-11 13:26:37.412490 ssdp-1.2.0/ssdp/_version.py
--rw-r--r--   0        0        0     1997 2023-06-11 13:26:21.152245 ssdp-1.2.0/ssdp/aio.py
--rw-r--r--   0        0        0      398 2023-06-11 13:26:21.152245 ssdp-1.2.0/ssdp/deprecation.py
--rw-r--r--   0        0        0     1627 2023-06-11 13:26:21.152245 ssdp-1.2.0/ssdp/lexers.py
--rw-r--r--   0        0        0     3607 2023-06-11 13:26:21.152245 ssdp-1.2.0/ssdp/messages.py
--rw-r--r--   0        0        0      874 2023-06-11 13:26:21.152245 ssdp-1.2.0/ssdp/network.py
--rw-r--r--   0        0        0     6979 1970-01-01 00:00:00.000000 ssdp-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-04 16:16:06.934184 ssdp-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5489 2023-07-04 16:16:06.934184 ssdp-1.3.0/README.md
+-rw-r--r--   0        0        0     1929 2023-07-04 16:16:06.934184 ssdp-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      491 2023-07-04 16:16:06.934184 ssdp-1.3.0/ssdp/__init__.py
+-rw-r--r--   0        0        0     2896 2023-07-04 16:16:06.934184 ssdp-1.3.0/ssdp/__main__.py
+-rw-r--r--   0        0        0      160 2023-07-04 16:16:24.934308 ssdp-1.3.0/ssdp/_version.py
+-rw-r--r--   0        0        0     1997 2023-07-04 16:16:06.934184 ssdp-1.3.0/ssdp/aio.py
+-rw-r--r--   0        0        0      398 2023-07-04 16:16:06.934184 ssdp-1.3.0/ssdp/deprecation.py
+-rw-r--r--   0        0        0     1627 2023-07-04 16:16:06.934184 ssdp-1.3.0/ssdp/lexers.py
+-rw-r--r--   0        0        0     4033 2023-07-04 16:16:06.934184 ssdp-1.3.0/ssdp/messages.py
+-rw-r--r--   0        0        0      874 2023-07-04 16:16:06.934184 ssdp-1.3.0/ssdp/network.py
+-rw-r--r--   0        0        0     6979 1970-01-01 00:00:00.000000 ssdp-1.3.0/PKG-INFO
```

### Comparing `ssdp-1.2.0/LICENSE` & `ssdp-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssdp-1.2.0/README.md` & `ssdp-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ssdp-1.2.0/pyproject.toml` & `ssdp-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ssdp-1.2.0/ssdp/__main__.py` & `ssdp-1.3.0/ssdp/__main__.py`

 * *Files identical despite different names*

### Comparing `ssdp-1.2.0/ssdp/aio.py` & `ssdp-1.3.0/ssdp/aio.py`

 * *Files identical despite different names*

### Comparing `ssdp-1.2.0/ssdp/lexers.py` & `ssdp-1.3.0/ssdp/lexers.py`

 * *Files identical despite different names*

### Comparing `ssdp-1.2.0/ssdp/messages.py` & `ssdp-1.3.0/ssdp/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     def __str__(self):
         """Return full HTTP message."""
         raise NotImplementedError()
 
     def __bytes__(self):
         """Return full HTTP message as bytes."""
-        return self.__str__().encode().replace(b"\n", b"\r\n") + b"\r\n\r\n"
+        return self.__str__().encode() + b"\r\n\r\n"
 
 
 class SSDPResponse(SSDPMessage):
     """Simple Service Discovery Protocol (SSDP) response."""
 
     def __init__(self, status_code, reason, **kwargs):
         self.status_code = int(status_code)
@@ -70,14 +70,28 @@
         lines = msg.splitlines()
         version, status_code, reason = lines[0].split()
         headers = cls.parse_headers("\r\n".join(lines[1:]))
         return cls(
             version=version, status_code=status_code, reason=reason, headers=headers
         )
 
+    def sendto(self, transport, addr):
+        """
+        Send response to a given address via given transport.
+
+        Args:
+            transport (asyncio.DatagramTransport):
+                Write transport to send the message on.
+            addr (Tuple[str, int]):
+                IP address and port pair to send the message to.
+
+        """
+        logger.debug("%s:%s - - %s", *(addr + (self,)))
+        transport.sendto(bytes(self), addr)
+
     def __str__(self):
         """Return complete SSDP response."""
         lines = list()
         lines.append(" ".join([self.version, str(self.status_code), self.reason]))
         for header in self.headers:
             lines.append("%s: %s" % header)
         return "\r\n".join(lines)
```

### Comparing `ssdp-1.2.0/ssdp/network.py` & `ssdp-1.3.0/ssdp/network.py`

 * *Files identical despite different names*

### Comparing `ssdp-1.2.0/PKG-INFO` & `ssdp-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssdp
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python asyncio library for Simple Service Discovery Protocol (SSDP).
 Keywords: ssdp,python,asyncio,upnp,iot
 Author-email: Johannes Maron <johannes@maron.family>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

