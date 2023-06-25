# Comparing `tmp/mypy-1.4.0.tar.gz` & `tmp/mypy-1.4.1-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-1.4.0.tar", last modified: Wed Jun 14 22:02:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

