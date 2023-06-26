# Comparing `tmp/transformer-lite-0.1.0.tar.gz` & `tmp/transformer_lite-0.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformer-lite-0.1.0.tar", last modified: Sat Jun 10 16:46:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

