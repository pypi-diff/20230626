# Comparing `tmp/django-envconfig-0.2.7.tar.gz` & `tmp/django-envconfig-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-envconfig-0.2.7.tar", last modified: Mon Apr  3 23:43:46 2023, max compression
+gzip compressed data, was "django-envconfig-0.3.0.tar", last modified: Mon Jun 26 04:17:10 2023, max compression
```

## Comparing `django-envconfig-0.2.7.tar` & `django-envconfig-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:43:46.675422 django-envconfig-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-03 23:43:35.000000 django-envconfig-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-04-03 23:43:46.675422 django-envconfig-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-03 23:43:35.000000 django-envconfig-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:43:46.675422 django-envconfig-0.2.7/django_envconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-04-03 23:43:46.000000 django-envconfig-0.2.7/django_envconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-03 23:43:46.000000 django-envconfig-0.2.7/django_envconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 23:43:46.000000 django-envconfig-0.2.7/django_envconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-03 23:43:46.000000 django-envconfig-0.2.7/django_envconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-03 23:43:46.000000 django-envconfig-0.2.7/django_envconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:43:46.675422 django-envconfig-0.2.7/envconfig/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 23:43:35.000000 django-envconfig-0.2.7/envconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-03 23:43:35.000000 django-envconfig-0.2.7/envconfig/dotenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-03 23:43:35.000000 django-envconfig-0.2.7/envconfig/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-04-03 23:43:35.000000 django-envconfig-0.2.7/envconfig/setting_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-03 23:43:35.000000 django-envconfig-0.2.7/envconfig/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-03 23:43:35.000000 django-envconfig-0.2.7/envconfig/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-03 23:43:35.000000 django-envconfig-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-03 23:43:46.675422 django-envconfig-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:43:46.675422 django-envconfig-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-03 23:43:35.000000 django-envconfig-0.2.7/tests/test_setting_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-03 23:43:35.000000 django-envconfig-0.2.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:17:10.260218 django-envconfig-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-26 04:16:53.000000 django-envconfig-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-26 04:17:10.260218 django-envconfig-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-26 04:16:53.000000 django-envconfig-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:17:10.256217 django-envconfig-0.3.0/django_envconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-26 04:17:10.000000 django-envconfig-0.3.0/django_envconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 04:17:10.000000 django-envconfig-0.3.0/django_envconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 04:17:10.000000 django-envconfig-0.3.0/django_envconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 04:17:10.000000 django-envconfig-0.3.0/django_envconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 04:17:10.000000 django-envconfig-0.3.0/django_envconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:17:10.256217 django-envconfig-0.3.0/envconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 04:16:53.000000 django-envconfig-0.3.0/envconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-26 04:16:53.000000 django-envconfig-0.3.0/envconfig/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-26 04:16:53.000000 django-envconfig-0.3.0/envconfig/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 04:16:53.000000 django-envconfig-0.3.0/envconfig/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-06-26 04:16:53.000000 django-envconfig-0.3.0/envconfig/setting_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-26 04:16:53.000000 django-envconfig-0.3.0/envconfig/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-26 04:16:53.000000 django-envconfig-0.3.0/envconfig/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-26 04:16:53.000000 django-envconfig-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 04:17:10.260218 django-envconfig-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:17:10.260218 django-envconfig-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-26 04:16:53.000000 django-envconfig-0.3.0/tests/test_setting_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-26 04:16:53.000000 django-envconfig-0.3.0/tests/test_utils.py
```

### Comparing `django-envconfig-0.2.7/LICENSE` & `django-envconfig-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-envconfig-0.2.7/PKG-INFO` & `django-envconfig-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: django-envconfig
-Version: 0.2.7
+Version: 0.3.0
 Summary: Configure Django using environment variables.
-Home-page: https://github.com/ely-as/django-envconfig
-Author: Elyas Khan
-Author-email: mail@ely.as
+Author-email: elyas <elyas@ely.as>
 License: MIT
+Project-URL: Issue Tracker, https://github.com/ely-as/django-envconfig/issues
 Project-URL: Source, https://github.com/ely-as/django-envconfig
-Project-URL: Tracker, https://github.com/ely-as/django-envconfig/issues
+Keywords: django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
@@ -27,21 +25,24 @@
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # django-envconfig
 
-![Test](https://github.com/ely-as/django-envconfig/workflows/Test/badge.svg)
-![License](https://img.shields.io/pypi/l/django-envconfig)
+[![Test](https://github.com/ely-as/django-envconfig/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ely-as/django-envconfig/actions/workflows/test.yml)
+[![Coverage](https://cov.ely.as/github/ely-as/django-envconfig/main/badge.svg)](https://cov.ely.as/github/ely-as/django-envconfig/main/latest/)
+[![Version](https://img.shields.io/pypi/v/django-envconfig)](https://pypi.org/project/django-envconfig/)
 
 ![Django](https://img.shields.io/pypi/djversions/django-envconfig)
 ![Python](https://img.shields.io/pypi/pyversions/django-envconfig)
 
 Configure Django using environment variables (envvars). `settings.py` optional.
 
 ## Getting started
```

### Comparing `django-envconfig-0.2.7/README.md` & `django-envconfig-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # django-envconfig
 
-![Test](https://github.com/ely-as/django-envconfig/workflows/Test/badge.svg)
-![License](https://img.shields.io/pypi/l/django-envconfig)
+[![Test](https://github.com/ely-as/django-envconfig/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ely-as/django-envconfig/actions/workflows/test.yml)
+[![Coverage](https://cov.ely.as/github/ely-as/django-envconfig/main/badge.svg)](https://cov.ely.as/github/ely-as/django-envconfig/main/latest/)
+[![Version](https://img.shields.io/pypi/v/django-envconfig)](https://pypi.org/project/django-envconfig/)
 
 ![Django](https://img.shields.io/pypi/djversions/django-envconfig)
 ![Python](https://img.shields.io/pypi/pyversions/django-envconfig)
 
 Configure Django using environment variables (envvars). `settings.py` optional.
 
 ## Getting started
```

### Comparing `django-envconfig-0.2.7/django_envconfig.egg-info/PKG-INFO` & `django-envconfig-0.3.0/django_envconfig.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: django-envconfig
-Version: 0.2.7
+Version: 0.3.0
 Summary: Configure Django using environment variables.
-Home-page: https://github.com/ely-as/django-envconfig
-Author: Elyas Khan
-Author-email: mail@ely.as
+Author-email: elyas <elyas@ely.as>
 License: MIT
+Project-URL: Issue Tracker, https://github.com/ely-as/django-envconfig/issues
 Project-URL: Source, https://github.com/ely-as/django-envconfig
-Project-URL: Tracker, https://github.com/ely-as/django-envconfig/issues
+Keywords: django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
@@ -27,21 +25,24 @@
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # django-envconfig
 
-![Test](https://github.com/ely-as/django-envconfig/workflows/Test/badge.svg)
-![License](https://img.shields.io/pypi/l/django-envconfig)
+[![Test](https://github.com/ely-as/django-envconfig/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ely-as/django-envconfig/actions/workflows/test.yml)
+[![Coverage](https://cov.ely.as/github/ely-as/django-envconfig/main/badge.svg)](https://cov.ely.as/github/ely-as/django-envconfig/main/latest/)
+[![Version](https://img.shields.io/pypi/v/django-envconfig)](https://pypi.org/project/django-envconfig/)
 
 ![Django](https://img.shields.io/pypi/djversions/django-envconfig)
 ![Python](https://img.shields.io/pypi/pyversions/django-envconfig)
 
 Configure Django using environment variables (envvars). `settings.py` optional.
 
 ## Getting started
```

### Comparing `django-envconfig-0.2.7/envconfig/dotenv.py` & `django-envconfig-0.3.0/envconfig/dotenv.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dotenv import find_dotenv as _find_dotenv
 
 MAX_DEPTH: int = 10
 
 
 def find_dotenv(
-    filename: str = '.env',
+    filename: str = ".env",
     raise_error_if_not_found: bool = False,
     usecwd: bool = False,
     extra_paths: Optional[Sequence[Union[Path, str]]] = None,
 ) -> str:
     """Find the path to a relevant dotenv file, or return an empty string.
 
     Extends :py:func:`dotenv.find_dotenv` by also searching in the execution
@@ -40,9 +40,9 @@
                 if (path / filename).is_file():
                     dotenv_path = str((path / filename).resolve())
                 path = path.parent
             # Return the first dotenv we find
             if dotenv_path:
                 break
     if not dotenv_path and raise_error_if_not_found:
-        raise IOError('File not found')
+        raise IOError("File not found")
     return dotenv_path
```

### Comparing `django-envconfig-0.2.7/envconfig/parser.py` & `django-envconfig-0.3.0/envconfig/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import Any, Union
 import json
 from json.decoder import JSONDecodeError
+from typing import Any, Union
 
 NoneType: type = type(None)
 
 
 class EnvParser:
     # case insensitive
-    bool_true_vals = ('1', 'on', 'true', 'yes')
-    bool_false_vals = ('0', 'off', 'false', 'no')
-    none_vals = ('none', 'null')
+    bool_true_vals = ("1", "on", "true", "yes")
+    bool_false_vals = ("0", "off", "false", "no")
+    none_vals = ("none", "null")
 
     @classmethod
     def parse(cls, val: str, *expected_types: type) -> Any:
         # Evaluate NoneType first if it's an expected type
         types_ = list(expected_types)
         if NoneType in types_ and types_[0] != NoneType:
             types_.insert(0, types_.pop(types_.index(NoneType)))
         # Attempt to parse val as each type. If all fails raise last ValueError
         for i, type_ in enumerate(types_, start=1):
             try:
-                return getattr(cls, f'_{type_.__name__}')(val)
+                return getattr(cls, f"_{type_.__name__}")(val)
             except ValueError:
                 if i < len(types_):
                     pass
                 else:
                     raise
 
     @classmethod
@@ -44,32 +44,32 @@
 
     @classmethod
     def _float(cls, val: str) -> float:
         return float(val)
 
     @classmethod
     def _int(cls, val: str) -> int:
-        if val.startswith('0o'):
+        if val.startswith("0o"):
             return int(val, 8)
-        elif val.startswith('0x'):
+        elif val.startswith("0x"):
             return int(val, 16)
         return int(val)
 
     @classmethod
     def _json(cls, val: str) -> Union[dict, list]:
         try:
             return json.loads(val)
         except JSONDecodeError:
-            raise ValueError("Invalid JSON")
+            raise ValueError("Invalid JSON") from None
 
     @classmethod
     def _list(cls, val: str) -> list:
-        if val.startswith('['):
+        if val.startswith("["):
             return cls._json(val)  # type: ignore  # noqa
-        return val.split(',')
+        return val.split(",")
 
     @classmethod
     def _NoneType(cls, val: str) -> None:
         if val.lower() in cls.none_vals:
             return
         raise ValueError  # don't need a message
```

### Comparing `django-envconfig-0.2.7/envconfig/setting_types.py` & `django-envconfig-0.3.0/envconfig/setting_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,180 +1,187 @@
 from typing import Dict, List
 
 # NOTE(elyas): pydantic (or similar) may offer a more robust method of
 # defining setting types. For example, JSON does not support storing Python
 # tuples, but settings like ADMINS (i.e. List[Tuple[str, str]]) may require
 # list elements to be cast to tuple.
 _setting_types: Dict[str, List[type]] = {
-    'ABSOLUTE_URL_OVERRIDES': [dict],
-    'ADMINS': [list],
-    'ALLOWED_HOSTS': [list],
-    'APPEND_SLASH': [bool],
-    'AUTHENTICATION_BACKENDS': [list],
-    'AUTH_PASSWORD_VALIDATORS': [list],
-    'AUTH_USER_MODEL': [str],
-    'CACHES': [dict],
-    'CACHE_MIDDLEWARE_ALIAS': [str],
-    'CACHE_MIDDLEWARE_KEY_PREFIX': [str],
-    'CACHE_MIDDLEWARE_SECONDS': [int],
-    'CSRF_COOKIE_AGE': [type(None), int],
-    'CSRF_COOKIE_DOMAIN': [type(None), str],
-    'CSRF_COOKIE_HTTPONLY': [bool],
-    'CSRF_COOKIE_MASKED': [bool],
-    'CSRF_COOKIE_NAME': [str],
-    'CSRF_COOKIE_PATH': [str],
-    'CSRF_COOKIE_SAMESITE': [str],  # 'None' is a valid str value, so don't coerce to NoneType  # noqa: E501
-    'CSRF_COOKIE_SECURE': [bool],
-    'CSRF_FAILURE_VIEW': [str],
-    'CSRF_HEADER_NAME': [str],
-    'CSRF_TRUSTED_ORIGINS': [list],
-    'CSRF_USE_SESSIONS': [bool],
-    'DATABASES': [dict],
-    'DATABASE_ROUTERS': [list],
-    'DATA_UPLOAD_MAX_MEMORY_SIZE': [type(None), int],
-    'DATA_UPLOAD_MAX_NUMBER_FIELDS': [type(None), int],
-    'DATA_UPLOAD_MAX_NUMBER_FILES': [int],
-    'DATETIME_FORMAT': [str],
-    'DATETIME_INPUT_FORMATS': [list],
-    'DATE_FORMAT': [str],
-    'DATE_INPUT_FORMATS': [list],
-    'DEBUG': [bool],
-    'DEBUG_PROPAGATE_EXCEPTIONS': [bool],
-    'DECIMAL_SEPARATOR': [str],
-    'DEFAULT_AUTO_FIELD': [str],
-    'DEFAULT_CHARSET': [str],
-    'DEFAULT_CONTENT_TYPE': [str],  # deprecated v2.0, removed v3.0
-    'DEFAULT_EXCEPTION_REPORTER': [str],
-    'DEFAULT_EXCEPTION_REPORTER_FILTER': [str],
-    'DEFAULT_FILE_STORAGE': [str],  # deprecated v4.2
-    'DEFAULT_FROM_EMAIL': [str],
-    'DEFAULT_HASHING_ALGORITHM': [str],
-    'DEFAULT_INDEX_TABLESPACE': [str],
-    'DEFAULT_TABLESPACE': [str],
-    'DISALLOWED_USER_AGENTS': [list],
-    'EMAIL_BACKEND': [str],
-    'EMAIL_HOST': [str],
-    'EMAIL_HOST_PASSWORD': [str],
-    'EMAIL_HOST_USER': [str],
-    'EMAIL_PORT': [int],
-    'EMAIL_SSL_CERTFILE': [type(None), str],
-    'EMAIL_SSL_KEYFILE': [type(None), str],
-    'EMAIL_SUBJECT_PREFIX': [str],
-    'EMAIL_TIMEOUT': [type(None), int],
-    'EMAIL_USE_LOCALTIME': [bool],
-    'EMAIL_USE_SSL': [bool],
-    'EMAIL_USE_TLS': [bool],
-    'FILE_CHARSET': [str],  # deprecated v2.2, removed v3.1
-    'FILE_UPLOAD_DIRECTORY_PERMISSIONS': [type(None), str],
-    'FILE_UPLOAD_HANDLERS': [list],
-    'FILE_UPLOAD_MAX_MEMORY_SIZE': [int],
-    'FILE_UPLOAD_PERMISSIONS': [type(None), int],
-    'FILE_UPLOAD_TEMP_DIR': [type(None), str],
-    'FIRST_DAY_OF_WEEK': [int],
-    'FIXTURE_DIRS': [list],
-    'FORCE_SCRIPT_NAME': [type(None), str],
-    'FORMAT_MODULE_PATH': [type(None), str, list],
-    'FORM_RENDERER': [str],
-    'IGNORABLE_404_URLS': [list],
-    'INSTALLED_APPS': [list],
-    'INTERNAL_IPS': [list],
-    'LANGUAGES': [list],
-    'LANGUAGES_BIDI': [list],
-    'LANGUAGE_CODE': [str],
-    'LANGUAGE_COOKIE_AGE': [type(None), int],
-    'LANGUAGE_COOKIE_DOMAIN': [type(None), str],
-    'LANGUAGE_COOKIE_HTTPONLY': [bool],
-    'LANGUAGE_COOKIE_NAME': [str],
-    'LANGUAGE_COOKIE_PATH': [str],
-    'LANGUAGE_COOKIE_SAMESITE': [type(None), str],
-    'LANGUAGE_COOKIE_SECURE': [bool],
-    'LOCALE_PATHS': [list],
-    'LOGGING': [dict],
-    'LOGGING_CONFIG': [type(None), str],
-    'LOGIN_REDIRECT_URL': [str],
-    'LOGIN_URL': [str],
-    'LOGOUT_REDIRECT_URL': [type(None), str],
-    'MANAGERS': [list],
-    'MEDIA_ROOT': [str],
-    'MEDIA_URL': [str],
-    'MESSAGE_STORAGE': [str],
-    'MIDDLEWARE': [type(None), list],
-    'MIDDLEWARE_CLASSES': [list],  # deprecated v1.10, removed v2.0
-    'MIGRATION_MODULES': [dict],
-    'MONTH_DAY_FORMAT': [str],
-    'NUMBER_GROUPING': [int],
-    'PASSWORD_HASHERS': [list],
-    'PASSWORD_RESET_TIMEOUT': [int],
-    'PASSWORD_RESET_TIMEOUT_DAYS': [int],
-    'PREPEND_WWW': [bool],
-    'SECRET_KEY': [str],
-    'SECRET_KEY_FALLBACKS': [list],
-    'SECURE_BROWSER_XSS_FILTER': [bool],
-    'SECURE_CONTENT_TYPE_NOSNIFF': [bool],
-    'SECURE_HSTS_INCLUDE_SUBDOMAINS': [bool],
-    'SECURE_HSTS_PRELOAD': [bool],
-    'SECURE_HSTS_SECONDS': [int],
-    'SECURE_CROSS_ORIGIN_OPENER_POLICY': [type(None), str],
-    'SECURE_PROXY_SSL_HEADER': [type(None), tuple],
-    'SECURE_REDIRECT_EXEMPT': [list],
-    'SECURE_REFERRER_POLICY': [type(None), str],  # v3.0 default None, v3.1 default str  # noqa: E501
-    'SECURE_SSL_HOST': [type(None), str],
-    'SECURE_SSL_REDIRECT': [bool],
-    'SERVER_EMAIL': [str],
-    'SESSION_CACHE_ALIAS': [str],
-    'SESSION_COOKIE_AGE': [int],
-    'SESSION_COOKIE_DOMAIN': [type(None), str],
-    'SESSION_COOKIE_HTTPONLY': [bool],
-    'SESSION_COOKIE_NAME': [str],
-    'SESSION_COOKIE_PATH': [str],
-    'SESSION_COOKIE_SAMESITE': [str, bool],  # 'None' is a valid str value, so don't coerce to NoneType  # noqa: E501
-    'SESSION_COOKIE_SECURE': [bool],
-    'SESSION_ENGINE': [str],
-    'SESSION_EXPIRE_AT_BROWSER_CLOSE': [bool],
-    'SESSION_FILE_PATH': [type(None), str],
-    'SESSION_SAVE_EVERY_REQUEST': [bool],
-    'SESSION_SERIALIZER': [str],
-    'SHORT_DATETIME_FORMAT': [str],
-    'SHORT_DATE_FORMAT': [str],
-    'SIGNING_BACKEND': [str],
-    'SILENCED_SYSTEM_CHECKS': [list],
-    'STATICFILES_DIRS': [list],
-    'STATICFILES_FINDERS': [list],
-    'STATICFILES_STORAGE': [str],  # deprecated v4.2
-    'STATIC_ROOT': [type(None), str],
-    'STATIC_URL': [type(None), str],
-    'STORAGES': [dict],
-    'TEMPLATES': [list],
+    "ABSOLUTE_URL_OVERRIDES": [dict],
+    "ADMINS": [list],
+    "ALLOWED_HOSTS": [list],
+    "APPEND_SLASH": [bool],
+    "AUTHENTICATION_BACKENDS": [list],
+    "AUTH_PASSWORD_VALIDATORS": [list],
+    "AUTH_USER_MODEL": [str],
+    "CACHES": [dict],
+    "CACHE_MIDDLEWARE_ALIAS": [str],
+    "CACHE_MIDDLEWARE_KEY_PREFIX": [str],
+    "CACHE_MIDDLEWARE_SECONDS": [int],
+    "CSRF_COOKIE_AGE": [type(None), int],
+    "CSRF_COOKIE_DOMAIN": [type(None), str],
+    "CSRF_COOKIE_HTTPONLY": [bool],
+    "CSRF_COOKIE_MASKED": [bool],
+    "CSRF_COOKIE_NAME": [str],
+    "CSRF_COOKIE_PATH": [str],
+    "CSRF_COOKIE_SAMESITE": [
+        str
+    ],  # 'None' is a valid str value, so don't coerce to NoneType
+    "CSRF_COOKIE_SECURE": [bool],
+    "CSRF_FAILURE_VIEW": [str],
+    "CSRF_HEADER_NAME": [str],
+    "CSRF_TRUSTED_ORIGINS": [list],
+    "CSRF_USE_SESSIONS": [bool],
+    "DATABASES": [dict],
+    "DATABASE_ROUTERS": [list],
+    "DATA_UPLOAD_MAX_MEMORY_SIZE": [type(None), int],
+    "DATA_UPLOAD_MAX_NUMBER_FIELDS": [type(None), int],
+    "DATA_UPLOAD_MAX_NUMBER_FILES": [int],
+    "DATETIME_FORMAT": [str],
+    "DATETIME_INPUT_FORMATS": [list],
+    "DATE_FORMAT": [str],
+    "DATE_INPUT_FORMATS": [list],
+    "DEBUG": [bool],
+    "DEBUG_PROPAGATE_EXCEPTIONS": [bool],
+    "DECIMAL_SEPARATOR": [str],
+    "DEFAULT_AUTO_FIELD": [str],
+    "DEFAULT_CHARSET": [str],
+    "DEFAULT_CONTENT_TYPE": [str],  # deprecated v2.0, removed v3.0
+    "DEFAULT_EXCEPTION_REPORTER": [str],
+    "DEFAULT_EXCEPTION_REPORTER_FILTER": [str],
+    "DEFAULT_FILE_STORAGE": [str],  # deprecated v4.2
+    "DEFAULT_FROM_EMAIL": [str],
+    "DEFAULT_HASHING_ALGORITHM": [str],
+    "DEFAULT_INDEX_TABLESPACE": [str],
+    "DEFAULT_TABLESPACE": [str],
+    "DISALLOWED_USER_AGENTS": [list],
+    "EMAIL_BACKEND": [str],
+    "EMAIL_HOST": [str],
+    "EMAIL_HOST_PASSWORD": [str],
+    "EMAIL_HOST_USER": [str],
+    "EMAIL_PORT": [int],
+    "EMAIL_SSL_CERTFILE": [type(None), str],
+    "EMAIL_SSL_KEYFILE": [type(None), str],
+    "EMAIL_SUBJECT_PREFIX": [str],
+    "EMAIL_TIMEOUT": [type(None), int],
+    "EMAIL_USE_LOCALTIME": [bool],
+    "EMAIL_USE_SSL": [bool],
+    "EMAIL_USE_TLS": [bool],
+    "FILE_CHARSET": [str],  # deprecated v2.2, removed v3.1
+    "FILE_UPLOAD_DIRECTORY_PERMISSIONS": [type(None), str],
+    "FILE_UPLOAD_HANDLERS": [list],
+    "FILE_UPLOAD_MAX_MEMORY_SIZE": [int],
+    "FILE_UPLOAD_PERMISSIONS": [type(None), int],
+    "FILE_UPLOAD_TEMP_DIR": [type(None), str],
+    "FIRST_DAY_OF_WEEK": [int],
+    "FIXTURE_DIRS": [list],
+    "FORCE_SCRIPT_NAME": [type(None), str],
+    "FORMAT_MODULE_PATH": [type(None), str, list],
+    "FORM_RENDERER": [str],
+    "IGNORABLE_404_URLS": [list],
+    "INSTALLED_APPS": [list],
+    "INTERNAL_IPS": [list],
+    "LANGUAGES": [list],
+    "LANGUAGES_BIDI": [list],
+    "LANGUAGE_CODE": [str],
+    "LANGUAGE_COOKIE_AGE": [type(None), int],
+    "LANGUAGE_COOKIE_DOMAIN": [type(None), str],
+    "LANGUAGE_COOKIE_HTTPONLY": [bool],
+    "LANGUAGE_COOKIE_NAME": [str],
+    "LANGUAGE_COOKIE_PATH": [str],
+    "LANGUAGE_COOKIE_SAMESITE": [type(None), str],
+    "LANGUAGE_COOKIE_SECURE": [bool],
+    "LOCALE_PATHS": [list],
+    "LOGGING": [dict],
+    "LOGGING_CONFIG": [type(None), str],
+    "LOGIN_REDIRECT_URL": [str],
+    "LOGIN_URL": [str],
+    "LOGOUT_REDIRECT_URL": [type(None), str],
+    "MANAGERS": [list],
+    "MEDIA_ROOT": [str],
+    "MEDIA_URL": [str],
+    "MESSAGE_STORAGE": [str],
+    "MIDDLEWARE": [type(None), list],
+    "MIDDLEWARE_CLASSES": [list],  # deprecated v1.10, removed v2.0
+    "MIGRATION_MODULES": [dict],
+    "MONTH_DAY_FORMAT": [str],
+    "NUMBER_GROUPING": [int],
+    "PASSWORD_HASHERS": [list],
+    "PASSWORD_RESET_TIMEOUT": [int],
+    "PASSWORD_RESET_TIMEOUT_DAYS": [int],
+    "PREPEND_WWW": [bool],
+    "SECRET_KEY": [str],
+    "SECRET_KEY_FALLBACKS": [list],
+    "SECURE_BROWSER_XSS_FILTER": [bool],
+    "SECURE_CONTENT_TYPE_NOSNIFF": [bool],
+    "SECURE_HSTS_INCLUDE_SUBDOMAINS": [bool],
+    "SECURE_HSTS_PRELOAD": [bool],
+    "SECURE_HSTS_SECONDS": [int],
+    "SECURE_CROSS_ORIGIN_OPENER_POLICY": [type(None), str],
+    "SECURE_PROXY_SSL_HEADER": [type(None), tuple],
+    "SECURE_REDIRECT_EXEMPT": [list],
+    "SECURE_REFERRER_POLICY": [
+        type(None),
+        str,
+    ],  # v3.0 default None, v3.1 default str
+    "SECURE_SSL_HOST": [type(None), str],
+    "SECURE_SSL_REDIRECT": [bool],
+    "SERVER_EMAIL": [str],
+    "SESSION_CACHE_ALIAS": [str],
+    "SESSION_COOKIE_AGE": [int],
+    "SESSION_COOKIE_DOMAIN": [type(None), str],
+    "SESSION_COOKIE_HTTPONLY": [bool],
+    "SESSION_COOKIE_NAME": [str],
+    "SESSION_COOKIE_PATH": [str],
+    "SESSION_COOKIE_SAMESITE": [
+        str,
+        bool,
+    ],  # 'None' is a valid str value, so don't coerce to NoneType
+    "SESSION_COOKIE_SECURE": [bool],
+    "SESSION_ENGINE": [str],
+    "SESSION_EXPIRE_AT_BROWSER_CLOSE": [bool],
+    "SESSION_FILE_PATH": [type(None), str],
+    "SESSION_SAVE_EVERY_REQUEST": [bool],
+    "SESSION_SERIALIZER": [str],
+    "SHORT_DATETIME_FORMAT": [str],
+    "SHORT_DATE_FORMAT": [str],
+    "SIGNING_BACKEND": [str],
+    "SILENCED_SYSTEM_CHECKS": [list],
+    "STATICFILES_DIRS": [list],
+    "STATICFILES_FINDERS": [list],
+    "STATICFILES_STORAGE": [str],  # deprecated v4.2
+    "STATIC_ROOT": [type(None), str],
+    "STATIC_URL": [type(None), str],
+    "STORAGES": [dict],
+    "TEMPLATES": [list],
     # 'TEMPLATE_DIRS': [list],  # deprecated v1.8, removed v1.10
-    'TEST_NON_SERIALIZED_APPS': [list],
-    'TEST_RUNNER': [str],
-    'THOUSAND_SEPARATOR': [str],
-    'TIME_FORMAT': [str],
-    'TIME_INPUT_FORMATS': [list],
-    'TIME_ZONE': [type(None), str],
-    'USE_DEPRECATED_PYTZ': [bool],  # introduced v4.0, will be removed v5.0
-    'USE_ETAGS': [bool],  # deprecated v1.11, removed v2.1
-    'USE_I18N': [bool],
-    'USE_L10N': [bool],
-    'USE_THOUSAND_SEPARATOR': [bool],
-    'USE_TZ': [bool],
-    'USE_X_FORWARDED_HOST': [bool],
-    'USE_X_FORWARDED_PORT': [bool],
-    'WSGI_APPLICATION': [type(None), str],
-    'X_FRAME_OPTIONS': [str],
-    'YEAR_MONTH_FORMAT': [str],
-
+    "TEST_NON_SERIALIZED_APPS": [list],
+    "TEST_RUNNER": [str],
+    "THOUSAND_SEPARATOR": [str],
+    "TIME_FORMAT": [str],
+    "TIME_INPUT_FORMATS": [list],
+    "TIME_ZONE": [type(None), str],
+    "USE_DEPRECATED_PYTZ": [bool],  # introduced v4.0, will be removed v5.0
+    "USE_ETAGS": [bool],  # deprecated v1.11, removed v2.1
+    "USE_I18N": [bool],
+    "USE_L10N": [bool],
+    "USE_THOUSAND_SEPARATOR": [bool],
+    "USE_TZ": [bool],
+    "USE_X_FORWARDED_HOST": [bool],
+    "USE_X_FORWARDED_PORT": [bool],
+    "WSGI_APPLICATION": [type(None), str],
+    "X_FRAME_OPTIONS": [str],
+    "YEAR_MONTH_FORMAT": [str],
     # django-envconfig settings
-    'ADD_INSTALLED_APPS': [list],
-    'REMOVE_INSTALLED_APPS': [list],
-    'ADD_MIDDLEWARE': [list],
-    'REMOVE_MIDDLEWARE': [list],
-    'PGDATABASE': [str],
-    'PGUSER': [str],
-    'PGPASSWORD': [str],
-    'PGHOST': [str],
-    'PGPORT': [int],
+    "ADD_INSTALLED_APPS": [list],
+    "REMOVE_INSTALLED_APPS": [list],
+    "ADD_MIDDLEWARE": [list],
+    "REMOVE_MIDDLEWARE": [list],
+    "PGDATABASE": [str],
+    "PGUSER": [str],
+    "PGPASSWORD": [str],
+    "PGHOST": [str],
+    "PGPORT": [int],
 }
 
 
 def get_setting_types():
     return _setting_types.copy()
```

### Comparing `django-envconfig-0.2.7/envconfig/settings.py` & `django-envconfig-0.3.0/envconfig/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
+import sys
 from os import environ, getenv
 from pathlib import Path
-import sys
 
 from django.core.exceptions import ImproperlyConfigured
 from dotenv import load_dotenv
 
+from envconfig import utils
 from envconfig.dotenv import find_dotenv
 from envconfig.parser import EnvParser
 from envconfig.setting_types import get_setting_types
-from envconfig import utils
 
 # Based on the command line arguments try and infer the project name and
 # the path to the base directory (to look for .env)
 project_name = None
 extra_paths = []
 for arg in sys.argv:
-    if arg.endswith('.asgi:application') or arg.endswith('.wsgi'):
-        project_name = arg.split('.')[0]
+    if arg.endswith(".asgi:application") or arg.endswith(".wsgi"):
+        project_name = arg.split(".")[0]
         try:
             extra_paths.append(utils.get_base_dir(project_name))
         except ModuleNotFoundError:
             pass
-    if arg.endswith('manage.py'):
+    if arg.endswith("manage.py"):
         base_dir = Path(arg).parent.absolute()
         project_name = utils.find_project_name(base_dir)
         extra_paths.append(base_dir)
 
 load_dotenv(dotenv_path=find_dotenv(extra_paths=extra_paths))
 
-project_name = getenv('DJANGO_PROJECT', project_name)
+project_name = getenv("DJANGO_PROJECT", project_name)
 if not project_name:
     raise ImproperlyConfigured(
         "Could not find Django project (i.e. module with wsgi.py or asgi.py). "
         "Please set environment variable 'DJANGO_PROJECT'."
     )
 
 # Generate default settings and values from startproject template settings.py
@@ -41,62 +41,62 @@
 mod_settings = utils.get_module_settings(project_name)
 # Overlay the default template settings with any settings module settings
 settings.update(mod_settings)
 
 # Get a lookup of built-in Django settings and their valid types
 setting_types = get_setting_types()
 # Add any custom settings and their default types
-setting_types.update({
-    s: [type(mod_settings[s])] for s in mod_settings if s not in setting_types
-})
+setting_types.update(
+    {s: [type(mod_settings[s])] for s in mod_settings if s not in setting_types}
+)
 
-if project_name not in settings['INSTALLED_APPS']:
-    settings['INSTALLED_APPS'].append(project_name)
+if project_name not in settings["INSTALLED_APPS"]:
+    settings["INSTALLED_APPS"].append(project_name)
 
 envsetting_names = [s for s in setting_types if s in environ]
 
 for name in envsetting_names:
     val = getenv(name)
     if val:
         try:
             settings[name] = EnvParser.parse(val, *setting_types[name])
         except ValueError as e:
             types_str = "', '".join(t.__name__ for t in setting_types[name])
             raise ImproperlyConfigured(
                 f"Environment variable '{name}' incorrectly set. "
                 f"Error: {str(e)}. Valid types include: '{types_str}'."
-            )
+            ) from None
 
 # django-envconfig settings
-settings['INSTALLED_APPS'] = utils.modify_list(
-    settings['INSTALLED_APPS'],
-    add=settings.get('ADD_INSTALLED_APPS', []),
-    remove=settings.get('REMOVE_INSTALLED_APPS', [])
+settings["INSTALLED_APPS"] = utils.modify_list(
+    settings["INSTALLED_APPS"],
+    add=settings.get("ADD_INSTALLED_APPS", []),
+    remove=settings.get("REMOVE_INSTALLED_APPS", []),
 )
 # Respect that MIDDLEWARE can be None
-if settings['MIDDLEWARE'] is not None or settings.get('ADD_MIDDLEWARE'):
-    settings['MIDDLEWARE'] = utils.modify_list(
-        settings.get('MIDDLEWARE') or [],
-        add=settings.get('ADD_MIDDLEWARE', []),
-        remove=settings.get('REMOVE_MIDDLEWARE', [])
+if settings["MIDDLEWARE"] is not None or settings.get("ADD_MIDDLEWARE"):
+    settings["MIDDLEWARE"] = utils.modify_list(
+        settings.get("MIDDLEWARE") or [],
+        add=settings.get("ADD_MIDDLEWARE", []),
+        remove=settings.get("REMOVE_MIDDLEWARE", []),
     )
 
 # PostgreSQL
 # https://www.postgresql.org/docs/current/libpq-envars.html
-if 'PGDATABASE' in settings:
-    settings['DATABASES'] = {
-        'default': {
-            'ENGINE': 'django.db.backends.postgresql',
-            'NAME': settings.get('PGDATABASE'),
-            'USER': settings.pop('PGUSER', ''),
-            'PASSWORD': settings.pop('PGPASSWORD', ''),
-            'HOST': settings.pop('PGHOST', ''),
-            'PORT': settings.pop('PGPORT', ''),
-            'TEST': {
-                'NAME': 'test_' + settings.pop('PGDATABASE'),
-            }
+if "PGDATABASE" in settings:
+    settings["DATABASES"] = {
+        "default": {
+            "ENGINE": "django.db.backends.postgresql",
+            "NAME": settings.get("PGDATABASE"),
+            "USER": settings.pop("PGUSER", ""),
+            "PASSWORD": settings.pop("PGPASSWORD", ""),
+            "HOST": settings.pop("PGHOST", ""),
+            "PORT": settings.pop("PGPORT", ""),
+            "TEST": {
+                "NAME": "test_" + settings.pop("PGDATABASE"),
+            },
         }
     }
 
 # Make all of the settings attributes of this module
 for name, val in settings.items():
     setattr(sys.modules[__name__], name, val)
```

### Comparing `django-envconfig-0.2.7/envconfig/utils.py` & `django-envconfig-0.3.0/envconfig/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,87 @@
 from importlib import import_module
 from importlib.machinery import SourceFileLoader
-from importlib.util import spec_from_loader, module_from_spec
+from importlib.util import module_from_spec, spec_from_loader
 from pathlib import Path
 from types import ModuleType
 from typing import List, Optional, Union
 
 import django
 from django.core.management.utils import get_random_secret_key
 
 # Relative path to settings.py template from django package root dir
-RELPATH_TO_SETTINGS_TPL = 'conf/project_template/project_name/settings.py-tpl'
+RELPATH_TO_SETTINGS_TPL = "conf/project_template/project_name/settings.py-tpl"
 
 
 def find_project_name(path: Path) -> Optional[str]:
-    search = list(set(
-        p.parent.name for p in path.glob('*/[a|w]sgi.py')
-        if p.parent.is_dir()
-    ))
+    search = list(
+        set(  # noqa: C401
+            p.parent.name for p in path.glob("*/[a|w]sgi.py") if p.parent.is_dir()
+        )
+    )
     return search[0] if len(search) == 1 else None
 
 
 def get_base_dir(project_name: str) -> Path:
     mod = import_module(project_name)
     return Path(mod.__file__).parent.parent.absolute()  # type: ignore  # noqa
 
 
 def get_module_settings(project_name: str) -> dict:
     try:
-        mod = import_module(f'{project_name}.settings')
+        mod = import_module(f"{project_name}.settings")
         setting_names = [s for s in dir(mod) if s.isupper()]
         return {s: getattr(mod, s) for s in setting_names}
     except ModuleNotFoundError:
         return {}
 
 
 def get_path_to_settings_template() -> Path:
     return Path(django.__file__).parent / RELPATH_TO_SETTINGS_TPL
 
 
 def get_template_settings(project_name: str) -> dict:
-    template_settings = import_module_from_file(
-        get_path_to_settings_template()
-    )
+    template_settings = import_module_from_file(get_path_to_settings_template())
     setting_names = [s for s in dir(template_settings) if s.isupper()]
     settings = {}
     for s in setting_names:
         val = getattr(template_settings, s)
-        if isinstance(val, str) and '{{ project_name }}' in val:
-            val = val.replace('{{ project_name }}', project_name)
+        if isinstance(val, str) and "{{ project_name }}" in val:
+            val = val.replace("{{ project_name }}", project_name)
         settings[s] = val
     # Find the correct BASE_DIR
     base_dir = get_base_dir(project_name)
     # Modify the DATABASES setting for correct BASE_DIR
-    db_name = settings['DATABASES']['default']['NAME']
+    db_name = settings["DATABASES"]["default"]["NAME"]
     if not isinstance(db_name, Path):
         db_name = Path(db_name)
     db_name = base_dir / db_name.name
     # Overwite some of the defaults
-    if isinstance(settings['BASE_DIR'], str):
-        settings['BASE_DIR'] = str(base_dir.resolve())
-        settings['DATABASES']['default']['NAME'] = str(db_name.resolve())
+    if isinstance(settings["BASE_DIR"], str):
+        settings["BASE_DIR"] = str(base_dir.resolve())
+        settings["DATABASES"]["default"]["NAME"] = str(db_name.resolve())
     else:
-        settings['BASE_DIR'] = base_dir
-        settings['DATABASES']['default']['NAME'] = db_name
-    settings['DEBUG'] = False  # Ensure DEBUG defaults to False
-    settings['SECRET_KEY'] = get_random_secret_key()
+        settings["BASE_DIR"] = base_dir
+        settings["DATABASES"]["default"]["NAME"] = db_name
+    settings["DEBUG"] = False  # Ensure DEBUG defaults to False
+    settings["SECRET_KEY"] = get_random_secret_key()
     return settings
 
 
 def import_module_from_file(path: Union[Path, str]) -> ModuleType:
     """Import a Python module based on file path rather than a dotted
     name.
     """
     if isinstance(path, str):
         path = Path(path)
-    name = path.name.split('.')[0]
+    name = path.name.split(".")[0]
     spec = spec_from_loader(name, SourceFileLoader(name, str(path.resolve())))
     mod = module_from_spec(spec)  # type: ignore  # noqa
     spec.loader.exec_module(mod)  # type: ignore  # noqa
     return mod
 
 
-def modify_list(
-    list_: List[str], add: List[str], remove: List[str]
-) -> List[str]:
+def modify_list(list_: List[str], add: List[str], remove: List[str]) -> List[str]:
     """Add and remove items from a list. Preserve order and prevent
     duplication.
     """
-    return ([a for a in list_ if a not in remove]
-            + [a for a in add if a not in list_])
+    return [a for a in list_ if a not in remove] + [a for a in add if a not in list_]
```

### Comparing `django-envconfig-0.2.7/tests/test_utils.py` & `django-envconfig-0.3.0/tests/test_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from pathlib import Path
 
 from pytest_mock import MockerFixture
 
 from envconfig import utils
 
-PATH_TO_TEST_TEMPLATE = Path(__file__).parent / 'fixtures/testmodule.py-tpl'
+PATH_TO_TEST_TEMPLATE = Path(__file__).parent / "fixtures/testmodule.py-tpl"
 
 
-def test_get_template_settings_sets_correct_type_for_BASE_DIR(mocker: MockerFixture) -> None:  # noqa: E501
+def test_get_template_settings_sets_correct_type_for_BASE_DIR(
+    mocker: MockerFixture,
+) -> None:
     default_template_settings = utils.import_module_from_file(
         utils.get_path_to_settings_template()
     )
-    mocker.patch('envconfig.utils.get_base_dir',
-                 return_value=Path('/path/to/base_dir'))
-    base_dir = utils.get_template_settings('foobar')['BASE_DIR']
+    mocker.patch("envconfig.utils.get_base_dir", return_value=Path("/path/to/base_dir"))
+    base_dir = utils.get_template_settings("foobar")["BASE_DIR"]
     assert type(default_template_settings.BASE_DIR) == type(base_dir)  # type: ignore  # noqa
 
 
 def test_target_template_settings_file_exists() -> None:
     path = utils.get_path_to_settings_template()
     assert path.exists()
 
 
 def test_import_module_from_file() -> None:
     mod = utils.import_module_from_file(PATH_TO_TEST_TEMPLATE)
-    assert mod.FOO == 'bar'  # type: ignore  # noqa
+    assert mod.FOO == "bar"  # type: ignore  # noqa
 
 
 def test_import_module_from_file_with_str() -> None:
     mod = utils.import_module_from_file(str(PATH_TO_TEST_TEMPLATE.resolve()))
-    assert mod.FOO == 'bar'  # type: ignore  # noqa
+    assert mod.FOO == "bar"  # type: ignore  # noqa
 
 
 def test_modify_list() -> None:
-    list_ = ['1', '2', '3', '4']
-    modified_list = utils.modify_list(list_, add=['3', '5'], remove=['2', '6'])
-    assert modified_list == ['1', '3', '4', '5']
+    list_ = ["1", "2", "3", "4"]
+    modified_list = utils.modify_list(list_, add=["3", "5"], remove=["2", "6"])
+    assert modified_list == ["1", "3", "4", "5"]
```

