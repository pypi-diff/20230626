# Comparing `tmp/auth-token-django-0.0.2.tar.gz` & `tmp/auth-token-django-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth-token-django-0.0.2.tar", last modified: Wed Jun  7 15:33:52 2023, max compression
+gzip compressed data, was "auth-token-django-0.0.3.tar", last modified: Mon Jun 26 11:15:20 2023, max compression
```

## Comparing `auth-token-django-0.0.2.tar` & `auth-token-django-0.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.205059 auth-token-django-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-06-07 15:33:52.205059 auth-token-django-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.201058 auth-token-django-0.0.2/auth_token_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-06-07 15:33:52.000000 auth-token-django-0.0.2/auth_token_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-06-07 15:33:52.000000 auth-token-django-0.0.2/auth_token_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 15:33:52.000000 auth-token-django-0.0.2/auth_token_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-07 15:33:52.000000 auth-token-django-0.0.2/auth_token_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-07 15:33:52.000000 auth-token-django-0.0.2/auth_token_django.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.201058 auth-token-django-0.0.2/djangoauthtoken/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.201058 auth-token-django-0.0.2/djangoauthtoken/middleware/
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/middleware/token_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.201058 auth-token-django-0.0.2/djangoauthtoken/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     6688 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.201058 auth-token-django-0.0.2/djangoauthtoken/models/
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      331 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/models/base_relation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.205059 auth-token-django-0.0.2/djangoauthtoken/models/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/models/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/models/custom_fields/case_insensitive_email_field.py
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/models/token.py
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/models/token_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.205059 auth-token-django-0.0.2/djangoauthtoken/serializers/
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/serializers/user.py
--rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.205059 auth-token-django-0.0.2/djangoauthtoken/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/utils/csrf_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      263 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/utils/datetime_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.205059 auth-token-django-0.0.2/djangoauthtoken/views/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/views/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/views/refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/views/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/views/user.py
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-07 15:33:52.205059 auth-token-django-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.135511 auth-token-django-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-06-26 11:15:20.135511 auth-token-django-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.127511 auth-token-django-0.0.3/auth_token_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-06-26 11:15:20.000000 auth-token-django-0.0.3/auth_token_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-06-26 11:15:20.000000 auth-token-django-0.0.3/auth_token_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 11:15:20.000000 auth-token-django-0.0.3/auth_token_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-26 11:15:20.000000 auth-token-django-0.0.3/auth_token_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-26 11:15:20.000000 auth-token-django-0.0.3/auth_token_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.127511 auth-token-django-0.0.3/djangoauthtoken/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.127511 auth-token-django-0.0.3/djangoauthtoken/middleware/
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/middleware/token_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.131511 auth-token-django-0.0.3/djangoauthtoken/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     6688 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.131511 auth-token-django-0.0.3/djangoauthtoken/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      331 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/models/base_relation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.131511 auth-token-django-0.0.3/djangoauthtoken/models/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/models/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/models/custom_fields/case_insensitive_email_field.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/models/token_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.131511 auth-token-django-0.0.3/djangoauthtoken/serializers/
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/serializers/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.135511 auth-token-django-0.0.3/djangoauthtoken/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/utils/csrf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/utils/datetime_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.135511 auth-token-django-0.0.3/djangoauthtoken/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/views/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/views/refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/views/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/views/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 11:15:20.135511 auth-token-django-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/setup.py
```

### Comparing `auth-token-django-0.0.2/PKG-INFO` & `auth-token-django-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-token-django
-Version: 0.0.2
+Version: 0.0.3
 Summary: Django token authentication
 Home-page: https://github.com/Shivin01/django_auth_token
 Author: Shivin Agarwal
 Author-email: shivin.agarwal15@gmail.com
 Keywords: django auth token
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `auth-token-django-0.0.2/README.md` & `auth-token-django-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.2/auth_token_django.egg-info/PKG-INFO` & `auth-token-django-0.0.3/auth_token_django.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-token-django
-Version: 0.0.2
+Version: 0.0.3
 Summary: Django token authentication
 Home-page: https://github.com/Shivin01/django_auth_token
 Author: Shivin Agarwal
 Author-email: shivin.agarwal15@gmail.com
 Keywords: django auth token
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `auth-token-django-0.0.2/auth_token_django.egg-info/SOURCES.txt` & `auth-token-django-0.0.3/auth_token_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.2/auth_token_django.egg-info/requires.txt` & `auth-token-django-0.0.3/auth_token_django.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.2/djangoauthtoken/middleware/token_authentication.py` & `auth-token-django-0.0.3/djangoauthtoken/middleware/token_authentication.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.2/djangoauthtoken/migrations/0001_initial.py` & `auth-token-django-0.0.3/djangoauthtoken/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.2/djangoauthtoken/models/token.py` & `auth-token-django-0.0.3/djangoauthtoken/models/token.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.2/djangoauthtoken/models/token_user.py` & `auth-token-django-0.0.3/djangoauthtoken/models/token_user.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.2/djangoauthtoken/settings.py` & `auth-token-django-0.0.3/djangoauthtoken/settings.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.2/djangoauthtoken/urls.py` & `auth-token-django-0.0.3/djangoauthtoken/urls.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.2/djangoauthtoken/views/login.py` & `auth-token-django-0.0.3/djangoauthtoken/views/login.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.2/djangoauthtoken/views/refresh_token.py` & `auth-token-django-0.0.3/djangoauthtoken/views/refresh_token.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.2/djangoauthtoken/views/sign_up.py` & `auth-token-django-0.0.3/djangoauthtoken/views/sign_up.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,18 @@
         data = request.data
         username = data['username']
         email = data['email']
         password = data['password']
 
         user, exists = TokenUser.objects.get_or_create(
             username=username,
-            email=email,
-            password=password
+            email=email
         )
+        user.set_password(password)
+        user.save()
 
         if not exists:
             raise Exception
         
         return Response({
             "username": user.username,
             "email": user.email,
```

### Comparing `auth-token-django-0.0.2/setup.py` & `auth-token-django-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             install_requires.append(line)
     return install_requires
 
 
 setup(
     name='auth-token-django',
     description='Django token authentication',
-    version = "0.0.2",
+    version = "0.0.3",
     author='Shivin Agarwal',
     long_description=get_file_contents('README.md'),
     author_email='shivin.agarwal15@gmail.com',
     url='https://github.com/Shivin01/django_auth_token',
     classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

