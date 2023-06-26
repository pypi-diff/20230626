# Comparing `tmp/pvxslibs-1.2.1a1.tar.gz` & `tmp/pvxslibs-1.2.2a1-cp310-cp310-manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvxslibs-1.2.1a1.tar", last modified: Wed May 31 05:09:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

