# Comparing `tmp/gcloud-connectors-0.1.92.tar.gz` & `tmp/gcloud-connectors-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmp1fmaod21/.tmp-1ryvslnt/gcloud-connectors-0.1.92.tar", last modified: Fri Feb 24 13:26:11 2023, max compression
+gzip compressed data, was "/tmp/tmpad_mvpa7/.tmp-ybbhd_cd/gcloud-connectors-0.1.94.tar", last modified: Mon Jun 26 13:10:08 2023, max compression
```

## Comparing `gcloud-connectors-0.1.92.tar` & `gcloud-connectors-0.1.94.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-24 13:26:11.000000 gcloud-connectors-0.1.92/
--rw-r--r--   0 runner    (1001) docker     (116)     2772 2023-02-24 13:26:11.000000 gcloud-connectors-0.1.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1950 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-24 13:26:11.000000 gcloud-connectors-0.1.92/df2gspread_ext/
--rw-r--r--   0 runner    (1001) docker     (116)      206 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/df2gspread_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      305 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/df2gspread_ext/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     6501 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/df2gspread_ext/df2gspread.py
--rw-r--r--   0 runner    (1001) docker     (116)     3233 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/df2gspread_ext/gfiles.py
--rw-r--r--   0 runner    (1001) docker     (116)     3959 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/df2gspread_ext/gspread2df.py
--rw-r--r--   0 runner    (1001) docker     (116)     5196 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/df2gspread_ext/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-24 13:26:11.000000 gcloud-connectors-0.1.92/gcloud_connectors/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/gcloud_connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7446 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/gcloud_connectors/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (116)      885 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/gcloud_connectors/currency_converter.py
--rw-r--r--   0 runner    (1001) docker     (116)     9558 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/gcloud_connectors/ga4.py
--rw-r--r--   0 runner    (1001) docker     (116)    12247 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/gcloud_connectors/ganalytics.py
--rw-r--r--   0 runner    (1001) docker     (116)     6493 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/gcloud_connectors/gdrive.py
--rw-r--r--   0 runner    (1001) docker     (116)     1738 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/gcloud_connectors/gsc.py
--rw-r--r--   0 runner    (1001) docker     (116)     5777 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/gcloud_connectors/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (116)     5964 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/gcloud_connectors/gstorage.py
--rw-r--r--   0 runner    (1001) docker     (116)      964 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/gcloud_connectors/logger.py
--rw-r--r--   0 runner    (1001) docker     (116)     2186 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/gcloud_connectors/ltv_calculator.py
--rw-r--r--   0 runner    (1001) docker     (116)      453 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/gcloud_connectors/pd_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-24 13:26:11.000000 gcloud-connectors-0.1.92/gcloud_connectors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2772 2023-02-24 13:26:11.000000 gcloud-connectors-0.1.92/gcloud_connectors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      801 2023-02-24 13:26:11.000000 gcloud-connectors-0.1.92/gcloud_connectors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-24 13:26:11.000000 gcloud-connectors-0.1.92/gcloud_connectors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-24 13:26:11.000000 gcloud-connectors-0.1.92/gcloud_connectors.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      658 2023-02-24 13:26:11.000000 gcloud-connectors-0.1.92/gcloud_connectors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       33 2023-02-24 13:26:11.000000 gcloud-connectors-0.1.92/gcloud_connectors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      391 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-24 13:26:11.000000 gcloud-connectors-0.1.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2662 2023-02-24 13:26:06.000000 gcloud-connectors-0.1.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:10:08.000000 gcloud-connectors-0.1.94/
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-26 13:10:08.000000 gcloud-connectors-0.1.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:10:08.000000 gcloud-connectors-0.1.94/df2gspread_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/df2gspread_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/df2gspread_ext/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/df2gspread_ext/df2gspread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/df2gspread_ext/gfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/df2gspread_ext/gspread2df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/df2gspread_ext/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:10:08.000000 gcloud-connectors-0.1.94/gcloud_connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/gcloud_connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/gcloud_connectors/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/gcloud_connectors/currency_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/gcloud_connectors/ga4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/gcloud_connectors/ganalytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/gcloud_connectors/gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/gcloud_connectors/gsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/gcloud_connectors/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/gcloud_connectors/gstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/gcloud_connectors/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/gcloud_connectors/ltv_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/gcloud_connectors/pd_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:10:08.000000 gcloud-connectors-0.1.94/gcloud_connectors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-26 13:10:08.000000 gcloud-connectors-0.1.94/gcloud_connectors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-26 13:10:08.000000 gcloud-connectors-0.1.94/gcloud_connectors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:10:08.000000 gcloud-connectors-0.1.94/gcloud_connectors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:10:08.000000 gcloud-connectors-0.1.94/gcloud_connectors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-26 13:10:08.000000 gcloud-connectors-0.1.94/gcloud_connectors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 13:10:08.000000 gcloud-connectors-0.1.94/gcloud_connectors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 13:10:08.000000 gcloud-connectors-0.1.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-26 13:09:58.000000 gcloud-connectors-0.1.94/setup.py
```

### Comparing `gcloud-connectors-0.1.92/PKG-INFO` & `gcloud-connectors-0.1.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcloud-connectors
-Version: 0.1.92
+Version: 0.1.94
 Summary: Python utilities to simplify connection with Google APIs
 Home-page: https://github.com/pualien/py-gcloud-connector
 Author: Matteo Senardi
 Author-email: pualien@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gcloud-connectors-0.1.92/README.md` & `gcloud-connectors-0.1.94/README.md`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/df2gspread_ext/df2gspread.py` & `gcloud-connectors-0.1.94/df2gspread_ext/df2gspread.py`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/df2gspread_ext/gfiles.py` & `gcloud-connectors-0.1.94/df2gspread_ext/gfiles.py`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/df2gspread_ext/gspread2df.py` & `gcloud-connectors-0.1.94/df2gspread_ext/gspread2df.py`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/df2gspread_ext/utils.py` & `gcloud-connectors-0.1.94/df2gspread_ext/utils.py`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/gcloud_connectors/bigquery.py` & `gcloud-connectors-0.1.94/gcloud_connectors/bigquery.py`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/gcloud_connectors/currency_converter.py` & `gcloud-connectors-0.1.94/gcloud_connectors/currency_converter.py`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/gcloud_connectors/ga4.py` & `gcloud-connectors-0.1.94/gcloud_connectors/ga4.py`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/gcloud_connectors/ganalytics.py` & `gcloud-connectors-0.1.94/gcloud_connectors/ganalytics.py`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/gcloud_connectors/gdrive.py` & `gcloud-connectors-0.1.94/gcloud_connectors/gdrive.py`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/gcloud_connectors/gsc.py` & `gcloud-connectors-0.1.94/gcloud_connectors/gsc.py`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/gcloud_connectors/gsheets.py` & `gcloud-connectors-0.1.94/gcloud_connectors/gsheets.py`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/gcloud_connectors/gstorage.py` & `gcloud-connectors-0.1.94/gcloud_connectors/gstorage.py`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/gcloud_connectors/logger.py` & `gcloud-connectors-0.1.94/gcloud_connectors/logger.py`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/gcloud_connectors/ltv_calculator.py` & `gcloud-connectors-0.1.94/gcloud_connectors/ltv_calculator.py`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/gcloud_connectors.egg-info/PKG-INFO` & `gcloud-connectors-0.1.94/gcloud_connectors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcloud-connectors
-Version: 0.1.92
+Version: 0.1.94
 Summary: Python utilities to simplify connection with Google APIs
 Home-page: https://github.com/pualien/py-gcloud-connector
 Author: Matteo Senardi
 Author-email: pualien@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gcloud-connectors-0.1.92/gcloud_connectors.egg-info/SOURCES.txt` & `gcloud-connectors-0.1.94/gcloud_connectors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcloud-connectors-0.1.92/gcloud_connectors.egg-info/requires.txt` & `gcloud-connectors-0.1.94/gcloud_connectors.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 cachetools==4.2.2
 gspread_pandas==3.2.2
-httplib2==0.19.1
-oauth2client==4.1.3
+httplib2==0.22.0
 gspread==5.4.0
-numpy==1.23.5
-pandas==1.3.3
+numpy==1.24.3
+pandas==1.5.3
 brotli==1.0.9
-Cython==0.29.24
+Cython==0.29.35
 docutils>=0.15.2
-google_api_python_client==2.18.0
-importlib_metadata==4.8.1
-keyring==23.1.0
+google_api_python_client==2.90.0
+importlib_metadata==6.7.0
+keyring==24.2.0
 lockfile==0.12.2
-lxml==4.9.1
-mock==4.0.3
+lxml==4.9.2
+mock==5.0.2
 ordereddict==1.1
-protobuf==3.20.2
-pyOpenSSL==20.0.1
-simplejson==3.17.5
+protobuf==4.23.3
+pyOpenSSL==23.2.0
+simplejson==3.19.1
 toml==0.10.2
-unicodedataplus==14.0.0.post2
+unicodedataplus==15.0.0.post2
 usercustomize==1.0.0
-zipp==3.6.0
-tornado==6.1
-cryptography==36.0.2
-pyarrow==8.0.0
-fastparquet==0.4.1
+zipp==3.15.0
+tornado==6.3.2
+cryptography==41.0.1
+pyarrow==12.0.1
+fastparquet==2023.4.0
 retry==0.9.2
-google-cloud-bigquery==3.6.0
-google-cloud-bigquery-storage==2.18.1
-gcsfs==0.7.1
+google-cloud-bigquery==3.11.2
+google-cloud-bigquery-storage==2.20.0
 oauth2client==4.1.3
-google-analytics-data==0.15.0
-db-dtypes==1.0.1
+google-analytics-data==0.16.2
+db-dtypes==1.1.1
```

### Comparing `gcloud-connectors-0.1.92/setup.py` & `gcloud-connectors-0.1.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         maybe_dep = maybe_dep.strip()
         if maybe_dep:
             dependencies.append(maybe_dep)
     return dependencies
 
 
 setup(name='gcloud-connectors',
-      version='0.1.92',
+      version='0.1.94',
       url='https://github.com/pualien/py-gcloud-connector',
       # download_url='https://github.com/pualien/py-gcloud-connectors/archive/0.1.23.tar.gz',
       license='MIT',
       author='Matteo Senardi',
       author_email='pualien@gmail.com',
       description='Python utilities to simplify connection with Google APIs',
       packages=find_packages(exclude=['tests']),
```

