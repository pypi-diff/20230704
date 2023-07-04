# Comparing `tmp/lakeapi2sql-0.3.0.tar.gz` & `tmp/lakeapi2sql-0.3.1.tar.gz`

## Comparing `lakeapi2sql-0.3.0.tar` & `lakeapi2sql-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 lakeapi2sql-0.3.0/Cargo.toml
--rw-r--r--   0     1001      123      118 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/.editorconfig
--rw-r--r--   0     1001      123     2804 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     3086 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/.gitignore
--rw-r--r--   0     1001      123     1081 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/LICENSE
--rw-r--r--   0     1001      123     1066 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/README.md
--rw-r--r--   0     1001      123        0 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/lakeapi2sql/__init__.py
--rw-r--r--   0     1001      123     2184 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/lakeapi2sql/bulk_insert.py
--rw-r--r--   0     1001      123        0 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/py.typed
--rw-r--r--   0     1001      123      656 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/pyproject.toml
--rw-r--r--   0     1001      123    12800 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/src/arrow_convert.rs
--rw-r--r--   0     1001      123     2504 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/src/bulk_insert.rs
--rw-r--r--   0     1001      123     1568 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/src/connect.rs
--rw-r--r--   0     1001      123     2757 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/test/__init__.py
--rw-r--r--   0     1001      123     1977 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/test/test_insert.py
--rw-r--r--   0     1001      123    57698 2023-07-03 11:49:20.000000 lakeapi2sql-0.3.0/Cargo.lock
--rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 lakeapi2sql-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 lakeapi2sql-0.3.1/Cargo.toml
+-rw-r--r--   0     1001      123      118 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/.editorconfig
+-rw-r--r--   0     1001      123     2804 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     3086 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/.gitignore
+-rw-r--r--   0     1001      123     1081 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/LICENSE
+-rw-r--r--   0     1001      123     1066 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/README.md
+-rw-r--r--   0     1001      123        0 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/lakeapi2sql/__init__.py
+-rw-r--r--   0     1001      123     2266 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/lakeapi2sql/bulk_insert.py
+-rw-r--r--   0     1001      123        0 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/py.typed
+-rw-r--r--   0     1001      123      656 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/pyproject.toml
+-rw-r--r--   0     1001      123    12800 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/src/arrow_convert.rs
+-rw-r--r--   0     1001      123     2504 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/src/bulk_insert.rs
+-rw-r--r--   0     1001      123     1568 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/src/connect.rs
+-rw-r--r--   0     1001      123     2757 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/test/__init__.py
+-rw-r--r--   0     1001      123     1977 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/test/test_insert.py
+-rw-r--r--   0     1001      123    57698 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/Cargo.lock
+-rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 lakeapi2sql-0.3.1/PKG-INFO
```

### Comparing `lakeapi2sql-0.3.0/Cargo.toml` & `lakeapi2sql-0.3.1/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.0/.github/workflows/CI.yml` & `lakeapi2sql-0.3.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.0/.gitignore` & `lakeapi2sql-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.0/LICENSE` & `lakeapi2sql-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.0/README.md` & `lakeapi2sql-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.0/lakeapi2sql/bulk_insert.py` & `lakeapi2sql-0.3.1/lakeapi2sql/bulk_insert.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,27 +12,28 @@
 
 async def insert_http_arrow_stream_to_sql(connection_string: str, table_name: str, url: str, basic_auth: tuple[str, str],  aad_token: str|None = None) -> BulkInfo:
     if "authentication" in connection_string.lower():
         parts = [ (kv[0:kv.index("=")], kv[kv.index("=")+1:]) for kv in  connection_string.split(';')]
         auth_part = next((p for p in parts if p[0].casefold()=="Authentication".casefold()))
         parts.remove(auth_part)
         credential= None
-        if auth_part[1] in ["ActiveDirectoryDefault"]:
+        lautchmechano = auth_part[1].lower()
+        if lautchmechano in ["ActiveDirectoryDefault".lower()]:
             from azure.identity.aio import DefaultAzureCredential
             credential = DefaultAzureCredential()
-        elif auth_part[1] in ["ActiveDirectoryMSI", "ActiveDirectoryManagedIdentity"]:
+        elif lautchmechano in ["ActiveDirectoryMSI".lower(), "ActiveDirectoryManagedIdentity".lower()]:
             from azure.identity.aio import ManagedIdentityCredential  
             client_part = next((p for p in parts if p[0].lower() in ["user", "msiclientid"]), None)
             if client_part:
                 parts.remove(client_part)
             credential = ManagedIdentityCredential(client_id=client_part[1] if client_part else None)
-        elif auth_part[1] == "ActiveDirectoryInteractive":
+        elif lautchmechano == "ActiveDirectoryInteractive".lower():
             from azure.identity import InteractiveBrowserCredential 
             credential = InteractiveBrowserCredential()
-        elif auth_part[1] == "SqlPassword":# that's kind of an no-op
+        elif lautchmechano == "SqlPassword":# that's kind of an no-op
             connection_string = ";".join((p[0] + "=" + p[1] for p in parts))
         if credential is not None:
             from azure.core.credentials import AccessToken
             res = credential.get_token("https://database.windows.net/.default")
             token : AccessToken= await res if inspect.isawaitable(res) else res # type: ignore
             aad_token = token.token
             connection_string = ";".join((p[0] + "=" + p[1] for p in parts))
```

### Comparing `lakeapi2sql-0.3.0/pyproject.toml` & `lakeapi2sql-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "lakeapi2sql"
 requires-python = ">=3.10"
-version = "0.3.0"
+version = "0.3.1"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 [project.optional-dependencies]
```

### Comparing `lakeapi2sql-0.3.0/src/arrow_convert.rs` & `lakeapi2sql-0.3.1/src/arrow_convert.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.0/src/bulk_insert.rs` & `lakeapi2sql-0.3.1/src/bulk_insert.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.0/src/connect.rs` & `lakeapi2sql-0.3.1/src/connect.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.0/src/lib.rs` & `lakeapi2sql-0.3.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.0/test/test_insert.py` & `lakeapi2sql-0.3.1/test/test_insert.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.0/Cargo.lock` & `lakeapi2sql-0.3.1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.0/PKG-INFO` & `lakeapi2sql-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakeapi2sql
-Version: 0.3.0
+Version: 0.3.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: azure-identity >=1.12.0 ; extra == 'azure'
 Provides-Extra: azure
 License-File: LICENSE
 Requires-Python: >=3.10
```

