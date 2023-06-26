# Comparing `tmp/pillar1-0.1.9.8.tar.gz` & `tmp/pillar1-0.1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.9.8.tar", last modified: Mon Jun 26 13:18:44 2023, max compression
+gzip compressed data, was "pillar1-0.1.9.9.tar", last modified: Mon Jun 26 13:54:44 2023, max compression
```

## Comparing `pillar1-0.1.9.8.tar` & `pillar1-0.1.9.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:18:44.485881 pillar1-0.1.9.8/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 13:18:44.485722 pillar1-0.1.9.8/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.9.8/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:18:44.484814 pillar1-0.1.9.8/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.9.8/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     6792 2023-06-26 13:11:05.000000 pillar1-0.1.9.8/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.9.8/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9050 2023-06-26 13:18:39.000000 pillar1-0.1.9.8/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:18:44.485467 pillar1-0.1.9.8/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 13:18:44.000000 pillar1-0.1.9.8/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-26 13:18:44.000000 pillar1-0.1.9.8/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-26 13:18:44.000000 pillar1-0.1.9.8/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-26 13:18:44.000000 pillar1-0.1.9.8/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-26 13:18:44.485926 pillar1-0.1.9.8/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-26 13:18:44.000000 pillar1-0.1.9.8/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:54:44.792126 pillar1-0.1.9.9/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 13:54:44.791985 pillar1-0.1.9.9/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.9.9/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:54:44.790918 pillar1-0.1.9.9/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.9.9/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     6826 2023-06-26 13:54:43.000000 pillar1-0.1.9.9/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.9.9/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9050 2023-06-26 13:18:39.000000 pillar1-0.1.9.9/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:54:44.791767 pillar1-0.1.9.9/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 13:54:44.000000 pillar1-0.1.9.9/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-26 13:54:44.000000 pillar1-0.1.9.9/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-26 13:54:44.000000 pillar1-0.1.9.9/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-26 13:54:44.000000 pillar1-0.1.9.9/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-26 13:54:44.792174 pillar1-0.1.9.9/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-26 13:54:44.000000 pillar1-0.1.9.9/setup.py
```

### Comparing `pillar1-0.1.9.8/PKG-INFO` & `pillar1-0.1.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.9.8
+Version: 0.1.9.9
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.9.8/README.md` & `pillar1-0.1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.9.8/pillar1/constants.py` & `pillar1-0.1.9.9/pillar1/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 STARCODER_BETA = """
 
+Here is the describe of the table
 Given this `claims` table description:
 
 col_name,data_type,comment
 source,string, The insurance company that submitted the claim, only used when insurance provider information is needed. example: FEP, PRIME, BCBS, NASCO, FACETS
 NetworkID,int,
 DiagCode,string, example (S31102, J09, M12021, G5760, S0282XA, S52044, S72141R, S83111)
 DiagDesc,string, various deseases such as diabetes or heart failure, etc will be documented here in sentence form. use this field for questions about diagnosis details and 
@@ -84,10 +85,10 @@
 
 The SQL statement to answer the question  
 
 use DiagDesc for patient condition queries
 
 """
 
-APPEND = " considering every selection where clause criteria without missing any, Columns in the select queries will be given appropriate names, always comparing strings with " \
+APPEND = " Considering every selection where clause criteria without missing any, Columns in the select queries will be given appropriate names, always comparing strings with " \
          "ILIKE (in case insensitive mode),  ILIKE will be used in string where clauses, where conditions which are not asked for explicitly will not be included, " \
          "correctnes is of highest priority, here is the SQL, ```sql"
```

### Comparing `pillar1-0.1.9.8/pillar1/constants_original.py` & `pillar1-0.1.9.9/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.9.8/pillar1/pillar1.py` & `pillar1-0.1.9.9/pillar1/pillar1.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.9.8/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.9.9/pillar1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.9.8
+Version: 0.1.9.9
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.9.8/setup.py` & `pillar1-0.1.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.9.8',
+    version='0.1.9.9',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

