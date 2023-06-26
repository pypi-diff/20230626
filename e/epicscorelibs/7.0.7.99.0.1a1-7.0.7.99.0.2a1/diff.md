# Comparing `tmp/epicscorelibs-7.0.7.99.0.1a1.tar.gz` & `tmp/epicscorelibs-7.0.7.99.0.2a1-cp39-cp39-manylinux2010_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/epicscorelibs-7.0.7.99.0.1a1.tar", last modified: Tue May 30 23:19:39 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

