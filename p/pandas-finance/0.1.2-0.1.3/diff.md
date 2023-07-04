# Comparing `tmp/pandas-finance-0.1.2.tar.gz` & `tmp/pandas_finance-0.1.3-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pandas-finance-0.1.2.tar", last modified: Mon Dec 26 02:24:25 2016, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

