# Comparing `tmp/inSis-1.6.0.6.tar.gz` & `tmp/inSis-1.6.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inSis-1.6.0.6.tar", last modified: Fri Jun 23 08:03:46 2023, max compression
+gzip compressed data, was "inSis-1.6.0.7.tar", last modified: Mon Jun 26 08:00:05 2023, max compression
```

## Comparing `inSis-1.6.0.6.tar` & `inSis-1.6.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 08:03:46.841252 inSis-1.6.0.6/
--rw-rw-rw-   0        0        0     1077 2023-06-23 08:01:38.000000 inSis-1.6.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0      547 2023-06-23 08:03:46.841252 inSis-1.6.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      110 2023-06-23 08:01:41.000000 inSis-1.6.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-23 08:03:46.809344 inSis-1.6.0.6/inSis/
--rw-rw-rw-   0        0        0     5433 2023-06-23 07:16:18.000000 inSis-1.6.0.6/inSis/Infoview.py
--rw-rw-rw-   0        0        0        0 2023-06-21 17:45:00.000000 inSis-1.6.0.6/inSis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 08:03:46.841252 inSis-1.6.0.6/inSis.egg-info/
--rw-rw-rw-   0        0        0      547 2023-06-23 08:03:46.000000 inSis-1.6.0.6/inSis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-06-23 08:03:46.000000 inSis-1.6.0.6/inSis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 08:03:46.000000 inSis-1.6.0.6/inSis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-23 08:03:46.000000 inSis-1.6.0.6/inSis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-06-23 08:03:46.000000 inSis-1.6.0.6/inSis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      554 2023-06-23 08:01:45.000000 inSis-1.6.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-23 08:03:46.841252 inSis-1.6.0.6/setup.cfg
--rw-rw-rw-   0        0        0      260 2023-06-23 07:52:29.000000 inSis-1.6.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:00:05.940652 inSis-1.6.0.7/
+-rw-rw-rw-   0        0        0     1077 2023-06-23 08:01:38.000000 inSis-1.6.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      561 2023-06-26 08:00:05.940652 inSis-1.6.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      110 2023-06-23 08:01:41.000000 inSis-1.6.0.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 08:00:05.919176 inSis-1.6.0.7/inSis/
+-rw-rw-rw-   0        0        0     6520 2023-06-26 06:21:31.000000 inSis-1.6.0.7/inSis/Infoview.py
+-rw-rw-rw-   0        0        0        0 2023-06-21 17:45:00.000000 inSis-1.6.0.7/inSis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:00:05.940652 inSis-1.6.0.7/inSis.egg-info/
+-rw-rw-rw-   0        0        0      561 2023-06-26 08:00:05.000000 inSis-1.6.0.7/inSis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-06-26 08:00:05.000000 inSis-1.6.0.7/inSis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 08:00:05.000000 inSis-1.6.0.7/inSis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-26 08:00:05.000000 inSis-1.6.0.7/inSis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-06-26 08:00:05.000000 inSis-1.6.0.7/inSis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      568 2023-06-26 07:58:21.000000 inSis-1.6.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 08:00:05.940652 inSis-1.6.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      260 2023-06-26 07:58:47.000000 inSis-1.6.0.7/setup.py
```

### Comparing `inSis-1.6.0.6/LICENSE.txt` & `inSis-1.6.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inSis-1.6.0.6/inSis/Infoview.py` & `inSis-1.6.0.7/inSis/Infoview.py`

 * *Files 9% similar despite different names*

```diff
@@ -135,9 +135,38 @@
             return reshis
         except requests.HTTPError:
             print("HTTP Error")
             return reshis
         except BaseException as ex:
             print(ex)
             return reshis
+    def SetManualData(self,publishdata):
+        print("Publishing the Manual Data..")
+        resSetData=[]
+        try:
+            server=self.Servername
+            usr=self.username
+            pwd=self.pdname
+            apikey=self.apikey
+            clientId=self.clientId
+            my_PubData = str(publishdata)
+            requrl=server+"/insis/api/data/PublishData?clientId="+clientId+"&Data="+my_PubData
+            headers={"insis_api_key":apikey,"insis_api_user":usr,"insis_api_pwd":pwd}
+            response = requests.post(requrl,headers=headers)
+            responseResult = response.content.decode('utf-8')
+            resSetData = json.loads(responseResult)           
+            return resSetData
+        except requests.exceptions.ConnectionError:
+            print("Connection Error...")
+            return resSetData
+        except requests.HTTPError:
+            print("HTTP Error..")
+            return resSetData
+        except BaseException as ex:
+            print(ex)
+            return resSetData
+            
+
+            
+
```

### Comparing `inSis-1.6.0.6/pyproject.toml` & `inSis-1.6.0.7/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inSis"
-version = "1.6.0.6"
+version = "1.6.0.7"
 authors = [
-  { name="Jaajitech", email="insis@jaajitech.com" },
+  { name="Sivarambrahmam", email="sivarambrahmam@jaajitech.com" },
 ]
 description = "inSis Infoview package"
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

