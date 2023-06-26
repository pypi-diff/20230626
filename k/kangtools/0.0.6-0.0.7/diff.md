# Comparing `tmp/kangtools-0.0.6.tar.gz` & `tmp/kangtools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kangtools-0.0.6.tar", last modified: Mon Jun 26 15:14:20 2023, max compression
+gzip compressed data, was "kangtools-0.0.7.tar", last modified: Mon Jun 26 15:29:28 2023, max compression
```

## Comparing `kangtools-0.0.6.tar` & `kangtools-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 15:14:20.117156 kangtools-0.0.6/
--rw-r--r--   0 kang       (501) staff       (20)     4615 2023-06-26 15:14:20.117039 kangtools-0.0.6/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)     4400 2023-06-26 15:10:15.000000 kangtools-0.0.6/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 15:14:20.116196 kangtools-0.0.6/kangtools/
--rw-r--r--   0 kang       (501) staff       (20)       86 2023-06-23 19:39:26.000000 kangtools-0.0.6/kangtools/__init__.py
--rwxr-xr-x   0 kang       (501) staff       (20)     1812 2023-06-26 15:06:30.000000 kangtools-0.0.6/kangtools/commit_version_to_git.py
--rwxr-xr-x   0 kang       (501) staff       (20)     1708 2023-06-26 15:03:27.000000 kangtools-0.0.6/kangtools/version_control.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 15:14:20.116896 kangtools-0.0.6/kangtools.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)     4615 2023-06-26 15:14:20.000000 kangtools-0.0.6/kangtools.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      272 2023-06-26 15:14:20.000000 kangtools-0.0.6/kangtools.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-26 15:14:20.000000 kangtools-0.0.6/kangtools.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)      148 2023-06-26 15:14:20.000000 kangtools-0.0.6/kangtools.egg-info/entry_points.txt
--rw-r--r--   0 kang       (501) staff       (20)       10 2023-06-26 15:14:20.000000 kangtools-0.0.6/kangtools.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-26 15:14:20.117190 kangtools-0.0.6/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      860 2023-06-26 15:14:12.000000 kangtools-0.0.6/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 15:29:28.813311 kangtools-0.0.7/
+-rw-r--r--   0 kang       (501) staff       (20)     9502 2023-06-26 15:29:28.813143 kangtools-0.0.7/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)     9287 2023-06-26 15:28:17.000000 kangtools-0.0.7/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 15:29:28.812387 kangtools-0.0.7/kangtools/
+-rw-r--r--   0 kang       (501) staff       (20)       86 2023-06-23 19:39:26.000000 kangtools-0.0.7/kangtools/__init__.py
+-rwxr-xr-x   0 kang       (501) staff       (20)     1807 2023-06-26 15:28:29.000000 kangtools-0.0.7/kangtools/commit_version_to_git.py
+-rwxr-xr-x   0 kang       (501) staff       (20)     1708 2023-06-26 15:03:27.000000 kangtools-0.0.7/kangtools/version_control.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 15:29:28.812995 kangtools-0.0.7/kangtools.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)     9502 2023-06-26 15:29:28.000000 kangtools-0.0.7/kangtools.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      272 2023-06-26 15:29:28.000000 kangtools-0.0.7/kangtools.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-26 15:29:28.000000 kangtools-0.0.7/kangtools.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)      148 2023-06-26 15:29:28.000000 kangtools-0.0.7/kangtools.egg-info/entry_points.txt
+-rw-r--r--   0 kang       (501) staff       (20)       10 2023-06-26 15:29:28.000000 kangtools-0.0.7/kangtools.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-26 15:29:28.813344 kangtools-0.0.7/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      860 2023-06-26 15:29:14.000000 kangtools-0.0.7/setup.py
```

### Comparing `kangtools-0.0.6/kangtools/commit_version_to_git.py` & `kangtools-0.0.7/kangtools/commit_version_to_git.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 #!/usr/bin/env python3
 import os
 import re
 import datetime
 import argparse
 
-def main(args):
+
+def main():
+    parser = argparse.ArgumentParser(description="This script handles versioning and git commit operations. The version number is stored in a text file, incremented, and then a new entry with the version number, a user-provided commit message, the user name, and the current timestamp is appended. These details are also used in the git commit message.")
+    parser.add_argument('-m', '--commit_message', type=str, help='Specify the commit message that will be used in both the version text file and the git commit. If not provided, the script will prompt for it.')
+    args = parser.parse_args()
+
     version_file_path = "version.txt"
 
     if args.commit_message:
         commit_message = args.commit_message
     else:
         commit_message = input("Enter commit message: ")
 
@@ -33,12 +38,10 @@
 
     os.system("git add -A")
     os.system(f'git commit -m "V.0.{new_version_number} - {commit_message}  ©KANG - {timestamp} "')
     os.system("git push")
 
     print(f"Committed Version V.0.{new_version_number}")
 
+
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description="This script handles versioning and git commit operations. The version number is stored in a text file, incremented, and then a new entry with the version number, a user-provided commit message, the user name, and the current timestamp is appended. These details are also used in the git commit message.")
-    parser.add_argument('-m', '--commit_message', type=str, help='Specify the commit message that will be used in both the version text file and the git commit. If not provided, the script will prompt for it.')
-    args = parser.parse_args()
-    main(args)
+    main()
```

### Comparing `kangtools-0.0.6/kangtools/version_control.py` & `kangtools-0.0.7/kangtools/version_control.py`

 * *Files identical despite different names*

### Comparing `kangtools-0.0.6/setup.py` & `kangtools-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='kangtools',  # 包的名字
-    version='0.0.6',  # 包的版本
+    version='0.0.7',  # 包的版本
     author='xiaowen kang',  # 你的名字
     author_email='kangxiaowen@gmail.com',  # 你的邮箱
     packages=['kangtools'],  # 包含的包，这是一个列表，如果你的项目包含多个包，都需要列在这里
     license='LICENSE',  # 许可证文件
     description='A Python package for version control.',  # 包的简短描述
     long_description=open('README.md').read(),  # 包的详细描述，通常从 README.md 文件读取
     long_description_content_type="text/markdown",  # 描述的格式，使用markdown格式
```

