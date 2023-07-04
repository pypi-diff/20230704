# Comparing `tmp/pypiqe-1.0.tar.gz` & `tmp/pypiqe-1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypiqe-1.0.tar", last modified: Tue Jul  4 19:03:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

