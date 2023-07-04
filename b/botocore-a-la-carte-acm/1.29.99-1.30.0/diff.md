# Comparing `tmp/botocore-a-la-carte-acm-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-acm-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-acm-1.29.99.tar", last modified: Sat Mar 25 01:22:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

