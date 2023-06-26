# Comparing `tmp/blitzml-0.8.0.tar.gz` & `tmp/blitzml-0.9.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blitzml-0.8.0.tar", last modified: Fri Jan 27 12:43:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

