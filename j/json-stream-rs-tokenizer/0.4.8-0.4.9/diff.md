# Comparing `tmp/json-stream-rs-tokenizer-0.4.8.tar.gz` & `tmp/json-stream-rs-tokenizer-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-stream-rs-tokenizer-0.4.8.tar", last modified: Wed Oct 12 00:26:37 2022, max compression
+gzip compressed data, was "json-stream-rs-tokenizer-0.4.9.tar", last modified: Wed Oct 12 21:03:16 2022, max compression
```

## Comparing `json-stream-rs-tokenizer-0.4.8.tar` & `json-stream-rs-tokenizer-0.4.9.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 00:26:37.574616 json-stream-rs-tokenizer-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-10-12 00:26:26.000000 json-stream-rs-tokenizer-0.4.8/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-10-12 00:26:26.000000 json-stream-rs-tokenizer-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-12 00:26:26.000000 json-stream-rs-tokenizer-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5172 2022-10-12 00:26:37.574616 json-stream-rs-tokenizer-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4388 2022-10-12 00:26:26.000000 json-stream-rs-tokenizer-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 00:26:37.574616 json-stream-rs-tokenizer-0.4.8/json_stream_rs_tokenizer/
--rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-10-12 00:26:26.000000 json-stream-rs-tokenizer-0.4.8/json_stream_rs_tokenizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 00:26:37.574616 json-stream-rs-tokenizer-0.4.8/json_stream_rs_tokenizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5172 2022-10-12 00:26:37.000000 json-stream-rs-tokenizer-0.4.8/json_stream_rs_tokenizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-12 00:26:37.000000 json-stream-rs-tokenizer-0.4.8/json_stream_rs_tokenizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 00:26:37.000000 json-stream-rs-tokenizer-0.4.8/json_stream_rs_tokenizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 00:26:37.000000 json-stream-rs-tokenizer-0.4.8/json_stream_rs_tokenizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-12 00:26:37.000000 json-stream-rs-tokenizer-0.4.8/json_stream_rs_tokenizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-12 00:26:37.000000 json-stream-rs-tokenizer-0.4.8/json_stream_rs_tokenizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-12 00:26:26.000000 json-stream-rs-tokenizer-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-12 00:26:37.574616 json-stream-rs-tokenizer-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-10-12 00:26:26.000000 json-stream-rs-tokenizer-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 00:26:37.574616 json-stream-rs-tokenizer-0.4.8/src/
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-10-12 00:26:26.000000 json-stream-rs-tokenizer-0.4.8/src/int.rs
--rw-r--r--   0 runner    (1001) docker     (121)    23441 2022-10-12 00:26:26.000000 json-stream-rs-tokenizer-0.4.8/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 21:03:16.891246 json-stream-rs-tokenizer-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      646 2022-10-12 21:03:05.000000 json-stream-rs-tokenizer-0.4.9/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-10-12 21:03:05.000000 json-stream-rs-tokenizer-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-12 21:03:05.000000 json-stream-rs-tokenizer-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5068 2022-10-12 21:03:16.891246 json-stream-rs-tokenizer-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4284 2022-10-12 21:03:05.000000 json-stream-rs-tokenizer-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 21:03:16.887246 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-10-12 21:03:05.000000 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 21:03:16.891246 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-12 21:03:05.000000 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-10-12 21:03:05.000000 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer/benchmark/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2319 2022-10-12 21:03:05.000000 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer/benchmark/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)      669 2022-10-12 21:03:05.000000 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer/benchmark/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4313 2022-10-12 21:03:05.000000 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer/benchmark/random_json_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 21:03:16.887246 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5068 2022-10-12 21:03:16.000000 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2022-10-12 21:03:16.000000 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 21:03:16.000000 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 21:03:16.000000 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-12 21:03:16.000000 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-12 21:03:16.000000 json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-12 21:03:05.000000 json-stream-rs-tokenizer-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-12 21:03:16.891246 json-stream-rs-tokenizer-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-10-12 21:03:05.000000 json-stream-rs-tokenizer-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 21:03:16.891246 json-stream-rs-tokenizer-0.4.9/src/
+-rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-10-12 21:03:05.000000 json-stream-rs-tokenizer-0.4.9/src/int.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    23441 2022-10-12 21:03:05.000000 json-stream-rs-tokenizer-0.4.9/src/lib.rs
```

### Comparing `json-stream-rs-tokenizer-0.4.8/Cargo.toml` & `json-stream-rs-tokenizer-0.4.9/Cargo.toml`

 * *Files identical despite different names*

### Comparing `json-stream-rs-tokenizer-0.4.8/LICENSE` & `json-stream-rs-tokenizer-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `json-stream-rs-tokenizer-0.4.8/PKG-INFO` & `json-stream-rs-tokenizer-0.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-stream-rs-tokenizer
-Version: 0.4.8
+Version: 0.4.9
 Summary: A faster tokenizer for the json-stream Python library
 Project-URL: Repository, https://github.com/smheidrich/py-json-stream-rs-tokenizer
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -85,23 +85,22 @@
 d = load(StringIO('{ "a": [1,2,3,4], "b": [5,6,7] }'))
 
 # ...
 ```
 
 ## Limitations
 
-- Arbitrary-size integers are not currently supported for PyPy nor when the
-  extension is built against Python's limited C API (`Py_LIMITED_API`). This is
-  due to a limitation of PyO3's
-  [`num-bigint` extension](https://pyo3.rs/main/doc/pyo3/num_bigint/).
-  However, [PyO3 PR #2626](https://github.com/PyO3/pyo3/pull/2626), which lifts
-  the restriction for PyPy, has been merged into PyO3 main and is expected to
-  make it into a release sooner or later.
-  To find out whether a given installation supports arbitrary-size integers,
-  the `json_stream_rs_tokenizer.supports_bigint()` can be called.
+- For PyPy, the speedup is only 1.0-1.5x (much lower than that for CPython).
+  This has yet to be
+  [investigated](https://github.com/smheidrich/py-json-stream-rs-tokenizer/issues/33).
+- In builds that don't support PyO3's
+  [`num-bigint` extension](https://pyo3.rs/main/doc/pyo3/num_bigint/)
+  (currently only PyPy builds and manual ones against Python's limited C API
+  (`Py_LIMITED_API`)), conversion of large integers is performed in Python
+  rather than in Rust, at a very small runtime cost.
 
 ## Benchmarks
 
 The package comes with a script for rudimentary benchmarks on randomly
 generated JSON data. To run it, you'll need to install the optional `benchmark`
 dependencies and a version of `json-stream` with
 [this patch](https://github.com/daggaz/json-stream/pull/17) applied:
```

### Comparing `json-stream-rs-tokenizer-0.4.8/README.md` & `json-stream-rs-tokenizer-0.4.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -66,23 +66,22 @@
 d = load(StringIO('{ "a": [1,2,3,4], "b": [5,6,7] }'))
 
 # ...
 ```
 
 ## Limitations
 
-- Arbitrary-size integers are not currently supported for PyPy nor when the
-  extension is built against Python's limited C API (`Py_LIMITED_API`). This is
-  due to a limitation of PyO3's
-  [`num-bigint` extension](https://pyo3.rs/main/doc/pyo3/num_bigint/).
-  However, [PyO3 PR #2626](https://github.com/PyO3/pyo3/pull/2626), which lifts
-  the restriction for PyPy, has been merged into PyO3 main and is expected to
-  make it into a release sooner or later.
-  To find out whether a given installation supports arbitrary-size integers,
-  the `json_stream_rs_tokenizer.supports_bigint()` can be called.
+- For PyPy, the speedup is only 1.0-1.5x (much lower than that for CPython).
+  This has yet to be
+  [investigated](https://github.com/smheidrich/py-json-stream-rs-tokenizer/issues/33).
+- In builds that don't support PyO3's
+  [`num-bigint` extension](https://pyo3.rs/main/doc/pyo3/num_bigint/)
+  (currently only PyPy builds and manual ones against Python's limited C API
+  (`Py_LIMITED_API`)), conversion of large integers is performed in Python
+  rather than in Rust, at a very small runtime cost.
 
 ## Benchmarks
 
 The package comes with a script for rudimentary benchmarks on randomly
 generated JSON data. To run it, you'll need to install the optional `benchmark`
 dependencies and a version of `json-stream` with
 [this patch](https://github.com/daggaz/json-stream/pull/17) applied:
```

### Comparing `json-stream-rs-tokenizer-0.4.8/json_stream_rs_tokenizer/__init__.py` & `json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `json-stream-rs-tokenizer-0.4.8/json_stream_rs_tokenizer.egg-info/PKG-INFO` & `json-stream-rs-tokenizer-0.4.9/json_stream_rs_tokenizer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-stream-rs-tokenizer
-Version: 0.4.8
+Version: 0.4.9
 Summary: A faster tokenizer for the json-stream Python library
 Project-URL: Repository, https://github.com/smheidrich/py-json-stream-rs-tokenizer
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -85,23 +85,22 @@
 d = load(StringIO('{ "a": [1,2,3,4], "b": [5,6,7] }'))
 
 # ...
 ```
 
 ## Limitations
 
-- Arbitrary-size integers are not currently supported for PyPy nor when the
-  extension is built against Python's limited C API (`Py_LIMITED_API`). This is
-  due to a limitation of PyO3's
-  [`num-bigint` extension](https://pyo3.rs/main/doc/pyo3/num_bigint/).
-  However, [PyO3 PR #2626](https://github.com/PyO3/pyo3/pull/2626), which lifts
-  the restriction for PyPy, has been merged into PyO3 main and is expected to
-  make it into a release sooner or later.
-  To find out whether a given installation supports arbitrary-size integers,
-  the `json_stream_rs_tokenizer.supports_bigint()` can be called.
+- For PyPy, the speedup is only 1.0-1.5x (much lower than that for CPython).
+  This has yet to be
+  [investigated](https://github.com/smheidrich/py-json-stream-rs-tokenizer/issues/33).
+- In builds that don't support PyO3's
+  [`num-bigint` extension](https://pyo3.rs/main/doc/pyo3/num_bigint/)
+  (currently only PyPy builds and manual ones against Python's limited C API
+  (`Py_LIMITED_API`)), conversion of large integers is performed in Python
+  rather than in Rust, at a very small runtime cost.
 
 ## Benchmarks
 
 The package comes with a script for rudimentary benchmarks on randomly
 generated JSON data. To run it, you'll need to install the optional `benchmark`
 dependencies and a version of `json-stream` with
 [this patch](https://github.com/daggaz/json-stream/pull/17) applied:
```

### Comparing `json-stream-rs-tokenizer-0.4.8/setup.py` & `json-stream-rs-tokenizer-0.4.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from setuptools_rust import Binding, RustExtension
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="json-stream-rs-tokenizer",
-    version="0.4.8",
+    version="0.4.9",
     rust_extensions=[
         RustExtension(
             "json_stream_rs_tokenizer.json_stream_rs_tokenizer",
             binding=Binding.PyO3,
             optional=True,
             py_limited_api=False,  # required for num_bigint compat.
             debug=False,  # pointless even in develop mode
         )
     ],
-    packages=["json_stream_rs_tokenizer"],
+    packages=["json_stream_rs_tokenizer", "json_stream_rs_tokenizer.benchmark"],
     zip_safe=False,
     description="A faster tokenizer for the json-stream Python library",
     readme="README.md",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license_files=["LICENSE"],
     project_urls={
```

### Comparing `json-stream-rs-tokenizer-0.4.8/src/int.rs` & `json-stream-rs-tokenizer-0.4.9/src/int.rs`

 * *Files identical despite different names*

### Comparing `json-stream-rs-tokenizer-0.4.8/src/lib.rs` & `json-stream-rs-tokenizer-0.4.9/src/lib.rs`

 * *Files identical despite different names*

