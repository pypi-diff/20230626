# Comparing `tmp/aws-s3-cli-0.0.1.tar.gz` & `tmp/aws-s3-cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-s3-cli-0.0.1.tar", last modified: Sun Jun 25 14:05:26 2023, max compression
+gzip compressed data, was "aws-s3-cli-0.0.2.tar", last modified: Mon Jun 26 16:01:22 2023, max compression
```

## Comparing `aws-s3-cli-0.0.1.tar` & `aws-s3-cli-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-25 14:05:26.555716 aws-s3-cli-0.0.1/
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     1069 2023-06-24 20:57:06.000000 aws-s3-cli-0.0.1/LICENSE
--rw-rw-r--   0 sujit     (1000) sujit     (1000)       26 2023-05-02 17:40:08.000000 aws-s3-cli-0.0.1/MANIFEST.in
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     2278 2023-06-25 14:05:26.555716 aws-s3-cli-0.0.1/PKG-INFO
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     1487 2023-06-24 21:20:07.000000 aws-s3-cli-0.0.1/README.md
-drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-25 14:05:26.551718 aws-s3-cli-0.0.1/aws_s3_cli/
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     4693 2023-06-24 21:16:55.000000 aws-s3-cli-0.0.1/aws_s3_cli/aws_s3_cli.py
-drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-25 14:05:26.555716 aws-s3-cli-0.0.1/aws_s3_cli.egg-info/
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     2278 2023-06-25 14:05:26.000000 aws-s3-cli-0.0.1/aws_s3_cli.egg-info/PKG-INFO
--rw-rw-r--   0 sujit     (1000) sujit     (1000)      199 2023-06-25 14:05:26.000000 aws-s3-cli-0.0.1/aws_s3_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)        1 2023-06-25 14:05:26.000000 aws-s3-cli-0.0.1/aws_s3_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)       11 2023-06-25 14:05:26.000000 aws-s3-cli-0.0.1/aws_s3_cli.egg-info/top_level.txt
--rw-rw-r--   0 sujit     (1000) sujit     (1000)       38 2023-06-25 14:05:26.555716 aws-s3-cli-0.0.1/setup.cfg
--rw-rw-r--   0 sujit     (1000) sujit     (1000)     1116 2023-06-24 21:09:49.000000 aws-s3-cli-0.0.1/setup.py
+drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-26 16:01:22.051408 aws-s3-cli-0.0.2/
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     1069 2023-06-24 20:57:06.000000 aws-s3-cli-0.0.2/LICENSE
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)       26 2023-05-02 17:40:08.000000 aws-s3-cli-0.0.2/MANIFEST.in
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     2799 2023-06-26 16:01:22.051408 aws-s3-cli-0.0.2/PKG-INFO
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     2008 2023-06-26 16:00:06.000000 aws-s3-cli-0.0.2/README.md
+drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-26 16:01:22.051408 aws-s3-cli-0.0.2/aws_s3_cli/
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     4693 2023-06-24 21:16:55.000000 aws-s3-cli-0.0.2/aws_s3_cli/aws_s3_cli.py
+drwxrwxr-x   0 sujit     (1000) sujit     (1000)        0 2023-06-26 16:01:22.051408 aws-s3-cli-0.0.2/aws_s3_cli.egg-info/
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     2799 2023-06-26 16:01:21.000000 aws-s3-cli-0.0.2/aws_s3_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)      232 2023-06-26 16:01:22.000000 aws-s3-cli-0.0.2/aws_s3_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)        1 2023-06-26 16:01:21.000000 aws-s3-cli-0.0.2/aws_s3_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)        6 2023-06-26 16:01:21.000000 aws-s3-cli-0.0.2/aws_s3_cli.egg-info/requires.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)       11 2023-06-26 16:01:21.000000 aws-s3-cli-0.0.2/aws_s3_cli.egg-info/top_level.txt
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)       38 2023-06-26 16:01:22.051408 aws-s3-cli-0.0.2/setup.cfg
+-rw-rw-r--   0 sujit     (1000) sujit     (1000)     1168 2023-06-26 16:00:51.000000 aws-s3-cli-0.0.2/setup.py
```

### Comparing `aws-s3-cli-0.0.1/LICENSE` & `aws-s3-cli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-s3-cli-0.0.1/PKG-INFO` & `aws-s3-cli-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-s3-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: upload, download, check file availability, and get all available list from AWS s3 bucket.
 Home-page: https://github.com/sujitmandal/aws-s3-cli
 Author: Sujit Mandal
 Author-email: mandals974@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
@@ -15,23 +15,34 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aws-s3-cli
+## Scrape Search Engine :
+[![Downloads](https://static.pepy.tech/badge/aws-s3-cli)](https://pepy.tech/project/aws-s3-cli)[![GitHub license](https://img.shields.io/github/license/sujitmandal/aws-s3-cli)](https://github.com/sujitmandal/aws-s3-cli/blob/master/LICENSE) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aws-s3-cli) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/aws-s3-cli) ![PyPI](https://img.shields.io/pypi/v/aws-s3-cli) 
+
+
+
+
 aws s3 bucket cli
+
 upload, download, check file availability, and get all available list from AWS s3 bucket.
 
 
 
+
+
 ## Package Installation  : 
 ```
 pip install aws-s3-cli
 ```
+[Pypi Package Link](https://pypi.org/project/aws-s3-cli/)
+
 
 ## How to import the module:
 ```python
 FILE_OBJ = "" # File object
 FILE_NAME = "" # File name
 S3_FILE_NAME = "" # S3 file name or uploaded file name
 BUCKET_NAME = "" # Bucket name
```

### Comparing `aws-s3-cli-0.0.1/aws_s3_cli/aws_s3_cli.py` & `aws-s3-cli-0.0.2/aws_s3_cli/aws_s3_cli.py`

 * *Files identical despite different names*

### Comparing `aws-s3-cli-0.0.1/aws_s3_cli.egg-info/PKG-INFO` & `aws-s3-cli-0.0.2/aws_s3_cli.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-s3-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: upload, download, check file availability, and get all available list from AWS s3 bucket.
 Home-page: https://github.com/sujitmandal/aws-s3-cli
 Author: Sujit Mandal
 Author-email: mandals974@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
@@ -15,23 +15,34 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aws-s3-cli
+## Scrape Search Engine :
+[![Downloads](https://static.pepy.tech/badge/aws-s3-cli)](https://pepy.tech/project/aws-s3-cli)[![GitHub license](https://img.shields.io/github/license/sujitmandal/aws-s3-cli)](https://github.com/sujitmandal/aws-s3-cli/blob/master/LICENSE) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aws-s3-cli) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/aws-s3-cli) ![PyPI](https://img.shields.io/pypi/v/aws-s3-cli) 
+
+
+
+
 aws s3 bucket cli
+
 upload, download, check file availability, and get all available list from AWS s3 bucket.
 
 
 
+
+
 ## Package Installation  : 
 ```
 pip install aws-s3-cli
 ```
+[Pypi Package Link](https://pypi.org/project/aws-s3-cli/)
+
 
 ## How to import the module:
 ```python
 FILE_OBJ = "" # File object
 FILE_NAME = "" # File name
 S3_FILE_NAME = "" # S3 file name or uploaded file name
 BUCKET_NAME = "" # Bucket name
```

### Comparing `aws-s3-cli-0.0.1/setup.py` & `aws-s3-cli-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open('README.md') as files:
         README = files.read()
 
     return(README)
 
 setup(
     name = 'aws-s3-cli',
-    version = '0.0.1',
+    version = '0.0.2',
     description = "upload, download, check file availability, and get all available list from AWS s3 bucket.",
     long_description = readme(),
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/sujitmandal/aws-s3-cli',
     author = 'Sujit Mandal',
     author_email = 'mandals974@gmail.com',
     license = 'MIT',
@@ -26,10 +26,14 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
 
+    install_requires=[
+        'boto3',
+    ],
+    
     packages = ['aws_s3_cli'],
     include_package_data = True,
 )
```

