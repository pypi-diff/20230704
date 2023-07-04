# Comparing `tmp/pydantic_core-2.0.2.tar.gz` & `tmp/pydantic_core-2.1.2-cp311-cp311-musllinux_1_1_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

