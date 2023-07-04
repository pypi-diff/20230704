# Comparing `tmp/SELDOMpy-0.6.9.tar.gz` & `tmp/SELDOMpy-0.7.0-py3.8-win-amd64.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.6.9.tar", last modified: Mon Jul  3 17:25:53 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

