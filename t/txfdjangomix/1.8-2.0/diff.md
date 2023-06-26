# Comparing `tmp/txfdjangomix-1.8.tar.gz` & `tmp/txfdjangomix-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txfdjangomix-1.8.tar", last modified: Thu May 25 06:40:26 2023, max compression
+gzip compressed data, was "txfdjangomix-2.0.tar", last modified: Mon Jun 26 09:59:04 2023, max compression
```

## Comparing `txfdjangomix-1.8.tar` & `txfdjangomix-2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.342841 txfdjangomix-1.8/
--rw-rw-rw-   0        0        0    11558 2022-06-17 08:26:46.000000 txfdjangomix-1.8/LICENSE
--rw-rw-rw-   0        0        0      425 2023-05-25 06:40:26.341844 txfdjangomix-1.8/PKG-INFO
--rw-rw-rw-   0        0        0       31 2022-06-17 09:05:06.000000 txfdjangomix-1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 06:40:26.342841 txfdjangomix-1.8/setup.cfg
--rw-rw-rw-   0        0        0      875 2023-05-25 06:38:18.000000 txfdjangomix-1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.229080 txfdjangomix-1.8/txfdjangomix/
--rw-rw-rw-   0        0        0     1205 2022-06-17 02:10:26.000000 txfdjangomix-1.8/txfdjangomix/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.250024 txfdjangomix-1.8/txfdjangomix/django_log/
--rw-rw-rw-   0        0        0     1205 2022-06-13 09:56:48.000000 txfdjangomix-1.8/txfdjangomix/django_log/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.292913 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/
--rw-rw-rw-   0        0        0        0 2022-06-13 09:59:01.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/__init__.py
--rw-rw-rw-   0        0        0       66 2022-06-13 09:59:01.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/admin.py
--rw-rw-rw-   0        0        0      151 2022-06-13 09:59:01.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/apps.py
--rw-rw-rw-   0        0        0     2279 2022-06-16 09:45:23.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/insert_django_sql.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.293907 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/migrations/
--rw-rw-rw-   0        0        0        0 2022-06-13 09:59:01.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/migrations/__init__.py
--rw-rw-rw-   0        0        0      936 2022-06-16 09:32:42.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/models.py
--rw-rw-rw-   0        0        0       63 2022-06-13 09:59:01.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/tests.py
--rw-rw-rw-   0        0        0       66 2022-06-13 09:59:01.000000 txfdjangomix-1.8/txfdjangomix/django_log/sql_log/views.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.319838 txfdjangomix-1.8/txfdjangomix/django_response_middleware/
--rw-rw-rw-   0        0        0      734 2021-12-06 02:22:57.000000 txfdjangomix-1.8/txfdjangomix/django_response_middleware/__init__.py
--rw-rw-rw-   0        0        0     3219 2022-09-22 09:05:48.000000 txfdjangomix-1.8/txfdjangomix/django_response_middleware/django_response_middleware.py
--rw-rw-rw-   0        0        0     3496 2021-12-06 02:22:57.000000 txfdjangomix-1.8/txfdjangomix/django_response_middleware/response_codes.py
--rw-rw-rw-   0        0        0     3500 2023-05-25 06:38:18.000000 txfdjangomix-1.8/txfdjangomix/django_response_middleware/response_data.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.329875 txfdjangomix-1.8/txfdjangomix/django_response_middleware/utils/
--rw-rw-rw-   0        0        0        0 2021-12-06 03:12:37.000000 txfdjangomix-1.8/txfdjangomix/django_response_middleware/utils/__init__.py
--rw-rw-rw-   0        0        0     1388 2022-06-06 01:56:29.000000 txfdjangomix-1.8/txfdjangomix/django_response_middleware/utils/json_cls.py
--rw-rw-rw-   0        0        0      755 2023-05-25 06:38:18.000000 txfdjangomix-1.8/txfdjangomix/django_response_middleware/utils/type_conversion.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.340846 txfdjangomix-1.8/txfdjangomix/utils/
--rw-rw-rw-   0        0        0        0 2022-07-05 11:50:18.000000 txfdjangomix-1.8/txfdjangomix/utils/__init__.py
--rw-rw-rw-   0        0        0     6381 2022-12-16 03:10:31.000000 txfdjangomix-1.8/txfdjangomix/utils/models.py
-drwxrwxrwx   0        0        0        0 2023-05-25 06:40:26.247032 txfdjangomix-1.8/txfdjangomix.egg-info/
--rw-rw-rw-   0        0        0      425 2023-05-25 06:40:26.000000 txfdjangomix-1.8/txfdjangomix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1132 2023-05-25 06:40:26.000000 txfdjangomix-1.8/txfdjangomix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 06:40:26.000000 txfdjangomix-1.8/txfdjangomix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-25 06:40:26.000000 txfdjangomix-1.8/txfdjangomix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-25 06:40:26.000000 txfdjangomix-1.8/txfdjangomix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-07-05 11:52:46.000000 txfdjangomix-1.8/txfdjangomix.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.707639 txfdjangomix-2.0/
+-rw-rw-rw-   0        0        0    11558 2022-06-17 08:26:46.000000 txfdjangomix-2.0/LICENSE
+-rw-rw-rw-   0        0        0      425 2023-06-26 09:59:04.706642 txfdjangomix-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2022-06-17 09:05:06.000000 txfdjangomix-2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 09:59:04.707639 txfdjangomix-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      875 2023-06-26 09:58:38.000000 txfdjangomix-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.580814 txfdjangomix-2.0/txfdjangomix/
+-rw-rw-rw-   0        0        0     1205 2022-06-17 02:10:26.000000 txfdjangomix-2.0/txfdjangomix/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.605891 txfdjangomix-2.0/txfdjangomix/django_log/
+-rw-rw-rw-   0        0        0     1205 2022-06-13 09:56:48.000000 txfdjangomix-2.0/txfdjangomix/django_log/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.651061 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/
+-rw-rw-rw-   0        0        0        0 2022-06-13 09:59:01.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/__init__.py
+-rw-rw-rw-   0        0        0       66 2022-06-13 09:59:01.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/admin.py
+-rw-rw-rw-   0        0        0      151 2022-06-13 09:59:01.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/apps.py
+-rw-rw-rw-   0        0        0     2279 2022-06-16 09:45:23.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/insert_django_sql.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.652059 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/migrations/
+-rw-rw-rw-   0        0        0        0 2022-06-13 09:59:01.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/migrations/__init__.py
+-rw-rw-rw-   0        0        0      936 2022-06-16 09:32:42.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/models.py
+-rw-rw-rw-   0        0        0       63 2022-06-13 09:59:01.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/tests.py
+-rw-rw-rw-   0        0        0       66 2022-06-13 09:59:01.000000 txfdjangomix-2.0/txfdjangomix/django_log/sql_log/views.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.678986 txfdjangomix-2.0/txfdjangomix/django_response_middleware/
+-rw-rw-rw-   0        0        0      734 2021-12-06 02:22:57.000000 txfdjangomix-2.0/txfdjangomix/django_response_middleware/__init__.py
+-rw-rw-rw-   0        0        0     2313 2023-06-26 09:58:18.000000 txfdjangomix-2.0/txfdjangomix/django_response_middleware/django_response_middleware.py
+-rw-rw-rw-   0        0        0     3496 2021-12-06 02:22:57.000000 txfdjangomix-2.0/txfdjangomix/django_response_middleware/response_codes.py
+-rw-rw-rw-   0        0        0     3500 2023-05-25 06:38:18.000000 txfdjangomix-2.0/txfdjangomix/django_response_middleware/response_data.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.695671 txfdjangomix-2.0/txfdjangomix/django_response_middleware/utils/
+-rw-rw-rw-   0        0        0        0 2021-12-06 03:12:37.000000 txfdjangomix-2.0/txfdjangomix/django_response_middleware/utils/__init__.py
+-rw-rw-rw-   0        0        0     1388 2022-06-06 01:56:29.000000 txfdjangomix-2.0/txfdjangomix/django_response_middleware/utils/json_cls.py
+-rw-rw-rw-   0        0        0      755 2023-05-25 06:38:18.000000 txfdjangomix-2.0/txfdjangomix/django_response_middleware/utils/type_conversion.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.706642 txfdjangomix-2.0/txfdjangomix/utils/
+-rw-rw-rw-   0        0        0        0 2022-07-05 11:50:18.000000 txfdjangomix-2.0/txfdjangomix/utils/__init__.py
+-rw-rw-rw-   0        0        0     6381 2022-12-16 03:10:31.000000 txfdjangomix-2.0/txfdjangomix/utils/models.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:59:04.602899 txfdjangomix-2.0/txfdjangomix.egg-info/
+-rw-rw-rw-   0        0        0      425 2023-06-26 09:59:04.000000 txfdjangomix-2.0/txfdjangomix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2023-06-26 09:59:04.000000 txfdjangomix-2.0/txfdjangomix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 09:59:04.000000 txfdjangomix-2.0/txfdjangomix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-26 09:59:04.000000 txfdjangomix-2.0/txfdjangomix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-26 09:59:04.000000 txfdjangomix-2.0/txfdjangomix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-07-05 11:52:46.000000 txfdjangomix-2.0/txfdjangomix.egg-info/zip-safe
```

### Comparing `txfdjangomix-1.8/LICENSE` & `txfdjangomix-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.8/setup.py` & `txfdjangomix-2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='txfdjangomix',  # 名字
-      version='1.8',  # 版本
+      version='2.0',  # 版本
       description='django response middleware',  # 简介一般我们放在readme.md
       classifiers=[
           'Programming Language :: Python',  # python
           'Intended Audience :: Developers',  # 受众人
           'Operating System :: OS Independent',  # 系统
       ],
       long_description_content_type="text/markdown",  # 类型
```

### Comparing `txfdjangomix-1.8/txfdjangomix/__init__.py` & `txfdjangomix-2.0/txfdjangomix/__init__.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.8/txfdjangomix/django_log/__init__.py` & `txfdjangomix-2.0/txfdjangomix/django_log/__init__.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.8/txfdjangomix/django_log/sql_log/insert_django_sql.py` & `txfdjangomix-2.0/txfdjangomix/django_log/sql_log/insert_django_sql.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.8/txfdjangomix/django_log/sql_log/models.py` & `txfdjangomix-2.0/txfdjangomix/django_log/sql_log/models.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.8/txfdjangomix/django_response_middleware/__init__.py` & `txfdjangomix-2.0/txfdjangomix/django_response_middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.8/txfdjangomix/django_response_middleware/django_response_middleware.py` & `txfdjangomix-2.0/txfdjangomix/django_response_middleware/django_response_middleware.py`

 * *Files 25% similar despite different names*

```diff
@@ -43,50 +43,31 @@
                     response.data = {
                         'code': '{}'.format(response.status_code),
                         'message': 'ok',
                         'datas': data
                     }
 
             else:
-                # django抛出的异常 如dfr序列化器反序列化异常
-                # data = 错误的具体信息
 
-                # ============  返回详情  ============
-                # {
-                #     "code": "400",
-                #     "message": "error",
-                #     "datas": {
-                #         "authentication_error": [
-                #             {
-                #                 "date": "Date has wrong format. Use one of these formats instead: YYYY-MM-DD."
-                #             },
-                #             {
-                #                 "total_amount": "This field is required."
-                #             }
-                #         ]
-                #     }
-                # }
-                # ============
+                code = response.status_code
                 response.status_code = 200
-                data = response.data
-                del response.data
                 response.data = {
-                    'code': '400',
-                    'message': 'error',
-                    'datas': {'authentication_error': list_str(data)},
+                    'code': code,
+                    'message': ';'.join(list(response.data.values())),
+                    'datas': response.data,
                 }
 
         return response
 
 
 class CustomizeExceptionMiddleware(MyBaseMiddleware):
     """服务器异常不对外爆露，使用自定义"""
 
     def process_exception(self, request, exception):
         logger.error({'process_exception捕获异常': exception})
 
         return HttpResponse(
             json.dumps({'code': '06537',
-                        'message': 'server_error',
-                        'datas': {"error_info": {'error_info': '请联系无敌后台哥哥(姐姐)解决!!'}}
+                        'message': str(exception),
+                        'datas': []
                         }),
             content_type="application/json")
```

### Comparing `txfdjangomix-1.8/txfdjangomix/django_response_middleware/response_codes.py` & `txfdjangomix-2.0/txfdjangomix/django_response_middleware/response_codes.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.8/txfdjangomix/django_response_middleware/response_data.py` & `txfdjangomix-2.0/txfdjangomix/django_response_middleware/response_data.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.8/txfdjangomix/django_response_middleware/utils/json_cls.py` & `txfdjangomix-2.0/txfdjangomix/django_response_middleware/utils/json_cls.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.8/txfdjangomix/django_response_middleware/utils/type_conversion.py` & `txfdjangomix-2.0/txfdjangomix/django_response_middleware/utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.8/txfdjangomix/utils/models.py` & `txfdjangomix-2.0/txfdjangomix/utils/models.py`

 * *Files identical despite different names*

### Comparing `txfdjangomix-1.8/txfdjangomix.egg-info/SOURCES.txt` & `txfdjangomix-2.0/txfdjangomix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

