# Comparing `tmp/sbpack-2022.3.16.tar.gz` & `tmp/sbpack-2023.6.20rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sbpack-2022.3.16.tar", last modified: Wed Mar 16 14:18:31 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

