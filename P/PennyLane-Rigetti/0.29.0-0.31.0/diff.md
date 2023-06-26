# Comparing `tmp/PennyLane-Rigetti-0.29.0.tar.gz` & `tmp/PennyLane_Rigetti-0.31.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PennyLane-Rigetti-0.29.0.tar", last modified: Tue Feb 28 22:20:01 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

