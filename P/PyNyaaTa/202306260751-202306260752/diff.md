# Comparing `tmp/PyNyaaTa-202306260751.tar.gz` & `tmp/PyNyaaTa-202306260752-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNyaaTa-202306260751.tar", last modified: Mon Jun 26 07:51:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

