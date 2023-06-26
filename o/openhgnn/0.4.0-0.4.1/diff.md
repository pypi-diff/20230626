# Comparing `tmp/openhgnn-0.4.0.tar.gz` & `tmp/openhgnn-0.4.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhgnn-0.4.0.tar", last modified: Fri Jan 13 08:53:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

