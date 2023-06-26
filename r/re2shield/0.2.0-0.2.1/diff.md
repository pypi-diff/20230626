# Comparing `tmp/re2shield-0.2.0.tar.gz` & `tmp/re2shield-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re2shield-0.2.0.tar", last modified: Fri Jun 23 05:39:28 2023, max compression
+gzip compressed data, was "re2shield-0.2.1.tar", last modified: Mon Jun 26 02:28:17 2023, max compression
```

## Comparing `re2shield-0.2.0.tar` & `re2shield-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:39:28.187744 re2shield-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     4957 2023-06-23 05:39:28.186744 re2shield-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3723 2023-06-23 05:39:22.000000 re2shield-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:39:28.186744 re2shield-0.2.0/re2shield/
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 07:41:51.000000 re2shield-0.2.0/re2shield/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2594 2023-06-23 05:39:11.000000 re2shield-0.2.0/re2shield/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:39:28.186744 re2shield-0.2.0/re2shield.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4957 2023-06-23 05:39:28.000000 re2shield-0.2.0/re2shield.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      259 2023-06-23 05:39:28.000000 re2shield-0.2.0/re2shield.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 05:39:28.000000 re2shield-0.2.0/re2shield.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-23 05:39:28.000000 re2shield-0.2.0/re2shield.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-23 05:39:28.000000 re2shield-0.2.0/re2shield.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 05:39:28.187744 re2shield-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      859 2023-06-23 05:39:25.000000 re2shield-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:39:28.186744 re2shield-0.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 07:41:51.000000 re2shield-0.2.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-23 04:23:35.000000 re2shield-0.2.0/tests/test_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:28:17.228328 re2shield-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-06-26 02:28:17.228328 re2shield-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3816 2023-06-26 02:27:34.000000 re2shield-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:28:17.227327 re2shield-0.2.1/re2shield/
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 07:41:51.000000 re2shield-0.2.1/re2shield/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2023-06-26 02:06:04.000000 re2shield-0.2.1/re2shield/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:28:17.227327 re2shield-0.2.1/re2shield.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-06-26 02:28:17.000000 re2shield-0.2.1/re2shield.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      259 2023-06-26 02:28:17.000000 re2shield-0.2.1/re2shield.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 02:28:17.000000 re2shield-0.2.1/re2shield.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-26 02:28:17.000000 re2shield-0.2.1/re2shield.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-26 02:28:17.000000 re2shield-0.2.1/re2shield.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 02:28:17.228328 re2shield-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      859 2023-06-26 01:03:47.000000 re2shield-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:28:17.228328 re2shield-0.2.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 07:41:51.000000 re2shield-0.2.1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      800 2023-06-26 02:17:23.000000 re2shield-0.2.1/tests/test_core.py
```

### Comparing `re2shield-0.2.0/PKG-INFO` & `re2shield-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re2shield
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.
 Home-page: https://github.com/Npc-coder/re2shield
 Author: mkCha
 Author-email: dxsaq0@gmail.com
 License: UNKNOWN
 Description: # re2shield
         `re2shield` is a Python library that provides a shield for working with regular expressions using the `re2` module. 
@@ -36,49 +36,49 @@
         ```shell
         git clone https://github.com/Npc-coder/re2shield.git
         cd re2shield
         pip install .
         ```
         
         ## Updates
-        ### Version 0.2.0
+        ### Version 0.2.1
         - Bug Fix
-            - Fixed a bug where pattern compile were not being overwrite.
+            - Removed flag
+        - Added type and date fields to the Re2Shield class for additional metadata.
+        - Updated dump and load functions to include the new type and date fields when saving and loading the compiled patterns.
+        - Enhanced the __str__ method of the Re2Shield class to include the new fields in the output.
         
         Please refer to the [Usage](#usage) section for examples of how to use these new features.
         
         ## Usage
         ### Importing the Library
         Here is a simple example demonstrating how to use re2shield:
         
         ```python
         import re2shield
         
         if __name__ == "__main__":
-            db = re2shield.Database()
-            print(db)
+            db = re2shield.Database(version='1.0.0')
             # Load patterns from file
             try:
                 db = re2shield.load('patterns.db')
-                print(db)  # Prints the number of patterns in the database
             except FileNotFoundError:
                 # If pattern file doesn't exist, compile the patterns
                 patterns = [
                     (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1),
                     (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2),
                     (r'\d+', 3)
                 ]
         
                 expressions, ids = zip(*patterns)
                 db.compile(expressions=expressions, ids=ids, overwrite=False)
-                print(db)  # Prints the number of patterns in the database and version
                 db.dump('patterns.db')
         
             # Find patterns in text
-            def match_handler(id, from_, to, flags, context):
+            def match_handler(id, from_, to, context):
                 print(f"Match found for pattern {id} from {from_} to {to}: {context}")
         
             db.scan('test@ex12ample12.com', match_handler)
         ```
         In this example, we create a re2shield.Database object, compile a list of patterns with their corresponding identifiers, and then search for those patterns in the provided text. 
         
         The match_handler function is called for each match found, allowing you to process the matches as desired.
```

### Comparing `re2shield-0.2.0/README.md` & `re2shield-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -28,49 +28,49 @@
 ```shell
 git clone https://github.com/Npc-coder/re2shield.git
 cd re2shield
 pip install .
 ```
 
 ## Updates
-### Version 0.2.0
+### Version 0.2.1
 - Bug Fix
-    - Fixed a bug where pattern compile were not being overwrite.
+    - Removed flag
+- Added type and date fields to the Re2Shield class for additional metadata.
+- Updated dump and load functions to include the new type and date fields when saving and loading the compiled patterns.
+- Enhanced the __str__ method of the Re2Shield class to include the new fields in the output.
 
 Please refer to the [Usage](#usage) section for examples of how to use these new features.
 
 ## Usage
 ### Importing the Library
 Here is a simple example demonstrating how to use re2shield:
 
 ```python
 import re2shield
 
 if __name__ == "__main__":
-    db = re2shield.Database()
-    print(db)
+    db = re2shield.Database(version='1.0.0')
     # Load patterns from file
     try:
         db = re2shield.load('patterns.db')
-        print(db)  # Prints the number of patterns in the database
     except FileNotFoundError:
         # If pattern file doesn't exist, compile the patterns
         patterns = [
             (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1),
             (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2),
             (r'\d+', 3)
         ]
 
         expressions, ids = zip(*patterns)
         db.compile(expressions=expressions, ids=ids, overwrite=False)
-        print(db)  # Prints the number of patterns in the database and version
         db.dump('patterns.db')
 
     # Find patterns in text
-    def match_handler(id, from_, to, flags, context):
+    def match_handler(id, from_, to, context):
         print(f"Match found for pattern {id} from {from_} to {to}: {context}")
 
     db.scan('test@ex12ample12.com', match_handler)
 ```
 In this example, we create a re2shield.Database object, compile a list of patterns with their corresponding identifiers, and then search for those patterns in the provided text. 
 
 The match_handler function is called for each match found, allowing you to process the matches as desired.
```

### Comparing `re2shield-0.2.0/re2shield/core.py` & `re2shield-0.2.1/re2shield/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,27 +6,31 @@
         self.re2_patterns = re2_patterns
         self.raw_patterns = raw_patterns
 
     def findall(self, text, callback):
         for id, pattern in self.re2_patterns.items():
             matches = pattern.finditer(text)
             for match in matches:
-                callback(id, match.start(), match.end(), None, match.group())
+                callback(id, match.start(), match.end(), match.group())
 
     def count_patterns(self):
         return len(self.re2_patterns)
 
 class Re2Shield:
-    def __init__(self, version=None, pattern_counts=0):
+    def __init__(self, version=None, type=None, date=None, pattern_counts=0):
         self.db = None
         self.version = version
         self.pattern_counts = pattern_counts
+        self.type = type
+        self.date = date
 
     def __str__(self):
         message = {
+            "type": self.type,
+            "date": self.date,
             "version": self.version,
             "pattern_counts": self.pattern_counts
         }
         return str(message)
 
     def compile(self, expressions, ids, overwrite=False):
         if len(expressions) != len(ids):
@@ -47,26 +51,26 @@
         self.db = Re2ShieldDatabase(re2_patterns, raw_patterns)
         self.pattern_counts = self.db.count_patterns()  # Update pattern_counts after compiling
 
 
     def dump(self, file_path):
         if self.db is not None:
             with open(file_path, 'wb') as f:
-                pickle.dump((self.version, self.db.raw_patterns, self.db.count_patterns()), f)
+                pickle.dump((self.type, self.date, self.version, self.db.raw_patterns, self.db.count_patterns()), f)
         else:
             raise ValueError("No compiled database found. Please compile patterns first.")
 
     def scan(self, text, callback):
         if self.db is not None:
             self.db.findall(text, callback)
         else:
             raise ValueError("No compiled database found. Please compile patterns first.")
 
 Database = Re2Shield
 
 def load(file_path):
     with open(file_path, 'rb') as f:
-        version, raw_patterns, pattern_counts = pickle.load(f)
+        type, date, version, raw_patterns, pattern_counts = pickle.load(f)
         re2_patterns = {id: re2.compile(expr) for id, expr in raw_patterns.items()}
-    re2_shield = Re2Shield(version=version, pattern_counts=pattern_counts)
+    re2_shield = Re2Shield(type=type, date=date, version=version, pattern_counts=pattern_counts)
     re2_shield.db = Re2ShieldDatabase(re2_patterns, raw_patterns)
     return re2_shield
```

### Comparing `re2shield-0.2.0/re2shield.egg-info/PKG-INFO` & `re2shield-0.2.1/re2shield.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re2shield
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.
 Home-page: https://github.com/Npc-coder/re2shield
 Author: mkCha
 Author-email: dxsaq0@gmail.com
 License: UNKNOWN
 Description: # re2shield
         `re2shield` is a Python library that provides a shield for working with regular expressions using the `re2` module. 
@@ -36,49 +36,49 @@
         ```shell
         git clone https://github.com/Npc-coder/re2shield.git
         cd re2shield
         pip install .
         ```
         
         ## Updates
-        ### Version 0.2.0
+        ### Version 0.2.1
         - Bug Fix
-            - Fixed a bug where pattern compile were not being overwrite.
+            - Removed flag
+        - Added type and date fields to the Re2Shield class for additional metadata.
+        - Updated dump and load functions to include the new type and date fields when saving and loading the compiled patterns.
+        - Enhanced the __str__ method of the Re2Shield class to include the new fields in the output.
         
         Please refer to the [Usage](#usage) section for examples of how to use these new features.
         
         ## Usage
         ### Importing the Library
         Here is a simple example demonstrating how to use re2shield:
         
         ```python
         import re2shield
         
         if __name__ == "__main__":
-            db = re2shield.Database()
-            print(db)
+            db = re2shield.Database(version='1.0.0')
             # Load patterns from file
             try:
                 db = re2shield.load('patterns.db')
-                print(db)  # Prints the number of patterns in the database
             except FileNotFoundError:
                 # If pattern file doesn't exist, compile the patterns
                 patterns = [
                     (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1),
                     (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2),
                     (r'\d+', 3)
                 ]
         
                 expressions, ids = zip(*patterns)
                 db.compile(expressions=expressions, ids=ids, overwrite=False)
-                print(db)  # Prints the number of patterns in the database and version
                 db.dump('patterns.db')
         
             # Find patterns in text
-            def match_handler(id, from_, to, flags, context):
+            def match_handler(id, from_, to, context):
                 print(f"Match found for pattern {id} from {from_} to {to}: {context}")
         
             db.scan('test@ex12ample12.com', match_handler)
         ```
         In this example, we create a re2shield.Database object, compile a list of patterns with their corresponding identifiers, and then search for those patterns in the provided text. 
         
         The match_handler function is called for each match found, allowing you to process the matches as desired.
```

### Comparing `re2shield-0.2.0/setup.py` & `re2shield-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='re2shield',
-    version='0.2.0',
+    version='0.2.1',
     url='https://github.com/Npc-coder/re2shield',  # Replace with your own GitHub project URL
     author='mkCha',
     author_email='dxsaq0@gmail.com',
     description='A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `re2shield-0.2.0/tests/test_core.py` & `re2shield-0.2.1/tests/test_core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 import re2shield
 
 if __name__ == "__main__":
     db = re2shield.Database(version='1.0.0')
-    print(db)
     # Load patterns from file
     try:
         db = re2shield.load('patterns.db')
-        print(db)  # Prints the number of patterns in the database
     except FileNotFoundError:
         # If pattern file doesn't exist, compile the patterns
         patterns = [
             (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1),
             (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2),
             (r'\d+', 3)
         ]
 
         expressions, ids = zip(*patterns)
         db.compile(expressions=expressions, ids=ids, overwrite=False)
-        print(db)  # Prints the number of patterns in the database and version
         db.dump('patterns.db')
 
     # Find patterns in text
-    def match_handler(id, from_, to, flags, context):
+    def match_handler(id, from_, to, context):
         print(f"Match found for pattern {id} from {from_} to {to}: {context}")
 
     db.scan('test@ex12ample12.com', match_handler)
-    print(db.version)
-    print(db.pattern_counts)
```

