# Comparing `tmp/processingtools-0.3.0.tar.gz` & `tmp/processingtools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\processingtools-0.3.0.tar", last modified: Sat Jun 24 03:41:03 2023, max compression
+gzip compressed data, was "dist\processingtools-0.3.1.tar", last modified: Mon Jun 26 12:31:16 2023, max compression
```

## Comparing `processingtools-0.3.0.tar` & `processingtools-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 03:41:03.536924 processingtools-0.3.0/
--rw-rw-rw-   0        0        0     1085 2022-04-02 13:28:58.000000 processingtools-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     1798 2023-06-24 03:41:03.535922 processingtools-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-24 03:41:03.528921 processingtools-0.3.0/ProcessingTools/
--rw-rw-rw-   0        0        0     7620 2023-06-24 03:39:10.000000 processingtools-0.3.0/ProcessingTools/EnvReco.py
--rw-rw-rw-   0        0        0     4347 2023-06-21 11:29:03.000000 processingtools-0.3.0/ProcessingTools/PrgressBar.py
--rw-rw-rw-   0        0        0      122 2023-06-23 14:29:11.000000 processingtools-0.3.0/ProcessingTools/__init__.py
--rw-rw-rw-   0        0        0     8357 2023-06-14 13:17:42.000000 processingtools-0.3.0/ProcessingTools/functions.py
--rw-rw-rw-   0        0        0    16364 2023-06-23 16:05:03.000000 processingtools-0.3.0/ProcessingTools/torch_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-24 03:41:03.526922 processingtools-0.3.0/ProcessingTools.egg-info/
--rw-rw-rw-   0        0        0     1798 2023-06-24 03:41:02.000000 processingtools-0.3.0/ProcessingTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2023-06-24 03:41:02.000000 processingtools-0.3.0/ProcessingTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 03:41:02.000000 processingtools-0.3.0/ProcessingTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-24 03:41:02.000000 processingtools-0.3.0/ProcessingTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-24 03:41:02.000000 processingtools-0.3.0/ProcessingTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1319 2022-11-25 07:38:38.000000 processingtools-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 03:41:03.536924 processingtools-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-06-23 14:29:11.000000 processingtools-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:31:16.225997 processingtools-0.3.1/
+-rw-rw-rw-   0        0        0     1085 2022-04-02 13:28:58.000000 processingtools-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     1800 2023-06-26 12:31:16.225997 processingtools-0.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 12:31:16.216997 processingtools-0.3.1/ProcessingTools/
+-rw-rw-rw-   0        0        0     7903 2023-06-26 12:30:59.000000 processingtools-0.3.1/ProcessingTools/EnvReco.py
+-rw-rw-rw-   0        0        0     4347 2023-06-21 11:29:03.000000 processingtools-0.3.1/ProcessingTools/PrgressBar.py
+-rw-rw-rw-   0        0        0      122 2023-06-23 14:29:11.000000 processingtools-0.3.1/ProcessingTools/__init__.py
+-rw-rw-rw-   0        0        0     8357 2023-06-14 13:17:42.000000 processingtools-0.3.1/ProcessingTools/functions.py
+-rw-rw-rw-   0        0        0    16364 2023-06-23 16:05:03.000000 processingtools-0.3.1/ProcessingTools/torch_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:31:16.214997 processingtools-0.3.1/ProcessingTools.egg-info/
+-rw-rw-rw-   0        0        0     1800 2023-06-26 12:31:15.000000 processingtools-0.3.1/ProcessingTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      677 2023-06-26 12:31:15.000000 processingtools-0.3.1/ProcessingTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 12:31:15.000000 processingtools-0.3.1/ProcessingTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-26 12:31:15.000000 processingtools-0.3.1/ProcessingTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-26 12:31:15.000000 processingtools-0.3.1/ProcessingTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1321 2023-06-26 12:30:59.000000 processingtools-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 12:31:16.225997 processingtools-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-06-26 12:30:59.000000 processingtools-0.3.1/setup.py
```

### Comparing `processingtools-0.3.0/LICENSE` & `processingtools-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.0/PKG-INFO` & `processingtools-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processingtools
-Version: 0.3.0
+Version: 0.3.1
 Summary: https://github.com/ysy9997/ProcessingTools.git
 Home-page: https://github.com/ysy9997/ProcessingTools.git
 Author: syy
 Author-email: ysy9997@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -34,15 +34,15 @@
     time.sleep(0.1)
 ```
 or
 ```
 import processingtools as pt
 import time
 
-for i in pt.ProgressBar(range(50), bar_length=40, start_mark=None, finish_mark='progress done!', max=False):
+for i in pt.ProgressBar(range(50), bar_length=40, start_mark=None, finish_mark='progress done!', total=False):
     time.sleep(0.1)
 ```
 Then, 
 ```
 |████████████████████████████████████████| 100.0% | 50/50 | 0s |  
 progress finished!(5311ms)
 ```
```

### Comparing `processingtools-0.3.0/ProcessingTools/EnvReco.py` & `processingtools-0.3.1/ProcessingTools/EnvReco.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 import os
 import shutil
 import json
 import time
 import datetime
-import functions
+import processingtools.functions
+
+
+def file_opener(input_function):
+    """
+    file opener
+    :param input_function: input function
+    return input function output
+    """
+    def wrapper(self, *args, **kwargs):
+        if self.logs.closed:
+            with open(f'{self.save_path}/logs.txt', 'a') as self.logs:
+                output = input_function(self, *args, **kwargs)
+        else:
+            output = input_function(self, *args, **kwargs)
+        return output
+
+    return wrapper
 
 
 class EnvReco:
     """
     The class of Environments recorder.
     """
     def __init__(self, save_path: str, project_root_path: str = None, space: str = '', varify_exist: bool = True):
@@ -20,15 +37,15 @@
         """
 
         self.save_path = os.path.abspath(save_path)
 
         if varify_exist and os.path.exists(self.save_path):
             raise OSError(f'{self.save_path} already exist.')
         if not os.path.exists(self.save_path):
-            functions.create_folder(self.save_path, warning=False)
+            processingtools.functions.create_folder(self.save_path, warning=False)
 
         self.logs = open(f'{save_path}/logs.txt', 'a')
         self.project_root_path = os.path.dirname(os.path.abspath(__file__)) if project_root_path is None else project_root_path
         self.timer = time.time()
         self.present = datetime.datetime
         self.__start = True
         self.space = space
@@ -52,139 +69,145 @@
                 raise OSError('[record_code] will save the current folder. '
                               'Thus, the save path must not include the current path.')
 
             shutil.copytree(f'{self.project_root_path}', f'{self.save_path}/{folder_name}/')
 
         return True
 
+    @file_opener
     def record_arg(self, args, save_type: str = 'txt', print_console: bool = True):
         """
         record input arguments
         :param args: input arguments
         :param print_console: if True you can see logs in the console as well
         :param save_type: if 'json', it will be attached the logs file
         :return: args dictionary and absolute path arg
         """
 
-        with open(f'{self.save_path}/logs.txt', 'a') as self.logs:
-            args = self.arg2abs(args)
+        args = self.arg2abs(args)
 
-            if save_type not in ['txt', 'text', 'json']:
-                raise ValueError('save_type must be \'txt\' or \'text\' or \'json\'')
+        if save_type not in ['txt', 'text', 'json']:
+            raise ValueError('save_type must be \'txt\' or \'text\' or \'json\'')
+
+        if save_type == 'json':
+            with open(f'{self.save_path}/args.json', 'w') as f:
+                json.dump(args.__dict__, f, indent=4)
+        else:
+            self.put_space(print_console)
+            self.print_if_true('Args: ', print_console)
+            args_dict = args.__dict__
+            print('{', file=self.logs)
+            for key in args_dict:
+                print(f'    {key}: {args_dict[key]}', file=self.logs)
+            print('}', file=self.logs)
 
-            if save_type == 'json':
-                with open(f'{self.save_path}/args.json', 'w') as f:
-                    json.dump(args.__dict__, f, indent=4)
-            else:
-                self.put_space(print_console)
-                self.print_if_true('Args: ', print_console)
-                args_dict = args.__dict__
-                print('{', file=self.logs)
-                for key in args_dict:
-                    print(f'    {key}: {args_dict[key]}', file=self.logs)
-                print('}', file=self.logs)
-
-            if print_console:
-                args_dict = args.__dict__
-                print('{')
-                for key in args_dict:
-                    print(f'    {key}: {args_dict[key]}')
-                print('}')
+        if print_console:
+            args_dict = args.__dict__
+            print('{')
+            for key in args_dict:
+                print(f'    {key}: {args_dict[key]}')
+            print('}')
 
-            self.args = args.__dict__
+        self.args = args.__dict__
 
         return self.args, args
 
+    @file_opener
     def record_os(self, keys: list = None, print_console: bool = True):
         """
         record os environments
         :param keys: if you insert key values, it will record only key environments
         :param print_console: if True you can see logs in the console as well
         :return: os dictionary
         """
 
-        with open(f'{self.save_path}/logs.txt', 'a') as self.logs:
-            self.put_space(print_console)
-            self.print_if_true('OS Env: ', print_console)
+        self.put_space(print_console)
+        self.print_if_true('OS Env: ', print_console)
 
-            os_env = os.environ
-            self.log_dict(os_env, keys, print_console)
+        os_env = os.environ
+        self.log_dict(os_env, keys, print_console)
 
-            self.os = os_env
+        self.os = os_env
 
         return self.os
 
+    @file_opener
     def record_gpu(self, keys: list = None, print_console: bool = True) -> dict:
         """
         record gpu environments
         :param keys: if you insert key values, it will record only key environments
         :param print_console: if True you can see logs in the console as well
         :return: gpu dictionary
         """
 
-        with open(f'{self.save_path}/logs.txt', 'a') as self.logs:
-            self.put_space(print_console)
-            self.print_if_true('GPU Info: ', print_console)
+        self.put_space(print_console)
+        self.print_if_true('GPU Info: ', print_console)
+
+        try:
+            import torch
 
-            try:
-                import torch
+            gpu = {'cuda': torch.cuda.is_available(),
+                   'num': torch.cuda.device_count(),
+                   'names': [torch.cuda.get_device_name(_) for _ in range(torch.cuda.device_count())]}
 
-                gpu = {'cuda': torch.cuda.is_available(),
-                       'num': torch.cuda.device_count(),
-                       'names': [torch.cuda.get_device_name(_) for _ in range(torch.cuda.device_count())]}
+        except Exception:
+            raise ImportError('this function is needed pytorch!')
 
-            except Exception:
-                raise ImportError('this function is needed pytorch!')
+        self.log_dict(gpu, keys, print_console)
+        self.gpu = gpu
 
-            self.log_dict(gpu, keys, print_console)
-            self.gpu = gpu
         return self.gpu
 
-    def record_present(self, log: str) -> True:
+    @file_opener
+    def print(self, log: str) -> True:
         """
         write and print log with present time
         :param log: log
         return True
         """
 
-        with open(f'{self.save_path}/logs.txt', 'a') as self.logs:
-            now = self.present.now()
-            print(f'\033[95m[{now.year}-{now.month}-{now.day} '
-                  f'{now.hour}:{now.minute}:{now.second}.{round(now.microsecond / 10000):02d}]\033[0m: {log}')
-            print(f'[{now.year}-{now.month}-{now.day} '
-                  f'{now.hour}:{now.minute}:{now.second}.{round(now.microsecond / 10000):02d}]: {log}', file=self.logs)
+        now = self.present.now()
+        print(f'\033[95m[{now.year}-{now.month}-{now.day} '
+              f'{now.hour}:{now.minute}:{now.second}.{round(now.microsecond / 10000):02d}]\033[0m: {log}')
+        print(f'[{now.year}-{now.month}-{now.day} '
+              f'{now.hour}:{now.minute}:{now.second}.{round(now.microsecond / 10000):02d}]: {log}', file=self.logs)
 
         return True
 
+    @file_opener
     def put_space(self, print_console: bool = True) -> bool:
         """
         insert space in the logs
         :param print_console: if True you can see logs in the console as well
         :return: True or False
         """
 
+        if self.logs.closed:
+            self.logs = open(f'{self.save_path}/logs.txt', 'a')
+
         if self.__start:
             self.__start = False
             return False
 
         else:
             self.print_if_true(self.space, print_console)
 
         return True
 
+    @file_opener
     def print_if_true(self, contents: str, print_console: bool) -> None:
         """
         if print_console true, print in the console as well
         :param contents: logs contents
         :param print_console: if True you can see logs in the console as well
         :return: None
         """
 
         if print_console:
-            functions.print_write(contents, self.logs)
+            processingtools.functions.print_write(contents, self.logs)
         else:
             print(contents, file=self.logs)
 
     @staticmethod
     def arg2abs(args):
         """
         if args have path, convert absolute path
```

### Comparing `processingtools-0.3.0/ProcessingTools/PrgressBar.py` & `processingtools-0.3.1/ProcessingTools/PrgressBar.py`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.0/ProcessingTools/functions.py` & `processingtools-0.3.1/ProcessingTools/functions.py`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.0/ProcessingTools/torch_tools.py` & `processingtools-0.3.1/ProcessingTools/torch_tools.py`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.0/ProcessingTools.egg-info/PKG-INFO` & `processingtools-0.3.1/ProcessingTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processingtools
-Version: 0.3.0
+Version: 0.3.1
 Summary: https://github.com/ysy9997/ProcessingTools.git
 Home-page: https://github.com/ysy9997/ProcessingTools.git
 Author: syy
 Author-email: ysy9997@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -34,15 +34,15 @@
     time.sleep(0.1)
 ```
 or
 ```
 import processingtools as pt
 import time
 
-for i in pt.ProgressBar(range(50), bar_length=40, start_mark=None, finish_mark='progress done!', max=False):
+for i in pt.ProgressBar(range(50), bar_length=40, start_mark=None, finish_mark='progress done!', total=False):
     time.sleep(0.1)
 ```
 Then, 
 ```
 |████████████████████████████████████████| 100.0% | 50/50 | 0s |  
 progress finished!(5311ms)
 ```
```

### Comparing `processingtools-0.3.0/ProcessingTools.egg-info/SOURCES.txt` & `processingtools-0.3.1/ProcessingTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.0/README.md` & `processingtools-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     time.sleep(0.1)
 ```
 or
 ```
 import processingtools as pt
 import time
 
-for i in pt.ProgressBar(range(50), bar_length=40, start_mark=None, finish_mark='progress done!', max=False):
+for i in pt.ProgressBar(range(50), bar_length=40, start_mark=None, finish_mark='progress done!', total=False):
     time.sleep(0.1)
 ```
 Then, 
 ```
 |████████████████████████████████████████| 100.0% | 50/50 | 0s |  
 progress finished!(5311ms)
 ```
```

### Comparing `processingtools-0.3.0/setup.py` & `processingtools-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="processingtools",
-    version="0.3.0",
+    version="0.3.1",
     install_requires=['opencv-python>=4.5.5.62',
                       'numpy>=1.19.4',
                       'matplotlib>=3.3.3'],
     license='MIT',
     author="syy",
     author_email="ysy9997@gmail.com",
     description="https://github.com/ysy9997/ProcessingTools.git",
```

