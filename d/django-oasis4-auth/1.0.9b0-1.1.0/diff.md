# Comparing `tmp/django-oasis4-auth-1.0.9b0.tar.gz` & `tmp/django-oasis4-auth-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oasis4-auth-1.0.9b0.tar", last modified: Thu Mar 16 19:27:28 2023, max compression
+gzip compressed data, was "django-oasis4-auth-1.1.0.tar", last modified: Mon Jun 26 19:38:40 2023, max compression
```

## Comparing `django-oasis4-auth-1.0.9b0.tar` & `django-oasis4-auth-1.1.0.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.095507 django-oasis4-auth-1.0.9b0/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-auth-1.0.9b0/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)       93 2023-01-18 12:21:52.000000 django-oasis4-auth-1.0.9b0/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    22677 2023-03-16 19:27:28.095507 django-oasis4-auth-1.0.9b0/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     9810 2023-02-15 19:15:25.000000 django-oasis4-auth-1.0.9b0/README.md
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.088507 django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    22677 2023-03-16 19:27:28.000000 django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1413 2023-03-16 19:27:28.000000 django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-03-16 19:27:28.000000 django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       67 2023-03-16 19:27:28.000000 django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       11 2023-03-16 19:27:28.000000 django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/top_level.txt
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.088507 django-oasis4-auth-1.0.9b0/oasis_auth/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-20 02:22:34.000000 django-oasis4-auth-1.0.9b0/oasis_auth/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.089506 django-oasis4-auth-1.0.9b0/oasis_auth/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      507 2023-01-07 20:01:29.000000 django-oasis4-auth-1.0.9b0/oasis_auth/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.089506 django-oasis4-auth-1.0.9b0/oasis_auth/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      578 2023-01-27 22:32:38.000000 django-oasis4-auth-1.0.9b0/oasis_auth/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      786 2023-01-27 22:44:36.000000 django-oasis4-auth-1.0.9b0/oasis_auth/api/serializers/user.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.089506 django-oasis4-auth-1.0.9b0/oasis_auth/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      590 2023-01-18 03:44:01.000000 django-oasis4-auth-1.0.9b0/oasis_auth/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    16006 2023-03-16 16:26:19.000000 django-oasis4-auth-1.0.9b0/oasis_auth/api/services/oasis_auth.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1090 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.090507 django-oasis4-auth-1.0.9b0/oasis_auth/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      509 2022-12-20 17:00:22.000000 django-oasis4-auth-1.0.9b0/oasis_auth/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.090507 django-oasis4-auth-1.0.9b0/oasis_auth/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      580 2023-01-18 20:29:06.000000 django-oasis4-auth-1.0.9b0/oasis_auth/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2368 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/lib/managers/user_profile.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.091507 django-oasis4-auth-1.0.9b0/oasis_auth/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      627 2023-01-18 15:44:17.000000 django-oasis4-auth-1.0.9b0/oasis_auth/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2944 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/lib/utils/auth_actions.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2207 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/lib/utils/send_code.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.086507 django-oasis4-auth-1.0.9b0/oasis_auth/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.086507 django-oasis4-auth-1.0.9b0/oasis_auth/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.091507 django-oasis4-auth-1.0.9b0/oasis_auth/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4792 2023-03-16 16:15:08.000000 django-oasis4-auth-1.0.9b0/oasis_auth/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     7121 2023-03-16 16:14:53.000000 django-oasis4-auth-1.0.9b0/oasis_auth/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.092507 django-oasis4-auth-1.0.9b0/oasis_auth/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2055 2023-01-18 02:10:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      438 2023-01-18 20:03:48.000000 django-oasis4-auth-1.0.9b0/oasis_auth/migrations/0002_remove_userprofile_first_name_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      598 2023-03-01 16:07:21.000000 django-oasis4-auth-1.0.9b0/oasis_auth/migrations/0003_userprofile_quota_userprofile_segment.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      354 2023-03-01 16:22:58.000000 django-oasis4-auth-1.0.9b0/oasis_auth/migrations/0004_remove_userprofile_quota.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-01-18 02:10:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2222 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.093506 django-oasis4-auth-1.0.9b0/oasis_auth/tasks/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      581 2023-02-15 14:18:51.000000 django-oasis4-auth-1.0.9b0/oasis_auth/tasks/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2211 2023-03-01 16:31:30.000000 django-oasis4-auth-1.0.9b0/oasis_auth/tasks/sync_users.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.094506 django-oasis4-auth-1.0.9b0/oasis_auth/templates/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2022-12-22 15:55:10.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/default.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-02 19:51:33.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/default.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2022-12-22 15:55:10.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/login.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-01 21:00:33.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/login.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      745 2023-01-18 04:44:01.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/register.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      509 2023-03-01 21:00:33.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/register.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      634 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/retrieve_password.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      405 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/retrieve_password.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1151 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/urls.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      851 2023-03-16 19:26:27.000000 django-oasis4-auth-1.0.9b0/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-03-16 19:27:28.095507 django-oasis4-auth-1.0.9b0/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.971400 django-oasis4-auth-1.1.0/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-auth-1.1.0/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)       93 2023-01-18 12:21:52.000000 django-oasis4-auth-1.1.0/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    22832 2023-06-26 19:38:40.971400 django-oasis4-auth-1.1.0/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     9954 2023-06-19 19:17:48.000000 django-oasis4-auth-1.1.0/README.md
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.961400 django-oasis4-auth-1.1.0/django_oasis4_auth.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    22832 2023-06-26 19:38:40.000000 django-oasis4-auth-1.1.0/django_oasis4_auth.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1471 2023-06-26 19:38:40.000000 django-oasis4-auth-1.1.0/django_oasis4_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-06-26 19:38:40.000000 django-oasis4-auth-1.1.0/django_oasis4_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       74 2023-06-26 19:38:40.000000 django-oasis4-auth-1.1.0/django_oasis4_auth.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       11 2023-06-26 19:38:40.000000 django-oasis4-auth-1.1.0/django_oasis4_auth.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.962400 django-oasis4-auth-1.1.0/oasis_auth/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-20 02:22:34.000000 django-oasis4-auth-1.1.0/oasis_auth/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.962400 django-oasis4-auth-1.1.0/oasis_auth/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      507 2023-01-07 20:01:29.000000 django-oasis4-auth-1.1.0/oasis_auth/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.962400 django-oasis4-auth-1.1.0/oasis_auth/api/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      578 2023-01-27 22:32:38.000000 django-oasis4-auth-1.1.0/oasis_auth/api/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      786 2023-01-27 22:44:36.000000 django-oasis4-auth-1.1.0/oasis_auth/api/serializers/user.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.963400 django-oasis4-auth-1.1.0/oasis_auth/api/services/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      590 2023-01-18 03:44:01.000000 django-oasis4-auth-1.1.0/oasis_auth/api/services/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    15973 2023-06-19 19:02:47.000000 django-oasis4-auth-1.1.0/oasis_auth/api/services/oasis_auth.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1180 2023-06-19 19:04:20.000000 django-oasis4-auth-1.1.0/oasis_auth/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.963400 django-oasis4-auth-1.1.0/oasis_auth/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      509 2022-12-20 17:00:22.000000 django-oasis4-auth-1.1.0/oasis_auth/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.964400 django-oasis4-auth-1.1.0/oasis_auth/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      580 2023-01-18 20:29:06.000000 django-oasis4-auth-1.1.0/oasis_auth/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2368 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0/oasis_auth/lib/managers/user_profile.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1033 2023-06-19 19:04:20.000000 django-oasis4-auth-1.1.0/oasis_auth/lib/signal_events.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      424 2023-06-19 18:55:26.000000 django-oasis4-auth-1.1.0/oasis_auth/lib/signals.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.964400 django-oasis4-auth-1.1.0/oasis_auth/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      627 2023-01-18 15:44:17.000000 django-oasis4-auth-1.1.0/oasis_auth/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2974 2023-05-23 13:18:45.000000 django-oasis4-auth-1.1.0/oasis_auth/lib/utils/auth_actions.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2207 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0/oasis_auth/lib/utils/send_code.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.960400 django-oasis4-auth-1.1.0/oasis_auth/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.960400 django-oasis4-auth-1.1.0/oasis_auth/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.965400 django-oasis4-auth-1.1.0/oasis_auth/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     4792 2023-03-16 16:15:08.000000 django-oasis4-auth-1.1.0/oasis_auth/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     7121 2023-03-16 16:14:53.000000 django-oasis4-auth-1.1.0/oasis_auth/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.969400 django-oasis4-auth-1.1.0/oasis_auth/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2055 2023-01-18 02:10:57.000000 django-oasis4-auth-1.1.0/oasis_auth/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      438 2023-01-18 20:03:48.000000 django-oasis4-auth-1.1.0/oasis_auth/migrations/0002_remove_userprofile_first_name_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      598 2023-03-01 16:07:21.000000 django-oasis4-auth-1.1.0/oasis_auth/migrations/0003_userprofile_quota_userprofile_segment.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      354 2023-03-01 16:22:58.000000 django-oasis4-auth-1.1.0/oasis_auth/migrations/0004_remove_userprofile_quota.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-01-18 02:10:57.000000 django-oasis4-auth-1.1.0/oasis_auth/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2222 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0/oasis_auth/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.969400 django-oasis4-auth-1.1.0/oasis_auth/tasks/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      581 2023-02-15 14:18:51.000000 django-oasis4-auth-1.1.0/oasis_auth/tasks/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2211 2023-03-01 16:31:30.000000 django-oasis4-auth-1.1.0/oasis_auth/tasks/sync_users.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:38:40.971400 django-oasis4-auth-1.1.0/oasis_auth/templates/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2022-12-22 15:55:10.000000 django-oasis4-auth-1.1.0/oasis_auth/templates/default.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-02 19:51:33.000000 django-oasis4-auth-1.1.0/oasis_auth/templates/default.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2022-12-22 15:55:10.000000 django-oasis4-auth-1.1.0/oasis_auth/templates/login.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-01 21:00:33.000000 django-oasis4-auth-1.1.0/oasis_auth/templates/login.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      745 2023-01-18 04:44:01.000000 django-oasis4-auth-1.1.0/oasis_auth/templates/register.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      509 2023-03-01 21:00:33.000000 django-oasis4-auth-1.1.0/oasis_auth/templates/register.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      634 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0/oasis_auth/templates/retrieve_password.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      405 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0/oasis_auth/templates/retrieve_password.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1151 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0/oasis_auth/urls.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      864 2023-06-26 19:36:05.000000 django-oasis4-auth-1.1.0/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-06-26 19:38:40.971400 django-oasis4-auth-1.1.0/setup.cfg
```

### Comparing `django-oasis4-auth-1.0.9b0/LICENSE` & `django-oasis4-auth-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/PKG-INFO` & `django-oasis4-auth-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4-auth
-Version: 1.0.9b0
+Version: 1.1.0
 Summary: Oasis 4 Authorization System for django
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
         
@@ -110,15 +110,15 @@
         IDIOMA; TRADUCCIONES. En el caso de que la versión en español de este Contrato esté acompañada por cualquier otra
         versión traducida a otro idioma, dicha versión traducida sólo se ofrece a título informativo y prevalecerá la versión
         en español.
         
 Keywords: django,OASIS4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -127,15 +127,15 @@
 [English](#oasis4-authentication-package-for-DJANGO&copy;)
 # Módulo de autenticación OASIS4 para DJANGO&copy;
 Este módulo permite a DJANGO&copy; interactuar con OASIS4 y realizar acciones como el registro de usuario y su autenticacíón, utilizando un sistema de dos pasos.
 
 El módulo ofrece tres (3) servicios API para el registro de los usuarios, ingreso al sistema y validación del código de autorización.
 
 ## Versiones
-
+* 1.1.0: Se elimina la dependencia del paquete zibanu.django.auth para el manejo de las señales. Depende de la versión 1.2.0 de zibanu-django.
 * 1.0.7: Incorpora una tarea para la sincronización de los usuarios desde la tabla origen en OASIS4.
 * 1.0.5: Corrige un bug que se presentaba con la autenticación anónima derivada de la actualización de librerías.
 * 1.0.4: Corrige un bug que creaba el usuario en la tabla de usuarios ignorando el segundo nombre y apellido.
 
 ## APIs
 * [Registro](#registro)
 * [Acceso al sistema](#login-1)
```

### Comparing `django-oasis4-auth-1.0.9b0/README.md` & `django-oasis4-auth-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [English](#oasis4-authentication-package-for-DJANGO&copy;)
 # Módulo de autenticación OASIS4 para DJANGO&copy;
 Este módulo permite a DJANGO&copy; interactuar con OASIS4 y realizar acciones como el registro de usuario y su autenticacíón, utilizando un sistema de dos pasos.
 
 El módulo ofrece tres (3) servicios API para el registro de los usuarios, ingreso al sistema y validación del código de autorización.
 
 ## Versiones
-
+* 1.1.0: Se elimina la dependencia del paquete zibanu.django.auth para el manejo de las señales. Depende de la versión 1.2.0 de zibanu-django.
 * 1.0.7: Incorpora una tarea para la sincronización de los usuarios desde la tabla origen en OASIS4.
 * 1.0.5: Corrige un bug que se presentaba con la autenticación anónima derivada de la actualización de librerías.
 * 1.0.4: Corrige un bug que creaba el usuario en la tabla de usuarios ignorando el segundo nombre y apellido.
 
 ## APIs
 * [Registro](#registro)
 * [Acceso al sistema](#login-1)
```

### Comparing `django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/PKG-INFO` & `django-oasis4-auth-1.1.0/django_oasis4_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4-auth
-Version: 1.0.9b0
+Version: 1.1.0
 Summary: Oasis 4 Authorization System for django
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
         
@@ -110,15 +110,15 @@
         IDIOMA; TRADUCCIONES. En el caso de que la versión en español de este Contrato esté acompañada por cualquier otra
         versión traducida a otro idioma, dicha versión traducida sólo se ofrece a título informativo y prevalecerá la versión
         en español.
         
 Keywords: django,OASIS4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -127,15 +127,15 @@
 [English](#oasis4-authentication-package-for-DJANGO&copy;)
 # Módulo de autenticación OASIS4 para DJANGO&copy;
 Este módulo permite a DJANGO&copy; interactuar con OASIS4 y realizar acciones como el registro de usuario y su autenticacíón, utilizando un sistema de dos pasos.
 
 El módulo ofrece tres (3) servicios API para el registro de los usuarios, ingreso al sistema y validación del código de autorización.
 
 ## Versiones
-
+* 1.1.0: Se elimina la dependencia del paquete zibanu.django.auth para el manejo de las señales. Depende de la versión 1.2.0 de zibanu-django.
 * 1.0.7: Incorpora una tarea para la sincronización de los usuarios desde la tabla origen en OASIS4.
 * 1.0.5: Corrige un bug que se presentaba con la autenticación anónima derivada de la actualización de librerías.
 * 1.0.4: Corrige un bug que creaba el usuario en la tabla de usuarios ignorando el segundo nombre y apellido.
 
 ## APIs
 * [Registro](#registro)
 * [Acceso al sistema](#login-1)
```

### Comparing `django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/SOURCES.txt` & `django-oasis4-auth-1.1.0/django_oasis4_auth.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 oasis_auth/urls.py
 oasis_auth/api/__init__.py
 oasis_auth/api/serializers/__init__.py
 oasis_auth/api/serializers/user.py
 oasis_auth/api/services/__init__.py
 oasis_auth/api/services/oasis_auth.py
 oasis_auth/lib/__init__.py
+oasis_auth/lib/signal_events.py
+oasis_auth/lib/signals.py
 oasis_auth/lib/managers/__init__.py
 oasis_auth/lib/managers/user_profile.py
 oasis_auth/lib/utils/__init__.py
 oasis_auth/lib/utils/auth_actions.py
 oasis_auth/lib/utils/send_code.py
 oasis_auth/locale/es/LC_MESSAGES/django.mo
 oasis_auth/locale/es/LC_MESSAGES/django.po
```

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/api/serializers/__init__.py` & `django-oasis4-auth-1.1.0/oasis_auth/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/api/serializers/user.py` & `django-oasis4-auth-1.1.0/oasis_auth/api/serializers/user.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/api/services/__init__.py` & `django-oasis4-auth-1.1.0/oasis_auth/api/services/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/api/services/oasis_auth.py` & `django-oasis4-auth-1.1.0/oasis_auth/api/services/oasis_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 from django.contrib.auth import get_user_model
 from django.core.cache import cache
 from django.core.exceptions import ObjectDoesNotExist
 from django.core.exceptions import ValidationError as CoreValidationError
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
 from oasis.models import Client
+from oasis_auth.lib.signals import change_password
+from oasis_auth.lib.signals import request_password
 from oasis_auth.lib.utils import AuthActions
 from oasis_auth.lib.utils import SendCode
 from rest_framework import permissions
 from rest_framework import status
 from rest_framework.response import Response
 from uuid import uuid4
-from zibanu.django.logging.lib.signals import change_password
-from zibanu.django.logging.lib.signals import retrieve_password
 from zibanu.django.rest_framework.exceptions import APIException
 from zibanu.django.rest_framework.exceptions import AuthenticationFailed
 from zibanu.django.rest_framework.exceptions import ValidationError
 from zibanu.django.rest_framework.viewsets import ViewSet
 from zibanu.django.utils import CodeGenerator
 from zibanu.django.utils import ErrorMessages
 
@@ -146,15 +146,15 @@
                     }
                     send_code = SendCode(to=user.email, action="retrieve_password", context=email_context)
                     if send_code.load_templates():
                         send_code.send()
                         user.set_password(email_context.get("new_password"))
                         user.save()
                         status_return = status.HTTP_200_OK
-                        retrieve_password.send(sender=self.__class__, user=user, action="retrieve_password",
+                        request_password.send(sender=self.__class__, user=user, action="request_password",
                                                request=request)
                     else:
                         raise ValidationError(_("Error loading email templates."))
                 else:
                     raise ValidationError(_("Email is not registered or does not match."))
             else:
                 raise ValidationError(ErrorMessages.DATA_REQUEST_NOT_FOUND)
@@ -262,15 +262,15 @@
                         data_cache["data"] = user
                         data_return = {
                             "token": cache_key
                         }
                         email_context = {
                             "customer_name": user.get_full_name(),
                             "customer_code": data_cache.get("code"),
-                            "code_timeout": self.__cache_timeout_seconds,
+                            "code_timeout": self.__cache_timeout,
                             "email_datetime": timezone.now().astimezone(tz=timezone.get_default_timezone()).strftime(
                                 "%Y-%m-%d %H:%M:%S"),
                             "email_id": str(uuid4())
                         }
                         # Send a second pass authentication code
                         send_code = SendCode(to=request.data.get("email"), action=data_cache.get("action"),
                                              context=email_context)
```

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/apps.py` & `django-oasis4-auth-1.1.0/oasis_auth/apps.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,13 +16,15 @@
 
 
 class CFHLAuth(AppConfig):
     default_auto_field = 'django.db.models.BigAutoField'
     name = 'oasis_auth'
 
     def ready(self):
+        # Import Signals
+        from oasis_auth.lib.signal_events import password_events
         # Code Timeout
         settings.OASIS_AUTH_CODE_TIMEOUT = getattr(settings, "OASIS_AUTH_CODE_TIMEOUT", 2)
         # High complex password
         settings.OASIS_AUTH_PASSWORD_COMPLEX = getattr(settings, "OASIS_AUTH_PASSWORD_COMPLEX", False)
         # Default length retrieve password
         settings.OASIS_AUTH_PASSWORD_LENGTH = getattr(settings, "OASIS_AUTH_PASSWORD_LENGTH", 12)
```

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/lib/managers/__init__.py` & `django-oasis4-auth-1.1.0/oasis_auth/lib/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/lib/managers/user_profile.py` & `django-oasis4-auth-1.1.0/oasis_auth/lib/managers/user_profile.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/lib/utils/__init__.py` & `django-oasis4-auth-1.1.0/oasis_auth/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/lib/utils/auth_actions.py` & `django-oasis4-auth-1.1.0/oasis_auth/lib/utils/auth_actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 # IDE:          PyCharm
 # Developed by: macercha
 # Date:         18/01/23 10:12 AM
 # Project:      CFHL Transactional Backend
 # Module Name:  auth_actions
 # Description:
 # ****************************************************************
-import inspect
 from django.contrib.auth.signals import user_logged_in
 from django.utils.translation import gettext_lazy as _
 from django.core.exceptions import ValidationError
 from oasis_auth.models import UserProfile
 from rest_framework_simplejwt.tokens import RefreshToken
 from typing import Any
 
 
 class AuthActions:
     """
     Class to encapsulate the different actions to be executed for auth package
     depending on action required.
     """
+
     def __init__(self, data: dict, request: Any):
         """
         Initialization method
         :param data: data dictionary with at least "data" and "action" keys.
         """
         self.__request = request
         if data is not None and {"data", "action"} <= data.keys():
@@ -66,17 +66,12 @@
                 "email": self.__data.email,
                 "phone": self.__data.profile.phone,
                 "mobile": self.__data.profile.mobile,
                 "location": self.__data.profile.location,
                 "address": self.__data.profile.address,
                 "last_login": self.__data.last_login,
                 "type": self.__data.profile.type,
-                "relationship": self.__data.profile.get_type_display()
+                "relationship": self.__data.profile.get_type_display(),
+                "is_staff": self.__data.is_staff
             }
         }
         return data_return
-
-
-
-
-
-
```

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/lib/utils/send_code.py` & `django-oasis4-auth-1.1.0/oasis_auth/lib/utils/send_code.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/locale/es/LC_MESSAGES/django.mo` & `django-oasis4-auth-1.1.0/oasis_auth/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/locale/es/LC_MESSAGES/django.po` & `django-oasis4-auth-1.1.0/oasis_auth/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/migrations/0001_initial.py` & `django-oasis4-auth-1.1.0/oasis_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/migrations/0003_userprofile_quota_userprofile_segment.py` & `django-oasis4-auth-1.1.0/oasis_auth/migrations/0003_userprofile_quota_userprofile_segment.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/models.py` & `django-oasis4-auth-1.1.0/oasis_auth/models.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/tasks/__init__.py` & `django-oasis4-auth-1.1.0/oasis_auth/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/tasks/sync_users.py` & `django-oasis4-auth-1.1.0/oasis_auth/tasks/sync_users.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/templates/default.html` & `django-oasis4-auth-1.1.0/oasis_auth/templates/default.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/templates/login.html` & `django-oasis4-auth-1.1.0/oasis_auth/templates/login.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/templates/register.html` & `django-oasis4-auth-1.1.0/oasis_auth/templates/register.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/templates/retrieve_password.html` & `django-oasis4-auth-1.1.0/oasis_auth/templates/retrieve_password.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/oasis_auth/urls.py` & `django-oasis4-auth-1.1.0/oasis_auth/urls.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9b0/pyproject.toml` & `django-oasis4-auth-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,35 +3,35 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "django-oasis4-auth"
-version = "1.0.9-beta.0"
+version = "1.1.0"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
 description = "Oasis 4 Authorization System for django"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     "License :: Other/Proprietary License",
     "Programming Language :: Python :: 3.9",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Framework :: Django",
     "Framework :: Django :: 4.1",
     "Environment :: Web Environment",
     "Operating System :: OS Independent",
     "Topic :: Internet :: WWW/HTTP"
 ]
 dependencies = [
     "Django>=4.1",
     "djangorestframework",
     "django-oasis4>=1.0.4",
-    "zibanu-django"
+    "zibanu-django>=1.2.0"
 ]
 keywords = [
     "django",
     "OASIS4"
 ]
```

