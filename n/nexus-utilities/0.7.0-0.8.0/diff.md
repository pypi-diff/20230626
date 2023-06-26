# Comparing `tmp/nexus-utilities-0.7.0.tar.gz` & `tmp/nexus-utilities-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.7.0.tar", last modified: Thu Jun 15 19:04:21 2023, max compression
+gzip compressed data, was "nexus-utilities-0.8.0.tar", last modified: Mon Jun 26 15:05:12 2023, max compression
```

## Comparing `nexus-utilities-0.7.0.tar` & `nexus-utilities-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:04:21.440708 nexus-utilities-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-15 19:04:21.440708 nexus-utilities-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:04:21.436708 nexus-utilities-0.7.0/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-15 19:04:21.000000 nexus-utilities-0.7.0/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-15 19:04:21.000000 nexus-utilities-0.7.0/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:04:21.000000 nexus-utilities-0.7.0/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-15 19:04:21.000000 nexus-utilities-0.7.0/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 19:04:21.000000 nexus-utilities-0.7.0/nexus_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:04:21.440708 nexus-utilities-0.7.0/nexus_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/flatfile_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/password_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:04:21.440708 nexus-utilities-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:05:12.174871 nexus-utilities-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-26 15:04:58.000000 nexus-utilities-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-26 15:05:12.174871 nexus-utilities-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33423 2023-06-26 15:04:58.000000 nexus-utilities-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:05:12.170871 nexus-utilities-0.8.0/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-26 15:05:11.000000 nexus-utilities-0.8.0/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-26 15:05:12.000000 nexus-utilities-0.8.0/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:05:11.000000 nexus-utilities-0.8.0/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 15:05:11.000000 nexus-utilities-0.8.0/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 15:05:11.000000 nexus-utilities-0.8.0/nexus_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:05:12.174871 nexus-utilities-0.8.0/nexus_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 15:04:58.000000 nexus-utilities-0.8.0/nexus_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-26 15:04:58.000000 nexus-utilities-0.8.0/nexus_utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-26 15:04:58.000000 nexus-utilities-0.8.0/nexus_utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-26 15:04:58.000000 nexus-utilities-0.8.0/nexus_utils/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30037 2023-06-26 15:04:58.000000 nexus-utilities-0.8.0/nexus_utils/email_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-06-26 15:04:58.000000 nexus-utilities-0.8.0/nexus_utils/flatfile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-26 15:04:58.000000 nexus-utilities-0.8.0/nexus_utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-26 15:04:58.000000 nexus-utilities-0.8.0/nexus_utils/password_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-26 15:04:58.000000 nexus-utilities-0.8.0/nexus_utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:05:12.174871 nexus-utilities-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-26 15:04:58.000000 nexus-utilities-0.8.0/setup.py
```

### Comparing `nexus-utilities-0.7.0/LICENSE.txt` & `nexus-utilities-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.7.0/PKG-INFO` & `nexus-utilities-0.8.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.7.0
+Version: 0.8.0
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.7.0/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.8.0/nexus_utilities.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.7.0
+Version: 0.8.0
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.7.0/nexus_utils/datetime_utils.py` & `nexus-utilities-0.8.0/nexus_utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.7.0/nexus_utils/flatfile_utils.py` & `nexus-utilities-0.8.0/nexus_utils/flatfile_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """Flatfile-related utilities"""
+#%%
+import os
 import chardet
 import pandas as pd
 from openpyxl import Workbook
 import gzip
 
+#%%
+
 def detect_encoding(file_path):
     """Attempt to determine the encoding of a file located at the provided file path"""
     # Check if the file path ends with '.gz' to identify gzipped files
     if file_path.endswith('.gz'):
         # Open the gzipped file in binary mode
         with gzip.open(file_path, 'rb') as f:
             # Read the first 2000 rows
@@ -35,14 +39,60 @@
 
         # Determine the encoding of the entire file
         result = chardet.detect(content)
         encoding = result['encoding']
 
     return encoding
 
+def extract_file_extension(filename, last_only=False):
+    extension_found = False
+    extension = ''
+    exclusions = ['.data','.script','.file','.image']
+    if os.path.isabs(filename) or os.path.sep in filename:
+        filename = os.path.basename(filename)
+    
+    if '.' not in filename:
+        return 'Invalid filename'#, extension_found
+    
+    if last_only:
+        extension = os.path.splitext(filename)[1]
+        extension_found = True
+        return extension#, extension_found
+    
+    parts = filename.split('.')
+    
+    if len(parts) == 2 and (len(parts[0]) == 0 or len(parts[1]) == 0):
+        return 'No Extension'#, extension_found
+    
+    working_dir = os.path.dirname(os.path.abspath(__file__))
+    file_path = os.path.join(working_dir, 'references', 'known_file_extensions.txt')
+
+    with open(file_path, 'r') as file:
+        # extensions = [ext[1:] if ext.startswith('.') else ext for ext in file.read().splitlines()]
+        extensions = [ext[1:] if ext.startswith('.') else ext for ext in file.read().splitlines() if ext not in exclusions]
+
+    match_string = None
+    
+    for part in parts[1:]:
+        if part in extensions:
+            match_string = part
+            break
+
+    if match_string is None:
+        return 'Unknown Extension'#, extension_found
+    
+    match_index = filename.find('.' + match_string)
+    extension = filename[match_index:]
+
+    if extension:
+        extension_found = True
+        return extension#, extension_found
+    else:
+        return 'Unknown Extension'#, extension_found
+
 def analyze_dataframe(df):
     """Analyze distinct values in a dataframe"""
     analysis_dict = {}
 
     for col in df.columns:
         column_dict = {}
 
@@ -188,8 +238,48 @@
             print(df.columns.to_list())
             sample_null_rows.fillna("<NULL>", inplace=True)
             for _, row in sample_null_rows.iterrows():
                 print(row.values.tolist())
     
     sample_issue_rows = pd.concat([sample_duplicate_rows, sample_null_rows], ignore_index=True)
     
-    return is_unique, no_nulls, sample_issue_rows
+    return is_unique, no_nulls, sample_issue_rows
+
+#%%
+
+if __name__ == '__main__':
+    # filename = 'Testfile.txt.gz'
+    # print(f'{filename}\n{extract_file_extension(filename)}\n\n')
+
+    # filename = 'Test.file.txt.gz'
+    # print(f'{filename}\n{extract_file_extension(filename)}\n\n')
+
+    filename = 'my.data.csv.gz'
+    print(f'{filename}\n{extract_file_extension(filename)}\n\n')
+
+    filename = 'my.report.docx.template'
+    print(f'{filename}\n{extract_file_extension(filename)}\n\n')
+
+    filename = 'my.archive.tar.gz'
+    print(f'{filename}\n{extract_file_extension(filename)}\n\n')
+
+    filename = 'my.image.jpg.thumbnail'
+    print(f'{filename}\n{extract_file_extension(filename)}\n\n')
+
+    filename = 'my.script.py.txt'
+    print(f'{filename}\n{extract_file_extension(filename, True)}\n\n')
+
+    # filename = 'My.test.file.backup.txt.gz'
+    # print(f'{filename}\n{extract_file_extension(filename)}\n\n')
+
+    # filename = r'C:\test_folder\My.test.file.backup.txt.gz'
+    # print(f'{filename}\n{extract_file_extension(filename)}\n\n')
+
+    # filename = r'C:\test_folder'
+    # print(f'{filename}\n{extract_file_extension(filename)}\n\n')
+
+    # filename = 'C:\\test_folder\\My.test.file.backup.txt.gz'
+    # print(f'{filename}\n{extract_file_extension(filename)}\n\n')
+
+    pass
+
+    #%%
```

### Comparing `nexus-utilities-0.7.0/nexus_utils/package_utils.py` & `nexus-utilities-0.8.0/nexus_utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.7.0/nexus_utils/password_utils.py` & `nexus-utilities-0.8.0/nexus_utils/password_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.7.0/nexus_utils/string_utils.py` & `nexus-utilities-0.8.0/nexus_utils/string_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,22 +25,23 @@
 
 def cleanse_string(
     string, 
     remove_symbols=True, 
     title_to_snake_case=False, 
     hyphen_to_underscore=True, 
     period_to_underscore=True, 
+    space_to_underscore=True, 
     to_upper=False, 
     to_lower=True
 ):
     """Cleanse strings with a number of parameters"""
 
     if isinstance(string, str):
         if remove_symbols:
-            characters_to_replace_with_underscore = [' ',':',';','&','@','^','+','=','~','/','\\','|','(','{','[','<']
+            characters_to_replace_with_underscore = [':',';','&','@','^','+','=','~','/','\\','|','(','{','[','<']
             characters_to_remove = [',','`','#','$','%','*','\'','"','?','!',')','}',']','>']
             
             string = string.replace('_', '†')
 
             for char in characters_to_replace_with_underscore:
                 string = string.replace(char, '_')
             string = string.replace('__', '_')
@@ -56,14 +57,17 @@
             string = re.sub(r'(?<=[a-z0-9])([A-Z])|(?<=[^_])([A-Z](?=[a-z]))', r'_\1\2', string)
 
         if hyphen_to_underscore:
             string = string.replace('-', '_')
 
         if period_to_underscore:
             string = string.replace('.', '_')
+
+        if space_to_underscore:
+            string = string.replace(' ', '_')
         
         if to_upper:
             string = string.upper()
         
         if to_lower:
             string = string.lower()
```

### Comparing `nexus-utilities-0.7.0/setup.py` & `nexus-utilities-0.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-utilities',
-    version='0.7.0',
+    version='0.8.0',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
     url='https://github.com/james-larsen/nexus-utilities',
     packages=['nexus_utils'],
```

