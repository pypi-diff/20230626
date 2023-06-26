# Comparing `tmp/filedata-0.2.3.tar.gz` & `tmp/filedata-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filedata-0.2.3.tar", last modified: Wed Jun 21 03:25:51 2023, max compression
+gzip compressed data, was "filedata-0.2.4.tar", last modified: Mon Jun 26 00:53:43 2023, max compression
```

## Comparing `filedata-0.2.3.tar` & `filedata-0.2.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 03:25:51.970338 filedata-0.2.3/
--rwxrwxrwx   0 root         (0) root         (0)      107 2023-06-21 00:08:49.000000 filedata-0.2.3/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      490 2023-06-21 03:25:51.970338 filedata-0.2.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       57 2023-06-21 00:08:49.000000 filedata-0.2.3/README.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 03:25:51.439215 filedata-0.2.3/filedata/
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-06-21 03:10:15.000000 filedata-0.2.3/filedata/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      841 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/config.py
--rwxrwxrwx   0 root         (0) root         (0)     3399 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/file.py
--rwxrwxrwx   0 root         (0) root         (0)     2895 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/html.py
--rwxrwxrwx   0 root         (0) root         (0)     6466 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/image.py
--rwxrwxrwx   0 root         (0) root         (0)      801 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/pdf.py
--rwxrwxrwx   0 root         (0) root         (0)     1198 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/retry.py
--rwxrwxrwx   0 root         (0) root         (0)      624 2023-06-21 01:07:06.000000 filedata-0.2.3/filedata/text.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 03:25:51.783080 filedata-0.2.3/filedata/text_algo/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:11:15.000000 filedata-0.2.3/filedata/text_algo/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4274 2023-06-21 03:21:30.000000 filedata-0.2.3/filedata/text_algo/ac.py
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/time.py
--rwxrwxrwx   0 root         (0) root         (0)      466 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/utils.py
--rwxrwxrwx   0 root         (0) root         (0)      252 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/video.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 03:25:51.704922 filedata-0.2.3/filedata.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      490 2023-06-21 03:25:50.000000 filedata-0.2.3/filedata.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      578 2023-06-21 03:25:51.000000 filedata-0.2.3/filedata.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 03:25:50.000000 filedata-0.2.3/filedata.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 01:08:29.000000 filedata-0.2.3/filedata.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)      124 2023-06-21 03:25:50.000000 filedata-0.2.3/filedata.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-06-21 03:25:50.000000 filedata-0.2.3/filedata.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 03:25:51.814346 filedata-0.2.3/requirements/
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-06-21 00:08:49.000000 filedata-0.2.3/requirements/test.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-21 03:25:51.970338 filedata-0.2.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1549 2023-06-21 00:08:49.000000 filedata-0.2.3/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 03:25:51.845596 filedata-0.2.3/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:08:49.000000 filedata-0.2.3/tests/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 03:25:51.939338 filedata-0.2.3/tests/test_text_algo/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:58:58.000000 filedata-0.2.3/tests/test_text_algo/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1292 2023-06-21 03:06:06.000000 filedata-0.2.3/tests/test_text_algo/test_ac.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 00:53:43.913476 filedata-0.2.4/
+-rwxrwxrwx   0 root         (0) root         (0)      107 2023-06-21 00:08:49.000000 filedata-0.2.4/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      490 2023-06-26 00:53:43.911044 filedata-0.2.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       57 2023-06-21 00:08:49.000000 filedata-0.2.4/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 00:53:43.644103 filedata-0.2.4/filedata/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-06-26 00:52:56.000000 filedata-0.2.4/filedata/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      841 2023-06-21 00:08:49.000000 filedata-0.2.4/filedata/config.py
+-rwxrwxrwx   0 root         (0) root         (0)     3406 2023-06-26 00:48:29.000000 filedata-0.2.4/filedata/file.py
+-rwxrwxrwx   0 root         (0) root         (0)     2895 2023-06-21 00:08:49.000000 filedata-0.2.4/filedata/html.py
+-rwxrwxrwx   0 root         (0) root         (0)     6466 2023-06-21 00:08:49.000000 filedata-0.2.4/filedata/image.py
+-rwxrwxrwx   0 root         (0) root         (0)      801 2023-06-21 00:08:49.000000 filedata-0.2.4/filedata/pdf.py
+-rwxrwxrwx   0 root         (0) root         (0)     1198 2023-06-21 00:08:49.000000 filedata-0.2.4/filedata/retry.py
+-rwxrwxrwx   0 root         (0) root         (0)      624 2023-06-21 01:07:06.000000 filedata-0.2.4/filedata/text.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 00:53:43.800816 filedata-0.2.4/filedata/text_algo/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:11:15.000000 filedata-0.2.4/filedata/text_algo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4274 2023-06-21 03:21:30.000000 filedata-0.2.4/filedata/text_algo/ac.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-06-21 00:08:49.000000 filedata-0.2.4/filedata/time.py
+-rwxrwxrwx   0 root         (0) root         (0)      466 2023-06-21 00:08:49.000000 filedata-0.2.4/filedata/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)      252 2023-06-21 00:08:49.000000 filedata-0.2.4/filedata/video.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 00:53:43.753719 filedata-0.2.4/filedata.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      490 2023-06-26 00:53:42.000000 filedata-0.2.4/filedata.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      578 2023-06-26 00:53:43.000000 filedata-0.2.4/filedata.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-26 00:53:42.000000 filedata-0.2.4/filedata.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 01:08:29.000000 filedata-0.2.4/filedata.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)      124 2023-06-26 00:53:42.000000 filedata-0.2.4/filedata.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-06-26 00:53:42.000000 filedata-0.2.4/filedata.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 00:53:43.816652 filedata-0.2.4/requirements/
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-06-21 00:08:49.000000 filedata-0.2.4/requirements/test.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-26 00:53:43.913476 filedata-0.2.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1549 2023-06-21 00:08:49.000000 filedata-0.2.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 00:53:43.837291 filedata-0.2.4/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:08:49.000000 filedata-0.2.4/tests/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 00:53:43.879794 filedata-0.2.4/tests/test_text_algo/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:58:58.000000 filedata-0.2.4/tests/test_text_algo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1292 2023-06-21 03:06:06.000000 filedata-0.2.4/tests/test_text_algo/test_ac.py
```

### Comparing `filedata-0.2.3/filedata/config.py` & `filedata-0.2.4/filedata/config.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.3/filedata/file.py` & `filedata-0.2.4/filedata/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,14 @@
         if _meta.content_type:
             data = ('data', io.BytesIO(source), _meta.content_type)
     if data is None:
         return
 
     payload = MultipartEncoder({'data': data})
     resp = requests.post(
-        f'{Config.PDF_CONVERTER_HOST}/lool/convert-to/pdf',
+        f'http://{Config.PDF_CONVERTER_HOST}/lool/convert-to/pdf',
         data=payload,
         headers={'Content-Type': payload.content_type},
         timeout=timeout,
     )
     resp.raise_for_status()
     return resp.content
```

### Comparing `filedata-0.2.3/filedata/html.py` & `filedata-0.2.4/filedata/html.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.3/filedata/image.py` & `filedata-0.2.4/filedata/image.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.3/filedata/pdf.py` & `filedata-0.2.4/filedata/pdf.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.3/filedata/retry.py` & `filedata-0.2.4/filedata/retry.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.3/filedata/text.py` & `filedata-0.2.4/filedata/text.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.3/filedata/text_algo/ac.py` & `filedata-0.2.4/filedata/text_algo/ac.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.3/filedata.egg-info/SOURCES.txt` & `filedata-0.2.4/filedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `filedata-0.2.3/setup.py` & `filedata-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.3/tests/test_text_algo/test_ac.py` & `filedata-0.2.4/tests/test_text_algo/test_ac.py`

 * *Files identical despite different names*

