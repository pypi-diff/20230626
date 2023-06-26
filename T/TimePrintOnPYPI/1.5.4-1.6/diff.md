# Comparing `tmp/TimePrintOnPYPI-1.5.4.tar.gz` & `tmp/TimePrintOnPYPI-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimePrintOnPYPI-1.5.4.tar", last modified: Sat May 27 10:28:24 2023, max compression
+gzip compressed data, was "TimePrintOnPYPI-1.6.tar", last modified: Mon Jun 26 21:00:35 2023, max compression
```

## Comparing `TimePrintOnPYPI-1.5.4.tar` & `TimePrintOnPYPI-1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 10:28:24.714994 TimePrintOnPYPI-1.5.4/
--rw-rw-rw-   0        0        0     4611 2023-05-27 10:28:24.713008 TimePrintOnPYPI-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     4121 2023-05-27 10:28:11.000000 TimePrintOnPYPI-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 10:28:24.689337 TimePrintOnPYPI-1.5.4/TimePrint/
--rw-rw-rw-   0        0        0     1820 2023-05-27 10:28:01.000000 TimePrintOnPYPI-1.5.4/TimePrint/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 10:28:24.708998 TimePrintOnPYPI-1.5.4/TimePrintOnPYPI.egg-info/
--rw-rw-rw-   0        0        0     4611 2023-05-27 10:28:24.000000 TimePrintOnPYPI-1.5.4/TimePrintOnPYPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-05-27 10:28:24.000000 TimePrintOnPYPI-1.5.4/TimePrintOnPYPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 10:28:24.000000 TimePrintOnPYPI-1.5.4/TimePrintOnPYPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-27 10:28:24.000000 TimePrintOnPYPI-1.5.4/TimePrintOnPYPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 10:28:24.715990 TimePrintOnPYPI-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1013 2023-05-27 10:28:06.000000 TimePrintOnPYPI-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 21:00:35.700509 TimePrintOnPYPI-1.6/
+-rw-rw-rw-   0        0        0     8029 2023-06-26 21:00:35.699508 TimePrintOnPYPI-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7541 2023-06-26 20:48:44.000000 TimePrintOnPYPI-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 21:00:35.671169 TimePrintOnPYPI-1.6/TimePrint/
+-rw-rw-rw-   0        0        0     2599 2023-06-26 21:00:15.000000 TimePrintOnPYPI-1.6/TimePrint/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 21:00:35.696987 TimePrintOnPYPI-1.6/TimePrintOnPYPI.egg-info/
+-rw-rw-rw-   0        0        0     8029 2023-06-26 21:00:35.000000 TimePrintOnPYPI-1.6/TimePrintOnPYPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-06-26 21:00:35.000000 TimePrintOnPYPI-1.6/TimePrintOnPYPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 21:00:35.000000 TimePrintOnPYPI-1.6/TimePrintOnPYPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 21:00:35.000000 TimePrintOnPYPI-1.6/TimePrintOnPYPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 21:00:35.700509 TimePrintOnPYPI-1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1011 2023-06-26 21:00:07.000000 TimePrintOnPYPI-1.6/setup.py
```

### Comparing `TimePrintOnPYPI-1.5.4/setup.py` & `TimePrintOnPYPI-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         print("Need Help ? Contact Me From e-mail: osmntn08@gmail.com")
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='TimePrintOnPYPI',
-    version='1.5.4',
+    version='1.6',
     description='A package for printing text with time delay between characters',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/SForces/TimePrint',
     author='Osman TUNA',
     author_email='osmntn08@gmail.com',
     license='MIT',
```

