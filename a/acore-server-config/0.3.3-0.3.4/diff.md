# Comparing `tmp/acore_server_config-0.3.3.tar.gz` & `tmp/acore_server_config-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_config-0.3.3.tar", last modified: Mon Jun 26 05:41:18 2023, max compression
+gzip compressed data, was "acore_server_config-0.3.4.tar", last modified: Mon Jun 26 16:47:54 2023, max compression
```

## Comparing `acore_server_config-0.3.3.tar` & `acore_server_config-0.3.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.096253 acore_server_config-0.3.3/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5264 2023-06-26 05:41:18.096090 acore_server_config-0.3.3/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4102 2023-06-26 05:40:34.000000 acore_server_config-0.3.3/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.091722 acore_server_config-0.3.3/acore_server_config/
--rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-18 01:38:46.000000 acore_server_config-0.3.3/acore_server_config/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-26 05:38:27.000000 acore_server_config-0.3.3/acore_server_config/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      492 2023-06-19 16:52:37.000000 acore_server_config-0.3.3/acore_server_config/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1149 2023-06-22 03:51:05.000000 acore_server_config-0.3.3/acore_server_config/boto_ses.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-06-16 18:25:58.000000 acore_server_config-0.3.3/acore_server_config/compat.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.093062 acore_server_config-0.3.3/acore_server_config/config/
--rw-r--r--   0 sanhehu    (501) staff       (20)       50 2023-06-19 17:13:43.000000 acore_server_config-0.3.3/acore_server_config/config/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.093872 acore_server_config-0.3.3/acore_server_config/config/define/
--rw-r--r--   0 sanhehu    (501) staff       (20)       98 2023-06-19 17:13:36.000000 acore_server_config-0.3.3/acore_server_config/config/define/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2672 2023-06-18 00:57:04.000000 acore_server_config-0.3.3/acore_server_config/config/define/main.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1565 2023-06-19 17:35:38.000000 acore_server_config-0.3.3/acore_server_config/config/define/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1634 2023-06-18 00:44:26.000000 acore_server_config-0.3.3/acore_server_config/config/init.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     8000 2023-06-26 05:34:11.000000 acore_server_config-0.3.3/acore_server_config/config/loader.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.094178 acore_server_config-0.3.3/acore_server_config/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/acore_server_config/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4080 2023-06-26 05:35:57.000000 acore_server_config-0.3.3/acore_server_config/in_ec2.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-17 20:38:51.000000 acore_server_config-0.3.3/acore_server_config/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2300 2023-06-22 03:31:06.000000 acore_server_config-0.3.3/acore_server_config/runtime.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.095120 acore_server_config-0.3.3/acore_server_config/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/acore_server_config/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      362 2023-06-19 16:31:24.000000 acore_server_config-0.3.3/acore_server_config/tests/dummy_config.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/acore_server_config/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-19 16:26:34.000000 acore_server_config-0.3.3/acore_server_config/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.095574 acore_server_config-0.3.3/acore_server_config/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/acore_server_config/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/acore_server_config/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.092421 acore_server_config-0.3.3/acore_server_config.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5264 2023-06-26 05:41:18.000000 acore_server_config-0.3.3/acore_server_config.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-26 05:41:18.000000 acore_server_config-0.3.3/acore_server_config.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-26 05:41:18.000000 acore_server_config-0.3.3/acore_server_config.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      315 2023-06-26 05:41:18.000000 acore_server_config-0.3.3/acore_server_config.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-26 05:41:18.000000 acore_server_config-0.3.3/acore_server_config.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     2973 2023-06-26 05:38:11.000000 acore_server_config-0.3.3/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-18 01:00:08.000000 acore_server_config-0.3.3/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-06-19 16:26:45.000000 acore_server_config-0.3.3/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      201 2023-06-26 05:32:50.000000 acore_server_config-0.3.3/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-26 05:41:18.096303 acore_server_config-0.3.3/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.095758 acore_server_config-0.3.3/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      501 2023-06-19 16:53:17.000000 acore_server_config-0.3.3/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 16:47:54.006109 acore_server_config-0.3.4/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 19:58:08.000000 acore_server_config-0.3.4/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-17 19:58:08.000000 acore_server_config-0.3.4/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-17 19:58:08.000000 acore_server_config-0.3.4/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5264 2023-06-26 16:47:54.005972 acore_server_config-0.3.4/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4102 2023-06-26 05:40:34.000000 acore_server_config-0.3.4/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 16:47:54.002353 acore_server_config-0.3.4/acore_server_config/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-18 01:38:46.000000 acore_server_config-0.3.4/acore_server_config/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-26 16:45:34.000000 acore_server_config-0.3.4/acore_server_config/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      492 2023-06-19 16:52:37.000000 acore_server_config-0.3.4/acore_server_config/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1149 2023-06-22 03:51:05.000000 acore_server_config-0.3.4/acore_server_config/boto_ses.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-06-16 18:25:58.000000 acore_server_config-0.3.4/acore_server_config/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 16:47:54.003567 acore_server_config-0.3.4/acore_server_config/config/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       50 2023-06-19 17:13:43.000000 acore_server_config-0.3.4/acore_server_config/config/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 16:47:54.004194 acore_server_config-0.3.4/acore_server_config/config/define/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       98 2023-06-19 17:13:36.000000 acore_server_config-0.3.4/acore_server_config/config/define/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2672 2023-06-18 00:57:04.000000 acore_server_config-0.3.4/acore_server_config/config/define/main.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1565 2023-06-19 17:35:38.000000 acore_server_config-0.3.4/acore_server_config/config/define/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1634 2023-06-18 00:44:26.000000 acore_server_config-0.3.4/acore_server_config/config/init.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8000 2023-06-26 05:34:11.000000 acore_server_config-0.3.4/acore_server_config/config/loader.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 16:47:54.004420 acore_server_config-0.3.4/acore_server_config/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 19:58:08.000000 acore_server_config-0.3.4/acore_server_config/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4080 2023-06-26 05:35:57.000000 acore_server_config-0.3.4/acore_server_config/in_ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-17 20:38:51.000000 acore_server_config-0.3.4/acore_server_config/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2378 2023-06-26 16:46:45.000000 acore_server_config-0.3.4/acore_server_config/runtime.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 16:47:54.005232 acore_server_config-0.3.4/acore_server_config/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 19:58:08.000000 acore_server_config-0.3.4/acore_server_config/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      362 2023-06-19 16:31:24.000000 acore_server_config-0.3.4/acore_server_config/tests/dummy_config.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 19:58:08.000000 acore_server_config-0.3.4/acore_server_config/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-19 16:26:34.000000 acore_server_config-0.3.4/acore_server_config/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 16:47:54.005573 acore_server_config-0.3.4/acore_server_config/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 19:58:08.000000 acore_server_config-0.3.4/acore_server_config/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 19:58:08.000000 acore_server_config-0.3.4/acore_server_config/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 16:47:54.003023 acore_server_config-0.3.4/acore_server_config.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5264 2023-06-26 16:47:53.000000 acore_server_config-0.3.4/acore_server_config.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-26 16:47:53.000000 acore_server_config-0.3.4/acore_server_config.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-26 16:47:53.000000 acore_server_config-0.3.4/acore_server_config.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      315 2023-06-26 16:47:53.000000 acore_server_config-0.3.4/acore_server_config.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-26 16:47:53.000000 acore_server_config-0.3.4/acore_server_config.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3167 2023-06-26 16:46:15.000000 acore_server_config-0.3.4/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 19:58:08.000000 acore_server_config-0.3.4/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-18 01:00:08.000000 acore_server_config-0.3.4/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 19:58:08.000000 acore_server_config-0.3.4/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-06-19 16:26:45.000000 acore_server_config-0.3.4/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      201 2023-06-26 05:32:50.000000 acore_server_config-0.3.4/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-26 16:47:54.006148 acore_server_config-0.3.4/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-17 19:58:08.000000 acore_server_config-0.3.4/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 16:47:54.005698 acore_server_config-0.3.4/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      501 2023-06-19 16:53:17.000000 acore_server_config-0.3.4/tests/test_api.py
```

### Comparing `acore_server_config-0.3.3/AUTHORS.rst` & `acore_server_config-0.3.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.3/LICENSE.txt` & `acore_server_config-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.3/PKG-INFO` & `acore_server_config-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_config
-Version: 0.3.3
+Version: 0.3.4
 Summary: Azerothcore World of Warcraft fleet of Servers configuration management.
 Home-page: https://github.com/MacHu-GWU/acore_server_config-project
-Download-URL: https://pypi.python.org/pypi/acore_server_config/0.3.3#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_config/0.3.4#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_config-0.3.3/README.rst` & `acore_server_config-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.3/acore_server_config/boto_ses.py` & `acore_server_config-0.3.4/acore_server_config/boto_ses.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.3/acore_server_config/config/define/main.py` & `acore_server_config-0.3.4/acore_server_config/config/define/main.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.3/acore_server_config/config/define/server.py` & `acore_server_config-0.3.4/acore_server_config/config/define/server.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.3/acore_server_config/config/init.py` & `acore_server_config-0.3.4/acore_server_config/config/init.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.3/acore_server_config/config/loader.py` & `acore_server_config-0.3.4/acore_server_config/config/loader.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.3/acore_server_config/in_ec2.py` & `acore_server_config-0.3.4/acore_server_config/in_ec2.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.3/acore_server_config/paths.py` & `acore_server_config-0.3.4/acore_server_config/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.3/acore_server_config/runtime.py` & `acore_server_config-0.3.4/acore_server_config/runtime.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,15 +36,17 @@
     batch = "batch"
     fargate = "fargate"
     unknown = "unknown"
 
 
 CURRENT_RUNTIME: str = RunTimeEnum.unknown.value
 
-if os.environ.get("HOME", "NA") == "/home/ubuntu":  # pragma: no cover
+# don't rely on $HOME env var, you may on EC2 and use sudo, then the $HOME is /root
+# but actually you are on EC2
+if os.path.exists("/home/ubuntu"):
     IS_EC2 = True
     CURRENT_RUNTIME = RunTimeEnum.ec2.value
 # if you use AWS CodeBuild for CI/CD
 # ref: https://docs.aws.amazon.com/codebuild/latest/userguide/build-env-ref-env-vars.html
 elif "CODEBUILD_CI" in os.environ:  # pragma: no cover
     IS_CODEBUILD_CI = True
     CURRENT_RUNTIME = RunTimeEnum.codebuild_ci.value
```

### Comparing `acore_server_config-0.3.3/acore_server_config/tests/mock_aws.py` & `acore_server_config-0.3.4/acore_server_config/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.3/acore_server_config/vendor/pytest_cov_helper.py` & `acore_server_config-0.3.4/acore_server_config/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.3/acore_server_config.egg-info/PKG-INFO` & `acore_server_config-0.3.4/acore_server_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-config
-Version: 0.3.3
+Version: 0.3.4
 Summary: Azerothcore World of Warcraft fleet of Servers configuration management.
 Home-page: https://github.com/MacHu-GWU/acore_server_config-project
-Download-URL: https://pypi.python.org/pypi/acore_server_config/0.3.3#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_config/0.3.4#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_config-0.3.3/acore_server_config.egg-info/SOURCES.txt` & `acore_server_config-0.3.4/acore_server_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.3/release-history.rst` & `acore_server_config-0.3.4/release-history.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.4 (2023-06-26)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- fix a bug that cannot detect it is a EC2 runtime when using ``sudo command``.
+
+
 0.3.3 (2023-06-26)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Miscellaneous**
 
 - upgrade dependencies, no API changes.
```

### Comparing `acore_server_config-0.3.3/requirements-doc.txt` & `acore_server_config-0.3.4/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.3/setup.py` & `acore_server_config-0.3.4/setup.py`

 * *Files identical despite different names*

