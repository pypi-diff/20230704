# Comparing `tmp/plemmy-0.2.5.tar.gz` & `tmp/plemmy-0.2.6-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plemmy-0.2.5.tar", last modified: Fri Jun 30 20:44:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

