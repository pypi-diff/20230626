# Comparing `tmp/garpix_user-3.8.0.tar.gz` & `tmp/garpix_user-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_user-3.8.0.tar", last modified: Fri Jun 23 07:45:01 2023, max compression
+gzip compressed data, was "garpix_user-3.8.1.tar", last modified: Mon Jun 26 12:00:42 2023, max compression
```

## Comparing `garpix_user-3.8.0.tar` & `garpix_user-3.8.1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.947341 garpix_user-3.8.0/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-06-23 07:45:01.000000 garpix_user-3.8.0/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    11422 2023-06-23 07:45:01.947041 garpix_user-3.8.0/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.938306 garpix_user-3.8.0/garpix_user/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5552 2023-06-23 07:44:40.000000 garpix_user-3.8.0/garpix_user/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-05 12:27:45.000000 garpix_user-3.8.0/garpix_user/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2022-10-05 13:12:08.000000 garpix_user-3.8.0/garpix_user/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10758 2023-06-23 07:44:40.000000 garpix_user-3.8.0/garpix_user/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3261 2022-10-05 12:27:45.000000 garpix_user-3.8.0/garpix_user/README.rst
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       57 2022-10-05 13:12:08.000000 garpix_user-3.8.0/garpix_user/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.939460 garpix_user-3.8.0/garpix_user/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      238 2022-10-27 08:16:59.000000 garpix_user-3.8.0/garpix_user/admin/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      204 2022-10-05 12:27:45.000000 garpix_user-3.8.0/garpix_user/admin/referral_type.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1113 2023-03-06 08:48:05.000000 garpix_user-3.8.0/garpix_user/admin/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      260 2022-10-27 08:16:59.000000 garpix_user-3.8.0/garpix_user/admin/user_session.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      128 2022-10-05 13:12:08.000000 garpix_user-3.8.0/garpix_user/apps.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1782 2023-04-11 08:24:40.000000 garpix_user-3.8.0/garpix_user/exceptions.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.939665 garpix_user-3.8.0/garpix_user/forms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2022-10-05 12:27:45.000000 garpix_user-3.8.0/garpix_user/forms/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1009 2023-05-31 03:44:48.000000 garpix_user-3.8.0/garpix_user/forms/login.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.935676 garpix_user-3.8.0/garpix_user/locale/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.935727 garpix_user-3.8.0/garpix_user/locale/ru/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.939905 garpix_user-3.8.0/garpix_user/locale/ru/LC_MESSAGES/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     7137 2023-06-23 07:44:40.000000 garpix_user-3.8.0/garpix_user/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9522 2023-06-23 07:44:40.000000 garpix_user-3.8.0/garpix_user/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.940026 garpix_user-3.8.0/garpix_user/mixins/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.8.0/garpix_user/mixins/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.940217 garpix_user-3.8.0/garpix_user/mixins/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       58 2022-10-27 08:16:59.000000 garpix_user-3.8.0/garpix_user/mixins/models/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.940651 garpix_user-3.8.0/garpix_user/mixins/models/confirm/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      114 2022-10-05 12:27:45.000000 garpix_user-3.8.0/garpix_user/mixins/models/confirm/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      637 2022-11-03 14:31:02.000000 garpix_user-3.8.0/garpix_user/mixins/models/confirm/code_length_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5477 2023-05-10 13:07:30.000000 garpix_user-3.8.0/garpix_user/mixins/models/confirm/email_confirm.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3562 2023-05-10 13:07:30.000000 garpix_user-3.8.0/garpix_user/mixins/models/confirm/phone_confirm.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5582 2023-06-23 07:44:40.000000 garpix_user-3.8.0/garpix_user/mixins/models/restore_password.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.940968 garpix_user-3.8.0/garpix_user/mixins/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      103 2023-01-19 12:18:01.000000 garpix_user-3.8.0/garpix_user/mixins/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-02-24 11:10:07.000000 garpix_user-3.8.0/garpix_user/mixins/serializers/password_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2022-10-24 09:55:11.000000 garpix_user-3.8.0/garpix_user/mixins/serializers/to_lower.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.941593 garpix_user-3.8.0/garpix_user/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      237 2022-10-27 08:16:59.000000 garpix_user-3.8.0/garpix_user/models/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      881 2022-11-07 08:16:45.000000 garpix_user-3.8.0/garpix_user/models/access_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      968 2022-10-05 12:27:45.000000 garpix_user-3.8.0/garpix_user/models/refferal.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      885 2022-11-07 08:16:45.000000 garpix_user-3.8.0/garpix_user/models/refresh_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3225 2023-03-01 08:01:40.000000 garpix_user-3.8.0/garpix_user/models/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4986 2023-04-24 07:29:27.000000 garpix_user-3.8.0/garpix_user/models/user_session.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.941784 garpix_user-3.8.0/garpix_user/rest/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.8.0/garpix_user/rest/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2702 2023-06-23 07:44:40.000000 garpix_user-3.8.0/garpix_user/rest/authentication.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.942971 garpix_user-3.8.0/garpix_user/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      820 2023-06-23 07:44:40.000000 garpix_user-3.8.0/garpix_user/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1393 2023-02-07 14:13:30.000000 garpix_user-3.8.0/garpix_user/serializers/auth_token_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      469 2022-10-05 12:27:45.000000 garpix_user-3.8.0/garpix_user/serializers/email_confirmation_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      247 2023-06-23 07:44:40.000000 garpix_user-3.8.0/garpix_user/serializers/jwt_data_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1584 2023-05-31 09:44:39.000000 garpix_user-3.8.0/garpix_user/serializers/passwrod_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      434 2022-10-05 12:27:45.000000 garpix_user-3.8.0/garpix_user/serializers/phone_confirmation_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2022-10-05 12:27:45.000000 garpix_user-3.8.0/garpix_user/serializers/refresh_token_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4248 2023-03-07 08:55:10.000000 garpix_user-3.8.0/garpix_user/serializers/registration_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-01-18 14:28:54.000000 garpix_user-3.8.0/garpix_user/serializers/user_session_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2090 2023-01-19 12:18:01.000000 garpix_user-3.8.0/garpix_user/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1557 2023-06-23 07:44:40.000000 garpix_user-3.8.0/garpix_user/setup.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.943225 garpix_user-3.8.0/garpix_user/tasks/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2023-03-06 10:42:24.000000 garpix_user-3.8.0/garpix_user/tasks/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1074 2023-03-15 14:13:43.000000 garpix_user-3.8.0/garpix_user/tasks/delete_unconfirmed_users.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.936386 garpix_user-3.8.0/garpix_user/templates/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.943346 garpix_user-3.8.0/garpix_user/templates/garpix_user/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      269 2022-10-27 08:16:59.000000 garpix_user-3.8.0/garpix_user/templates/garpix_user/send_confirm.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.943585 garpix_user-3.8.0/garpix_user/tests/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2022-10-27 08:16:59.000000 garpix_user-3.8.0/garpix_user/tests/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.944064 garpix_user-3.8.0/garpix_user/tests/test_api/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2022-10-27 08:16:59.000000 garpix_user-3.8.0/garpix_user/tests/test_api/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.944292 garpix_user-3.8.0/garpix_user/tests/test_api/_trial_temp/
--rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-01-19 12:18:01.000000 garpix_user-3.8.0/garpix_user/tests/test_api/_trial_temp/_trial_marker
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       41 2022-10-26 15:07:44.000000 garpix_user-3.8.0/garpix_user/tests/test_api/_trial_temp/test.log
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8303 2022-10-27 08:16:59.000000 garpix_user-3.8.0/garpix_user/tests/test_api/api_login.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    14883 2023-01-19 12:18:01.000000 garpix_user-3.8.0/garpix_user/tests/test_api/api_registration.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5000 2023-04-07 13:05:13.000000 garpix_user-3.8.0/garpix_user/tests/test_api/api_user_session_restore_password.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2122 2023-01-19 12:18:01.000000 garpix_user-3.8.0/garpix_user/tests/test_views.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.944604 garpix_user-3.8.0/garpix_user/tests/utils/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-27 08:16:59.000000 garpix_user-3.8.0/garpix_user/tests/utils/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      681 2022-10-27 08:16:59.000000 garpix_user-3.8.0/garpix_user/tests/utils/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1294 2022-10-27 08:16:59.000000 garpix_user-3.8.0/garpix_user/tests/utils/test_case_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2661 2023-06-21 15:22:29.000000 garpix_user-3.8.0/garpix_user/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.945261 garpix_user-3.8.0/garpix_user/utils/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-10-27 08:16:59.000000 garpix_user-3.8.0/garpix_user/utils/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      855 2023-06-22 15:00:39.000000 garpix_user-3.8.0/garpix_user/utils/backends.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2022-10-05 12:27:45.000000 garpix_user-3.8.0/garpix_user/utils/current_date.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      406 2022-10-26 12:08:38.000000 garpix_user-3.8.0/garpix_user/utils/drf_spectacular.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      329 2023-06-23 07:44:40.000000 garpix_user-3.8.0/garpix_user/utils/get_token_from_request.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      542 2023-02-24 11:10:07.000000 garpix_user-3.8.0/garpix_user/utils/repluralize.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.946741 garpix_user-3.8.0/garpix_user/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      603 2023-01-19 12:18:01.000000 garpix_user-3.8.0/garpix_user/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1154 2023-01-19 12:18:01.000000 garpix_user-3.8.0/garpix_user/views/change_password_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3914 2023-04-19 13:51:11.000000 garpix_user-3.8.0/garpix_user/views/email_confirmation_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2426 2023-06-23 07:44:40.000000 garpix_user-3.8.0/garpix_user/views/login_views.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1211 2022-10-05 12:27:45.000000 garpix_user-3.8.0/garpix_user/views/logout_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2942 2023-06-23 07:44:40.000000 garpix_user-3.8.0/garpix_user/views/obtain_auth_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3292 2023-02-24 11:10:07.000000 garpix_user-3.8.0/garpix_user/views/phone_confirmation_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-01-19 12:18:01.000000 garpix_user-3.8.0/garpix_user/views/referral_links_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1781 2023-03-17 09:50:52.000000 garpix_user-3.8.0/garpix_user/views/refresh_token_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      739 2023-01-19 12:18:01.000000 garpix_user-3.8.0/garpix_user/views/registration_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3452 2023-05-31 09:44:39.000000 garpix_user-3.8.0/garpix_user/views/restore_password_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1261 2023-01-19 12:18:01.000000 garpix_user-3.8.0/garpix_user/views/user_session_view.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-23 07:45:01.939007 garpix_user-3.8.0/garpix_user.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    11422 2023-06-23 07:45:01.000000 garpix_user-3.8.0/garpix_user.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3187 2023-06-23 07:45:01.000000 garpix_user-3.8.0/garpix_user.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-23 07:45:01.000000 garpix_user-3.8.0/garpix_user.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-23 07:45:01.000000 garpix_user-3.8.0/garpix_user.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      279 2023-06-23 07:45:01.000000 garpix_user-3.8.0/garpix_user.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       12 2023-06-23 07:45:01.000000 garpix_user-3.8.0/garpix_user.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-06-23 07:45:01.947390 garpix_user-3.8.0/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1557 2023-06-23 07:45:01.000000 garpix_user-3.8.0/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.815034 garpix_user-3.8.1/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-06-26 12:00:42.000000 garpix_user-3.8.1/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    11422 2023-06-26 12:00:42.814795 garpix_user-3.8.1/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.805172 garpix_user-3.8.1/garpix_user/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5614 2023-06-26 12:00:32.000000 garpix_user-3.8.1/garpix_user/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2022-10-05 13:12:08.000000 garpix_user-3.8.1/garpix_user/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10758 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3261 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/README.rst
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       57 2022-10-05 13:12:08.000000 garpix_user-3.8.1/garpix_user/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.806377 garpix_user-3.8.1/garpix_user/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      238 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/admin/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      204 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/admin/referral_type.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1113 2023-03-06 08:48:05.000000 garpix_user-3.8.1/garpix_user/admin/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      260 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/admin/user_session.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      128 2022-10-05 13:12:08.000000 garpix_user-3.8.1/garpix_user/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1782 2023-04-11 08:24:40.000000 garpix_user-3.8.1/garpix_user/exceptions.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.806587 garpix_user-3.8.1/garpix_user/forms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/forms/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1009 2023-05-31 03:44:48.000000 garpix_user-3.8.1/garpix_user/forms/login.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.802440 garpix_user-3.8.1/garpix_user/locale/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.802491 garpix_user-3.8.1/garpix_user/locale/ru/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.806815 garpix_user-3.8.1/garpix_user/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     7137 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9522 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.806926 garpix_user-3.8.1/garpix_user/mixins/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/mixins/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.807106 garpix_user-3.8.1/garpix_user/mixins/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       58 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/mixins/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.808653 garpix_user-3.8.1/garpix_user/mixins/models/confirm/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      114 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/mixins/models/confirm/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      637 2022-11-03 14:31:02.000000 garpix_user-3.8.1/garpix_user/mixins/models/confirm/code_length_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5477 2023-05-10 13:07:30.000000 garpix_user-3.8.1/garpix_user/mixins/models/confirm/email_confirm.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3562 2023-05-10 13:07:30.000000 garpix_user-3.8.1/garpix_user/mixins/models/confirm/phone_confirm.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5552 2023-06-26 12:00:32.000000 garpix_user-3.8.1/garpix_user/mixins/models/restore_password.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.809071 garpix_user-3.8.1/garpix_user/mixins/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      103 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/mixins/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-02-24 11:10:07.000000 garpix_user-3.8.1/garpix_user/mixins/serializers/password_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2022-10-24 09:55:11.000000 garpix_user-3.8.1/garpix_user/mixins/serializers/to_lower.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.809809 garpix_user-3.8.1/garpix_user/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      237 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/models/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      881 2022-11-07 08:16:45.000000 garpix_user-3.8.1/garpix_user/models/access_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      968 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/models/refferal.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      885 2022-11-07 08:16:45.000000 garpix_user-3.8.1/garpix_user/models/refresh_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3225 2023-03-01 08:01:40.000000 garpix_user-3.8.1/garpix_user/models/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4986 2023-04-24 07:29:27.000000 garpix_user-3.8.1/garpix_user/models/user_session.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.810002 garpix_user-3.8.1/garpix_user/rest/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/rest/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2702 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/rest/authentication.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.810956 garpix_user-3.8.1/garpix_user/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      820 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1393 2023-02-07 14:13:30.000000 garpix_user-3.8.1/garpix_user/serializers/auth_token_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      469 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/serializers/email_confirmation_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      247 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/serializers/jwt_data_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1584 2023-05-31 09:44:39.000000 garpix_user-3.8.1/garpix_user/serializers/passwrod_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      434 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/serializers/phone_confirmation_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/serializers/refresh_token_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4248 2023-03-07 08:55:10.000000 garpix_user-3.8.1/garpix_user/serializers/registration_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-01-18 14:28:54.000000 garpix_user-3.8.1/garpix_user/serializers/user_session_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2090 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1557 2023-06-26 12:00:32.000000 garpix_user-3.8.1/garpix_user/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.811184 garpix_user-3.8.1/garpix_user/tasks/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2023-03-06 10:42:24.000000 garpix_user-3.8.1/garpix_user/tasks/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1074 2023-03-15 14:13:43.000000 garpix_user-3.8.1/garpix_user/tasks/delete_unconfirmed_users.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.803145 garpix_user-3.8.1/garpix_user/templates/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.811293 garpix_user-3.8.1/garpix_user/templates/garpix_user/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      269 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/templates/garpix_user/send_confirm.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.811515 garpix_user-3.8.1/garpix_user/tests/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/tests/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.812014 garpix_user-3.8.1/garpix_user/tests/test_api/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/tests/test_api/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.812240 garpix_user-3.8.1/garpix_user/tests/test_api/_trial_temp/
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/tests/test_api/_trial_temp/_trial_marker
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       41 2022-10-26 15:07:44.000000 garpix_user-3.8.1/garpix_user/tests/test_api/_trial_temp/test.log
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8303 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/tests/test_api/api_login.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    14883 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/tests/test_api/api_registration.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5000 2023-04-07 13:05:13.000000 garpix_user-3.8.1/garpix_user/tests/test_api/api_user_session_restore_password.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2122 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/tests/test_views.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.812606 garpix_user-3.8.1/garpix_user/tests/utils/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/tests/utils/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      681 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/tests/utils/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1294 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/tests/utils/test_case_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2661 2023-06-21 15:22:29.000000 garpix_user-3.8.1/garpix_user/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.813293 garpix_user-3.8.1/garpix_user/utils/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-10-27 08:16:59.000000 garpix_user-3.8.1/garpix_user/utils/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      855 2023-06-22 15:00:39.000000 garpix_user-3.8.1/garpix_user/utils/backends.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/utils/current_date.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      406 2022-10-26 12:08:38.000000 garpix_user-3.8.1/garpix_user/utils/drf_spectacular.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      329 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/utils/get_token_from_request.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      542 2023-02-24 11:10:07.000000 garpix_user-3.8.1/garpix_user/utils/repluralize.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.814594 garpix_user-3.8.1/garpix_user/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      603 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1154 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/views/change_password_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3914 2023-04-19 13:51:11.000000 garpix_user-3.8.1/garpix_user/views/email_confirmation_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2426 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/views/login_views.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1211 2022-10-05 12:27:45.000000 garpix_user-3.8.1/garpix_user/views/logout_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2942 2023-06-23 07:44:40.000000 garpix_user-3.8.1/garpix_user/views/obtain_auth_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3292 2023-02-24 11:10:07.000000 garpix_user-3.8.1/garpix_user/views/phone_confirmation_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/views/referral_links_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1781 2023-03-17 09:50:52.000000 garpix_user-3.8.1/garpix_user/views/refresh_token_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      739 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/views/registration_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3452 2023-05-31 09:44:39.000000 garpix_user-3.8.1/garpix_user/views/restore_password_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1261 2023-01-19 12:18:01.000000 garpix_user-3.8.1/garpix_user/views/user_session_view.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:00:42.805906 garpix_user-3.8.1/garpix_user.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    11422 2023-06-26 12:00:42.000000 garpix_user-3.8.1/garpix_user.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3187 2023-06-26 12:00:42.000000 garpix_user-3.8.1/garpix_user.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-26 12:00:42.000000 garpix_user-3.8.1/garpix_user.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-26 12:00:42.000000 garpix_user-3.8.1/garpix_user.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      279 2023-06-26 12:00:42.000000 garpix_user-3.8.1/garpix_user.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       12 2023-06-26 12:00:42.000000 garpix_user-3.8.1/garpix_user.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-06-26 12:00:42.815072 garpix_user-3.8.1/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1557 2023-06-26 12:00:42.000000 garpix_user-3.8.1/setup.py
```

### Comparing `garpix_user-3.8.0/PKG-INFO` & `garpix_user-3.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_user
-Version: 3.8.0
+Version: 3.8.1
 Home-page: https://github.com/garpixcms/garpix_user
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_user-3.8.0/garpix_user/CHANGELOG.md` & `garpix_user-3.8.1/garpix_user/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+### 3.8.1 (26.06.2023)
+
+- Password restore by username fixed
+
 ### 3.8.0 (22.06.2023)
 
 - JWT token authorization added (see `Readme.md`)
 - `REST_AUTH_HEADER_KEY` setting added (see `Readme.md`)
 - Password restore by username fixed
 
 ### 3.7.1 (21.06.2023)
```

### Comparing `garpix_user-3.8.0/garpix_user/CONTRIBUTING.md` & `garpix_user-3.8.1/garpix_user/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/README.md` & `garpix_user-3.8.1/garpix_user/README.md`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/README.rst` & `garpix_user-3.8.1/garpix_user/README.rst`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/admin/user.py` & `garpix_user-3.8.1/garpix_user/admin/user.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/exceptions.py` & `garpix_user-3.8.1/garpix_user/exceptions.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/forms/login.py` & `garpix_user-3.8.1/garpix_user/forms/login.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/locale/ru/LC_MESSAGES/django.mo` & `garpix_user-3.8.1/garpix_user/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/locale/ru/LC_MESSAGES/django.po` & `garpix_user-3.8.1/garpix_user/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/mixins/models/confirm/code_length_mixin.py` & `garpix_user-3.8.1/garpix_user/mixins/models/confirm/code_length_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/mixins/models/confirm/email_confirm.py` & `garpix_user-3.8.1/garpix_user/mixins/models/confirm/email_confirm.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/mixins/models/confirm/phone_confirm.py` & `garpix_user-3.8.1/garpix_user/mixins/models/confirm/phone_confirm.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/mixins/models/restore_password.py` & `garpix_user-3.8.1/garpix_user/mixins/models/restore_password.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.db import models, transaction
-from django.db.models import Q
 from django.utils.translation import gettext as _
 from garpix_utils.string import get_random_string
 import string
 from datetime import datetime, timezone, timedelta
 
 from garpix_user.exceptions import NotConfirmedException
 from garpix_user.exceptions import IncorrectCodeException, NoTimeLeftException, WaitException, UserUnregisteredException
@@ -24,22 +23,22 @@
 
     def _check_and_get_user(self, username):
 
         User = get_user_model()
 
         USERNAME_FIELDS = getattr(User, 'USERNAME_FIELDS', ('email',))
 
-        user_data = Q()
+        user_data = {}
 
         for field in USERNAME_FIELDS:
-            user_data |= Q(**{field: username})
+            user_data.update({field: username})
             if field != 'username':
-                user_data |= Q(**{f'is_{field}_confirmed': True})
+                user_data.update({f'is_{field}_confirmed': True})
 
-        if user := User.active_objects.filter(user_data).first():
+        if user := User.active_objects.filter(**user_data).first():
             return True, user
 
         return False, UserUnregisteredException(field='username',
                                                 extra_data={'value': username})
 
     def _check_request_time(self):
```

### Comparing `garpix_user-3.8.0/garpix_user/mixins/serializers/password_mixin.py` & `garpix_user-3.8.1/garpix_user/mixins/serializers/password_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/models/access_token.py` & `garpix_user-3.8.1/garpix_user/models/access_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/models/refferal.py` & `garpix_user-3.8.1/garpix_user/models/refferal.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/models/refresh_token.py` & `garpix_user-3.8.1/garpix_user/models/refresh_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/models/user.py` & `garpix_user-3.8.1/garpix_user/models/user.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/models/user_session.py` & `garpix_user-3.8.1/garpix_user/models/user_session.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/rest/authentication.py` & `garpix_user-3.8.1/garpix_user/rest/authentication.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/serializers/__init__.py` & `garpix_user-3.8.1/garpix_user/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/serializers/auth_token_serializer.py` & `garpix_user-3.8.1/garpix_user/serializers/auth_token_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/serializers/passwrod_serializer.py` & `garpix_user-3.8.1/garpix_user/serializers/passwrod_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/serializers/registration_serializer.py` & `garpix_user-3.8.1/garpix_user/serializers/registration_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/settings.py` & `garpix_user-3.8.1/garpix_user/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/setup.py` & `garpix_user-3.8.1/garpix_user/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_user')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_user',
-    version='3.8.0',
+    version='3.8.1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_user',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

### Comparing `garpix_user-3.8.0/garpix_user/tasks/delete_unconfirmed_users.py` & `garpix_user-3.8.1/garpix_user/tasks/delete_unconfirmed_users.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/tests/test_api/api_login.py` & `garpix_user-3.8.1/garpix_user/tests/test_api/api_login.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/tests/test_api/api_registration.py` & `garpix_user-3.8.1/garpix_user/tests/test_api/api_registration.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/tests/test_api/api_user_session_restore_password.py` & `garpix_user-3.8.1/garpix_user/tests/test_api/api_user_session_restore_password.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/tests/test_views.py` & `garpix_user-3.8.1/garpix_user/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/tests/utils/settings.py` & `garpix_user-3.8.1/garpix_user/tests/utils/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/tests/utils/test_case_mixin.py` & `garpix_user-3.8.1/garpix_user/tests/utils/test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/urls.py` & `garpix_user-3.8.1/garpix_user/urls.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/utils/backends.py` & `garpix_user-3.8.1/garpix_user/utils/backends.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/utils/repluralize.py` & `garpix_user-3.8.1/garpix_user/utils/repluralize.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/views/__init__.py` & `garpix_user-3.8.1/garpix_user/views/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/views/change_password_view.py` & `garpix_user-3.8.1/garpix_user/views/change_password_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/views/email_confirmation_view.py` & `garpix_user-3.8.1/garpix_user/views/email_confirmation_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/views/login_views.py` & `garpix_user-3.8.1/garpix_user/views/login_views.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/views/logout_view.py` & `garpix_user-3.8.1/garpix_user/views/logout_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/views/obtain_auth_token.py` & `garpix_user-3.8.1/garpix_user/views/obtain_auth_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/views/phone_confirmation_view.py` & `garpix_user-3.8.1/garpix_user/views/phone_confirmation_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/views/referral_links_view.py` & `garpix_user-3.8.1/garpix_user/views/referral_links_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/views/refresh_token_view.py` & `garpix_user-3.8.1/garpix_user/views/refresh_token_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/views/registration_view.py` & `garpix_user-3.8.1/garpix_user/views/registration_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/views/restore_password_view.py` & `garpix_user-3.8.1/garpix_user/views/restore_password_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user/views/user_session_view.py` & `garpix_user-3.8.1/garpix_user/views/user_session_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/garpix_user.egg-info/PKG-INFO` & `garpix_user-3.8.1/garpix_user.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-user
-Version: 3.8.0
+Version: 3.8.1
 Home-page: https://github.com/garpixcms/garpix_user
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_user-3.8.0/garpix_user.egg-info/SOURCES.txt` & `garpix_user-3.8.1/garpix_user.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_user-3.8.0/setup.py` & `garpix_user-3.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_user')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_user',
-    version='3.8.0',
+    version='3.8.1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_user',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

