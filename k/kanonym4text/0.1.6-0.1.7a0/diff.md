# Comparing `tmp/kanonym4text-0.1.6.tar.gz` & `tmp/kanonym4text-0.1.7a0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanonym4text-0.1.6.tar", last modified: Sat Jul  1 20:53:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

