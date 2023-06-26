# Comparing `tmp/ess-cloud-utils-0.8.tar.gz` & `tmp/ess-cloud-utils-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ess-cloud-utils-0.8.tar", last modified: Wed Apr 27 09:40:34 2022, max compression
+gzip compressed data, was "ess-cloud-utils-0.9.tar", last modified: Tue Feb 28 09:21:08 2023, max compression
```

## Comparing `ess-cloud-utils-0.8.tar` & `ess-cloud-utils-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-04-27 09:40:34.103023 ess-cloud-utils-0.8/
--rw-rw-rw-   0        0        0    10967 2022-04-27 09:29:50.000000 ess-cloud-utils-0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      304 2022-04-27 09:40:34.103023 ess-cloud-utils-0.8/PKG-INFO
--rw-rw-rw-   0        0        0      477 2022-04-27 09:29:50.000000 ess-cloud-utils-0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-04-27 09:40:34.087961 ess-cloud-utils-0.8/ess_cloud_utils/
--rw-rw-rw-   0        0        0      171 2022-04-27 09:29:50.000000 ess-cloud-utils-0.8/ess_cloud_utils/__init__.py
--rw-rw-rw-   0        0        0     1167 2022-04-27 09:35:26.000000 ess-cloud-utils-0.8/ess_cloud_utils/apis_client.py
--rw-rw-rw-   0        0        0     2896 2022-04-27 09:29:50.000000 ess-cloud-utils-0.8/ess_cloud_utils/eureka.py
--rw-rw-rw-   0        0        0      691 2022-04-27 09:29:50.000000 ess-cloud-utils-0.8/ess_cloud_utils/host_info_service.py
-drwxrwxrwx   0        0        0        0 2022-04-27 09:40:34.100999 ess-cloud-utils-0.8/ess_cloud_utils.egg-info/
--rw-rw-rw-   0        0        0      304 2022-04-27 09:40:33.000000 ess-cloud-utils-0.8/ess_cloud_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2022-04-27 09:40:34.000000 ess-cloud-utils-0.8/ess_cloud_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-27 09:40:33.000000 ess-cloud-utils-0.8/ess_cloud_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2022-04-27 09:40:33.000000 ess-cloud-utils-0.8/ess_cloud_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-04-27 09:40:33.000000 ess-cloud-utils-0.8/ess_cloud_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-04-27 09:40:34.104959 ess-cloud-utils-0.8/setup.cfg
--rw-rw-rw-   0        0        0      411 2022-04-27 09:35:19.000000 ess-cloud-utils-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-28 09:21:08.136036 ess-cloud-utils-0.9/
+-rw-rw-rw-   0        0        0    10967 2023-02-28 08:40:40.000000 ess-cloud-utils-0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      304 2023-02-28 09:21:08.136036 ess-cloud-utils-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-02-28 08:40:40.000000 ess-cloud-utils-0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-28 09:21:08.127029 ess-cloud-utils-0.9/ess_cloud_utils/
+-rw-rw-rw-   0        0        0      171 2023-02-28 08:40:40.000000 ess-cloud-utils-0.9/ess_cloud_utils/__init__.py
+-rw-rw-rw-   0        0        0     1181 2023-02-28 09:01:43.000000 ess-cloud-utils-0.9/ess_cloud_utils/apis_client.py
+-rw-rw-rw-   0        0        0     2896 2023-02-28 08:40:40.000000 ess-cloud-utils-0.9/ess_cloud_utils/eureka.py
+-rw-rw-rw-   0        0        0      691 2023-02-28 08:40:40.000000 ess-cloud-utils-0.9/ess_cloud_utils/host_info_service.py
+drwxrwxrwx   0        0        0        0 2023-02-28 09:21:08.135036 ess-cloud-utils-0.9/ess_cloud_utils.egg-info/
+-rw-rw-rw-   0        0        0      304 2023-02-28 09:21:07.000000 ess-cloud-utils-0.9/ess_cloud_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-02-28 09:21:08.000000 ess-cloud-utils-0.9/ess_cloud_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-28 09:21:07.000000 ess-cloud-utils-0.9/ess_cloud_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-02-28 09:21:07.000000 ess-cloud-utils-0.9/ess_cloud_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-02-28 09:21:07.000000 ess-cloud-utils-0.9/ess_cloud_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-02-28 09:21:08.137036 ess-cloud-utils-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      411 2023-02-28 09:20:50.000000 ess-cloud-utils-0.9/setup.py
```

### Comparing `ess-cloud-utils-0.8/LICENSE.txt` & `ess-cloud-utils-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ess-cloud-utils-0.8/ess_cloud_utils/apis_client.py` & `ess-cloud-utils-0.9/ess_cloud_utils/apis_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .eureka import Eureka
 
 
 class ApisClient(object):
     @staticmethod
     def get(service_name, endpoint, headers=None):
         url = Eureka.get_application_address(service_name) + endpoint
-        response = requests.get(url, headers=headers).json()
+        response = requests.get(url, headers=headers, timeout=None).json()
         return response
 
     @staticmethod
     def post(service_name, endpoint, body=None, headers=None, json=None, files=None):
         url = Eureka.get_application_address(service_name) + endpoint
         response = requests.post(url, data=body, headers=headers, json=json, files=files)
         return response
```

### Comparing `ess-cloud-utils-0.8/ess_cloud_utils/eureka.py` & `ess-cloud-utils-0.9/ess_cloud_utils/eureka.py`

 * *Files identical despite different names*

### Comparing `ess-cloud-utils-0.8/ess_cloud_utils/host_info_service.py` & `ess-cloud-utils-0.9/ess_cloud_utils/host_info_service.py`

 * *Files identical despite different names*

