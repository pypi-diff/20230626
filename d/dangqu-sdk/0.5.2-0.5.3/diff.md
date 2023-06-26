# Comparing `tmp/dangqu-sdk-0.5.2.tar.gz` & `tmp/dangqu-sdk-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dangqu-sdk-0.5.2.tar", last modified: Thu Apr 13 03:19:19 2023, max compression
+gzip compressed data, was "dangqu-sdk-0.5.3.tar", last modified: Mon May 15 05:56:34 2023, max compression
```

## Comparing `dangqu-sdk-0.5.2.tar` & `dangqu-sdk-0.5.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 03:19:19.891060 dangqu-sdk-0.5.2/
--rw-rw-rw-   0        0        0      474 2023-04-13 03:19:19.890061 dangqu-sdk-0.5.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 03:19:19.878067 dangqu-sdk-0.5.2/dangqu_sdk/
--rw-rw-rw-   0        0        0       57 2023-04-03 02:36:01.000000 dangqu-sdk-0.5.2/dangqu_sdk/__init__.py
--rw-rw-rw-   0        0        0     1998 2023-04-13 03:18:51.000000 dangqu-sdk-0.5.2/dangqu_sdk/client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:19:19.888042 dangqu-sdk-0.5.2/dangqu_sdk.egg-info/
--rw-rw-rw-   0        0        0      474 2023-04-13 03:19:19.000000 dangqu-sdk-0.5.2/dangqu_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-13 03:19:19.000000 dangqu-sdk-0.5.2/dangqu_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 03:19:19.000000 dangqu-sdk-0.5.2/dangqu_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-04-13 03:19:19.000000 dangqu-sdk-0.5.2/dangqu_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-13 03:19:19.000000 dangqu-sdk-0.5.2/dangqu_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 03:19:19.891060 dangqu-sdk-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-04-13 03:18:51.000000 dangqu-sdk-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:56:34.625983 dangqu-sdk-0.5.3/
+-rw-rw-rw-   0        0        0      474 2023-05-15 05:56:34.625014 dangqu-sdk-0.5.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-15 05:56:34.612983 dangqu-sdk-0.5.3/dangqu_sdk/
+-rw-rw-rw-   0        0        0       58 2023-05-15 05:46:43.000000 dangqu-sdk-0.5.3/dangqu_sdk/__init__.py
+-rw-rw-rw-   0        0        0     2022 2023-05-15 05:49:56.000000 dangqu-sdk-0.5.3/dangqu_sdk/client.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:56:34.622982 dangqu-sdk-0.5.3/dangqu_sdk.egg-info/
+-rw-rw-rw-   0        0        0      474 2023-05-15 05:56:34.000000 dangqu-sdk-0.5.3/dangqu_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-05-15 05:56:34.000000 dangqu-sdk-0.5.3/dangqu_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 05:56:34.000000 dangqu-sdk-0.5.3/dangqu_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-15 05:56:34.000000 dangqu-sdk-0.5.3/dangqu_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-15 05:56:34.000000 dangqu-sdk-0.5.3/dangqu_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 05:56:34.625983 dangqu-sdk-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      698 2023-05-15 05:54:48.000000 dangqu-sdk-0.5.3/setup.py
```

### Comparing `dangqu-sdk-0.5.2/dangqu_sdk/client.py` & `dangqu-sdk-0.5.3/dangqu_sdk/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,11 +54,11 @@
             "isSync"            : True,
             "isReturnResult"    : True,
             "hostTenant"        : host_tenant,
             "unifiedId"         : unified_id,
             "inputParameterJson": json.dumps(request_body)
         }
 
-        _headers = {'Authorization': 'Bearer %s' % self.token}
+        _headers = {'Authorization': 'Bearer %s' % self.token.get('access_token', '')}
         response = requests.post(self.logical_url, headers=_headers, json=body)
 
         return response
```

### Comparing `dangqu-sdk-0.5.2/setup.py` & `dangqu-sdk-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dangqu-sdk',
-    version='0.5.2',
+    version='0.5.3',
     description='dangqu sdk',
     author='ZhaoHui',
     author_email='myemail@example.com',
     packages=find_packages(),
     install_requires=[
         'requests',
         'oauthlib',
```

