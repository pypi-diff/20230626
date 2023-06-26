# Comparing `tmp/python-bash-utils-0.3.2.tar.gz` & `tmp/python_bash_utils-0.4.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-bash-utils-0.3.2.tar", last modified: Thu Apr 26 18:32:35 2018, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

