# Comparing `tmp/mflag-1.6.6.tar.gz` & `tmp/mflag-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mflag-1.6.6.tar", last modified: Sat Jun 24 11:02:07 2023, max compression
+gzip compressed data, was "mflag-1.6.7.tar", last modified: Mon Jun 26 13:15:26 2023, max compression
```

## Comparing `mflag-1.6.6.tar` & `mflag-1.6.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.597144 mflag-1.6.6/
--rwxrwxrwx   0 root         (0) root         (0)     1071 2023-06-24 10:44:31.000000 mflag-1.6.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     2209 2023-06-24 11:02:07.597003 mflag-1.6.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2026 2023-06-24 10:44:31.000000 mflag-1.6.6/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.594468 mflag-1.6.6/mflag/
--rwxrwxrwx   0 root         (0) root         (0)      202 2023-06-24 10:49:16.000000 mflag-1.6.6/mflag/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.595604 mflag-1.6.6/mflag/src/
--rwxrwxrwx   0 root         (0) root         (0)     4962 2023-06-24 10:44:31.000000 mflag-1.6.6/mflag/src/flag.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.593740 mflag-1.6.6/mflag/src/rcmng/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.596006 mflag-1.6.6/mflag/src/rcmng/client/
--rwxrwxrwx   0 root         (0) root         (0)     1631 2023-06-24 10:41:50.000000 mflag-1.6.6/mflag/src/rcmng/client/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      433 2023-06-24 09:19:59.000000 mflag-1.6.6/mflag/src/rcmng/client/run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.596393 mflag-1.6.6/mflag/src/rcmng/server/
--rwxrwxrwx   0 root         (0) root         (0)     6832 2023-06-24 10:42:40.000000 mflag-1.6.6/mflag/src/rcmng/server/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      255 2023-06-24 08:55:53.000000 mflag-1.6.6/mflag/src/rcmng/server/run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.596762 mflag-1.6.6/mflag/src/rcmng/submit/
--rwxrwxrwx   0 root         (0) root         (0)      844 2023-06-24 10:18:10.000000 mflag-1.6.6/mflag/src/rcmng/submit/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      444 2023-06-24 10:33:05.000000 mflag-1.6.6/mflag/src/rcmng/submit/run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.595414 mflag-1.6.6/mflag.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     2209 2023-06-24 11:02:07.000000 mflag-1.6.6/mflag.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      401 2023-06-24 11:02:07.000000 mflag-1.6.6/mflag.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-24 11:02:07.000000 mflag-1.6.6/mflag.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       26 2023-06-24 11:02:07.000000 mflag-1.6.6/mflag.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2023-06-24 11:02:07.000000 mflag-1.6.6/mflag.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-24 11:02:07.597189 mflag-1.6.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      483 2023-06-24 11:02:05.000000 mflag-1.6.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.356387 mflag-1.6.7/
+-rwxrwxrwx   0 root         (0) root         (0)     1071 2023-06-24 10:44:31.000000 mflag-1.6.7/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     2209 2023-06-26 13:15:26.356224 mflag-1.6.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2026 2023-06-24 10:44:31.000000 mflag-1.6.7/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.352756 mflag-1.6.7/mflag/
+-rwxrwxrwx   0 root         (0) root         (0)      226 2023-06-26 13:13:23.000000 mflag-1.6.7/mflag/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.354441 mflag-1.6.7/mflag/src/
+-rwxrwxrwx   0 root         (0) root         (0)     4559 2023-06-26 13:11:50.000000 mflag-1.6.7/mflag/src/flag.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.351447 mflag-1.6.7/mflag/src/rcmng/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.354963 mflag-1.6.7/mflag/src/rcmng/client/
+-rwxrwxrwx   0 root         (0) root         (0)     1631 2023-06-24 10:41:50.000000 mflag-1.6.7/mflag/src/rcmng/client/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      433 2023-06-24 09:19:59.000000 mflag-1.6.7/mflag/src/rcmng/client/run.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.355433 mflag-1.6.7/mflag/src/rcmng/server/
+-rwxrwxrwx   0 root         (0) root         (0)     6832 2023-06-24 10:42:40.000000 mflag-1.6.7/mflag/src/rcmng/server/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      255 2023-06-24 08:55:53.000000 mflag-1.6.7/mflag/src/rcmng/server/run.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.355935 mflag-1.6.7/mflag/src/rcmng/submit/
+-rwxrwxrwx   0 root         (0) root         (0)      844 2023-06-24 10:18:10.000000 mflag-1.6.7/mflag/src/rcmng/submit/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      444 2023-06-24 10:33:05.000000 mflag-1.6.7/mflag/src/rcmng/submit/run.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 13:15:26.354189 mflag-1.6.7/mflag.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     2209 2023-06-26 13:15:26.000000 mflag-1.6.7/mflag.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      401 2023-06-26 13:15:26.000000 mflag-1.6.7/mflag.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-26 13:15:26.000000 mflag-1.6.7/mflag.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       26 2023-06-26 13:15:26.000000 mflag-1.6.7/mflag.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2023-06-26 13:15:26.000000 mflag-1.6.7/mflag.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-26 13:15:26.356447 mflag-1.6.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      516 2023-06-26 13:13:56.000000 mflag-1.6.7/setup.py
```

### Comparing `mflag-1.6.6/LICENSE` & `mflag-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mflag-1.6.6/PKG-INFO` & `mflag-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflag
-Version: 1.6.6
+Version: 1.6.7
 Summary: put/remove flags for files and folders
 Author: Moses Dastmard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mflag: powerful Python toolkit for mark/unmark files and directories 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pandas.svg)](https://pypi.org/project/mflag/)
```

### Comparing `mflag-1.6.6/README.md` & `mflag-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `mflag-1.6.6/mflag/src/flag.py` & `mflag-1.6.7/mflag/src/flag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 import os
 import sys
 from os.path import join
-import pandas as pd
 from mpath import get_path_info
 from datetime import datetime
+import json
 flag_extention = '.flg'
 
 class Flag:
     def __init__(self, process_name, hidden=True) -> None:
         self.process_name = process_name
         self.hidden = hidden
         self.get_path_info = get_path_info
@@ -69,61 +69,55 @@
         
         
 class SkipWithBlock(Exception):
     pass
 
 
 class JobManager:
-    def __init__(self, job_file_path, job_id, job_name="", job_description="", process_name=""):
-        self.job_file_path = Path(job_file_path)
-        assert not os.path.isdir(self.job_file_path), f"job_file_path={self.job_file_path} is not a valid file path"
+    def __init__(self, job_dir_path, job_id, job_name="", job_description="", process_name=""):
+        self.job_dir_path = Path(job_dir_path)
         self.job_id = job_id
         self.job_name = job_name
         self.job_description = job_description
         self.process_name = process_name
-        self.job_file_dir = self.job_file_path.parent.absolute()
+        self.job_file_path = os.path.join(self.job_dir_path, self.job_id + ".json")
         
     def __initial_check(self):
-        os.makedirs(self.job_file_dir, exist_ok=True)
-        if not os.path.exists(self.job_file_path):
-            self.__create_empty_job_file()
-    
-    def __create_empty_job_file(self):
-        job_df = pd.DataFrame(columns=['job_id', 'job_name', 'job_description', 'process_name', 'issue_date', 'finish_date'])
-        job_df.set_index('job_id', inplace=True)
-        job_df.to_csv(self.job_file_path)
+        os.makedirs(self.job_dir_path, exist_ok=True)
     
     def __is_job_done(self):
-        job_df = pd.read_csv(self.job_file_path, index_col=0)
-        if self.job_id not in job_df.index:
-            for col, value in {'job_name':self.job_name, 'job_description':self.job_description, 'process_name':self.process_name, 'issue_date':datetime.now(), 'finish_date':None}.items():
-                job_df.loc[self.job_id, col] = value
-            job_df.to_csv(self.job_file_path)
-            return True
-        job_row = job_df.loc[self.job_id]
-        if pd.isna(job_row['finish_date']):
-            return True
+        if not os.path.exists(self.job_file_path):
+            job_dict = {'job_id':self.job_id, 'job_name':self.job_name, 'job_description':self.job_description, 'process_name':self.process_name, 'issue_date':str(datetime.now())}
+            with open(self.job_file_path, 'w') as f:
+                json.dump(job_dict, f)
+            return False
         else:
-            print(f"job_id={self.job_id} is already done, no need to run it again")
+            with open(self.job_file_path, 'r') as f:
+                job_dict = json.load(f)
+                if 'finish_date' in job_dict.keys():
+                    print(f"job_id={self.job_id} is already done, no need to run it again")
+                    return True
             return False
 
     def __enter__(self):
         self.__initial_check()
-        if not self.__is_job_done():
+        if self.__is_job_done():
             sys.settrace(lambda *args, **keys: None)
             frame = sys._getframe(1)
             frame.f_trace = self.trace
 
     def trace(self, frame, event, arg):
         raise SkipWithBlock()
     
     def __finish_job(self):
-        job_df = pd.read_csv(self.job_file_path, index_col=0)
-        job_df.loc[self.job_id, 'finish_date'] = datetime.now()
-        job_df.to_csv(self.job_file_path)
+        with open(self.job_file_path, 'r') as f:
+            job_dict = json.load(f)
+            job_dict['finish_date'] = str(datetime.now())
+        with open(self.job_file_path, 'w') as f:
+            json.dump(job_dict, f)
         
     def __exit__(self, type, value, traceback):
         if type is None:
             self.__finish_job()
             return  # No exception
 
         if issubclass(type, SkipWithBlock):
```

### Comparing `mflag-1.6.6/mflag/src/rcmng/client/__init__.py` & `mflag-1.6.7/mflag/src/rcmng/client/__init__.py`

 * *Files identical despite different names*

### Comparing `mflag-1.6.6/mflag/src/rcmng/server/__init__.py` & `mflag-1.6.7/mflag/src/rcmng/server/__init__.py`

 * *Files identical despite different names*

### Comparing `mflag-1.6.6/mflag/src/rcmng/submit/__init__.py` & `mflag-1.6.7/mflag/src/rcmng/submit/__init__.py`

 * *Files identical despite different names*

### Comparing `mflag-1.6.6/mflag.egg-info/PKG-INFO` & `mflag-1.6.7/mflag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflag
-Version: 1.6.6
+Version: 1.6.7
 Summary: put/remove flags for files and folders
 Author: Moses Dastmard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mflag: powerful Python toolkit for mark/unmark files and directories 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pandas.svg)](https://pypi.org/project/mflag/)
```

