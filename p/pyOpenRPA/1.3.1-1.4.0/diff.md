# Comparing `tmp/pyOpenRPA-1.3.1.tar.gz` & `tmp/pyOpenRPA-1.4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyOpenRPA-1.3.1.tar", last modified: Mon Oct 10 18:25:15 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

