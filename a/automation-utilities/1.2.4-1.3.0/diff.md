# Comparing `tmp/automation-utilities-1.2.4.tar.gz` & `tmp/automation-utilities-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-utilities-1.2.4.tar", last modified: Mon Jun 26 15:36:54 2023, max compression
+gzip compressed data, was "automation-utilities-1.3.0.tar", last modified: Mon Jun 26 15:51:24 2023, max compression
```

## Comparing `automation-utilities-1.2.4.tar` & `automation-utilities-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 15:36:54.572846 automation-utilities-1.2.4/
-drwxrwxrwx   0        0        0        0 2023-06-26 15:36:54.566152 automation-utilities-1.2.4/Automation_Utilities.egg-info/
--rw-rw-rw-   0        0        0      134 2023-06-26 15:36:54.000000 automation-utilities-1.2.4/Automation_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-06-26 15:36:54.000000 automation-utilities-1.2.4/Automation_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 15:36:54.000000 automation-utilities-1.2.4/Automation_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-26 15:36:54.000000 automation-utilities-1.2.4/Automation_Utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-06-26 15:36:54.571839 automation-utilities-1.2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 15:36:54.570796 automation-utilities-1.2.4/automation_utilities/
--rw-rw-rw-   0        0        0      646 2023-06-26 15:36:32.000000 automation-utilities-1.2.4/automation_utilities/Data.py
--rw-rw-rw-   0        0        0      497 2023-06-26 15:36:32.000000 automation-utilities-1.2.4/automation_utilities/Files.py
--rw-rw-rw-   0        0        0      237 2023-06-26 15:36:32.000000 automation-utilities-1.2.4/automation_utilities/Input.py
--rw-rw-rw-   0        0        0        0 2023-06-26 15:36:31.000000 automation-utilities-1.2.4/automation_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-26 15:36:54.572846 automation-utilities-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      248 2023-06-26 15:36:52.000000 automation-utilities-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:51:24.431946 automation-utilities-1.3.0/
+drwxrwxrwx   0        0        0        0 2023-06-26 15:51:24.425495 automation-utilities-1.3.0/Automation_Utilities.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-06-26 15:51:24.000000 automation-utilities-1.3.0/Automation_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-06-26 15:51:24.000000 automation-utilities-1.3.0/Automation_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 15:51:24.000000 automation-utilities-1.3.0/Automation_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-26 15:51:24.000000 automation-utilities-1.3.0/Automation_Utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-06-26 15:51:24.431946 automation-utilities-1.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 15:51:24.429941 automation-utilities-1.3.0/automation_utilities/
+-rw-rw-rw-   0        0        0      646 2023-06-26 15:36:32.000000 automation-utilities-1.3.0/automation_utilities/Data.py
+-rw-rw-rw-   0        0        0      354 2023-06-26 15:50:11.000000 automation-utilities-1.3.0/automation_utilities/Files.py
+-rw-rw-rw-   0        0        0      143 2023-06-26 15:50:11.000000 automation-utilities-1.3.0/automation_utilities/Input.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 15:36:31.000000 automation-utilities-1.3.0/automation_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 15:51:24.431946 automation-utilities-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      248 2023-06-26 15:51:19.000000 automation-utilities-1.3.0/setup.py
```

### Comparing `automation-utilities-1.2.4/automation_utilities/Data.py` & `automation-utilities-1.3.0/automation_utilities/Data.py`

 * *Files identical despite different names*

