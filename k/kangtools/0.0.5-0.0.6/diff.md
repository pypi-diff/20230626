# Comparing `tmp/kangtools-0.0.5.tar.gz` & `tmp/kangtools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kangtools-0.0.5.tar", last modified: Mon Jun 26 14:46:25 2023, max compression
+gzip compressed data, was "kangtools-0.0.6.tar", last modified: Mon Jun 26 15:14:20 2023, max compression
```

## Comparing `kangtools-0.0.5.tar` & `kangtools-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 14:46:25.103304 kangtools-0.0.5/
--rw-r--r--   0 kang       (501) staff       (20)     4451 2023-06-26 14:46:25.103196 kangtools-0.0.5/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)     4236 2023-06-26 14:44:08.000000 kangtools-0.0.5/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 14:46:25.102342 kangtools-0.0.5/kangtools/
--rw-r--r--   0 kang       (501) staff       (20)       86 2023-06-23 19:39:26.000000 kangtools-0.0.5/kangtools/__init__.py
--rwxr-xr-x   0 kang       (501) staff       (20)     1517 2023-06-26 14:42:53.000000 kangtools-0.0.5/kangtools/version_control.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 14:46:25.103048 kangtools-0.0.5/kangtools.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)     4451 2023-06-26 14:46:25.000000 kangtools-0.0.5/kangtools.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      237 2023-06-26 14:46:25.000000 kangtools-0.0.5/kangtools.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-26 14:46:25.000000 kangtools-0.0.5/kangtools.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)       77 2023-06-26 14:46:25.000000 kangtools-0.0.5/kangtools.egg-info/entry_points.txt
--rw-r--r--   0 kang       (501) staff       (20)       10 2023-06-26 14:46:25.000000 kangtools-0.0.5/kangtools.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-26 14:46:25.103337 kangtools-0.0.5/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      780 2023-06-26 14:45:51.000000 kangtools-0.0.5/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 15:14:20.117156 kangtools-0.0.6/
+-rw-r--r--   0 kang       (501) staff       (20)     4615 2023-06-26 15:14:20.117039 kangtools-0.0.6/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)     4400 2023-06-26 15:10:15.000000 kangtools-0.0.6/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 15:14:20.116196 kangtools-0.0.6/kangtools/
+-rw-r--r--   0 kang       (501) staff       (20)       86 2023-06-23 19:39:26.000000 kangtools-0.0.6/kangtools/__init__.py
+-rwxr-xr-x   0 kang       (501) staff       (20)     1812 2023-06-26 15:06:30.000000 kangtools-0.0.6/kangtools/commit_version_to_git.py
+-rwxr-xr-x   0 kang       (501) staff       (20)     1708 2023-06-26 15:03:27.000000 kangtools-0.0.6/kangtools/version_control.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 15:14:20.116896 kangtools-0.0.6/kangtools.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)     4615 2023-06-26 15:14:20.000000 kangtools-0.0.6/kangtools.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      272 2023-06-26 15:14:20.000000 kangtools-0.0.6/kangtools.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-26 15:14:20.000000 kangtools-0.0.6/kangtools.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)      148 2023-06-26 15:14:20.000000 kangtools-0.0.6/kangtools.egg-info/entry_points.txt
+-rw-r--r--   0 kang       (501) staff       (20)       10 2023-06-26 15:14:20.000000 kangtools-0.0.6/kangtools.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-26 15:14:20.117190 kangtools-0.0.6/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      860 2023-06-26 15:14:12.000000 kangtools-0.0.6/setup.py
```

### Comparing `kangtools-0.0.5/PKG-INFO` & `kangtools-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kangtools
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python package for version control.
 Author: xiaowen kang
 Author-email: kangxiaowen@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 
 # kangtools
@@ -124,7 +124,10 @@
 ```
 
 这将会运行 `version_control.py` 文件中的 `main` 函数。
 
 -----
 ------
 添加了内容。- add date- kang.
+
+-----
+将version_control.py 更新为 commit_version_to_git.py  因为原命令的名称，并不清晰。 越清晰，我们越好操作。也不容易忘记。
```

### Comparing `kangtools-0.0.5/README.md` & `kangtools-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -115,7 +115,10 @@
 ```
 
 这将会运行 `version_control.py` 文件中的 `main` 函数。
 
 -----
 ------
 添加了内容。- add date- kang.
+
+-----
+将version_control.py 更新为 commit_version_to_git.py  因为原命令的名称，并不清晰。 越清晰，我们越好操作。也不容易忘记。
```

### Comparing `kangtools-0.0.5/kangtools/version_control.py` & `kangtools-0.0.6/kangtools/commit_version_to_git.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 #!/usr/bin/env python3
-
 import os
 import re
 import datetime
+import argparse
 
-def main():
+def main(args):
     version_file_path = "version.txt"
-    commit_message = input("Enter commit message: ")
 
-    # Check if version.txt exists, create it if it doesn't
+    if args.commit_message:
+        commit_message = args.commit_message
+    else:
+        commit_message = input("Enter commit message: ")
+
     if not os.path.exists(version_file_path):
         with open(version_file_path, 'w') as f:
             f.write("V.0.1\n")
 
-    # Read previous version and commit history
     with open(version_file_path, 'r') as f:
         content = f.readlines()
-        # Initialize version as default
         version = "V.0.1"
-        # Start from the last line and move upwards
         for line in reversed(content):
-            # If this line looks like a version number, use it and stop
             if line.strip().startswith("V.0."):
                 version = line.strip()
                 break
 
-    # Extract version number
     version_number = int(re.search(r'\d+(?=\s|$)', version).group())
-
-    # Increment version number
     new_version_number = version_number + 1
-
-    # Get current timestamp
     timestamp = datetime.datetime.now().strftime('%Y-%m-%d')
 
-    # Update version file
     with open(version_file_path, 'a') as f:
         f.write(f"V.0.{new_version_number} - {commit_message}  ©KANG - {timestamp}  \n")
 
-    # Execute git commands
     os.system("git add -A")
     os.system(f'git commit -m "V.0.{new_version_number} - {commit_message}  ©KANG - {timestamp} "')
     os.system("git push")
 
     print(f"Committed Version V.0.{new_version_number}")
 
 if __name__ == "__main__":
-    main()
+    parser = argparse.ArgumentParser(description="This script handles versioning and git commit operations. The version number is stored in a text file, incremented, and then a new entry with the version number, a user-provided commit message, the user name, and the current timestamp is appended. These details are also used in the git commit message.")
+    parser.add_argument('-m', '--commit_message', type=str, help='Specify the commit message that will be used in both the version text file and the git commit. If not provided, the script will prompt for it.')
+    args = parser.parse_args()
+    main(args)
```

### Comparing `kangtools-0.0.5/kangtools.egg-info/PKG-INFO` & `kangtools-0.0.6/kangtools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kangtools
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python package for version control.
 Author: xiaowen kang
 Author-email: kangxiaowen@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 
 # kangtools
@@ -124,7 +124,10 @@
 ```
 
 这将会运行 `version_control.py` 文件中的 `main` 函数。
 
 -----
 ------
 添加了内容。- add date- kang.
+
+-----
+将version_control.py 更新为 commit_version_to_git.py  因为原命令的名称，并不清晰。 越清晰，我们越好操作。也不容易忘记。
```

### Comparing `kangtools-0.0.5/setup.py` & `kangtools-0.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup
 
 setup(
     name='kangtools',  # 包的名字
-    version='0.0.5',  # 包的版本
+    version='0.0.6',  # 包的版本
     author='xiaowen kang',  # 你的名字
     author_email='kangxiaowen@gmail.com',  # 你的邮箱
     packages=['kangtools'],  # 包含的包，这是一个列表，如果你的项目包含多个包，都需要列在这里
     license='LICENSE',  # 许可证文件
     description='A Python package for version control.',  # 包的简短描述
     long_description=open('README.md').read(),  # 包的详细描述，通常从 README.md 文件读取
     long_description_content_type="text/markdown",  # 描述的格式，使用markdown格式
     entry_points={
     'console_scripts': [
-        'kangtools_version_control=kangtools.version_control:main',],
+        'kangtools_version_control=kangtools.version_control:main',
+        'kangtools_commit_version_to_git=kangtools.commit_version_to_git:main',],
     },
 
 )
```

