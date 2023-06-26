# Comparing `tmp/idem-spotinst-0.2.0.tar.gz` & `tmp/idem-spotinst-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-spotinst-0.2.0.tar", last modified: Mon May 22 15:18:30 2023, max compression
+gzip compressed data, was "idem-spotinst-1.0.0.tar", last modified: Mon Jun 26 15:48:14 2023, max compression
```

## Comparing `idem-spotinst-0.2.0.tar` & `idem-spotinst-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/
--rw-r--r--   0 root         (0) root         (0)    11336 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6174 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5377 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/acct/spotinst/
--rw-r--r--   0 root         (0) root         (0)      536 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/acct/spotinst/init.py
--rw-r--r--   0 root         (0) root         (0)     1351 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/exec/spotinst/
--rw-r--r--   0 root         (0) root         (0)      231 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/exec/spotinst/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/states/spotinst/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/states/spotinst/ocean/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/states/spotinst/ocean/aws/
--rw-r--r--   0 root         (0) root         (0)    20832 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/states/spotinst/ocean/aws/k8s_cluster.py
--rw-r--r--   0 root         (0) root         (0)    23325 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/states/spotinst/ocean/aws/launch_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/
--rw-r--r--   0 root         (0) root         (0)     1080 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/comment_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/aws/
--rw-r--r--   0 root         (0) root         (0)     2862 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/aws/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2830 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/aws/k8s_cluster_utils.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/aws/tag_utils.py
--rw-r--r--   0 root         (0) root         (0)     3145 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/state_comparison_utils.py
--rw-r--r--   0 root         (0) root         (0)      856 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/state_utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-22 15:18:30.000000 idem-spotinst-0.2.0/idem_spotinst/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6174 2023-05-22 15:18:30.000000 idem-spotinst-0.2.0/idem_spotinst.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-22 15:18:30.000000 idem-spotinst-0.2.0/idem_spotinst.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 15:18:30.000000 idem-spotinst-0.2.0/idem_spotinst.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-22 15:18:30.000000 idem-spotinst-0.2.0/idem_spotinst.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-05-22 15:18:30.000000 idem-spotinst-0.2.0/idem_spotinst.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-22 15:18:30.000000 idem-spotinst-0.2.0/idem_spotinst.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2720 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.913855 idem-spotinst-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11336 2023-06-26 15:48:01.000000 idem-spotinst-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6174 2023-06-26 15:48:14.913855 idem-spotinst-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5377 2023-06-26 15:48:01.000000 idem-spotinst-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.909855 idem-spotinst-1.0.0/idem_spotinst/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.909855 idem-spotinst-1.0.0/idem_spotinst/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.909855 idem-spotinst-1.0.0/idem_spotinst/acct/spotinst/
+-rw-r--r--   0 root         (0) root         (0)      536 2023-06-26 15:48:01.000000 idem-spotinst-1.0.0/idem_spotinst/acct/spotinst/init.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2023-06-26 15:48:01.000000 idem-spotinst-1.0.0/idem_spotinst/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.909855 idem-spotinst-1.0.0/idem_spotinst/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.909855 idem-spotinst-1.0.0/idem_spotinst/exec/spotinst/
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-26 15:48:01.000000 idem-spotinst-1.0.0/idem_spotinst/exec/spotinst/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.909855 idem-spotinst-1.0.0/idem_spotinst/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.909855 idem-spotinst-1.0.0/idem_spotinst/states/spotinst/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.909855 idem-spotinst-1.0.0/idem_spotinst/states/spotinst/ocean/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.909855 idem-spotinst-1.0.0/idem_spotinst/states/spotinst/ocean/aws/
+-rw-r--r--   0 root         (0) root         (0)    20832 2023-06-26 15:48:01.000000 idem-spotinst-1.0.0/idem_spotinst/states/spotinst/ocean/aws/k8s_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    23325 2023-06-26 15:48:01.000000 idem-spotinst-1.0.0/idem_spotinst/states/spotinst/ocean/aws/launch_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.909855 idem-spotinst-1.0.0/idem_spotinst/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.913855 idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-06-26 15:48:01.000000 idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/comment_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.909855 idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/ocean/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.913855 idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/ocean/aws/
+-rw-r--r--   0 root         (0) root         (0)     2862 2023-06-26 15:48:01.000000 idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/ocean/aws/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-06-26 15:48:01.000000 idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/ocean/aws/k8s_cluster_utils.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-06-26 15:48:01.000000 idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/ocean/aws/tag_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3145 2023-06-26 15:48:01.000000 idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/state_comparison_utils.py
+-rw-r--r--   0 root         (0) root         (0)      856 2023-06-26 15:48:01.000000 idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/state_utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-26 15:48:14.000000 idem-spotinst-1.0.0/idem_spotinst/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:48:14.909855 idem-spotinst-1.0.0/idem_spotinst.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6174 2023-06-26 15:48:14.000000 idem-spotinst-1.0.0/idem_spotinst.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      800 2023-06-26 15:48:14.000000 idem-spotinst-1.0.0/idem_spotinst.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 15:48:14.000000 idem-spotinst-1.0.0/idem_spotinst.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 15:48:14.000000 idem-spotinst-1.0.0/idem_spotinst.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-06-26 15:48:14.000000 idem-spotinst-1.0.0/idem_spotinst.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-26 15:48:14.000000 idem-spotinst-1.0.0/idem_spotinst.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 15:48:14.913855 idem-spotinst-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-06-26 15:48:01.000000 idem-spotinst-1.0.0/setup.py
```

### Comparing `idem-spotinst-0.2.0/LICENSE` & `idem-spotinst-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.2.0/PKG-INFO` & `idem-spotinst-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-spotinst
-Version: 0.2.0
+Version: 1.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Prerna
 Author-email: prjain@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-spotinst-0.2.0/README.rst` & `idem-spotinst-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.2.0/idem_spotinst/acct/spotinst/init.py` & `idem-spotinst-1.0.0/idem_spotinst/acct/spotinst/init.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.2.0/idem_spotinst/conf.py` & `idem-spotinst-1.0.0/idem_spotinst/conf.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.2.0/idem_spotinst/states/spotinst/ocean/aws/k8s_cluster.py` & `idem-spotinst-1.0.0/idem_spotinst/states/spotinst/ocean/aws/k8s_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.2.0/idem_spotinst/states/spotinst/ocean/aws/launch_spec.py` & `idem-spotinst-1.0.0/idem_spotinst/states/spotinst/ocean/aws/launch_spec.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/comment_utils.py` & `idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/comment_utils.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/aws/conversion_utils.py` & `idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/ocean/aws/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/aws/k8s_cluster_utils.py` & `idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/ocean/aws/k8s_cluster_utils.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/aws/tag_utils.py` & `idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/ocean/aws/tag_utils.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/state_comparison_utils.py` & `idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/state_comparison_utils.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/state_utils.py` & `idem-spotinst-1.0.0/idem_spotinst/tool/spotinst/state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.2.0/idem_spotinst.egg-info/PKG-INFO` & `idem-spotinst-1.0.0/idem_spotinst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-spotinst
-Version: 0.2.0
+Version: 1.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Prerna
 Author-email: prjain@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-spotinst-0.2.0/idem_spotinst.egg-info/SOURCES.txt` & `idem-spotinst-1.0.0/idem_spotinst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.2.0/setup.py` & `idem-spotinst-1.0.0/setup.py`

 * *Files identical despite different names*

