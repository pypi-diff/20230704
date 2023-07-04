# Comparing `tmp/osgpy-0.1.3.tar.gz` & `tmp/osgpy-0.1.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osgpy-0.1.3.tar", last modified: Mon Mar  6 06:47:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

