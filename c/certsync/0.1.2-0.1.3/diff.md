# Comparing `tmp/certsync-0.1.2.tar.gz` & `tmp/certsync-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certsync-0.1.2.tar", max compression
+gzip compressed data, was "certsync-0.1.3.tar", max compression
```

## Comparing `certsync-0.1.2.tar` & `certsync-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-04-15 14:59:30.740372 certsync-0.1.2/LICENSE
--rw-r--r--   0        0        0     6623 2023-04-15 14:59:30.740372 certsync-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-15 14:59:30.740372 certsync-0.1.2/certsync/__init__.py
--rw-r--r--   0        0        0    20331 2023-04-15 14:59:30.740372 certsync-0.1.2/certsync/entry.py
--rw-r--r--   0        0        0      790 2023-04-15 14:59:30.740372 certsync-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7568 1970-01-01 00:00:00.000000 certsync-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-12 07:56:17.995952 certsync-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6623 2023-04-12 07:56:17.995952 certsync-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 07:56:17.995952 certsync-0.1.3/certsync/__init__.py
+-rw-r--r--   0        0        0    20420 2023-07-04 09:42:59.779015 certsync-0.1.3/certsync/entry.py
+-rw-r--r--   0        0        0      790 2023-07-04 09:43:15.879015 certsync-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7520 1970-01-01 00:00:00.000000 certsync-0.1.3/PKG-INFO
```

### Comparing `certsync-0.1.2/LICENSE` & `certsync-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `certsync-0.1.2/README.md` & `certsync-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `certsync-0.1.2/certsync/entry.py` & `certsync-0.1.3/certsync/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,16 @@
             dc_ip = options.dc_ip,
             dns_tcp = options.dns_tcp,
             do_kerberos = options.k,
             hashes = options.hashes,
             no_pass = options.no_pass,
             ns = options.ns,
             aes = options.aesKey,
-            target_ip = options.dc_ip)
+            target_ip = options.dc_ip,
+            remote_name = options.kdcHost)
 
         self.ca_ip = options.ca_ip
         self.user_search_filter = options.ldap_filter
         self.scheme = options.scheme
         self.timeout = options.timeout
         self.jitter = options.jitter
         self.randomize = options.randomize
@@ -207,15 +208,16 @@
                 domain = self.target.domain,
                 username = self.target.username,
                 password = self.target.password,
                 dc_ip = self.target.dc_ip,
                 do_kerberos = self.target.do_kerberos,
                 hashes = self.options.hashes,
                 aes = self.target.aes,
-                remote_name = self.ca_ip_address)
+                remote_name = self.ca_dns_name,
+                no_pass = self.options.no_pass)
 
             ca_module = CA(target=ca_target, ca=self.ca_name)
             self.backup_ca_pki(ca_module)
         else:
             logging.info("Loading CA certificate and private key from %s" % self.options.ca_pfx)
             self.ca_key, self.ca_cert = load_pfx(self.ca_pfx)
```

### Comparing `certsync-0.1.2/pyproject.toml` & `certsync-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "certsync"
-version = "0.1.2"
+version = "0.1.3"
 description = "Dump NTDS with golden certificates and UnPAC the hash"
 readme = "README.md"
 homepage = "https://github.com/zblurx/certsync"
 repository = "https://github.com/zblurx/certsync"
 keywords = ["ntds", "certificate", "hashes"]
 authors = ["zblurx <seigneuret.thomas@protonmail.com>"]
 license = "MIT"
```

### Comparing `certsync-0.1.2/PKG-INFO` & `certsync-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certsync
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dump NTDS with golden certificates and UnPAC the hash
 Home-page: https://github.com/zblurx/certsync
 License: MIT
 Keywords: ntds,certificate,hashes
 Author: zblurx
 Author-email: seigneuret.thomas@protonmail.com
 Requires-Python: >=3.7,<4.0
@@ -12,15 +12,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Requires-Dist: certipy-ad (>=4.4.0,<5.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Project-URL: Repository, https://github.com/zblurx/certsync
 Description-Content-Type: text/markdown
 
 # certsync
```

