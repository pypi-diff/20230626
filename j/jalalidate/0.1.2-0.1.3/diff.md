# Comparing `tmp/jalalidate-0.1.2.tar.gz` & `tmp/jalalidate-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jalalidate-0.1.2.tar", last modified: Sun Feb 27 11:10:53 2022, max compression
+gzip compressed data, was "jalalidate-0.1.3.tar", last modified: Mon Jun 26 06:26:14 2023, max compression
```

## Comparing `jalalidate-0.1.2.tar` & `jalalidate-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,7 @@
-drwxr-xr-x   0 j.jahedi   (501) staff       (20)        0 2022-02-27 11:10:53.975909 jalalidate-0.1.2/
--rw-r--r--   0 j.jahedi   (501) staff       (20)     1065 2022-02-27 10:26:30.000000 jalalidate-0.1.2/LICENSE.txt
--rw-r--r--   0 j.jahedi   (501) staff       (20)      448 2022-02-27 11:10:53.975963 jalalidate-0.1.2/PKG-INFO
--rw-r--r--   0 j.jahedi   (501) staff       (20)       14 2022-02-27 10:26:30.000000 jalalidate-0.1.2/README.md
-drwxr-xr-x   0 j.jahedi   (501) staff       (20)        0 2022-02-27 11:10:53.975391 jalalidate-0.1.2/jalalidate/
--rw-r--r--   0 j.jahedi   (501) staff       (20)        0 2022-02-27 09:14:18.000000 jalalidate-0.1.2/jalalidate/__init__.py
--rw-r--r--   0 j.jahedi   (501) staff       (20)     3880 2022-02-27 11:06:28.000000 jalalidate-0.1.2/jalalidate/jalali.py
-drwxr-xr-x   0 j.jahedi   (501) staff       (20)        0 2022-02-27 11:10:53.975819 jalalidate-0.1.2/jalalidate.egg-info/
--rw-r--r--   0 j.jahedi   (501) staff       (20)      448 2022-02-27 11:10:53.000000 jalalidate-0.1.2/jalalidate.egg-info/PKG-INFO
--rw-r--r--   0 j.jahedi   (501) staff       (20)      220 2022-02-27 11:10:53.000000 jalalidate-0.1.2/jalalidate.egg-info/SOURCES.txt
--rw-r--r--   0 j.jahedi   (501) staff       (20)        1 2022-02-27 11:10:53.000000 jalalidate-0.1.2/jalalidate.egg-info/dependency_links.txt
--rw-r--r--   0 j.jahedi   (501) staff       (20)       11 2022-02-27 11:10:53.000000 jalalidate-0.1.2/jalalidate.egg-info/top_level.txt
--rw-r--r--   0 j.jahedi   (501) staff       (20)       79 2022-02-27 11:10:53.976180 jalalidate-0.1.2/setup.cfg
--rw-r--r--   0 j.jahedi   (501) staff       (20)      630 2022-02-27 11:10:27.000000 jalalidate-0.1.2/setup.py
+drwxr-xr-x   0 j.jahedi   (501) staff       (20)        0 2023-06-26 06:26:14.373360 jalalidate-0.1.3/
+-rw-r--r--   0 j.jahedi   (501) staff       (20)      433 2023-06-26 06:26:14.373421 jalalidate-0.1.3/PKG-INFO
+drwxr-xr-x   0 j.jahedi   (501) staff       (20)        0 2023-06-26 06:26:14.373332 jalalidate-0.1.3/jalalidate/
+-rw-r--r--   0 j.jahedi   (501) staff       (20)        0 2022-02-27 09:14:18.522000 jalalidate-0.1.3/jalalidate/__init__.py
+-rw-r--r--   0 j.jahedi   (501) staff       (20)     4008 2023-06-26 06:22:29.018508 jalalidate-0.1.3/jalalidate/jalali.py
+-rw-r--r--   0 j.jahedi   (501) staff       (20)       61 2022-02-27 10:26:30.821000 jalalidate-0.1.3/setup.cfg
+-rw-r--r--   0 j.jahedi   (501) staff       (20)      630 2023-06-26 06:22:08.738575 jalalidate-0.1.3/setup.py
```

### Comparing `jalalidate-0.1.2/jalalidate/jalali.py` & `jalalidate-0.1.3/jalalidate/jalali.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,18 @@
 
 class Date(g_date):
     def __init__(self,year,month,day) -> None:
         super().__init__()
         self.__gregorian_days_in_month = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
         self.__jalali_days_in_month = [31, 31, 31, 31, 31, 31, 30, 30, 30, 30, 30, 29]
 
+    @staticmethod
+    def datetime_convert(datetime):
+        return Date(datetime.year, datetime.month, datetime.day)
+        
     def gregorian_to_jalali(self):
         year = self.year - 1600
         month = self.month - 1
         day = self.day - 1
 
         gregorian_day_no = 365 * year + (year + 3) // 4 - (year + 99) // 100 + (year + 399) // 400
```

### Comparing `jalalidate-0.1.2/setup.py` & `jalalidate-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'jalalidate',
   packages = ['jalalidate'],
-  version = '0.1.2',
+  version = '0.1.3',
   license='MIT',
   description = 'change date between gregorian and jalali date',
   author = 'Javad Jahedi',
   author_email = 'javad.jahedi@gmail.com',
   url = 'https://github.com/j-jahedi/jalali-date',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/j-jahedi/jalali-date/archive/refs/heads/master.zip',    # I explain this later on
   keywords = ['Jalali', 'Jalali-date'],
```

