# Comparing `tmp/s3local-0.4.0.tar.gz` & `tmp/s3local-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3local-0.4.0.tar", last modified: Wed May 31 12:35:36 2023, max compression
+gzip compressed data, was "s3local-0.4.1.tar", last modified: Mon Jun 26 07:52:49 2023, max compression
```

## Comparing `s3local-0.4.0.tar` & `s3local-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-05-31 12:35:36.263472 s3local-0.4.0/
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     4195 2023-05-31 12:35:36.263318 s3local-0.4.0/PKG-INFO
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     3628 2023-05-31 01:44:34.000000 s3local-0.4.0/README.md
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)       38 2023-05-31 12:35:36.263522 s3local-0.4.0/setup.cfg
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     1183 2023-05-31 12:30:10.000000 s3local-0.4.0/setup.py
-drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-05-31 12:35:36.258824 s3local-0.4.0/src/
-drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-05-31 12:35:36.261051 s3local-0.4.0/src/s3local/
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      199 2023-05-29 11:53:08.000000 s3local-0.4.0/src/s3local/__init__.py
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     2913 2023-05-29 11:53:08.000000 s3local-0.4.0/src/s3local/commands.py
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      153 2023-05-29 11:53:08.000000 s3local-0.4.0/src/s3local/constants.py
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     2010 2023-05-31 12:16:10.000000 s3local-0.4.0/src/s3local/core.py
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     2140 2023-05-29 11:53:08.000000 s3local-0.4.0/src/s3local/downloader.py
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      301 2023-05-29 11:53:08.000000 s3local-0.4.0/src/s3local/logger.py
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     2108 2023-05-31 12:16:10.000000 s3local-0.4.0/src/s3local/uploader.py
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      885 2023-05-29 11:53:08.000000 s3local-0.4.0/src/s3local/util.py
-drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-05-31 12:35:36.262478 s3local-0.4.0/src/s3local.egg-info/
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     4195 2023-05-31 12:35:36.000000 s3local-0.4.0/src/s3local.egg-info/PKG-INFO
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      491 2023-05-31 12:35:36.000000 s3local-0.4.0/src/s3local.egg-info/SOURCES.txt
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)        1 2023-05-31 12:35:36.000000 s3local-0.4.0/src/s3local.egg-info/dependency_links.txt
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)       50 2023-05-31 12:35:36.000000 s3local-0.4.0/src/s3local.egg-info/entry_points.txt
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)        1 2023-05-30 12:42:58.000000 s3local-0.4.0/src/s3local.egg-info/not-zip-safe
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)       29 2023-05-31 12:35:36.000000 s3local-0.4.0/src/s3local.egg-info/requires.txt
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)        8 2023-05-31 12:35:36.000000 s3local-0.4.0/src/s3local.egg-info/top_level.txt
-drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-05-31 12:35:36.262977 s3local-0.4.0/tests/
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      686 2023-05-29 11:53:08.000000 s3local-0.4.0/tests/test_commands.py
--rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      402 2023-05-29 11:53:08.000000 s3local-0.4.0/tests/test_util.py
+drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-06-26 07:52:49.676890 s3local-0.4.1/
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     4195 2023-06-26 07:52:49.676728 s3local-0.4.1/PKG-INFO
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     3628 2023-05-31 01:44:34.000000 s3local-0.4.1/README.md
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)       38 2023-06-26 07:52:49.676945 s3local-0.4.1/setup.cfg
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     1183 2023-06-26 07:51:08.000000 s3local-0.4.1/setup.py
+drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-06-26 07:52:49.673562 s3local-0.4.1/src/
+drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-06-26 07:52:49.675126 s3local-0.4.1/src/s3local/
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      199 2023-05-29 11:53:08.000000 s3local-0.4.1/src/s3local/__init__.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     2913 2023-05-29 11:53:08.000000 s3local-0.4.1/src/s3local/commands.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      153 2023-05-29 11:53:08.000000 s3local-0.4.1/src/s3local/constants.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     1507 2023-06-26 07:50:09.000000 s3local-0.4.1/src/s3local/core.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     2589 2023-06-26 07:50:09.000000 s3local-0.4.1/src/s3local/downloader.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      301 2023-05-29 11:53:08.000000 s3local-0.4.1/src/s3local/logger.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     2585 2023-06-26 07:50:09.000000 s3local-0.4.1/src/s3local/uploader.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      885 2023-05-29 11:53:08.000000 s3local-0.4.1/src/s3local/util.py
+drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-06-26 07:52:49.676214 s3local-0.4.1/src/s3local.egg-info/
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     4195 2023-06-26 07:52:49.000000 s3local-0.4.1/src/s3local.egg-info/PKG-INFO
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      491 2023-06-26 07:52:49.000000 s3local-0.4.1/src/s3local.egg-info/SOURCES.txt
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)        1 2023-06-26 07:52:49.000000 s3local-0.4.1/src/s3local.egg-info/dependency_links.txt
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)       50 2023-06-26 07:52:49.000000 s3local-0.4.1/src/s3local.egg-info/entry_points.txt
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)        1 2023-05-30 12:42:58.000000 s3local-0.4.1/src/s3local.egg-info/not-zip-safe
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)       29 2023-06-26 07:52:49.000000 s3local-0.4.1/src/s3local.egg-info/requires.txt
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)        8 2023-06-26 07:52:49.000000 s3local-0.4.1/src/s3local.egg-info/top_level.txt
+drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-06-26 07:52:49.676507 s3local-0.4.1/tests/
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      686 2023-06-14 12:41:50.000000 s3local-0.4.1/tests/test_commands.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      402 2023-05-29 11:53:08.000000 s3local-0.4.1/tests/test_util.py
```

### Comparing `s3local-0.4.0/PKG-INFO` & `s3local-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3local
-Version: 0.4.0
+Version: 0.4.1
 Summary: Command Line utility for s3 local caching.
 Home-page: https://github.com/toyama0919/s3local
 Author: Hiroshi Toyama
 Author-email: toyama0919@gmail.com
 License: MIT
 Keywords: s3local tool aws s3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `s3local-0.4.0/README.md` & `s3local-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `s3local-0.4.0/setup.py` & `s3local-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 install_requires = ["boto3", "click>=7.0"]
 extras_require = {"test": ["tox"]}
 
 setup(
     name="s3local",
-    version="0.4.0",
+    version="0.4.1",
     description="Command Line utility for s3 local caching.",
     long_description=open(os.path.join(here, "README.md")).read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `s3local-0.4.0/src/s3local/commands.py` & `s3local-0.4.1/src/s3local/commands.py`

 * *Files identical despite different names*

### Comparing `s3local-0.4.0/src/s3local/core.py` & `s3local-0.4.1/src/s3local/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,19 +43,7 @@
                 Prefix=self.prefix,
             ).delete()
         else:
             os.remove(self.local_path)
             self.bucket.delete_object(
                 Key=self.prefix,
             )
-
-    def should_skip(self, objects_collection, key: str, source_path: str) -> bool:
-        objects = [o for o in objects_collection if o.key == key]
-        if len(objects) > 0:
-            size = objects[0].size
-            print(objects[0].__class__)
-            if os.path.getsize(source_path) == size:
-                self.logger.info(
-                    f"skip upload. match filesize ({size} byte) s3://{self.bucket_name}/{key}"
-                )
-                return True
-        return False
```

### Comparing `s3local-0.4.0/src/s3local/downloader.py` & `s3local-0.4.1/src/s3local/downloader.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,49 +4,58 @@
 
 
 class Downloader(Core):
     def download_file(
         self,
         key: str,
         dryrun: bool = False,
-        skip_exist: bool = True,
         dst_path: str = None,
     ):
-        dst_path = dst_path or f"{self.root}/{key}"
+        # make dir
         dst_dir_path = os.path.dirname(dst_path)
-        s3_url = f"s3://{self.bucket_name}/{key}"
         os.makedirs(dst_dir_path, exist_ok=True)
-        if os.path.exists(dst_path) and skip_exist:
-            self.logger.info(f"skip already exists in local: {s3_url} > {dst_path}")
-        else:
-            self.logger.info(f"Copying: {s3_url} > {dst_path}")
-            if not dryrun:
-                self.bucket.download_file(key, dst_path)
+
+        s3_url = f"s3://{self.bucket_name}/{key}"
+        self.logger.info(f"Copying: {s3_url} > {dst_path}")
+        if not dryrun:
+            self.bucket.download_file(key, dst_path)
         self.download_paths.append(dst_path)
 
     def download(
         self, dryrun: bool = False, skip_exist: bool = True, dst_path: str = None
     ):
         if self.recursive:
             objects = self.bucket.objects.filter(
                 Prefix=self.prefix,
             )
-            for key in [o.key for o in objects]:
-                self.download_file(
-                    key,
-                    dryrun,
-                    skip_exist=skip_exist,
-                    dst_path=(
-                        f"{dst_path}/{os.path.basename(key)}" if dst_path else None
-                    ),
-                )
+            for o in objects:
+                local_dst_path = (
+                    f"{dst_path}/{os.path.basename(o.key)}" if dst_path else None
+                ) or f"{self.root}/{o.key}"
+                if not (skip_exist and self.should_skip(o.key, local_dst_path)):
+                    self.download_file(
+                        o.key,
+                        dryrun,
+                        dst_path=local_dst_path,
+                    )
         else:
-            self.download_file(
-                self.prefix, dryrun, skip_exist=skip_exist, dst_path=dst_path
-            )
+            local_dst_path = dst_path or f"{self.root}/{self.prefix}"
+            if not (skip_exist and self.should_skip(self.prefix, local_dst_path)):
+                self.download_file(self.prefix, dryrun, dst_path=local_dst_path)
+
+    def should_skip(self, key: str, source_path: str) -> bool:
+        size = self.bucket.Object(key).content_length
+
+        if os.path.exists(source_path) and os.path.isfile(source_path):
+            if os.path.getsize(source_path) == size:
+                self.logger.info(
+                    f"skip download. match filesize ({size} byte) s3://{self.bucket_name}/{key} > {source_path}"
+                )
+                return True
+        return False
 
     def list_download_path(self):
         self.download()
         return self.download_paths
 
     def list_local_path(self, download: bool = False):
         if download:
```

### Comparing `s3local-0.4.0/src/s3local/uploader.py` & `s3local-0.4.1/src/s3local/uploader.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,7 +55,18 @@
         shutil.copyfile(local_path, dst_path)
 
         # copy s3
         self.logger.info(
             f"Copying to s3: {local_path} => s3://{self.bucket_name}/{key}"
         )
         self.bucket.upload_file(local_path, key, ExtraArgs=extra_args)
+
+    def should_skip(self, objects_collection, key: str, source_path: str) -> bool:
+        objects = [o for o in objects_collection if o.key == key]
+        if len(objects) > 0:
+            size = objects[0].size
+            if os.path.getsize(source_path) == size:
+                self.logger.info(
+                    f"skip copy. match filesize ({size} byte) {source_path} > s3://{self.bucket_name}/{key}"
+                )
+                return True
+        return False
```

### Comparing `s3local-0.4.0/src/s3local/util.py` & `s3local-0.4.1/src/s3local/util.py`

 * *Files identical despite different names*

### Comparing `s3local-0.4.0/src/s3local.egg-info/PKG-INFO` & `s3local-0.4.1/src/s3local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3local
-Version: 0.4.0
+Version: 0.4.1
 Summary: Command Line utility for s3 local caching.
 Home-page: https://github.com/toyama0919/s3local
 Author: Hiroshi Toyama
 Author-email: toyama0919@gmail.com
 License: MIT
 Keywords: s3local tool aws s3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `s3local-0.4.0/tests/test_commands.py` & `s3local-0.4.1/tests/test_commands.py`

 * *Files identical despite different names*

