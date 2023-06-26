# Comparing `tmp/kalm-0.7.8.tar.gz` & `tmp/kalm-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.7.8.tar", max compression
+gzip compressed data, was "kalm-0.7.9.tar", max compression
```

## Comparing `kalm-0.7.8.tar` & `kalm-0.7.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.7.8/LICENSE.txt
--rw-r--r--   0        0        0     2181 2023-06-22 11:02:53.757727 kalm-0.7.8/pyproject.toml
--rw-r--r--   0        0        0    10437 2023-06-22 10:49:45.901051 kalm-0.7.8/src/kalm/__init__.py
--rw-r--r--   0        0        0      219 2023-06-16 06:22:57.918975 kalm-0.7.8/src/kalm/common.py
--rw-r--r--   0        0        0     1255 2023-06-20 12:39:02.436562 kalm-0.7.8/src/kalm/dns/__init__.py
--rw-r--r--   0        0        0     3166 2023-06-20 12:39:02.436562 kalm-0.7.8/src/kalm/dns/dns.py
--rw-r--r--   0        0        0      834 2023-06-20 12:39:02.436562 kalm-0.7.8/src/kalm/gitea/__init__.py
--rw-r--r--   0        0        0      130 2023-06-20 12:39:02.436562 kalm-0.7.8/src/kalm/gitea/gitea.py
--rw-r--r--   0        0        0     1062 2023-06-13 13:07:33.595735 kalm-0.7.8/src/kalm/inabox/__init__.py
--rw-r--r--   0        0        0    10171 2023-06-13 13:34:51.253238 kalm-0.7.8/src/kalm/inabox/inabox.py
--rw-r--r--   0        0        0     1415 2023-06-20 12:41:22.849280 kalm-0.7.8/src/kalm/jenkins/__init__.py
--rw-r--r--   0        0        0     1877 2023-06-20 12:51:23.364410 kalm-0.7.8/src/kalm/jenkins/jenkins.py
--rw-r--r--   0        0        0    35899 2023-06-22 11:02:41.929657 kalm-0.7.8/src/kalm/kalm.py
--rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.7.8/src/kalm/package_data.dat
--rw-r--r--   0        0        0      774 2023-06-13 13:07:33.595735 kalm-0.7.8/src/kalm/pypi/__init__.py
--rw-r--r--   0        0        0      536 2023-06-13 13:34:51.253238 kalm-0.7.8/src/kalm/pypi/pypi.py
--rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.7.8/src/kalm/toolbox.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 12:32:33.321460 kalm-0.7.9/LICENSE.txt
+-rw-r--r--   0        0        0     2181 2023-06-22 11:05:05.206502 kalm-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0    10437 2023-06-22 10:49:45.901051 kalm-0.7.9/src/kalm/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-16 06:22:57.918975 kalm-0.7.9/src/kalm/common.py
+-rw-r--r--   0        0        0     1255 2023-06-20 12:39:02.436562 kalm-0.7.9/src/kalm/dns/__init__.py
+-rw-r--r--   0        0        0     3166 2023-06-20 12:39:02.436562 kalm-0.7.9/src/kalm/dns/dns.py
+-rw-r--r--   0        0        0      834 2023-06-20 12:39:02.436562 kalm-0.7.9/src/kalm/gitea/__init__.py
+-rw-r--r--   0        0        0      130 2023-06-20 12:39:02.436562 kalm-0.7.9/src/kalm/gitea/gitea.py
+-rw-r--r--   0        0        0     1062 2023-06-13 13:07:33.595735 kalm-0.7.9/src/kalm/inabox/__init__.py
+-rw-r--r--   0        0        0    10171 2023-06-13 13:34:51.253238 kalm-0.7.9/src/kalm/inabox/inabox.py
+-rw-r--r--   0        0        0     1415 2023-06-20 12:41:22.849280 kalm-0.7.9/src/kalm/jenkins/__init__.py
+-rw-r--r--   0        0        0     1877 2023-06-20 12:51:23.364410 kalm-0.7.9/src/kalm/jenkins/jenkins.py
+-rw-r--r--   0        0        0    35924 2023-06-22 11:04:55.710446 kalm-0.7.9/src/kalm/kalm.py
+-rw-r--r--   0        0        0        9 2023-05-09 12:32:33.321460 kalm-0.7.9/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      774 2023-06-13 13:07:33.595735 kalm-0.7.9/src/kalm/pypi/__init__.py
+-rw-r--r--   0        0        0      536 2023-06-13 13:34:51.253238 kalm-0.7.9/src/kalm/pypi/pypi.py
+-rw-r--r--   0        0        0      312 2023-05-09 12:32:33.321460 kalm-0.7.9/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 kalm-0.7.9/PKG-INFO
```

### Comparing `kalm-0.7.8/LICENSE.txt` & `kalm-0.7.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.7.8/pyproject.toml` & `kalm-0.7.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kalm"
-version = "0.7.8"
+version = "0.7.9"
 description = "Knowit Automation lifecycle management"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://kalm.openknowit.com"
 repository = "https://github.com/miracle-as/openknowit_kalm.git"
 
 [tool.poetry.scripts]
@@ -28,15 +28,15 @@
 python-jenkins = "^1.7.0"
 urllib3 = "^2.0.2"
 
 
 
 [project]
 name = "kalm"  
-version = "0.7.07" 
+version = "0.7.08" 
 description = "Knowit automation lifecycle management"
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["kalm", "awx", "ansible", "automation"]  
 authors = [
   {name = "Jakob Holst", email = "jho@miracle.dk" }
```

### Comparing `kalm-0.7.8/src/kalm/__init__.py` & `kalm-0.7.9/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.8/src/kalm/dns/__init__.py` & `kalm-0.7.9/src/kalm/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.8/src/kalm/dns/dns.py` & `kalm-0.7.9/src/kalm/dns/dns.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.8/src/kalm/gitea/__init__.py` & `kalm-0.7.9/src/kalm/gitea/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.8/src/kalm/inabox/__init__.py` & `kalm-0.7.9/src/kalm/inabox/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.8/src/kalm/inabox/inabox.py` & `kalm-0.7.9/src/kalm/inabox/inabox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.8/src/kalm/jenkins/__init__.py` & `kalm-0.7.9/src/kalm/jenkins/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.8/src/kalm/jenkins/jenkins.py` & `kalm-0.7.9/src/kalm/jenkins/jenkins.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.8/src/kalm/kalm.py` & `kalm-0.7.9/src/kalm/kalm.py`

 * *Files 1% similar despite different names*

```diff
@@ -812,14 +812,15 @@
     except:
       prettyllog("config", "initialize", "projects", orgname, "000",  "No projects found")
     ######################################
     # Subprojects
     ######################################
     try:
       subprojects = org['subprojects']
+      print(subprojects)
       for subproject in subprojects:
         print(subproject)
         subprojectname = subproject['name']
         key = os.getenv("TOWER_HOST") +":projects:orphan:" + subprojectname
         r.delete(key)
         awx_create_project(subprojectname, orgname, mytoken, r)
         awx_get_id("projects", subprojectname, r)
```

### Comparing `kalm-0.7.8/src/kalm/pypi/__init__.py` & `kalm-0.7.9/src/kalm/pypi/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.8/src/kalm/pypi/pypi.py` & `kalm-0.7.9/src/kalm/pypi/pypi.py`

 * *Files identical despite different names*

### Comparing `kalm-0.7.8/PKG-INFO` & `kalm-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.7.8
+Version: 0.7.9
 Summary: Knowit Automation lifecycle management
 Home-page: https://kalm.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

