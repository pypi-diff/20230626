# Comparing `tmp/kangtools-0.0.8.tar.gz` & `tmp/kangtools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kangtools-0.0.8.tar", last modified: Mon Jun 26 16:51:36 2023, max compression
+gzip compressed data, was "kangtools-0.0.9.tar", last modified: Mon Jun 26 16:58:09 2023, max compression
```

## Comparing `kangtools-0.0.8.tar` & `kangtools-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 16:51:36.270017 kangtools-0.0.8/
--rw-r--r--   0 kang       (501) staff       (20)    11512 2023-06-26 16:51:36.269849 kangtools-0.0.8/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)    11297 2023-06-26 15:32:07.000000 kangtools-0.0.8/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 16:51:36.269097 kangtools-0.0.8/kangtools/
--rw-r--r--   0 kang       (501) staff       (20)       86 2023-06-26 16:29:17.000000 kangtools-0.0.8/kangtools/__init__.py
--rwxr-xr-x   0 kang       (501) staff       (20)     1807 2023-06-26 16:29:16.000000 kangtools-0.0.8/kangtools/commit_version_to_git.py
--rwxr-xr-x   0 kang       (501) staff       (20)     1708 2023-06-26 15:03:27.000000 kangtools-0.0.8/kangtools/version_control.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 16:51:36.269699 kangtools-0.0.8/kangtools.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)    11512 2023-06-26 16:51:36.000000 kangtools-0.0.8/kangtools.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      272 2023-06-26 16:51:36.000000 kangtools-0.0.8/kangtools.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-26 16:51:36.000000 kangtools-0.0.8/kangtools.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)      148 2023-06-26 16:51:36.000000 kangtools-0.0.8/kangtools.egg-info/entry_points.txt
--rw-r--r--   0 kang       (501) staff       (20)       10 2023-06-26 16:51:36.000000 kangtools-0.0.8/kangtools.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-26 16:51:36.270047 kangtools-0.0.8/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      860 2023-06-26 16:51:35.000000 kangtools-0.0.8/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 16:58:09.611510 kangtools-0.0.9/
+-rw-r--r--   0 kang       (501) staff       (20)    11512 2023-06-26 16:58:09.611345 kangtools-0.0.9/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)    11297 2023-06-26 15:32:07.000000 kangtools-0.0.9/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 16:58:09.610624 kangtools-0.0.9/kangtools/
+-rw-r--r--   0 kang       (501) staff       (20)       86 2023-06-26 16:29:17.000000 kangtools-0.0.9/kangtools/__init__.py
+-rwxr-xr-x   0 kang       (501) staff       (20)     1807 2023-06-26 16:29:16.000000 kangtools-0.0.9/kangtools/commit_version_to_git.py
+-rwxr-xr-x   0 kang       (501) staff       (20)     1708 2023-06-26 15:03:27.000000 kangtools-0.0.9/kangtools/version_control.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-26 16:58:09.611181 kangtools-0.0.9/kangtools.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)    11512 2023-06-26 16:58:09.000000 kangtools-0.0.9/kangtools.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      272 2023-06-26 16:58:09.000000 kangtools-0.0.9/kangtools.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-26 16:58:09.000000 kangtools-0.0.9/kangtools.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)      148 2023-06-26 16:58:09.000000 kangtools-0.0.9/kangtools.egg-info/entry_points.txt
+-rw-r--r--   0 kang       (501) staff       (20)       10 2023-06-26 16:58:09.000000 kangtools-0.0.9/kangtools.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-26 16:58:09.611546 kangtools-0.0.9/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      860 2023-06-26 16:58:09.000000 kangtools-0.0.9/setup.py
```

### Comparing `kangtools-0.0.8/PKG-INFO` & `kangtools-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kangtools
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package for version control.
 Author: xiaowen kang
 Author-email: kangxiaowen@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 
 # kangtools
```

### Comparing `kangtools-0.0.8/README.md` & `kangtools-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kangtools-0.0.8/kangtools/commit_version_to_git.py` & `kangtools-0.0.9/kangtools/commit_version_to_git.py`

 * *Files identical despite different names*

### Comparing `kangtools-0.0.8/kangtools/version_control.py` & `kangtools-0.0.9/kangtools/version_control.py`

 * *Files identical despite different names*

### Comparing `kangtools-0.0.8/kangtools.egg-info/PKG-INFO` & `kangtools-0.0.9/kangtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kangtools
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package for version control.
 Author: xiaowen kang
 Author-email: kangxiaowen@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 
 # kangtools
```

### Comparing `kangtools-0.0.8/setup.py` & `kangtools-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='kangtools',  # 包的名字
-    version='0.0.8',  # 包的版本
+    version='0.0.9',  # 包的版本
     author='xiaowen kang',  # 你的名字
     author_email='kangxiaowen@gmail.com',  # 你的邮箱
     packages=['kangtools'],  # 包含的包，这是一个列表，如果你的项目包含多个包，都需要列在这里
     license='LICENSE',  # 许可证文件
     description='A Python package for version control.',  # 包的简短描述
     long_description=open('README.md').read(),  # 包的详细描述，通常从 README.md 文件读取
     long_description_content_type="text/markdown",  # 描述的格式，使用markdown格式
```

