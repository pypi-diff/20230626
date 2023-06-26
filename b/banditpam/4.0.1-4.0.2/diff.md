# Comparing `tmp/banditpam-4.0.1.tar.gz` & `tmp/banditpam-4.0.2-cp39-cp39-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banditpam-4.0.1.tar", last modified: Mon Mar 27 04:18:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

