# Comparing `tmp/recurtx-0.0.7.tar.gz` & `tmp/recurtx-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurtx-0.0.7.tar", last modified: Fri Jun 30 15:35:49 2023, max compression
+gzip compressed data, was "recurtx-0.0.8.tar", last modified: Tue Jul  4 13:18:58 2023, max compression
```

## Comparing `recurtx-0.0.7.tar` & `recurtx-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:35:49.950000 recurtx-0.0.7/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-30 14:54:37.000000 recurtx-0.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-30 15:35:49.950000 recurtx-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5703 2023-06-30 14:54:37.000000 recurtx-0.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)      543 2023-06-30 14:54:37.000000 recurtx-0.0.7/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:35:49.940000 recurtx-0.0.7/recurtx/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-30 14:54:37.000000 recurtx-0.0.7/recurtx/__init__.py
--rw-r--r--   0 root         (0) root         (0)      722 2023-06-30 14:54:37.000000 recurtx-0.0.7/recurtx/__main__.py
--rw-r--r--   0 root         (0) root         (0)     3723 2023-06-30 14:54:37.000000 recurtx-0.0.7/recurtx/ll.py
--rw-r--r--   0 root         (0) root         (0)     7134 2023-06-30 15:06:35.000000 recurtx-0.0.7/recurtx/pandas.py
--rw-r--r--   0 root         (0) root         (0)     4960 2023-06-30 14:54:37.000000 recurtx-0.0.7/recurtx/polars.py
--rw-r--r--   0 root         (0) root         (0)     4026 2023-06-30 14:54:38.000000 recurtx-0.0.7/recurtx/recur.py
--rw-r--r--   0 root         (0) root         (0)     3257 2023-06-30 14:54:38.000000 recurtx-0.0.7/recurtx/search.py
--rw-r--r--   0 root         (0) root         (0)     1771 2023-06-30 14:54:38.000000 recurtx-0.0.7/recurtx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:35:49.950000 recurtx-0.0.7/recurtx.egg-info/
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-30 15:35:49.000000 recurtx-0.0.7/recurtx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      411 2023-06-30 15:35:49.000000 recurtx-0.0.7/recurtx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 15:35:49.000000 recurtx-0.0.7/recurtx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      279 2023-06-30 15:35:49.000000 recurtx-0.0.7/recurtx.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 15:35:49.000000 recurtx-0.0.7/recurtx.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-30 15:35:49.000000 recurtx-0.0.7/recurtx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-30 15:35:49.000000 recurtx-0.0.7/recurtx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-30 15:35:49.950000 recurtx-0.0.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1547 2023-06-30 14:54:39.000000 recurtx-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:18:58.720000 recurtx-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-30 15:42:22.000000 recurtx-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      683 2023-07-04 13:18:58.720000 recurtx-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-06-30 15:42:22.000000 recurtx-0.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)      529 2023-07-01 00:45:28.000000 recurtx-0.0.8/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:18:58.720000 recurtx-0.0.8/recurtx/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-30 15:42:22.000000 recurtx-0.0.8/recurtx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-07-01 15:45:17.000000 recurtx-0.0.8/recurtx/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2023-07-04 12:47:23.000000 recurtx-0.0.8/recurtx/ll.py
+-rw-r--r--   0 root         (0) root         (0)     7134 2023-06-30 15:42:22.000000 recurtx-0.0.8/recurtx/pandas.py
+-rw-r--r--   0 root         (0) root         (0)     5003 2023-07-01 15:43:03.000000 recurtx-0.0.8/recurtx/polars.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-07-04 13:12:02.000000 recurtx-0.0.8/recurtx/recur.py
+-rw-r--r--   0 root         (0) root         (0)     3257 2023-06-30 15:42:23.000000 recurtx-0.0.8/recurtx/search.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-07-04 12:47:05.000000 recurtx-0.0.8/recurtx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:18:58.720000 recurtx-0.0.8/recurtx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      683 2023-07-04 13:18:58.000000 recurtx-0.0.8/recurtx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      411 2023-07-04 13:18:58.000000 recurtx-0.0.8/recurtx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 13:18:58.000000 recurtx-0.0.8/recurtx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      279 2023-07-04 13:18:58.000000 recurtx-0.0.8/recurtx.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 13:18:58.000000 recurtx-0.0.8/recurtx.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-04 13:18:58.000000 recurtx-0.0.8/recurtx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-04 13:18:58.000000 recurtx-0.0.8/recurtx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-04 13:18:58.730000 recurtx-0.0.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1547 2023-06-30 15:42:23.000000 recurtx-0.0.8/setup.py
```

### Comparing `recurtx-0.0.7/LICENSE` & `recurtx-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.7/PKG-INFO` & `recurtx-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.7
+Version: 0.0.8
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `recurtx-0.0.7/README.md` & `recurtx-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.7/pyproject.toml` & `recurtx-0.0.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -13,18 +13,17 @@
     "BLE001",
     "C901",
     "COM812",
     "D100",
     "D103",
     "D104",
     "D202",
-    "ERA001",
     "E501",
-    "EXE002",
     "ERA001",
+    "EXE002",
     "FBT001",
     "FBT002",
     "PD901",
     "PGH001",
     "PTH123",
     "PLR0912",
     "PLR0913",
```

### Comparing `recurtx-0.0.7/recurtx/__main__.py` & `recurtx-0.0.8/recurtx/__main__.py`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.7/recurtx/ll.py` & `recurtx-0.0.8/recurtx/ll.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 from collections import Counter
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
-from .utils import upath
+from .utils import to_glob, upath
 
 
 def ll(
     *paths: str,
     depth: int = 1,
     glob: str = "**/*",
     type: Optional[str] = None,
@@ -18,16 +18,15 @@
     info: bool = True,
     extension_most_common: int = 1,
 ) -> None:
     """Compute statistics for the directory recursively."""
 
     paths = paths or (".",)
 
-    if depth:
-        glob = "".join(["*/"] * (depth - 1)) + "*"
+    glob = to_glob(depth) or glob
 
     stat_ls = []
 
     for path in paths:
         _path = Path(upath(path))
 
         if type:
```

### Comparing `recurtx-0.0.7/recurtx/pandas.py` & `recurtx-0.0.8/recurtx/pandas.py`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.7/recurtx/polars.py` & `recurtx-0.0.8/recurtx/polars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from pathlib import Path
 from typing import Any, List, Optional
 
-import polars as pl
-
 from .utils import infer_format, stdout_lines
 
 DATA_TYPES = {
     "csv",
     "ipc",
     "parquet",
     "database",
@@ -16,26 +14,14 @@
     "excel",
     "delta",
 }
 
 TRUE_VALUES = {"", "True", "true", "T", "t", "1"}
 
 
-def activate(
-    df: pl.LazyFrame,
-    fetch: Optional[int] = None,
-    streaming: bool = False,
-) -> pl.DataFrame:
-    return (
-        df.fetch(n_rows=fetch, streaming=streaming)
-        if fetch
-        else df.collect(streaming=streaming)
-    )
-
-
 def polars(
     *paths: str,
     input_format: Optional[str] = None,
     columns: Optional[List[str]] = None,
     excluding_columns: Optional[List[str]] = None,
     filepath_column: Optional[str] = None,
     streaming: Optional[str] = None,  # actually bool
@@ -81,14 +67,27 @@
             output_format, output_path, DATA_TYPES.union({"markdown"}), polars=True
         )
         or "csv"
     )
 
     streaming_flag = streaming in TRUE_VALUES
 
+    import polars as pl
+
+    def activate(
+        df: pl.LazyFrame,
+        fetch: Optional[int] = None,
+        streaming: bool = False,
+    ) -> pl.DataFrame:
+        return (
+            df.fetch(n_rows=fetch, streaming=streaming)
+            if fetch
+            else df.collect(streaming=streaming)
+        )
+
     ls = []
     for path in paths:
         _input_format = infer_format(input_format, path, DATA_TYPES, polars=True)
         if not _input_format:
             continue
 
         _kwargs = kwargs.copy()
```

### Comparing `recurtx-0.0.7/recurtx/recur.py` & `recurtx-0.0.8/recurtx/recur.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import re
 import sys
 from pathlib import Path
 from typing import Any, List, Tuple
 
-from .utils import get_exception_msg, subprocess_run, upath
+from .utils import get_exception_msg, subprocess_run, to_glob, upath
 
 
 def recur(
     path: str,
     *scripts: str,
     **kwargs: Any,
 ) -> Tuple[List[str], List[str], str, bool]:
     glob = kwargs.pop("glob", "**/*")
+    depth = kwargs.pop("depth", None)
+
+    glob = to_glob(depth) or glob
+
     regex = kwargs.pop(
         "regex",
         r"^(?!.*(\.git\/|__pycache__\/|\.ipynb_checkpoints\/|\.pytest_cache\/|\.vscode\/|\.idea\/|\.DS_Store)).*$",
     )
-    type = kwargs.pop("type", "file")
+    type = kwargs.pop("type", None)
     sort_paths = kwargs.pop("sort_paths", "asc")
     replace_str = kwargs.pop("replace_str", "@@")
     show_paths = kwargs.pop("show_paths", False)
     show_scripts = kwargs.pop("show_scripts", False)
 
     rx = re.compile(regex) if regex else None
 
@@ -51,15 +55,17 @@
 
     _path = Path(upath(path))
     assert _path.exists(), str(_path.resolve()) + " does not exist."
 
     if _path.is_file():
         path_ls = [str(_path)]
     else:
-        path_ls = [str(p) for p in _path.glob(glob) if getattr(p, "is_" + type)()]
+        path_ls = [
+            str(p) for p in _path.glob(glob) if (not type) or getattr(p, "is_" + type)()
+        ]
         if rx:
             path_ls = [p for p in path_ls if rx.match(p)]
         if sort_paths:
             assert isinstance(sort_paths, str), sort_paths
             path_ls.sort(reverse=(sort_paths.lower().startswith("desc")))
 
     if show_paths:
```

### Comparing `recurtx-0.0.7/recurtx/search.py` & `recurtx-0.0.8/recurtx/search.py`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.7/recurtx/utils.py` & `recurtx-0.0.8/recurtx/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,7 +62,13 @@
         _format = path.split(".")[-1]
         _format = _format.replace("md", "markdown")
         if polars:
             _format = _format.replace("jsonl", "ndjson")
         if _format in supported_types:
             return _format
     return None
+
+
+def to_glob(depth: Optional[int] = None) -> Optional[str]:
+    if depth:
+        return "".join(["*/"] * (depth - 1)) + "*"
+    return None
```

### Comparing `recurtx-0.0.7/recurtx.egg-info/PKG-INFO` & `recurtx-0.0.8/recurtx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.7
+Version: 0.0.8
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `recurtx-0.0.7/setup.py` & `recurtx-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 long_description = """
 Please see:
 https://github.com/Minyus/recurtx
 """
 
 setup(
     name="recurtx",
-    version="0.0.7",
+    version="0.0.8",
     packages=find_packages(exclude=["tests"]),
     entry_points={"console_scripts": console_scripts},
     install_requires=requires,
     description="CLI to transform text files recursively",
     license="Apache Software License (Apache 2.0)",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

