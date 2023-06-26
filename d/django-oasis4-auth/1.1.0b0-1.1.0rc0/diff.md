# Comparing `tmp/django-oasis4-auth-1.1.0b0.tar.gz` & `tmp/django-oasis4-auth-1.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oasis4-auth-1.1.0b0.tar", last modified: Mon Jun 19 19:18:43 2023, max compression
+gzip compressed data, was "django-oasis4-auth-1.1.0rc0.tar", last modified: Mon Jun 26 19:19:30 2023, max compression
```

## Comparing `django-oasis4-auth-1.1.0b0.tar` & `django-oasis4-auth-1.1.0rc0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.975986 django-oasis4-auth-1.1.0b0/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-auth-1.1.0b0/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)       93 2023-01-18 12:21:52.000000 django-oasis4-auth-1.1.0b0/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    22834 2023-06-19 19:18:43.975986 django-oasis4-auth-1.1.0b0/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     9954 2023-06-19 19:17:48.000000 django-oasis4-auth-1.1.0b0/README.md
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.966986 django-oasis4-auth-1.1.0b0/django_oasis4_auth.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    22834 2023-06-19 19:18:43.000000 django-oasis4-auth-1.1.0b0/django_oasis4_auth.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1471 2023-06-19 19:18:43.000000 django-oasis4-auth-1.1.0b0/django_oasis4_auth.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-06-19 19:18:43.000000 django-oasis4-auth-1.1.0b0/django_oasis4_auth.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       67 2023-06-19 19:18:43.000000 django-oasis4-auth-1.1.0b0/django_oasis4_auth.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       11 2023-06-19 19:18:43.000000 django-oasis4-auth-1.1.0b0/django_oasis4_auth.egg-info/top_level.txt
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.967986 django-oasis4-auth-1.1.0b0/oasis_auth/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-20 02:22:34.000000 django-oasis4-auth-1.1.0b0/oasis_auth/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.967986 django-oasis4-auth-1.1.0b0/oasis_auth/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      507 2023-01-07 20:01:29.000000 django-oasis4-auth-1.1.0b0/oasis_auth/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.969986 django-oasis4-auth-1.1.0b0/oasis_auth/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      578 2023-01-27 22:32:38.000000 django-oasis4-auth-1.1.0b0/oasis_auth/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      786 2023-01-27 22:44:36.000000 django-oasis4-auth-1.1.0b0/oasis_auth/api/serializers/user.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.969986 django-oasis4-auth-1.1.0b0/oasis_auth/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      590 2023-01-18 03:44:01.000000 django-oasis4-auth-1.1.0b0/oasis_auth/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    15973 2023-06-19 19:02:47.000000 django-oasis4-auth-1.1.0b0/oasis_auth/api/services/oasis_auth.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1180 2023-06-19 19:04:20.000000 django-oasis4-auth-1.1.0b0/oasis_auth/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.970986 django-oasis4-auth-1.1.0b0/oasis_auth/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      509 2022-12-20 17:00:22.000000 django-oasis4-auth-1.1.0b0/oasis_auth/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.971986 django-oasis4-auth-1.1.0b0/oasis_auth/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      580 2023-01-18 20:29:06.000000 django-oasis4-auth-1.1.0b0/oasis_auth/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2368 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0b0/oasis_auth/lib/managers/user_profile.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1033 2023-06-19 19:04:20.000000 django-oasis4-auth-1.1.0b0/oasis_auth/lib/signal_events.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      424 2023-06-19 18:55:26.000000 django-oasis4-auth-1.1.0b0/oasis_auth/lib/signals.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.971986 django-oasis4-auth-1.1.0b0/oasis_auth/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      627 2023-01-18 15:44:17.000000 django-oasis4-auth-1.1.0b0/oasis_auth/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2974 2023-05-23 13:18:45.000000 django-oasis4-auth-1.1.0b0/oasis_auth/lib/utils/auth_actions.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2207 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0b0/oasis_auth/lib/utils/send_code.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.963986 django-oasis4-auth-1.1.0b0/oasis_auth/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.964986 django-oasis4-auth-1.1.0b0/oasis_auth/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.972986 django-oasis4-auth-1.1.0b0/oasis_auth/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4792 2023-03-16 16:15:08.000000 django-oasis4-auth-1.1.0b0/oasis_auth/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     7121 2023-03-16 16:14:53.000000 django-oasis4-auth-1.1.0b0/oasis_auth/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.973986 django-oasis4-auth-1.1.0b0/oasis_auth/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2055 2023-01-18 02:10:57.000000 django-oasis4-auth-1.1.0b0/oasis_auth/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      438 2023-01-18 20:03:48.000000 django-oasis4-auth-1.1.0b0/oasis_auth/migrations/0002_remove_userprofile_first_name_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      598 2023-03-01 16:07:21.000000 django-oasis4-auth-1.1.0b0/oasis_auth/migrations/0003_userprofile_quota_userprofile_segment.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      354 2023-03-01 16:22:58.000000 django-oasis4-auth-1.1.0b0/oasis_auth/migrations/0004_remove_userprofile_quota.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-01-18 02:10:57.000000 django-oasis4-auth-1.1.0b0/oasis_auth/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2222 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0b0/oasis_auth/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.973986 django-oasis4-auth-1.1.0b0/oasis_auth/tasks/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      581 2023-02-15 14:18:51.000000 django-oasis4-auth-1.1.0b0/oasis_auth/tasks/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2211 2023-03-01 16:31:30.000000 django-oasis4-auth-1.1.0b0/oasis_auth/tasks/sync_users.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-19 19:18:43.974986 django-oasis4-auth-1.1.0b0/oasis_auth/templates/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2022-12-22 15:55:10.000000 django-oasis4-auth-1.1.0b0/oasis_auth/templates/default.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-02 19:51:33.000000 django-oasis4-auth-1.1.0b0/oasis_auth/templates/default.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2022-12-22 15:55:10.000000 django-oasis4-auth-1.1.0b0/oasis_auth/templates/login.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-01 21:00:33.000000 django-oasis4-auth-1.1.0b0/oasis_auth/templates/login.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      745 2023-01-18 04:44:01.000000 django-oasis4-auth-1.1.0b0/oasis_auth/templates/register.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      509 2023-03-01 21:00:33.000000 django-oasis4-auth-1.1.0b0/oasis_auth/templates/register.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      634 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0b0/oasis_auth/templates/retrieve_password.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      405 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0b0/oasis_auth/templates/retrieve_password.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1151 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0b0/oasis_auth/urls.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      864 2023-06-19 19:17:02.000000 django-oasis4-auth-1.1.0b0/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-06-19 19:18:43.975986 django-oasis4-auth-1.1.0b0/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.437446 django-oasis4-auth-1.1.0rc0/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-auth-1.1.0rc0/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)       93 2023-01-18 12:21:52.000000 django-oasis4-auth-1.1.0rc0/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    22835 2023-06-26 19:19:30.437446 django-oasis4-auth-1.1.0rc0/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     9954 2023-06-19 19:17:48.000000 django-oasis4-auth-1.1.0rc0/README.md
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.430446 django-oasis4-auth-1.1.0rc0/django_oasis4_auth.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    22835 2023-06-26 19:19:30.000000 django-oasis4-auth-1.1.0rc0/django_oasis4_auth.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1471 2023-06-26 19:19:30.000000 django-oasis4-auth-1.1.0rc0/django_oasis4_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-06-26 19:19:30.000000 django-oasis4-auth-1.1.0rc0/django_oasis4_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       74 2023-06-26 19:19:30.000000 django-oasis4-auth-1.1.0rc0/django_oasis4_auth.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       11 2023-06-26 19:19:30.000000 django-oasis4-auth-1.1.0rc0/django_oasis4_auth.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.431446 django-oasis4-auth-1.1.0rc0/oasis_auth/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-20 02:22:34.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.431446 django-oasis4-auth-1.1.0rc0/oasis_auth/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      507 2023-01-07 20:01:29.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.431446 django-oasis4-auth-1.1.0rc0/oasis_auth/api/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      578 2023-01-27 22:32:38.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/api/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      786 2023-01-27 22:44:36.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/api/serializers/user.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.432446 django-oasis4-auth-1.1.0rc0/oasis_auth/api/services/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      590 2023-01-18 03:44:01.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/api/services/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    15973 2023-06-19 19:02:47.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/api/services/oasis_auth.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1180 2023-06-19 19:04:20.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.432446 django-oasis4-auth-1.1.0rc0/oasis_auth/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      509 2022-12-20 17:00:22.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.433446 django-oasis4-auth-1.1.0rc0/oasis_auth/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      580 2023-01-18 20:29:06.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2368 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/lib/managers/user_profile.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1033 2023-06-19 19:04:20.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/lib/signal_events.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      424 2023-06-19 18:55:26.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/lib/signals.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.433446 django-oasis4-auth-1.1.0rc0/oasis_auth/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      627 2023-01-18 15:44:17.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2974 2023-05-23 13:18:45.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/lib/utils/auth_actions.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2207 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/lib/utils/send_code.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.427446 django-oasis4-auth-1.1.0rc0/oasis_auth/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.428446 django-oasis4-auth-1.1.0rc0/oasis_auth/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.434446 django-oasis4-auth-1.1.0rc0/oasis_auth/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     4792 2023-03-16 16:15:08.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     7121 2023-03-16 16:14:53.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.435446 django-oasis4-auth-1.1.0rc0/oasis_auth/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2055 2023-01-18 02:10:57.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      438 2023-01-18 20:03:48.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/migrations/0002_remove_userprofile_first_name_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      598 2023-03-01 16:07:21.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/migrations/0003_userprofile_quota_userprofile_segment.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      354 2023-03-01 16:22:58.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/migrations/0004_remove_userprofile_quota.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-01-18 02:10:57.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2222 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.435446 django-oasis4-auth-1.1.0rc0/oasis_auth/tasks/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      581 2023-02-15 14:18:51.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/tasks/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2211 2023-03-01 16:31:30.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/tasks/sync_users.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:19:30.437446 django-oasis4-auth-1.1.0rc0/oasis_auth/templates/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2022-12-22 15:55:10.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/templates/default.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-02 19:51:33.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/templates/default.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2022-12-22 15:55:10.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/templates/login.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-01 21:00:33.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/templates/login.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      745 2023-01-18 04:44:01.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/templates/register.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      509 2023-03-01 21:00:33.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/templates/register.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      634 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/templates/retrieve_password.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      405 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/templates/retrieve_password.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1151 2023-03-16 14:42:57.000000 django-oasis4-auth-1.1.0rc0/oasis_auth/urls.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      869 2023-06-26 19:16:35.000000 django-oasis4-auth-1.1.0rc0/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-06-26 19:19:30.437446 django-oasis4-auth-1.1.0rc0/setup.cfg
```

### Comparing `django-oasis4-auth-1.1.0b0/LICENSE` & `django-oasis4-auth-1.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/PKG-INFO` & `django-oasis4-auth-1.1.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4-auth
-Version: 1.1.0b0
+Version: 1.1.0rc0
 Summary: Oasis 4 Authorization System for django
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
```

### Comparing `django-oasis4-auth-1.1.0b0/README.md` & `django-oasis4-auth-1.1.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/django_oasis4_auth.egg-info/PKG-INFO` & `django-oasis4-auth-1.1.0rc0/django_oasis4_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4-auth
-Version: 1.1.0b0
+Version: 1.1.0rc0
 Summary: Oasis 4 Authorization System for django
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
```

### Comparing `django-oasis4-auth-1.1.0b0/django_oasis4_auth.egg-info/SOURCES.txt` & `django-oasis4-auth-1.1.0rc0/django_oasis4_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/api/serializers/__init__.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/api/serializers/user.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/api/serializers/user.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/api/services/__init__.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/api/services/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/api/services/oasis_auth.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/api/services/oasis_auth.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/apps.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/apps.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/lib/managers/__init__.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/lib/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/lib/managers/user_profile.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/lib/managers/user_profile.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/lib/signal_events.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/lib/signal_events.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/lib/utils/__init__.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/lib/utils/auth_actions.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/lib/utils/auth_actions.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/lib/utils/send_code.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/lib/utils/send_code.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/locale/es/LC_MESSAGES/django.mo` & `django-oasis4-auth-1.1.0rc0/oasis_auth/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/locale/es/LC_MESSAGES/django.po` & `django-oasis4-auth-1.1.0rc0/oasis_auth/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/migrations/0001_initial.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/migrations/0003_userprofile_quota_userprofile_segment.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/migrations/0003_userprofile_quota_userprofile_segment.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/models.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/models.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/tasks/__init__.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/tasks/sync_users.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/tasks/sync_users.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/templates/default.html` & `django-oasis4-auth-1.1.0rc0/oasis_auth/templates/default.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/templates/login.html` & `django-oasis4-auth-1.1.0rc0/oasis_auth/templates/login.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/templates/register.html` & `django-oasis4-auth-1.1.0rc0/oasis_auth/templates/register.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/templates/retrieve_password.html` & `django-oasis4-auth-1.1.0rc0/oasis_auth/templates/retrieve_password.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/oasis_auth/urls.py` & `django-oasis4-auth-1.1.0rc0/oasis_auth/urls.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.1.0b0/pyproject.toml` & `django-oasis4-auth-1.1.0rc0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "django-oasis4-auth"
-version = "1.1.0-beta.0"
+version = "1.1.0-rc.0"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
 description = "Oasis 4 Authorization System for django"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
@@ -25,13 +25,13 @@
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

