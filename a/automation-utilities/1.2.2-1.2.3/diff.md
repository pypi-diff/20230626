# Comparing `tmp/automation-utilities-1.2.2.tar.gz` & `tmp/automation-utilities-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-utilities-1.2.2.tar", last modified: Sun Jun 25 18:47:09 2023, max compression
+gzip compressed data, was "automation-utilities-1.2.3.tar", last modified: Mon Jun 26 15:19:27 2023, max compression
```

## Comparing `automation-utilities-1.2.2.tar` & `automation-utilities-1.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 18:47:09.682307 automation-utilities-1.2.2/
-drwxrwxrwx   0        0        0        0 2023-06-25 18:47:09.679309 automation-utilities-1.2.2/Automation_Utilities.egg-info/
--rw-rw-rw-   0        0        0      134 2023-06-25 18:47:09.000000 automation-utilities-1.2.2/Automation_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-06-25 18:47:09.000000 automation-utilities-1.2.2/Automation_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 18:47:09.000000 automation-utilities-1.2.2/Automation_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-25 18:47:09.000000 automation-utilities-1.2.2/Automation_Utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-06-25 18:47:09.681307 automation-utilities-1.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-25 18:47:09.679309 automation-utilities-1.2.2/automation_utilities/
--rw-rw-rw-   0        0        0     1053 2023-06-25 18:46:54.000000 automation-utilities-1.2.2/automation_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-25 18:47:09.682307 automation-utilities-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      248 2023-06-25 18:47:04.000000 automation-utilities-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:19:27.490241 automation-utilities-1.2.3/
+drwxrwxrwx   0        0        0        0 2023-06-26 15:19:27.477106 automation-utilities-1.2.3/Automation_Utilities.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-06-26 15:19:27.000000 automation-utilities-1.2.3/Automation_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-06-26 15:19:27.000000 automation-utilities-1.2.3/Automation_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 15:19:27.000000 automation-utilities-1.2.3/Automation_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-26 15:19:27.000000 automation-utilities-1.2.3/Automation_Utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-06-26 15:19:27.489151 automation-utilities-1.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 15:19:27.487106 automation-utilities-1.2.3/automation_utilities/
+-rw-rw-rw-   0        0        0     1366 2023-06-26 15:16:21.000000 automation-utilities-1.2.3/automation_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 15:19:27.490241 automation-utilities-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      248 2023-06-26 15:16:53.000000 automation-utilities-1.2.3/setup.py
```

### Comparing `automation-utilities-1.2.2/automation_utilities/__init__.py` & `automation-utilities-1.2.3/automation_utilities/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,24 +20,36 @@
             Data.lock.release()
             return self.data[key] - 1
         else:
             return self.data[key]
 
 
 class Files:
-
     lock = threading.Lock()
 
+    def __init__(self):
+        pass
+
     @staticmethod
     def add(text: str, to: str) -> None:
         Files.lock.acquire()
         open(to, 'a').write(text)
         Files.lock.release()
 
+    @staticmethod
+    def load(*file_names: str):
+        lists = []
+        for file_name in file_names:
+            lists.append(open(file_name, 'r').read().split('\n'))
+        return lists if len(lists) > 1 else lists[0]
+
 
 class Input:
+    def __init__(self):
+        pass
+
     @staticmethod
     def int_input(prompt: str, default: int) -> int:
         try:
             return int(input(prompt))
         except ValueError:
             return default
```

