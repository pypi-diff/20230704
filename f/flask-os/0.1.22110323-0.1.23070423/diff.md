# Comparing `tmp/flask_os-0.1.22110323.tar.gz` & `tmp/flask_os-0.1.23070423-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\flask_os-0.1.22110323.tar", last modified: Thu Nov  3 15:24:58 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

