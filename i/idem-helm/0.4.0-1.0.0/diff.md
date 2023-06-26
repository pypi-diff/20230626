# Comparing `tmp/idem-helm-0.4.0.tar.gz` & `tmp/idem-helm-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-helm-0.4.0.tar", last modified: Thu Jun  1 23:20:20 2023, max compression
+gzip compressed data, was "idem-helm-1.0.0.tar", last modified: Mon Jun 26 15:45:06 2023, max compression
```

## Comparing `idem-helm-0.4.0.tar` & `idem-helm-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:20:20.810191 idem-helm-0.4.0/
--rw-r--r--   0 root         (0) root         (0)    11345 2023-06-01 23:20:06.000000 idem-helm-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5330 2023-06-01 23:20:20.810191 idem-helm-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4526 2023-06-01 23:20:06.000000 idem-helm-0.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:20:20.810191 idem-helm-0.4.0/idem_helm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:20:20.810191 idem-helm-0.4.0/idem_helm/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:20:20.810191 idem-helm-0.4.0/idem_helm/acct/helm/
--rw-r--r--   0 root         (0) root         (0)      552 2023-06-01 23:20:06.000000 idem-helm-0.4.0/idem_helm/acct/helm/init.py
--rw-r--r--   0 root         (0) root         (0)     1275 2023-06-01 23:20:06.000000 idem-helm-0.4.0/idem_helm/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:20:20.810191 idem-helm-0.4.0/idem_helm/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:20:20.810191 idem-helm-0.4.0/idem_helm/exec/helm/
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-01 23:20:06.000000 idem-helm-0.4.0/idem_helm/exec/helm/init.py
--rw-r--r--   0 root         (0) root         (0)     3701 2023-06-01 23:20:06.000000 idem-helm-0.4.0/idem_helm/exec/helm/release.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:20:20.810191 idem-helm-0.4.0/idem_helm/states/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 23:20:06.000000 idem-helm-0.4.0/idem_helm/states/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:20:20.810191 idem-helm-0.4.0/idem_helm/states/helm/
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-01 23:20:06.000000 idem-helm-0.4.0/idem_helm/states/helm/init.py
--rw-r--r--   0 root         (0) root         (0)    14946 2023-06-01 23:20:06.000000 idem-helm-0.4.0/idem_helm/states/helm/release.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:20:20.810191 idem-helm-0.4.0/idem_helm/tool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 23:20:06.000000 idem-helm-0.4.0/idem_helm/tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:20:20.810191 idem-helm-0.4.0/idem_helm/tool/helm/
--rw-r--r--   0 root         (0) root         (0)     3403 2023-06-01 23:20:06.000000 idem-helm-0.4.0/idem_helm/tool/helm/command_utils.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-06-01 23:20:06.000000 idem-helm-0.4.0/idem_helm/tool/helm/comment_utils.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-06-01 23:20:06.000000 idem-helm-0.4.0/idem_helm/tool/helm/release_utils.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-06-01 23:20:06.000000 idem-helm-0.4.0/idem_helm/tool/helm/test_state_utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-01 23:20:20.000000 idem-helm-0.4.0/idem_helm/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 23:20:20.810191 idem-helm-0.4.0/idem_helm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5330 2023-06-01 23:20:20.000000 idem-helm-0.4.0/idem_helm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      633 2023-06-01 23:20:20.000000 idem-helm-0.4.0/idem_helm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 23:20:20.000000 idem-helm-0.4.0/idem_helm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-01 23:20:20.000000 idem-helm-0.4.0/idem_helm.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-01 23:20:20.000000 idem-helm-0.4.0/idem_helm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-01 23:20:20.000000 idem-helm-0.4.0/idem_helm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-01 23:20:20.810191 idem-helm-0.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2719 2023-06-01 23:20:06.000000 idem-helm-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:45:06.107268 idem-helm-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11345 2023-06-26 15:44:52.000000 idem-helm-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-06-26 15:45:06.107268 idem-helm-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4526 2023-06-26 15:44:52.000000 idem-helm-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:45:06.107268 idem-helm-1.0.0/idem_helm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:45:06.103268 idem-helm-1.0.0/idem_helm/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:45:06.107268 idem-helm-1.0.0/idem_helm/acct/helm/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-06-26 15:44:52.000000 idem-helm-1.0.0/idem_helm/acct/helm/init.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2023-06-26 15:44:52.000000 idem-helm-1.0.0/idem_helm/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:45:06.103268 idem-helm-1.0.0/idem_helm/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:45:06.107268 idem-helm-1.0.0/idem_helm/exec/helm/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-26 15:44:52.000000 idem-helm-1.0.0/idem_helm/exec/helm/init.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2023-06-26 15:44:52.000000 idem-helm-1.0.0/idem_helm/exec/helm/release.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:45:06.107268 idem-helm-1.0.0/idem_helm/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 15:44:52.000000 idem-helm-1.0.0/idem_helm/states/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:45:06.107268 idem-helm-1.0.0/idem_helm/states/helm/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-26 15:44:52.000000 idem-helm-1.0.0/idem_helm/states/helm/init.py
+-rw-r--r--   0 root         (0) root         (0)    14946 2023-06-26 15:44:52.000000 idem-helm-1.0.0/idem_helm/states/helm/release.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:45:06.107268 idem-helm-1.0.0/idem_helm/tool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 15:44:52.000000 idem-helm-1.0.0/idem_helm/tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:45:06.107268 idem-helm-1.0.0/idem_helm/tool/helm/
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-06-26 15:44:52.000000 idem-helm-1.0.0/idem_helm/tool/helm/command_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-06-26 15:44:52.000000 idem-helm-1.0.0/idem_helm/tool/helm/comment_utils.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-06-26 15:44:52.000000 idem-helm-1.0.0/idem_helm/tool/helm/release_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-06-26 15:44:52.000000 idem-helm-1.0.0/idem_helm/tool/helm/test_state_utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-26 15:45:05.000000 idem-helm-1.0.0/idem_helm/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:45:06.107268 idem-helm-1.0.0/idem_helm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-06-26 15:45:06.000000 idem-helm-1.0.0/idem_helm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      633 2023-06-26 15:45:06.000000 idem-helm-1.0.0/idem_helm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 15:45:06.000000 idem-helm-1.0.0/idem_helm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 15:45:06.000000 idem-helm-1.0.0/idem_helm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-26 15:45:06.000000 idem-helm-1.0.0/idem_helm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-26 15:45:06.000000 idem-helm-1.0.0/idem_helm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 15:45:06.107268 idem-helm-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-06-26 15:44:52.000000 idem-helm-1.0.0/setup.py
```

### Comparing `idem-helm-0.4.0/LICENSE` & `idem-helm-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-helm-0.4.0/PKG-INFO` & `idem-helm-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-helm
-Version: 0.4.0
+Version: 1.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-helm-0.4.0/README.rst` & `idem-helm-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `idem-helm-0.4.0/idem_helm/acct/helm/init.py` & `idem-helm-1.0.0/idem_helm/acct/helm/init.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.4.0/idem_helm/conf.py` & `idem-helm-1.0.0/idem_helm/conf.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.4.0/idem_helm/exec/helm/release.py` & `idem-helm-1.0.0/idem_helm/exec/helm/release.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.4.0/idem_helm/states/helm/release.py` & `idem-helm-1.0.0/idem_helm/states/helm/release.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.4.0/idem_helm/tool/helm/command_utils.py` & `idem-helm-1.0.0/idem_helm/tool/helm/command_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.4.0/idem_helm/tool/helm/comment_utils.py` & `idem-helm-1.0.0/idem_helm/tool/helm/comment_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.4.0/idem_helm/tool/helm/release_utils.py` & `idem-helm-1.0.0/idem_helm/tool/helm/release_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.4.0/idem_helm/tool/helm/test_state_utils.py` & `idem-helm-1.0.0/idem_helm/tool/helm/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.4.0/idem_helm.egg-info/PKG-INFO` & `idem-helm-1.0.0/idem_helm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-helm
-Version: 0.4.0
+Version: 1.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-helm-0.4.0/idem_helm.egg-info/SOURCES.txt` & `idem-helm-1.0.0/idem_helm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-helm-0.4.0/setup.py` & `idem-helm-1.0.0/setup.py`

 * *Files identical despite different names*

