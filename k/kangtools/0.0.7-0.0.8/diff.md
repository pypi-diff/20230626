# Comparing `tmp/kangtools-0.0.7.tar.gz` & `tmp/kangtools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kangtools-0.0.7.tar", last modified: Mon Jun 26 15:29:28 2023, max compression
+gzip compressed data, was "kangtools-0.0.8.tar", last modified: Mon Jun 26 16:51:36 2023, max compression
```

## Comparing `kangtools-0.0.7.tar` & `kangtools-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 15:29:28.813311 kangtools-0.0.7/
--rw-r--r--   0 kang       (501) staff       (20)     9502 2023-06-26 15:29:28.813143 kangtools-0.0.7/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)     9287 2023-06-26 15:28:17.000000 kangtools-0.0.7/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 15:29:28.812387 kangtools-0.0.7/kangtools/
--rw-r--r--   0 kang       (501) staff       (20)       86 2023-06-23 19:39:26.000000 kangtools-0.0.7/kangtools/__init__.py
--rwxr-xr-x   0 kang       (501) staff       (20)     1807 2023-06-26 15:28:29.000000 kangtools-0.0.7/kangtools/commit_version_to_git.py
--rwxr-xr-x   0 kang       (501) staff       (20)     1708 2023-06-26 15:03:27.000000 kangtools-0.0.7/kangtools/version_control.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 15:29:28.812995 kangtools-0.0.7/kangtools.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)     9502 2023-06-26 15:29:28.000000 kangtools-0.0.7/kangtools.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      272 2023-06-26 15:29:28.000000 kangtools-0.0.7/kangtools.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-26 15:29:28.000000 kangtools-0.0.7/kangtools.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)      148 2023-06-26 15:29:28.000000 kangtools-0.0.7/kangtools.egg-info/entry_points.txt
--rw-r--r--   0 kang       (501) staff       (20)       10 2023-06-26 15:29:28.000000 kangtools-0.0.7/kangtools.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-26 15:29:28.813344 kangtools-0.0.7/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      860 2023-06-26 15:29:14.000000 kangtools-0.0.7/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 16:51:36.270017 kangtools-0.0.8/
+-rw-r--r--   0 kang       (501) staff       (20)    11512 2023-06-26 16:51:36.269849 kangtools-0.0.8/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)    11297 2023-06-26 15:32:07.000000 kangtools-0.0.8/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 16:51:36.269097 kangtools-0.0.8/kangtools/
+-rw-r--r--   0 kang       (501) staff       (20)       86 2023-06-26 16:29:17.000000 kangtools-0.0.8/kangtools/__init__.py
+-rwxr-xr-x   0 kang       (501) staff       (20)     1807 2023-06-26 16:29:16.000000 kangtools-0.0.8/kangtools/commit_version_to_git.py
+-rwxr-xr-x   0 kang       (501) staff       (20)     1708 2023-06-26 15:03:27.000000 kangtools-0.0.8/kangtools/version_control.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 16:51:36.269699 kangtools-0.0.8/kangtools.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)    11512 2023-06-26 16:51:36.000000 kangtools-0.0.8/kangtools.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      272 2023-06-26 16:51:36.000000 kangtools-0.0.8/kangtools.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-26 16:51:36.000000 kangtools-0.0.8/kangtools.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)      148 2023-06-26 16:51:36.000000 kangtools-0.0.8/kangtools.egg-info/entry_points.txt
+-rw-r--r--   0 kang       (501) staff       (20)       10 2023-06-26 16:51:36.000000 kangtools-0.0.8/kangtools.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-26 16:51:36.270047 kangtools-0.0.8/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      860 2023-06-26 16:51:35.000000 kangtools-0.0.8/setup.py
```

### Comparing `kangtools-0.0.7/PKG-INFO` & `kangtools-0.0.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: kangtools
-Version: 0.0.7
-Summary: A Python package for version control.
-Author: xiaowen kang
-Author-email: kangxiaowen@gmail.com
-License: LICENSE
-Description-Content-Type: text/markdown
-
 # kangtools
 kangtools
 
 - git remote
 - renew verison.
 - upload add date. 
 
@@ -185,8 +176,49 @@
 
 然而，在 `main()` 函数内部，你可以定义其他的变量或者使用其他函数，这些函数可能需要参数。在你的脚本中，你使用了 `argparse` 库来处理命令行参数。虽然这些参数没有直接传递给 `main()` 函数，但是在 `main()` 函数内部，你调用了 `argparse` 的 `parse_args()` 函数，这个函数可以读取命令行参数并返回一个对象（在你的脚本中是 `args` 对象），这个对象包含了所有的命令行参数值。因此，尽管这些参数没有直接传给 `main()` 函数，你仍然可以在 `main()` 函数内部访问它们。
 
 这样设计的目的是为了让 `main()` 函数可以独立于外部环境运行，使得代码更加模块化，更容易测试和复用。只有当你明确需要让函数接受外部参数时，你才在函数定义中添加参数。
 ---
 我将argparse的代码移到main()函数内部，并去掉了main(args)。这是因为我们希望main()函数可以处理其自己的命令行参数，而不需要从外部传递参数。
 --
+---
+kang@Love-Grace williampolicy.github.io$ kangtools_commit_version_to_git -h
+usage: kangtools_commit_version_to_git [-h] [-m COMMIT_MESSAGE]
+
+This script handles versioning and git commit operations. The version number is stored in a text file, incremented, and then a new entry with the version number, a user-provided commit
+message, the user name, and the current timestamp is appended. These details are also used in the git commit message.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -m COMMIT_MESSAGE, --commit_message COMMIT_MESSAGE
+                        Specify the commit message that will be used in both the version text file and the git commit. If not provided, the script will prompt for it.
+kang@Love-Grace williampolicy.github.io$ kangtools_commit_version_to_git -m "good commit pip install kangtools. it works. Great! and with help"
+[main 58179fc] V.0.7 - good commit pip install kangtools. it works. Great! and with help  ©KANG - 2023-06-26
+ 1 file changed, 1 insertion(+)
+Enumerating objects: 5, done.
+Counting objects: 100% (5/5), done.
+Delta compression using up to 8 threads
+Compressing objects: 100% (3/3), done.
+Writing objects: 100% (3/3), 445 bytes | 445.00 KiB/s, done.
+Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
+remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
+To https://github.com/williampolicy/williampolicy.github.io.git
+   3a398e3..58179fc  main -> main
+Committed Version V.0.7
+kang@Love-Grace williampolicy.github.io$ cat version.txt 
+V.0.3V.0.4
+V.0.4 - add function to write history in version.text
+V.0.5
+V.0.5 - this is a great work for upload_new_version_v1.py
+V.0.5
+V.0.5 - try to make a test 
+V.0.5
+V.0.5 - try to make a test
+V.0.5
+V.0.5 - test more
+V.0.6 - test kangtools_version_control  ©KANG - 2023-06-26  
+V.0.7 - good commit pip install kangtools. it works. Great! and with help  ©KANG - 2023-06-26  
+------it works. 
+-------------
+
+下面我们尝试    setup 版本的自动更新。 Try.
```

### Comparing `kangtools-0.0.7/kangtools/commit_version_to_git.py` & `kangtools-0.0.8/kangtools/commit_version_to_git.py`

 * *Files identical despite different names*

### Comparing `kangtools-0.0.7/kangtools/version_control.py` & `kangtools-0.0.8/kangtools/version_control.py`

 * *Files identical despite different names*

### Comparing `kangtools-0.0.7/setup.py` & `kangtools-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='kangtools',  # 包的名字
-    version='0.0.7',  # 包的版本
+    version='0.0.8',  # 包的版本
     author='xiaowen kang',  # 你的名字
     author_email='kangxiaowen@gmail.com',  # 你的邮箱
     packages=['kangtools'],  # 包含的包，这是一个列表，如果你的项目包含多个包，都需要列在这里
     license='LICENSE',  # 许可证文件
     description='A Python package for version control.',  # 包的简短描述
     long_description=open('README.md').read(),  # 包的详细描述，通常从 README.md 文件读取
     long_description_content_type="text/markdown",  # 描述的格式，使用markdown格式
```

