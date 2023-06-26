# Comparing `tmp/kangtools-0.0.4.tar.gz` & `tmp/kangtools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kangtools-0.0.4.tar", last modified: Fri Jun 23 19:40:09 2023, max compression
+gzip compressed data, was "kangtools-0.0.5.tar", last modified: Mon Jun 26 14:46:25 2023, max compression
```

## Comparing `kangtools-0.0.4.tar` & `kangtools-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:40:09.967411 kangtools-0.0.4/
--rw-r--r--   0 kang       (501) staff       (20)     4408 2023-06-23 19:40:09.967294 kangtools-0.0.4/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)     4193 2023-06-23 19:34:01.000000 kangtools-0.0.4/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:40:09.966546 kangtools-0.0.4/kangtools/
--rw-r--r--   0 kang       (501) staff       (20)       86 2023-06-23 19:39:26.000000 kangtools-0.0.4/kangtools/__init__.py
--rwxr-xr-x   0 kang       (501) staff       (20)     1478 2023-06-23 19:31:19.000000 kangtools-0.0.4/kangtools/version_control.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:40:09.967157 kangtools-0.0.4/kangtools.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)     4408 2023-06-23 19:40:09.000000 kangtools-0.0.4/kangtools.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      237 2023-06-23 19:40:09.000000 kangtools-0.0.4/kangtools.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-23 19:40:09.000000 kangtools-0.0.4/kangtools.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)       77 2023-06-23 19:40:09.000000 kangtools-0.0.4/kangtools.egg-info/entry_points.txt
--rw-r--r--   0 kang       (501) staff       (20)       10 2023-06-23 19:40:09.000000 kangtools-0.0.4/kangtools.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-23 19:40:09.967442 kangtools-0.0.4/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      780 2023-06-23 19:39:42.000000 kangtools-0.0.4/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 14:46:25.103304 kangtools-0.0.5/
+-rw-r--r--   0 kang       (501) staff       (20)     4451 2023-06-26 14:46:25.103196 kangtools-0.0.5/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)     4236 2023-06-26 14:44:08.000000 kangtools-0.0.5/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 14:46:25.102342 kangtools-0.0.5/kangtools/
+-rw-r--r--   0 kang       (501) staff       (20)       86 2023-06-23 19:39:26.000000 kangtools-0.0.5/kangtools/__init__.py
+-rwxr-xr-x   0 kang       (501) staff       (20)     1517 2023-06-26 14:42:53.000000 kangtools-0.0.5/kangtools/version_control.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 14:46:25.103048 kangtools-0.0.5/kangtools.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)     4451 2023-06-26 14:46:25.000000 kangtools-0.0.5/kangtools.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      237 2023-06-26 14:46:25.000000 kangtools-0.0.5/kangtools.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-26 14:46:25.000000 kangtools-0.0.5/kangtools.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)       77 2023-06-26 14:46:25.000000 kangtools-0.0.5/kangtools.egg-info/entry_points.txt
+-rw-r--r--   0 kang       (501) staff       (20)       10 2023-06-26 14:46:25.000000 kangtools-0.0.5/kangtools.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-26 14:46:25.103337 kangtools-0.0.5/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      780 2023-06-26 14:45:51.000000 kangtools-0.0.5/setup.py
```

### Comparing `kangtools-0.0.4/PKG-INFO` & `kangtools-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kangtools
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package for version control.
 Author: xiaowen kang
 Author-email: kangxiaowen@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 
 # kangtools
@@ -122,7 +122,9 @@
 ```bash
 kangtools_version_control
 ```
 
 这将会运行 `version_control.py` 文件中的 `main` 函数。
 
 -----
+------
+添加了内容。- add date- kang.
```

### Comparing `kangtools-0.0.4/README.md` & `kangtools-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -113,7 +113,9 @@
 ```bash
 kangtools_version_control
 ```
 
 这将会运行 `version_control.py` 文件中的 `main` 函数。
 
 -----
+------
+添加了内容。- add date- kang.
```

### Comparing `kangtools-0.0.4/kangtools/version_control.py` & `kangtools-0.0.5/kangtools/version_control.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 import os
 import re
-
+import datetime
 
 def main():
     version_file_path = "version.txt"
     commit_message = input("Enter commit message: ")
 
     # Check if version.txt exists, create it if it doesn't
     if not os.path.exists(version_file_path):
@@ -23,27 +23,27 @@
             # If this line looks like a version number, use it and stop
             if line.strip().startswith("V.0."):
                 version = line.strip()
                 break
 
     # Extract version number
     version_number = int(re.search(r'\d+(?=\s|$)', version).group())
-    # version_number = int(re.search(r'\d+$', version).group())
 
     # Increment version number
     new_version_number = version_number + 1
 
+    # Get current timestamp
+    timestamp = datetime.datetime.now().strftime('%Y-%m-%d')
+
     # Update version file
     with open(version_file_path, 'a') as f:
-        # f.write(f"V.0.{new_version_number}\n")
-        f.write(f"V.0.{new_version_number} - {commit_message}\n")
+        f.write(f"V.0.{new_version_number} - {commit_message}  ©KANG - {timestamp}  \n")
 
     # Execute git commands
     os.system("git add -A")
-    os.system(f'git commit -m "V.0.{new_version_number} - {commit_message}"')
+    os.system(f'git commit -m "V.0.{new_version_number} - {commit_message}  ©KANG - {timestamp} "')
     os.system("git push")
 
     print(f"Committed Version V.0.{new_version_number}")
 
-
 if __name__ == "__main__":
-    main()
+    main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kangtools-0.0.4/kangtools.egg-info/PKG-INFO` & `kangtools-0.0.5/kangtools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kangtools
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package for version control.
 Author: xiaowen kang
 Author-email: kangxiaowen@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 
 # kangtools
@@ -122,7 +122,9 @@
 ```bash
 kangtools_version_control
 ```
 
 这将会运行 `version_control.py` 文件中的 `main` 函数。
 
 -----
+------
+添加了内容。- add date- kang.
```

### Comparing `kangtools-0.0.4/setup.py` & `kangtools-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='kangtools',  # 包的名字
-    version='0.0.4',  # 包的版本
+    version='0.0.5',  # 包的版本
     author='xiaowen kang',  # 你的名字
     author_email='kangxiaowen@gmail.com',  # 你的邮箱
     packages=['kangtools'],  # 包含的包，这是一个列表，如果你的项目包含多个包，都需要列在这里
     license='LICENSE',  # 许可证文件
     description='A Python package for version control.',  # 包的简短描述
     long_description=open('README.md').read(),  # 包的详细描述，通常从 README.md 文件读取
     long_description_content_type="text/markdown",  # 描述的格式，使用markdown格式
```

