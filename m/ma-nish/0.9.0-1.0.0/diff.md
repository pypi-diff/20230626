# Comparing `tmp/ma-nish-0.9.0.tar.gz` & `tmp/ma_nish-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ma-nish-0.9.0.tar", last modified: Thu Apr 20 08:33:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

