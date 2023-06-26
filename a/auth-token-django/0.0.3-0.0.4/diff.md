# Comparing `tmp/auth-token-django-0.0.3.tar.gz` & `tmp/auth-token-django-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth-token-django-0.0.3.tar", last modified: Mon Jun 26 11:15:20 2023, max compression
+gzip compressed data, was "auth-token-django-0.0.4.tar", last modified: Mon Jun 26 11:20:01 2023, max compression
```

## Comparing `auth-token-django-0.0.3.tar` & `auth-token-django-0.0.4.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.135511 auth-token-django-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-06-26 11:15:20.135511 auth-token-django-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.127511 auth-token-django-0.0.3/auth_token_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-06-26 11:15:20.000000 auth-token-django-0.0.3/auth_token_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-06-26 11:15:20.000000 auth-token-django-0.0.3/auth_token_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 11:15:20.000000 auth-token-django-0.0.3/auth_token_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-26 11:15:20.000000 auth-token-django-0.0.3/auth_token_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-26 11:15:20.000000 auth-token-django-0.0.3/auth_token_django.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.127511 auth-token-django-0.0.3/djangoauthtoken/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.127511 auth-token-django-0.0.3/djangoauthtoken/middleware/
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/middleware/token_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.131511 auth-token-django-0.0.3/djangoauthtoken/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     6688 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.131511 auth-token-django-0.0.3/djangoauthtoken/models/
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      331 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/models/base_relation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.131511 auth-token-django-0.0.3/djangoauthtoken/models/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/models/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/models/custom_fields/case_insensitive_email_field.py
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/models/token.py
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/models/token_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.131511 auth-token-django-0.0.3/djangoauthtoken/serializers/
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/serializers/user.py
--rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.135511 auth-token-django-0.0.3/djangoauthtoken/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/utils/csrf_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      263 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/utils/datetime_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:15:20.135511 auth-token-django-0.0.3/djangoauthtoken/views/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/views/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/views/refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/views/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/views/user.py
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/djangoauthtoken/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 11:15:20.135511 auth-token-django-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-26 11:15:07.000000 auth-token-django-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:20:01.588117 auth-token-django-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-06-26 11:20:01.588117 auth-token-django-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:20:01.584117 auth-token-django-0.0.4/auth_token_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-06-26 11:20:01.000000 auth-token-django-0.0.4/auth_token_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-06-26 11:20:01.000000 auth-token-django-0.0.4/auth_token_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 11:20:01.000000 auth-token-django-0.0.4/auth_token_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-26 11:20:01.000000 auth-token-django-0.0.4/auth_token_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-26 11:20:01.000000 auth-token-django-0.0.4/auth_token_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:20:01.584117 auth-token-django-0.0.4/djangoauthtoken/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:20:01.584117 auth-token-django-0.0.4/djangoauthtoken/middleware/
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/middleware/token_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:20:01.584117 auth-token-django-0.0.4/djangoauthtoken/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     6688 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/migrations/0002_alter_tokenuser_email.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:20:01.584117 auth-token-django-0.0.4/djangoauthtoken/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      331 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/models/base_relation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:20:01.584117 auth-token-django-0.0.4/djangoauthtoken/models/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/models/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/models/custom_fields/case_insensitive_email_field.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/models/token_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:20:01.584117 auth-token-django-0.0.4/djangoauthtoken/serializers/
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/serializers/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:20:01.584117 auth-token-django-0.0.4/djangoauthtoken/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/utils/csrf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/utils/datetime_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:20:01.588117 auth-token-django-0.0.4/djangoauthtoken/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/views/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/views/refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/views/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/views/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/djangoauthtoken/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 11:20:01.588117 auth-token-django-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-26 11:19:47.000000 auth-token-django-0.0.4/setup.py
```

### Comparing `auth-token-django-0.0.3/PKG-INFO` & `auth-token-django-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-token-django
-Version: 0.0.3
+Version: 0.0.4
 Summary: Django token authentication
 Home-page: https://github.com/Shivin01/django_auth_token
 Author: Shivin Agarwal
 Author-email: shivin.agarwal15@gmail.com
 Keywords: django auth token
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `auth-token-django-0.0.3/README.md` & `auth-token-django-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.3/auth_token_django.egg-info/PKG-INFO` & `auth-token-django-0.0.4/auth_token_django.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-token-django
-Version: 0.0.3
+Version: 0.0.4
 Summary: Django token authentication
 Home-page: https://github.com/Shivin01/django_auth_token
 Author: Shivin Agarwal
 Author-email: shivin.agarwal15@gmail.com
 Keywords: django auth token
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `auth-token-django-0.0.3/auth_token_django.egg-info/SOURCES.txt` & `auth-token-django-0.0.4/auth_token_django.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 djangoauthtoken/asgi.py
 djangoauthtoken/settings.py
 djangoauthtoken/urls.py
 djangoauthtoken/wsgi.py
 djangoauthtoken/middleware/__init__.py
 djangoauthtoken/middleware/token_authentication.py
 djangoauthtoken/migrations/0001_initial.py
+djangoauthtoken/migrations/0002_alter_tokenuser_email.py
 djangoauthtoken/migrations/__init__.py
 djangoauthtoken/models/__init__.py
 djangoauthtoken/models/base_relation.py
 djangoauthtoken/models/token.py
 djangoauthtoken/models/token_user.py
 djangoauthtoken/models/custom_fields/__init__.py
 djangoauthtoken/models/custom_fields/case_insensitive_email_field.py
```

### Comparing `auth-token-django-0.0.3/auth_token_django.egg-info/requires.txt` & `auth-token-django-0.0.4/auth_token_django.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.3/djangoauthtoken/middleware/token_authentication.py` & `auth-token-django-0.0.4/djangoauthtoken/middleware/token_authentication.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.3/djangoauthtoken/migrations/0001_initial.py` & `auth-token-django-0.0.4/djangoauthtoken/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.3/djangoauthtoken/models/token.py` & `auth-token-django-0.0.4/djangoauthtoken/models/token.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.3/djangoauthtoken/models/token_user.py` & `auth-token-django-0.0.4/djangoauthtoken/models/token_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 
 phone_regex = RegexValidator(
     regex=r'^\+?1?\d{9,15}',
     message="Phone numbers must be in International format: '+14169058762'. Up to 15 digits "
 )
 
 class TokenUser(AbstractUser, Base):
-    email = CaseInsensitiveEmailField(max_length=Base.MAX_LENGTH_MEDIUM)
+    email = CaseInsensitiveEmailField(max_length=Base.MAX_LENGTH_MEDIUM, unique=True)
     phone_number = models.CharField(validators=[phone_regex], max_length=17)
     
     def __str__(self) -> str:
         return self.email
```

### Comparing `auth-token-django-0.0.3/djangoauthtoken/settings.py` & `auth-token-django-0.0.4/djangoauthtoken/settings.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.3/djangoauthtoken/urls.py` & `auth-token-django-0.0.4/djangoauthtoken/urls.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.3/djangoauthtoken/views/login.py` & `auth-token-django-0.0.4/djangoauthtoken/views/login.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.3/djangoauthtoken/views/refresh_token.py` & `auth-token-django-0.0.4/djangoauthtoken/views/refresh_token.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     """
     try:
         data = request.data
         refresh_token = data['refresh_token']
         refresh_token_decode = jwt.decode(refresh_token,
                                         settings.JWT_SECRET,
                                         algorithms=settings.JWT_ALGO)
-
-        print(refresh_token_decode)
-
+        # Check for user.
         user = TokenUser.objects.get(id=refresh_token_decode['user_id'])
-        user_token = Token.objects.get(user=user, refresh_token=refresh_token)
+        # check for token.
+        Token.objects.get(user=user, refresh_token=refresh_token)
+        # save new token.
         token = Token(user=user)
         token.save()
         print(token.id)
 
         return Response({
                     "id": user.id,
                     "username": user.username,
```

### Comparing `auth-token-django-0.0.3/djangoauthtoken/views/sign_up.py` & `auth-token-django-0.0.4/djangoauthtoken/views/sign_up.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.3/setup.py` & `auth-token-django-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             install_requires.append(line)
     return install_requires
 
 
 setup(
     name='auth-token-django',
     description='Django token authentication',
-    version = "0.0.3",
+    version = "0.0.4",
     author='Shivin Agarwal',
     long_description=get_file_contents('README.md'),
     author_email='shivin.agarwal15@gmail.com',
     url='https://github.com/Shivin01/django_auth_token',
     classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

