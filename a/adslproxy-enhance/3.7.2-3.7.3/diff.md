# Comparing `tmp/adslproxy-enhance-3.7.2.tar.gz` & `tmp/adslproxy-enhance-3.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adslproxy-enhance-3.7.2.tar", last modified: Fri May 26 02:20:17 2023, max compression
+gzip compressed data, was "adslproxy-enhance-3.7.3.tar", last modified: Mon Jun 26 09:27:37 2023, max compression
```

## Comparing `adslproxy-enhance-3.7.2.tar` & `adslproxy-enhance-3.7.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-26 02:20:17.484336 adslproxy-enhance-3.7.2/
--rw-r--r--   0 andylee    (501) staff       (20)     1076 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/LICENSE
--rw-r--r--   0 andylee    (501) staff       (20)     3142 2023-05-26 02:20:17.484015 adslproxy-enhance-3.7.2/PKG-INFO
--rw-r--r--   0 andylee    (501) staff       (20)     2501 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/README.md
-drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-26 02:20:17.471512 adslproxy-enhance-3.7.2/adslproxy/
--rw-r--r--   0 andylee    (501) staff       (20)      165 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/__init__.py
--rw-r--r--   0 andylee    (501) staff       (20)       94 2023-05-26 02:20:16.000000 adslproxy-enhance-3.7.2/adslproxy/__version__.py
-drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-26 02:20:17.472846 adslproxy-enhance-3.7.2/adslproxy/checker/
--rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/checker/__init__.py
--rw-r--r--   0 andylee    (501) staff       (20)     2141 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/checker/checker.py
--rw-r--r--   0 andylee    (501) staff       (20)     3871 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/cmd.py
--rw-r--r--   0 andylee    (501) staff       (20)     2229 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/db.py
-drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-26 02:20:17.474185 adslproxy-enhance-3.7.2/adslproxy/sender/
--rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/sender/__init__.py
--rw-r--r--   0 andylee    (501) staff       (20)     5028 2023-05-26 02:19:53.000000 adslproxy-enhance-3.7.2/adslproxy/sender/sender.py
-drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-26 02:20:17.475201 adslproxy-enhance-3.7.2/adslproxy/server/
--rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/server/__init__.py
--rw-r--r--   0 andylee    (501) staff       (20)     1981 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.2/adslproxy/server/server.py
--rw-r--r--   0 andylee    (501) staff       (20)     1311 2023-05-26 02:19:42.000000 adslproxy-enhance-3.7.2/adslproxy/settings.py
-drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-05-26 02:20:17.483398 adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/
--rw-r--r--   0 andylee    (501) staff       (20)     3142 2023-05-26 02:20:17.000000 adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/PKG-INFO
--rw-r--r--   0 andylee    (501) staff       (20)      547 2023-05-26 02:20:17.000000 adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/SOURCES.txt
--rw-r--r--   0 andylee    (501) staff       (20)        1 2023-05-26 02:20:17.000000 adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/dependency_links.txt
--rw-r--r--   0 andylee    (501) staff       (20)       48 2023-05-26 02:20:17.000000 adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/entry_points.txt
--rw-r--r--   0 andylee    (501) staff       (20)       47 2023-05-26 02:20:17.000000 adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/requires.txt
--rw-r--r--   0 andylee    (501) staff       (20)       10 2023-05-26 02:20:17.000000 adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/top_level.txt
--rw-r--r--   0 andylee    (501) staff       (20)       38 2023-05-26 02:20:17.484421 adslproxy-enhance-3.7.2/setup.cfg
--rw-r--r--   0 andylee    (501) staff       (20)     3338 2023-05-25 14:43:35.000000 adslproxy-enhance-3.7.2/setup.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-06-26 09:27:37.493029 adslproxy-enhance-3.7.3/
+-rw-r--r--   0 andylee    (501) staff       (20)     1076 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.3/LICENSE
+-rw-r--r--   0 andylee    (501) staff       (20)     3142 2023-06-26 09:27:37.492588 adslproxy-enhance-3.7.3/PKG-INFO
+-rw-r--r--   0 andylee    (501) staff       (20)     2501 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.3/README.md
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-06-26 09:27:37.487058 adslproxy-enhance-3.7.3/adslproxy/
+-rw-r--r--   0 andylee    (501) staff       (20)      165 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.3/adslproxy/__init__.py
+-rw-r--r--   0 andylee    (501) staff       (20)       94 2023-06-26 09:22:25.000000 adslproxy-enhance-3.7.3/adslproxy/__version__.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-06-26 09:27:37.487575 adslproxy-enhance-3.7.3/adslproxy/checker/
+-rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.3/adslproxy/checker/__init__.py
+-rw-r--r--   0 andylee    (501) staff       (20)     2141 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.3/adslproxy/checker/checker.py
+-rw-r--r--   0 andylee    (501) staff       (20)     3871 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.3/adslproxy/cmd.py
+-rw-r--r--   0 andylee    (501) staff       (20)     2229 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.3/adslproxy/db.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-06-26 09:27:37.488531 adslproxy-enhance-3.7.3/adslproxy/sender/
+-rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.3/adslproxy/sender/__init__.py
+-rw-r--r--   0 andylee    (501) staff       (20)     5049 2023-06-26 09:22:25.000000 adslproxy-enhance-3.7.3/adslproxy/sender/sender.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-06-26 09:27:37.489382 adslproxy-enhance-3.7.3/adslproxy/server/
+-rw-r--r--   0 andylee    (501) staff       (20)        0 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.3/adslproxy/server/__init__.py
+-rw-r--r--   0 andylee    (501) staff       (20)     1981 2023-05-25 13:52:29.000000 adslproxy-enhance-3.7.3/adslproxy/server/server.py
+-rw-r--r--   0 andylee    (501) staff       (20)     1376 2023-06-26 09:22:25.000000 adslproxy-enhance-3.7.3/adslproxy/settings.py
+drwxr-xr-x   0 andylee    (501) staff       (20)        0 2023-06-26 09:27:37.492038 adslproxy-enhance-3.7.3/adslproxy_enhance.egg-info/
+-rw-r--r--   0 andylee    (501) staff       (20)     3142 2023-06-26 09:27:37.000000 adslproxy-enhance-3.7.3/adslproxy_enhance.egg-info/PKG-INFO
+-rw-r--r--   0 andylee    (501) staff       (20)      547 2023-06-26 09:27:37.000000 adslproxy-enhance-3.7.3/adslproxy_enhance.egg-info/SOURCES.txt
+-rw-r--r--   0 andylee    (501) staff       (20)        1 2023-06-26 09:27:37.000000 adslproxy-enhance-3.7.3/adslproxy_enhance.egg-info/dependency_links.txt
+-rw-r--r--   0 andylee    (501) staff       (20)       48 2023-06-26 09:27:37.000000 adslproxy-enhance-3.7.3/adslproxy_enhance.egg-info/entry_points.txt
+-rw-r--r--   0 andylee    (501) staff       (20)       47 2023-06-26 09:27:37.000000 adslproxy-enhance-3.7.3/adslproxy_enhance.egg-info/requires.txt
+-rw-r--r--   0 andylee    (501) staff       (20)       10 2023-06-26 09:27:37.000000 adslproxy-enhance-3.7.3/adslproxy_enhance.egg-info/top_level.txt
+-rw-r--r--   0 andylee    (501) staff       (20)       38 2023-06-26 09:27:37.493176 adslproxy-enhance-3.7.3/setup.cfg
+-rw-r--r--   0 andylee    (501) staff       (20)     3338 2023-05-25 14:43:35.000000 adslproxy-enhance-3.7.3/setup.py
```

### Comparing `adslproxy-enhance-3.7.2/LICENSE` & `adslproxy-enhance-3.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.7.2/PKG-INFO` & `adslproxy-enhance-3.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adslproxy-enhance
-Version: 3.7.2
+Version: 3.7.3
 Summary: ADSL Proxy Pool Tool 
 Home-page: https://github.com/thefantasystudio/AdslProxy
 Author: Germey
 Author-email: cqc@cuiqingcai.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `adslproxy-enhance-3.7.2/README.md` & `adslproxy-enhance-3.7.3/README.md`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.7.2/adslproxy/checker/checker.py` & `adslproxy-enhance-3.7.3/adslproxy/checker/checker.py`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.7.2/adslproxy/cmd.py` & `adslproxy-enhance-3.7.3/adslproxy/cmd.py`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.7.2/adslproxy/db.py` & `adslproxy-enhance-3.7.3/adslproxy/db.py`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.7.2/adslproxy/sender/sender.py` & `adslproxy-enhance-3.7.3/adslproxy/sender/sender.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 'https': 'http://' + proxy
             }, timeout=TEST_TIMEOUT)
             if response.status_code == 200:
                 return True
         except (ConnectionError, ReadTimeout):
             return False
 
-    @retry(retry_on_result=lambda x: x is not True, stop_max_attempt_number=10)
+    @retry(retry_on_result=lambda x: x is not True, stop_max_attempt_number=STOP_MAX_ATTEMPT_NUMBER)
     def remove_proxy(self):
         """
         移除代理
         :return: None
         """
         logger.info(f'Removing {CLIENT_NAME}...')
         try:
```

### Comparing `adslproxy-enhance-3.7.2/adslproxy/server/server.py` & `adslproxy-enhance-3.7.3/adslproxy/server/server.py`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.7.2/adslproxy/settings.py` & `adslproxy-enhance-3.7.3/adslproxy/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 # Redis数据库密码, 如无则填None
 REDIS_PASSWORD = env.str('REDIS_PASSWORD', '1111')
 # Redis数据库端口
 REDIS_PORT = env.int('REDIS_PORT', 33479)
 # 代理池键名
 REDIS_KEY = env.str('REDIS_KEY', 'adsl')
 
+STOP_MAX_ATTEMPT_NUMBER = env.int('STOP_MAX_ATTEMPT_NUMBER', 1)
+
 # 测试URL
 TEST_URL = env.str('TEST_URL', 'http://www.baidu.com')
 # 测试最大失败次数
 TEST_MAX_ERROR_COUNT = env.int('TEST_MAX_ERROR_COUNT', 10)
 # 测试超时时间
 TEST_TIMEOUT = env.int('TEST_TIMEOUT', 20)
 # 测试周期
```

### Comparing `adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/PKG-INFO` & `adslproxy-enhance-3.7.3/adslproxy_enhance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adslproxy-enhance
-Version: 3.7.2
+Version: 3.7.3
 Summary: ADSL Proxy Pool Tool 
 Home-page: https://github.com/thefantasystudio/AdslProxy
 Author: Germey
 Author-email: cqc@cuiqingcai.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `adslproxy-enhance-3.7.2/adslproxy_enhance.egg-info/SOURCES.txt` & `adslproxy-enhance-3.7.3/adslproxy_enhance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adslproxy-enhance-3.7.2/setup.py` & `adslproxy-enhance-3.7.3/setup.py`

 * *Files identical despite different names*

