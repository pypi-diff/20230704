# Comparing `tmp/lakeapi2sql-0.3.1.tar.gz` & `tmp/lakeapi2sql-0.3.2.tar.gz`

## Comparing `lakeapi2sql-0.3.1.tar` & `lakeapi2sql-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 lakeapi2sql-0.3.1/Cargo.toml
--rw-r--r--   0     1001      123      118 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/.editorconfig
--rw-r--r--   0     1001      123     2804 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     3086 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/.gitignore
--rw-r--r--   0     1001      123     1081 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/LICENSE
--rw-r--r--   0     1001      123     1066 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/README.md
--rw-r--r--   0     1001      123        0 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/lakeapi2sql/__init__.py
--rw-r--r--   0     1001      123     2266 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/lakeapi2sql/bulk_insert.py
--rw-r--r--   0     1001      123        0 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/py.typed
--rw-r--r--   0     1001      123      656 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/pyproject.toml
--rw-r--r--   0     1001      123    12800 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/src/arrow_convert.rs
--rw-r--r--   0     1001      123     2504 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/src/bulk_insert.rs
--rw-r--r--   0     1001      123     1568 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/src/connect.rs
--rw-r--r--   0     1001      123     2757 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/test/__init__.py
--rw-r--r--   0     1001      123     1977 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/test/test_insert.py
--rw-r--r--   0     1001      123    57698 2023-07-03 13:29:32.000000 lakeapi2sql-0.3.1/Cargo.lock
--rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 lakeapi2sql-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 lakeapi2sql-0.3.2/Cargo.toml
+-rw-r--r--   0     1001      123      118 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/.editorconfig
+-rw-r--r--   0     1001      123     2804 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     3086 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/.gitignore
+-rw-r--r--   0     1001      123     1081 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/LICENSE
+-rw-r--r--   0     1001      123     1066 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/README.md
+-rw-r--r--   0     1001      123        0 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/lakeapi2sql/__init__.py
+-rw-r--r--   0     1001      123     2266 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/lakeapi2sql/bulk_insert.py
+-rw-r--r--   0     1001      123        0 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/py.typed
+-rw-r--r--   0     1001      123      656 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/pyproject.toml
+-rw-r--r--   0     1001      123    13593 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/src/arrow_convert.rs
+-rw-r--r--   0     1001      123     3285 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/src/bulk_insert.rs
+-rw-r--r--   0     1001      123     1568 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/src/connect.rs
+-rw-r--r--   0     1001      123     2757 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/test/__init__.py
+-rw-r--r--   0     1001      123     1977 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/test/test_insert.py
+-rw-r--r--   0     1001      123    57698 2023-07-04 04:25:08.000000 lakeapi2sql-0.3.2/Cargo.lock
+-rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 lakeapi2sql-0.3.2/PKG-INFO
```

### Comparing `lakeapi2sql-0.3.1/Cargo.toml` & `lakeapi2sql-0.3.2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.1/.github/workflows/CI.yml` & `lakeapi2sql-0.3.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.1/.gitignore` & `lakeapi2sql-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.1/LICENSE` & `lakeapi2sql-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.1/README.md` & `lakeapi2sql-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.1/lakeapi2sql/bulk_insert.py` & `lakeapi2sql-0.3.2/lakeapi2sql/bulk_insert.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.1/pyproject.toml` & `lakeapi2sql-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "lakeapi2sql"
 requires-python = ">=3.10"
-version = "0.3.1"
+version = "0.3.2"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 [project.optional-dependencies]
```

### Comparing `lakeapi2sql-0.3.1/src/arrow_convert.rs` & `lakeapi2sql-0.3.2/src/arrow_convert.rs`

 * *Files 3% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 use arrow::array::Time32SecondArray;
 use arrow::array::TimestampMicrosecondArray;
 use arrow::array::TimestampMillisecondArray;
 use arrow::array::UInt16Array;
 use arrow::array::UInt32Array;
 use arrow::array::UInt64Array;
 use arrow::array::UInt8Array;
+use arrow::datatypes::DataType;
 use arrow::record_batch::RecordBatch;
+use pyo3::exceptions::PyValueError;
 use std::borrow::Cow;
+use std::fmt::Display;
 use std::time::Duration as StdDuration;
 use tiberius::time::time::Date;
 use tiberius::time::time::PrimitiveDateTime;
 use tiberius::time::time::Time;
 use tiberius::ColumnData;
 use tiberius::IntoSql;
 use tiberius::ToSql;
 use tiberius::TokenRow;
 use time::Duration;
 
+
 // These functions loop like a hack, because, well, there are probably a hack
 fn to_datetime(val: Option<PrimitiveDateTime>) -> ColumnData<'static> {
     return match val.to_sql() {
         ColumnData::DateTime2(x) => ColumnData::DateTime2(x),
         _ => panic!("should be mapped"),
     };
 }
@@ -45,22 +49,46 @@
 }
 fn to_time(val: Option<Time>) -> ColumnData<'static> {
     return match val.to_sql() {
         ColumnData::Time(x) => ColumnData::Time(x),
         _ => panic!("should be mapped"),
     };
 }
+#[derive(Debug)]
+pub(crate) struct  NotSupportedError {
+    dtype: DataType
+}
+impl Display for NotSupportedError {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        f.write_fmt(format_args!("Cannot use data type {}", self.dtype))
+    }
+}
+impl  std::error::Error for NotSupportedError{
+    fn source(&self) -> Option<&(dyn std::error::Error + 'static)> {
+        None
+    }
+
+
+    fn description(&self) -> &str {
+        "description() is deprecated; use Display"
+    }
+
+    fn cause(&self) -> Option<&dyn std::error::Error> {
+        self.source()
+    }
+
+}
 
-pub(crate) fn get_token_rows<'a>(batch: &'a RecordBatch) -> Vec<TokenRow<'a>> {
+pub(crate) fn get_token_rows<'a>(batch: &'a RecordBatch) -> Result<Vec<TokenRow<'a>>, Box<dyn std::error::Error + Send + Sync>> {
     let unix_min_date =
-        Date::from_calendar_date(1970, tiberius::time::time::Month::January, 1).unwrap();
-    let unix_min: PrimitiveDateTime = unix_min_date.with_time(Time::from_hms(0, 0, 0).unwrap());
+        Date::from_calendar_date(1970, tiberius::time::time::Month::January, 1)?;
+    let unix_min: PrimitiveDateTime = unix_min_date.with_time(Time::from_hms(0, 0, 0)?);
 
     let rows = batch.num_rows();
-    let mut token_rows: Vec<TokenRow> = vec![TokenRow::new(); rows.try_into().unwrap()];
+    let mut token_rows: Vec<TokenRow> = vec![TokenRow::new(); rows.try_into()?];
     for col in batch.columns() {
         //For docs: col.data_type().to_physical_type()
         match col.data_type() {
             arrow::datatypes::DataType::Boolean => {
                 let ba = col.as_any().downcast_ref::<BooleanArray>().unwrap();
 
                 let mut rowindex = 0;
@@ -308,12 +336,12 @@
                         None => None,
                     };
                     token_rows[rowindex].push(to_time(dt_val));
                     rowindex += 1;
                 }
             }
             
-            _ => todo!(), //other => panic!("Not supported {:?}", other),
+            dt => return Err(Box::new(NotSupportedError { dtype : dt.clone() })), //other => panic!("Not supported {:?}", other),
         }
     }
-    token_rows
+    Ok(token_rows)
 }
```

### Comparing `lakeapi2sql-0.3.1/src/bulk_insert.rs` & `lakeapi2sql-0.3.2/src/bulk_insert.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,49 @@
-use std::sync::Arc;
+use std::{sync::Arc, fmt::Display};
 
 use arrow::{
-    ipc::reader::{StreamReader}, datatypes::Schema, record_batch::RecordBatch,
+    ipc::reader::{StreamReader}, datatypes::Schema, record_batch::RecordBatch, error::ArrowError,
 };
 use futures::stream::TryStreamExt;
 use tiberius::Client;
 use tokio::net::TcpStream;
 use tokio_util::compat::Compat;
 use tokio_util::compat::FuturesAsyncReadCompatExt;
 use tokio_util::io::SyncIoBridge;
 use log::info;
 
 use tokio::sync::mpsc;
 
 use crate::arrow_convert::get_token_rows;
 
+#[derive(Debug)]
+pub(crate) struct  ArrowErrorWrap {
+    error: ArrowError
+}
+impl Display for ArrowErrorWrap {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        f.write_fmt(format_args!("arrow error {}", self.error))
+    }
+}
+impl  std::error::Error for ArrowErrorWrap{
+    fn source(&self) -> Option<&(dyn std::error::Error + 'static)> {
+        None
+    }
+
+
+    fn description(&self) -> &str {
+        "description() is deprecated; use Display"
+    }
+
+    fn cause(&self) -> Option<&dyn std::error::Error> {
+        self.source()
+    }
+
+}
+
 pub async fn bulk_insert<'a>(
     db_client: &'a mut Client<Compat<TcpStream>>,
     table_name: &str,
     url: &str,
     user: &str,
     password: &str,
 ) -> Result<Arc<Schema>, Box<dyn std::error::Error + Send + Sync>> {
@@ -43,15 +68,19 @@
         .map_err(|e| futures::io::Error::new(futures::io::ErrorKind::Other, e))
         .into_async_read()
         .compat();
     let (tx, mut rx) = mpsc::channel::<RecordBatch>(2);
     let syncstr = SyncIoBridge::new(res);
     let worker = tokio::task::spawn_blocking(move || {       
         
-        let mut reader = StreamReader::try_new(syncstr, None).unwrap();
+        let reader = StreamReader::try_new(syncstr, None);
+        if let Err(err) = reader {
+            return  Err(ArrowErrorWrap { error: err});
+        }
+        let mut reader = reader.unwrap();
         let schema = reader.schema();
         loop {
             match reader.next() {
                 Some(x) => match x {
                     Ok(b) => {
                         tx.blocking_send(b).unwrap();
                     }
@@ -62,22 +91,22 @@
         }
         Ok(schema)
     });
 
     while let Some(v) = rx.recv().await {
         let nrows = v.num_rows();
         info!("received {nrows}");
-        let rows = get_token_rows(&v);        
+        let rows = get_token_rows(&v)?;        
         let mut blk: tiberius::BulkLoadRequest<'_, Compat<TcpStream>> =
             db_client.bulk_insert(table_name).await?;
         for row in rows {
             blk.send(row).await?;
         }
         blk.finalize().await?;
         info!("Written {nrows}");
     }
     let schema = worker.await?;
     if let Err(e) = schema {
-        return e;
+        return Err(Box::new(e));
     }
     Ok(schema.unwrap())
 }
```

### Comparing `lakeapi2sql-0.3.1/src/connect.rs` & `lakeapi2sql-0.3.2/src/connect.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.1/src/lib.rs` & `lakeapi2sql-0.3.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.1/test/test_insert.py` & `lakeapi2sql-0.3.2/test/test_insert.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.1/Cargo.lock` & `lakeapi2sql-0.3.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.3.1/PKG-INFO` & `lakeapi2sql-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakeapi2sql
-Version: 0.3.1
+Version: 0.3.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: azure-identity >=1.12.0 ; extra == 'azure'
 Provides-Extra: azure
 License-File: LICENSE
 Requires-Python: >=3.10
```

