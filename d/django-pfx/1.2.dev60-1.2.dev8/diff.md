# Comparing `tmp/django-pfx-1.2.dev60.tar.gz` & `tmp/django-pfx-1.2.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pfx-1.2.dev60.tar", last modified: Mon Jun 26 11:57:40 2023, max compression
+gzip compressed data, was "django-pfx-1.2.dev8.tar", last modified: Thu Mar 30 14:30:10 2023, max compression
```

## Comparing `django-pfx-1.2.dev60.tar` & `django-pfx-1.2.dev8.tar`

### file list

```diff
@@ -1,132 +1,100 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.356449 django-pfx-1.2.dev60/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      486 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1692 2023-06-26 11:57:40.356449 django-pfx-1.2.dev60/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.340449 django-pfx-1.2.dev60/django_pfx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1692 2023-06-26 11:57:40.000000 django-pfx-1.2.dev60/django_pfx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3388 2023-06-26 11:57:40.000000 django-pfx-1.2.dev60/django_pfx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 11:57:40.000000 django-pfx-1.2.dev60/django_pfx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-06-26 11:57:40.000000 django-pfx-1.2.dev60/django_pfx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-26 11:57:40.000000 django-pfx-1.2.dev60/django_pfx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.340449 django-pfx-1.2.dev60/img/
--rw-rw-rw-   0 root         (0) root         (0)     3190 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/img/pfx.png
--rw-rw-rw-   0 root         (0) root         (0)     2682 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/img/pfx.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.340449 django-pfx-1.2.dev60/pfx/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.342449 django-pfx-1.2.dev60/pfx/pfxcore/
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.342449 django-pfx-1.2.dev60/pfx/pfxcore/apidoc/
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/apidoc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/apidoc/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/apidoc/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.343449 django-pfx-1.2.dev60/pfx/pfxcore/decorator/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/decorator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2082 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/decorator/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/default_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.343449 django-pfx-1.2.dev60/pfx/pfxcore/http/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/http/json_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.335449 django-pfx-1.2.dev60/pfx/pfxcore/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.335449 django-pfx-1.2.dev60/pfx/pfxcore/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.343449 django-pfx-1.2.dev60/pfx/pfxcore/locale/fr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     3331 2023-06-26 11:57:36.000000 django-pfx-1.2.dev60/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     5332 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.344449 django-pfx-1.2.dev60/pfx/pfxcore/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.344449 django-pfx-1.2.dev60/pfx/pfxcore/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4985 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/management/commands/makeapidoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.345449 django-pfx-1.2.dev60/pfx/pfxcore/middleware/
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/middleware/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2706 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/middleware/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/middleware/locale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.345449 django-pfx-1.2.dev60/pfx/pfxcore/models/
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/models/cache_mixins.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/models/not_null_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     2793 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/models/pfx_models.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/models/user_filtered_queryset_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.346449 django-pfx-1.2.dev60/pfx/pfxcore/serializers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/serializers/json.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2936 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/shortcuts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.346449 django-pfx-1.2.dev60/pfx/pfxcore/storage/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2131 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/storage/s3_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.336449 django-pfx-1.2.dev60/pfx/pfxcore/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.347449 django-pfx-1.2.dev60/pfx/pfxcore/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      511 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/templates/registration/password_reset_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/templates/registration/welcome_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/templates/registration/welcome_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)    10198 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/test.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.348449 django-pfx-1.2.dev60/pfx/pfxcore/views/
--rw-rw-rw-   0 root         (0) root         (0)      628 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11581 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/authentication_views.py
--rw-rw-rw-   0 root         (0) root         (0)     9398 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     4491 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/filters_views.py
--rw-rw-rw-   0 root         (0) root         (0)      912 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/locale_views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.351449 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      566 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/date_format.py
--rw-rw-rw-   0 root         (0) root         (0)      970 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      492 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/list_count.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/list_items.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/list_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/list_order.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/list_search.py
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/media_redirect.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/meta_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/meta_filters.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/meta_orders.py
--rw-rw-rw-   0 root         (0) root         (0)     1412 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/subset.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/subset_limit.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/subset_offset.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/subset_page.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/subset_page_size.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/parameters/subset_page_subset.py
--rw-rw-rw-   0 root         (0) root         (0)    23920 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pfx/pfxcore/views/rest_views.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      440 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/runtest.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-06-26 11:57:40.357449 django-pfx-1.2.dev60/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.352449 django-pfx-1.2.dev60/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.353449 django-pfx-1.2.dev60/tests/settings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/settings/ci.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/settings/common.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/settings/dev.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/settings/dev_custom_example.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/settings/dev_default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:57:40.356449 django-pfx-1.2.dev60/tests/tests/
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/basic_api_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    46979 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/basic_api_test.py
--rw-rw-rw-   0 root         (0) root         (0)    10373 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/test_api_doc.py
--rw-rw-rw-   0 root         (0) root         (0)    29106 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/test_auth_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4221 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     9909 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/test_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/test_filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/test_locale_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/test_perm_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     3725 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/test_perms_api.py
--rw-rw-rw-   0 root         (0) root         (0)     6810 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/test_shortcuts.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/test_timezone_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     3395 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/test_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/test_user_queryset.py
--rw-rw-rw-   0 root         (0) root         (0)     3558 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/test_view_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7356 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/tests/test_view_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     8269 2023-06-26 11:56:57.000000 django-pfx-1.2.dev60/tests/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.246585 django-pfx-1.2.dev8/
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-03-30 14:30:10.246585 django-pfx-1.2.dev8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.223583 django-pfx-1.2.dev8/django_pfx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-03-30 14:30:10.000000 django-pfx-1.2.dev8/django_pfx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-03-30 14:30:10.000000 django-pfx-1.2.dev8/django_pfx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 14:30:10.000000 django-pfx-1.2.dev8/django_pfx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-03-30 14:30:10.000000 django-pfx-1.2.dev8/django_pfx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-03-30 14:30:10.000000 django-pfx-1.2.dev8/django_pfx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.224583 django-pfx-1.2.dev8/img/
+-rw-rw-rw-   0 root         (0) root         (0)     3190 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/img/pfx.png
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/img/pfx.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.224583 django-pfx-1.2.dev8/pfx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.227583 django-pfx-1.2.dev8/pfx/pfxcore/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.228583 django-pfx-1.2.dev8/pfx/pfxcore/decorator/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/decorator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1824 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/decorator/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.228583 django-pfx-1.2.dev8/pfx/pfxcore/http/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/http/json_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.214582 django-pfx-1.2.dev8/pfx/pfxcore/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.214582 django-pfx-1.2.dev8/pfx/pfxcore/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.229583 django-pfx-1.2.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     3331 2023-03-30 14:30:03.000000 django-pfx-1.2.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     5332 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.230583 django-pfx-1.2.dev8/pfx/pfxcore/middleware/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/middleware/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/middleware/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/middleware/locale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.232584 django-pfx-1.2.dev8/pfx/pfxcore/models/
+-rw-rw-rw-   0 root         (0) root         (0)      303 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/models/cache_mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/models/not_null_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     2793 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/models/pfx_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/models/user_filtered_queryset_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.233584 django-pfx-1.2.dev8/pfx/pfxcore/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/serializers/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2761 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/shortcuts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.233584 django-pfx-1.2.dev8/pfx/pfxcore/storage/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/storage/s3_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.216582 django-pfx-1.2.dev8/pfx/pfxcore/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.235584 django-pfx-1.2.dev8/pfx/pfxcore/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/templates/registration/password_reset_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/templates/registration/welcome_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/templates/registration/welcome_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)     9419 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.237584 django-pfx-1.2.dev8/pfx/pfxcore/views/
+-rw-rw-rw-   0 root         (0) root         (0)      628 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10536 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/views/authentication_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     9169 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/views/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3754 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/views/filters_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/views/locale_views.py
+-rw-rw-rw-   0 root         (0) root         (0)    16585 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/views/rest_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      440 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/runtest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-03-30 14:30:10.247585 django-pfx-1.2.dev8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.238584 django-pfx-1.2.dev8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6123 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.241585 django-pfx-1.2.dev8/tests/settings/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/settings/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/settings/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/settings/dev.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/settings/dev_custom_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/settings/dev_default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.246585 django-pfx-1.2.dev8/tests/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2042 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/basic_api_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    40170 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/basic_api_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    26641 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_auth_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4221 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     9813 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_locale_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_perm_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     3725 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_perms_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     6810 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_shortcuts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_timezone_middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     2990 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_user_queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)     7356 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_view_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     6443 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/views.py
```

### Comparing `django-pfx-1.2.dev60/.gitlab-ci.yml` & `django-pfx-1.2.dev8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/LICENSE` & `django-pfx-1.2.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/PKG-INFO` & `django-pfx-1.2.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pfx
-Version: 1.2.dev60
+Version: 1.2.dev8
 Summary: Django PFX is a toolkit to build web APIs dedicated to be used by React progressive web app.
 Author: Hervé Martinet
 Author-email: herve.martinet@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://gitlab.com/hmartinet/django-pfx
 Project-URL: Tracker, https://gitlab.com/hmartinet/django-pfx/-/issues
 Classifier: Environment :: Web Environment
```

### Comparing `django-pfx-1.2.dev60/README.md` & `django-pfx-1.2.dev8/README.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/django_pfx.egg-info/PKG-INFO` & `django-pfx-1.2.dev8/django_pfx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pfx
-Version: 1.2.dev60
+Version: 1.2.dev8
 Summary: Django PFX is a toolkit to build web APIs dedicated to be used by React progressive web app.
 Author: Hervé Martinet
 Author-email: herve.martinet@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://gitlab.com/hmartinet/django-pfx
 Project-URL: Tracker, https://gitlab.com/hmartinet/django-pfx/-/issues
 Classifier: Environment :: Web Environment
```

### Comparing `django-pfx-1.2.dev60/django_pfx.egg-info/SOURCES.txt` & `django-pfx-1.2.dev8/django_pfx.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,33 +15,25 @@
 django_pfx.egg-info/requires.txt
 django_pfx.egg-info/top_level.txt
 img/pfx.png
 img/pfx.svg
 pfx/__init__.py
 pfx/pfxcore/__init__.py
 pfx/pfxcore/apps.py
-pfx/pfxcore/default_settings.py
 pfx/pfxcore/exceptions.py
 pfx/pfxcore/fields.py
-pfx/pfxcore/settings.py
 pfx/pfxcore/shortcuts.py
 pfx/pfxcore/test.py
 pfx/pfxcore/urls.py
-pfx/pfxcore/apidoc/__init__.py
-pfx/pfxcore/apidoc/parameters.py
-pfx/pfxcore/apidoc/tags.py
 pfx/pfxcore/decorator/__init__.py
 pfx/pfxcore/decorator/rest.py
 pfx/pfxcore/http/__init__.py
 pfx/pfxcore/http/json_response.py
 pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
 pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
-pfx/pfxcore/management/__init__.py
-pfx/pfxcore/management/commands/__init__.py
-pfx/pfxcore/management/commands/makeapidoc.py
 pfx/pfxcore/middleware/__init__.py
 pfx/pfxcore/middleware/authentication.py
 pfx/pfxcore/middleware/locale.py
 pfx/pfxcore/models/__init__.py
 pfx/pfxcore/models/cache_mixins.py
 pfx/pfxcore/models/not_null_fields.py
 pfx/pfxcore/models/pfx_models.py
@@ -56,52 +48,32 @@
 pfx/pfxcore/templates/registration/welcome_subject.txt
 pfx/pfxcore/views/__init__.py
 pfx/pfxcore/views/authentication_views.py
 pfx/pfxcore/views/fields.py
 pfx/pfxcore/views/filters_views.py
 pfx/pfxcore/views/locale_views.py
 pfx/pfxcore/views/rest_views.py
-pfx/pfxcore/views/parameters/__init__.py
-pfx/pfxcore/views/parameters/date_format.py
-pfx/pfxcore/views/parameters/groups.py
-pfx/pfxcore/views/parameters/list_count.py
-pfx/pfxcore/views/parameters/list_items.py
-pfx/pfxcore/views/parameters/list_mode.py
-pfx/pfxcore/views/parameters/list_order.py
-pfx/pfxcore/views/parameters/list_search.py
-pfx/pfxcore/views/parameters/media_redirect.py
-pfx/pfxcore/views/parameters/meta_fields.py
-pfx/pfxcore/views/parameters/meta_filters.py
-pfx/pfxcore/views/parameters/meta_orders.py
-pfx/pfxcore/views/parameters/subset.py
-pfx/pfxcore/views/parameters/subset_limit.py
-pfx/pfxcore/views/parameters/subset_offset.py
-pfx/pfxcore/views/parameters/subset_page.py
-pfx/pfxcore/views/parameters/subset_page_size.py
-pfx/pfxcore/views/parameters/subset_page_subset.py
 tests/__init__.py
 tests/models.py
 tests/urls.py
 tests/views.py
 tests/settings/__init__.py
 tests/settings/ci.py
 tests/settings/common.py
 tests/settings/dev.py
 tests/settings/dev_custom_example.py
 tests/settings/dev_default.py
 tests/tests/__init__.py
 tests/tests/basic_api_errors.py
 tests/tests/basic_api_test.py
-tests/tests/test_api_doc.py
 tests/tests/test_auth_api.py
 tests/tests/test_cache.py
 tests/tests/test_fields.py
 tests/tests/test_filters.py
 tests/tests/test_locale_api.py
 tests/tests/test_perm_tests.py
 tests/tests/test_perms_api.py
 tests/tests/test_shortcuts.py
 tests/tests/test_timezone_middleware.py
 tests/tests/test_tools.py
 tests/tests/test_user_queryset.py
-tests/tests/test_view_decorators.py
 tests/tests/test_view_fields.py
```

### Comparing `django-pfx-1.2.dev60/img/pfx.png` & `django-pfx-1.2.dev8/img/pfx.png`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/img/pfx.svg` & `django-pfx-1.2.dev8/img/pfx.svg`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/exceptions.py` & `django-pfx-1.2.dev8/pfx/pfxcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/fields.py` & `django-pfx-1.2.dev8/pfx/pfxcore/fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo` & `django-pfx-1.2.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po` & `django-pfx-1.2.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/middleware/authentication.py` & `django-pfx-1.2.dev8/pfx/pfxcore/middleware/authentication.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,19 @@
         if (has_cache):
             user.cache()
         return user
 
     @classmethod
     def decode_jwt(cls, token):
         try:
+            opts = ({"require": ["exp"]} if settings.PFX_TOKEN_VALIDITY
+                    else {})
             decoded = jwt.decode(
                 token, settings.PFX_SECRET_KEY,
-                options=dict(require=["exp"]),
+                options=opts,
                 algorithms="HS256")
             return cls.get_cached_user(decoded['pfx_user_pk'])
         except get_user_model().DoesNotExist:
             raise
         except DecodeError as e:
             logger.exception(e)
             raise
```

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/middleware/locale.py` & `django-pfx-1.2.dev8/pfx/pfxcore/middleware/locale.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/models/cache_mixins.py` & `django-pfx-1.2.dev8/pfx/pfxcore/models/cache_mixins.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/models/pfx_models.py` & `django-pfx-1.2.dev8/pfx/pfxcore/models/pfx_models.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/shortcuts.py` & `django-pfx-1.2.dev8/pfx/pfxcore/shortcuts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 
 import logging
 from datetime import date
 
+from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
 from django.utils.translation import gettext_lazy as _
 
-from pfx.pfxcore.settings import PFXSettings
-
-settings = PFXSettings()
-
 logger = logging.getLogger(__name__)
 
 
 def f(tmpl, **kwargs):
     return tmpl.format(**kwargs)
 
 
@@ -106,16 +103,9 @@
             key=key))
 
 
 def delete_token_cookie(response):
     response.delete_cookie(
         'token',
         domain=settings.PFX_COOKIE_DOMAIN,
-        samesite=settings.PFX_COOKIE_SAMESITE)
+        samesite=settings.PFX_COOKIE_SAMESITE or 'None')
     return response
-
-
-def register_views(*views):
-    def _register():
-        for v in views:
-            yield from v.as_urlpatterns()
-    return list(_register())
```

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/storage/s3_storage.py` & `django-pfx-1.2.dev8/pfx/pfxcore/storage/s3_storage.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/test.py` & `django-pfx-1.2.dev8/pfx/pfxcore/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,44 +33,34 @@
 
 def get_auth_cookie(response):
     return [
         v for k, v in response.client.cookies.items()
         if k == 'token'][0]
 
 
-def get_url(path, **params):
-    if params:
-        param_string = "&".join([f"{k}={v}" for k, v in params.items()])
-        return f"{path}?{param_string}"
-    return path
-
-
 class APIClient(DjangoClient):
 
     token = None
     default_locale = None
     auth_cookie = None
 
     def __init__(self, enforce_csrf_checks=False, raise_request_exception=True,
                  default_locale=None, with_cookie=False, **defaults):
         super().__init__(enforce_csrf_checks, raise_request_exception,
                          **defaults)
         self.default_locale = default_locale
         self.with_cookie = with_cookie
 
     def login(self, username, password='test',
-              path='/api/auth/login', locale=None, remember_me=False):
+              path='/api/auth/login', locale=None):
         self.token = None
         response = self.post(
-            get_url(path, mode=(self.with_cookie and 'cookie' or 'jwt')),
-            dict(
-                username=username,
-                password=password,
-                remember_me=remember_me),
-            locale=locale)
+            f"{path}{self.with_cookie and '?mode=cookie' or ''}", {
+                'username': username,
+                'password': password}, locale=locale)
         if response.status_code == 200:
             if self.with_cookie:
                 self.auth_cookie = get_auth_cookie(response)
                 regex = r".*token=([\w\._-]*);.*"
                 self.token = re.findall(regex, str(self.auth_cookie))[0]
             else:
                 self.token = response.json_content['token']
@@ -155,103 +145,85 @@
 class TestAssertMixin:
 
     # assert response status code
     def assertRC(self, response, code, msg=None):
         msg = '\n'.join([msg or '', response.formatted()])
         return self.assertEqual(response.status_code, code, msg=msg)
 
-    def format_json(self, src):
-        if isinstance(src, dict):
-            return json.dumps(src, indent=2)
-        return src.formatted()
-
-    def get_json(self, src):
-        return src if isinstance(src, dict) else src.json_content
-
-    def get_val(self, src, key, msg=None):
+    def get_val(self, response, key):
         def _p(k):
             return int(k[1:]) if k[0] == '@' else k
-
         try:
-            return reduce(
-                lambda c, k: c[_p(k)], key.split("."), self.get_json(src))
+            return reduce(lambda c, k: c[_p(k)], key.split("."),
+                          response.json_content)
         except IndexError:
-            assert False, f"'{key}' index not found in:" + msg
+            print(format_response(response, f'Index Error for key "{key}"'))
+            raise Exception(f'Index Error for key "{key}"')
         except KeyError:
-            assert False, f"'{key}' not found in:" + msg
+            print(format_response(response, f'Key Error for key "{key}"'))
+            raise Exception(f'Key Error for key "{key}"')
 
     # assert JSON content at key equals value
-    def assertJE(self, src, key, value, msg=None):
-        msg = '\n'.join([msg or '', self.format_json(src)])
-        return self.assertEqual(self.get_val(
-            src, key, msg=msg), value, msg=msg)
+    def assertJE(self, response, key, value, msg=None):
+        msg = '\n'.join([msg or '', response.formatted()])
+        return self.assertEqual(self.get_val(response, key), value, msg=msg)
 
     # assert JSON content at key not equals value
-    def assertNJE(self, src, key, value, msg=None):
-        msg = '\n'.join([msg or '', self.format_json(src)])
+    def assertNJE(self, response, key, value, msg=None):
+        msg = '\n'.join([msg or '', response.formatted()])
         return self.assertNotEqual(
-            self.get_val(src, key, msg=msg), value, msg=msg)
+            self.get_val(response, key), value, msg=msg)
 
     # assert JSON content at key exists
-    def assertJEExists(self, src, key, msg=None):
-        msg = '\n'.join([msg or '', self.format_json(src)])
+    def assertJEExists(self, response, key, msg=None):
+        msg = '\n'.join([msg or '', response.formatted()])
         if '.' not in key:
-            return self.assertIn(key, self.get_json(src), msg=msg)
+            return self.assertIn(key, response.json_content, msg=msg)
         path, name = key.rsplit('.', 1)
-        return self.assertIn(name, self.get_val(src, path, msg=msg), msg=msg)
+        return self.assertIn(name, self.get_val(response, path), msg=msg)
 
     # assert JSON content at key not exists
-    def assertJENotExists(self, src, key, msg=None):
-        msg = '\n'.join([msg or '', self.format_json(src)])
+    def assertJENotExists(self, response, key, msg=None):
+        msg = '\n'.join([msg or '', response.formatted()])
         if '.' not in key:
-            return self.assertNotIn(key, self.get_json(src), msg=msg)
+            return self.assertNotIn(key, response.json_content, msg=msg)
         path, name = key.rsplit('.', 1)
-        return self.assertNotIn(
-            name, self.get_val(src, path, msg=msg), msg=msg)
+        return self.assertNotIn(name, self.get_val(response, path), msg=msg)
 
     # assert JSON array size
-    def assertSize(self, src, key, size, msg=None):
-        msg = '\n'.join([msg or '', self.format_json(src)])
+    def assertSize(self, response, key, size, msg=None):
+        msg = '\n'.join([msg or '', response.formatted()])
         return self.assertEqual(
-            len(self.get_val(src, key, msg=msg)), size, msg=msg)
+            len(self.get_val(response, key)), size, msg=msg)
 
     # assert JSON array contains
-    def assertJIn(self, src, key, element, msg=None):
-        msg = '\n'.join([msg or '', self.format_json(src)])
+    def assertJIn(self, response, key, element, msg=None):
+        msg = '\n'.join([msg or '', response.formatted()])
         return self.assertIn(
-            element, self.get_val(src, key, msg=msg), msg=msg)
+            element, self.get_val(response, key), msg=msg)
 
 
 class TestPermsAssertMixin(TestAssertMixin):
     USER_TESTS = {}
 
     def assertPerms(self, **methods):
-        ops = ['size']
         for method, result in methods.items():
-            method_split = method.split('__')
-            method = method_split.pop(0)
-            op = (
-                method_split and method_split[-1] in ops and
-                method_split.pop(-1))
-            test = '.'.join(method_split)
+            test = None
+            if '__' in method:
+                method, test = method.split('__')
             with transaction.atomic():
                 sid = transaction.savepoint()
                 with self.subTest(msg=method):
                     response = getattr(self, method)()
                     msg = (
                         hasattr(self, '_logged_user') and
                         f"User {self._logged_user}" or None)
                     if test == 'count':
                         self.assertJE(response, 'meta.count', result, msg)
                         self.assertSize(response, 'items', result, msg)
-                    elif test:
-                        if op == 'size':
-                            self.assertSize(response, test, result, msg)
-                        else:
-                            self.assertJE(response, test, result, msg)
                     else:
                         self.assertRC(response, result, msg)
                 transaction.savepoint_rollback(sid)
 
     def test_all_users(self):
         for user, perms in self.USER_TESTS.items():
             self.client.login(username=user)
```

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/views/__init__.py` & `django-pfx-1.2.dev8/pfx/pfxcore/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/views/authentication_views.py` & `django-pfx-1.2.dev8/pfx/pfxcore/views/authentication_views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from datetime import datetime, timedelta
 
+from django.conf import settings
 from django.contrib.auth import (
     authenticate,
     get_user_model,
     password_validation,
 )
 from django.contrib.auth.tokens import default_token_generator
 from django.core.exceptions import ValidationError
@@ -16,34 +17,29 @@
 from django.utils.http import urlsafe_base64_decode, urlsafe_base64_encode
 from django.utils.translation import gettext_lazy as _
 from django.views.decorators.cache import never_cache
 from django.views.decorators.debug import sensitive_post_parameters
 
 import jwt
 
-from pfx.pfxcore.apidoc import Tag
 from pfx.pfxcore.decorator import rest_api, rest_view
 from pfx.pfxcore.exceptions import AuthenticationError
 from pfx.pfxcore.http import JsonResponse
 from pfx.pfxcore.models import CacheableMixin
-from pfx.pfxcore.settings import PFXSettings
 from pfx.pfxcore.shortcuts import delete_token_cookie
 
 from .rest_views import BaseRestView, BodyMixin, CreateRestViewMixin
 
-settings = PFXSettings()
 logger = logging.getLogger(__name__)
+
 UserModel = get_user_model()
-AUTHENTICATION_TAG = Tag("Authentication")
 
 
 @rest_view("/auth")
 class AuthenticationView(BodyMixin, BaseRestView):
-    tags = [AUTHENTICATION_TAG]
-
     token_generator = default_token_generator
 
     def login_error_response(self):
         raise AuthenticationError()
 
     @method_decorator(sensitive_post_parameters())
     @method_decorator(never_cache)
@@ -52,34 +48,34 @@
         data = self.deserialize_body()
         user = authenticate(self.request, username=data.get('username'),
                             password=data.get('password'))
         if isinstance(user, CacheableMixin):
             user.cache_delete()
         if user is not None:
             mode = self.request.GET.get('mode', 'jwt')
-            remember_me = data.get('remember_me', False)
-            return self._login_success(user, mode, remember_me)
+            return self._login_success(user, mode)
         return self.login_error_response()
 
-    def _login_success(self, user, mode, remember_me=False):
-        token = self._prepare_token(user, remember_me)
+    def _login_success(self, user, mode):
+        token = self._prepare_token(user)
         if mode == 'cookie':
-            if remember_me:
+            if settings.PFX_TOKEN_VALIDITY:
                 expires = datetime.utcnow() + timedelta(
-                    **settings.PFX_TOKEN_LONG_VALIDITY)
+                    **settings.PFX_TOKEN_VALIDITY)
             else:
-                expires = None  # create a session cookie
+                expires = None
 
             res = JsonResponse({
                 'user': self.get_user_information(user)
             })
             res.set_cookie(
-                'token', token, secure=settings.PFX_COOKIE_SECURE,
+                'token', token, secure=settings.PFX_COOKIE_SECURE is None
+                and True or settings.PFX_COOKIE_SECURE,
                 expires=expires, domain=settings.PFX_COOKIE_DOMAIN,
-                httponly=True, samesite=settings.PFX_COOKIE_SAMESITE)
+                httponly=True, samesite=settings.PFX_COOKIE_SAMESITE or 'None')
             return res
         else:
             return JsonResponse({
                 'token': token,
                 'user': self.get_user_information(user)
             })
 
@@ -112,24 +108,21 @@
             errors['old_password'] = [_("Incorrect password")]
         if not data.get('new_password'):
             errors.setdefault('new_password', []).append(
                 _("Empty password is not allowed"))
         return JsonResponse(
             ValidationError(errors), status=422)
 
-    def _prepare_token(self, user, remember_me):
-        if remember_me:
-            exp = datetime.utcnow() + timedelta(
-                **settings.PFX_TOKEN_LONG_VALIDITY)
-        else:
-            exp = datetime.utcnow() + timedelta(
-                **settings.PFX_TOKEN_SHORT_VALIDITY)
-        payload = dict(
-            pfx_user_pk=user.pk,
-            exp=exp)
+    def _prepare_token(self, user):
+        payload = {
+            'pfx_user_pk': user.pk,
+        }
+        if settings.PFX_TOKEN_VALIDITY:
+            exp = datetime.utcnow() + timedelta(**settings.PFX_TOKEN_VALIDITY)
+            payload.update(exp=exp)
         payload.update(self.get_extra_payload(user))
         return jwt.encode(
             payload, settings.PFX_SECRET_KEY, algorithm="HS256")
 
     def get_extra_payload(self, user):
         return {}
 
@@ -138,30 +131,14 @@
             'username': user.get_username(),
             'first_name': user.first_name,
             'last_name': user.last_name,
             'email': user.email}
 
     @method_decorator(sensitive_post_parameters())
     @method_decorator(never_cache)
-    @rest_api("/validate-user-token", public=True, method="post")
-    def validate_user_token(self, *args, **kwargs):
-        data = self.deserialize_body()
-        assert 'uidb64' in data and 'token' in data
-
-        user = self.get_user(data['uidb64'])
-
-        if (user is not None and
-                self.token_generator.check_token(user, data['token'])):
-            return JsonResponse(
-                ValidationError(_('User and token are valid')), status=200)
-        return JsonResponse(
-            ValidationError(_('User or token is invalid')), status=422)
-
-    @method_decorator(sensitive_post_parameters())
-    @method_decorator(never_cache)
     @rest_api("/set-password", public=True, method="post")
     def set_password(self, *args, **kwargs):
         data = self.deserialize_body()
         assert 'uidb64' in data and 'token' in data
 
         user = self.get_user(data['uidb64'])
 
@@ -253,35 +230,33 @@
     token_generator = default_token_generator
     extra_email_context = None
     from_email = None
     html_email_template_name = None
     default_public = True
     model = UserModel
     fields = ['first_name', 'last_name', 'username', 'email']
-    tags = [AUTHENTICATION_TAG]
 
     def validate(self, obj, **kwargs):
         obj.set_unusable_password()
         super().validate(obj, **kwargs)
 
-    def is_valid(self, obj, created=True, **kwargs):
-        r = super().is_valid(obj, created, **kwargs)
+    def is_valid(self, obj, created=True):
+        r = super().is_valid(obj, created)
         self.send_token_message(obj)
         return r
 
 
 @rest_view("/auth")
 class ForgottenPasswordView(SendMessageTokenMixin, BodyMixin, BaseRestView):
     email_template_name = 'registration/password_reset_email.txt'
     subject_template_name = 'registration/password_reset_subject.txt'
     token_generator = default_token_generator
     extra_email_context = None
     from_email = None
     html_email_template_name = None
-    tags = [AUTHENTICATION_TAG]
 
     @method_decorator(sensitive_post_parameters())
     @method_decorator(never_cache)
     @rest_api("/forgotten-password", public=True, method="post")
     def forgotten_password(self, *args, **kwargs):
         data = self.deserialize_body()
         email = data.get('email')
```

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/views/fields.py` & `django-pfx-1.2.dev8/pfx/pfxcore/views/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,14 @@
 
 
 def setifnone(kwargs, k, default):
     if kwargs.get(k) is None:
         kwargs[k] = default
 
 
-class ModelList(list):
-    pass
-
-
 class FieldType:
     CharField = "CharField"
     TextField = "TextField"
     BooleanField = "BooleanField"
     IntegerField = "IntegerField"
     FloatField = "FloatField"
     DateField = "DateField"
@@ -44,15 +40,14 @@
         (models.FloatField, FloatField),
         (models.DateTimeField, DateTimeField),
         (models.DateField, DateField),
         (models.TextField, TextField),
         (models.CharField, CharField),
         (models.ForeignObject, ModelObject),
         (models.ForeignObjectRel, ModelObjectList),
-        (models.ManyToManyField, ModelObjectList),
         (models.JSONField, JsonObject)
     ]
 
     @classmethod
     def register_binding(cls, field_class, field_type):
         cls.MODEL_FIELD_BINDING.insert(0, (field_class, field_type))
 
@@ -204,26 +199,22 @@
         res = super().meta()
         res['required'] = not (
             getattr(self.model_field, 'null', False) or
             getattr(self.model_field, 'blank', False))
         return res
 
     def to_model_value(self, value, get_related_queryset):
-        def _get_obj(v):
-            pk = v['pk'] if isinstance(v, dict) and 'pk' in v else v
-            return pk and get_object(
-                get_related_queryset(self.model_field.related_model),
-                related_field=self.name, pk=pk) or None
-
         field = self.model_field
         if self.field_type == FieldType.ModelObject:
-            value = _get_obj(value)
-        elif self.field_type == FieldType.ModelObjectList:
-            value = ModelList(_get_obj(v) for v in value)
-        elif hasattr(field, 'choices') and field.choices:
+            pk = (value['pk'] if isinstance(value, dict) and 'pk' in value
+                  else value)
+            value = pk and get_object(
+                get_related_queryset(self.model_field.related_model),
+                related_field=self.name, pk=pk) or None
+        if hasattr(field, 'choices') and field.choices:
             value = (value['value']
                      if isinstance(value, dict) and 'value' in value
                      else value)
         elif self.field_type == FieldType.DateField:
             value = (value['value']
                      if isinstance(value, dict) and 'value' in value
                      else value)
```

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/views/filters_views.py` & `django-pfx-1.2.dev8/pfx/pfxcore/views/filters_views.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,26 +27,24 @@
     def query(self, params):
         return Q(*[f.query(params) for f in self.filters])
 
 
 class Filter():
     def __init__(
             self, name, label, type=None, filter_func=None,
-            filter_func_and=False, filter_func_list=False, choices=None,
-            related_model=None, technical=False, defaults=None, ):
+            filter_func_list=False, choices=None,
+            related_model=None, technical=False):
         self.name = name
         self.label = label
         self.type = type
         self.filter_func = filter_func
-        self.filter_func_and = filter_func_and
         self.filter_func_list = filter_func_list
         self.choices = choices
         self.related_model = related_model
         self.technical = technical
-        self.defaults = defaults or []
 
     @property
     def meta(self):
         res = dict(
             label=_(self.label),
             name=self.name,
             type=self.type,
@@ -69,66 +67,49 @@
             return parse_date(value)
         return value
 
     def _call_filter_func(self, values):
         if self.filter_func_list:
             return self.filter_func(values)
         return reduce(
-            lambda x, y: x & y if self.filter_func_and else x | y,
-            [self.filter_func(v) for v in values])
-
-    def _get_values(self, params):
-        values = [self._parse_value(v) for v in params.getlist(self.name)]
-        return values or self.defaults
+            lambda x, y: x | y, [self.filter_func(v) for v in values])
 
     def query(self, params):
-        values = self._get_values(params)
+        values = [self._parse_value(v) for v in params.getlist(self.name)]
         return self._call_filter_func(values) if values else Q()
 
 
 class ModelFilter(Filter):
     def __init__(
-            self, model, name, label=None, type=None,
-            filter_func=None, filter_func_and=False, filter_func_list=False,
-            choices=None, related_model=None, technical=False, defaults=None):
+            self, model, name, label=None, type=None, filter_func=None,
+            filter_func_list=False, choices=None, related_model=None,
+            technical=False):
         self.model = model
         self.field = model._meta.get_field(name)
         super().__init__(
             name, label or self.field.verbose_name,
-            type or self._type_from_model,
-            filter_func, filter_func_and, filter_func_list,
-            choices or self.field.choices,
+            type or FieldType.from_model_field(self.field.__class__),
+            filter_func, filter_func_list, choices or self.field.choices,
             related_model or (
                 self.field.remote_field and
-                self.field.remote_field.model.__name__),
-            technical=technical, defaults=defaults)
-
-    @property
-    def _type_from_model(self):
-        model_type = FieldType.from_model_field(self.field.__class__)
-        if model_type == FieldType.ModelObjectList:
-            # For list related fields (OneToMany, ManyToMany, …) the field
-            # type is ModelObjectList, but the filter type should be
-            # ModelObject.
-            return FieldType.ModelObject
-        return model_type
+                self.field.remote_field.model.__name__), technical=technical)
 
     @property
     def meta(self):
         res = dict(
             is_group=False, label=_(self.label), name=self.name,
             type=self.type, technical=self.technical)
         if self.choices:
             res['choices'] = [
                 dict(label=_(v), value=k) for k, v in self.choices]
         if self.related_model:
             res['related_model'] = self.related_model
         return res
 
     def query(self, params):
-        values = self._get_values(params)
+        values = [self._parse_value(v) for v in params.getlist(self.name)]
         if self.filter_func and values:
             return self._call_filter_func(values)
         elif values:
             return reduce(
                 lambda x, y: x | y, [Q(**{self.name: v}) for v in values])
         return Q()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/views/locale_views.py` & `django-pfx-1.2.dev8/pfx/pfxcore/views/locale_views.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from django.conf import settings
 from django.core.cache import cache
 from django.utils import translation
 
 from babel import Locale
 
-from pfx.pfxcore.apidoc import Tag
 from pfx.pfxcore.decorator import rest_api, rest_view
 from pfx.pfxcore.http import JsonResponse
 
 from .rest_views import BaseRestView
 
-LOCALE_TAG = Tag("Locale")
-
 
 def get_locales():
     return [
         dict(
             pk=code,
             name=Locale.parse(translation.to_locale(code)).get_display_name())
         for code, __ in settings.LANGUAGES]
@@ -25,13 +22,11 @@
     locales = get_locales()
     return {
         'items': locales, 'meta': {'count': len(locales)}}
 
 
 @rest_view("/locales")
 class LocaleRestView(BaseRestView):
-    tags = [LOCALE_TAG]
-
     @rest_api('/languages', public=True)
     def locales(self):
         data = cache.get_or_set('pfx.languages', get_languages_json, 60 * 60)
         return JsonResponse(data)
```

### Comparing `django-pfx-1.2.dev60/pfx/pfxcore/views/rest_views.py` & `django-pfx-1.2.dev8/pfx/pfxcore/views/rest_views.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 import json
 import logging
-import re
 from json import JSONDecodeError
 
 from django.conf import settings
 from django.core.exceptions import FieldDoesNotExist, ValidationError
 from django.db import IntegrityError, transaction
 from django.db.models import ForeignKey, Q
 from django.shortcuts import redirect
-from django.urls import path
 from django.utils.translation import gettext_lazy as _
 from django.views import View
 
-from pfx.pfxcore import __PFX_VIEWS__
-from pfx.pfxcore.apidoc import Tag
 from pfx.pfxcore.decorator import rest_api
 from pfx.pfxcore.exceptions import (
     APIError,
     ForbiddenError,
     JsonErrorAPIError,
     NotFoundError,
     UnauthorizedError,
 )
 from pfx.pfxcore.fields import MediaField
 from pfx.pfxcore.http import JsonResponse
-from pfx.pfxcore.models import JSONReprMixin, UserFilteredQuerySetMixin
+from pfx.pfxcore.models import UserFilteredQuerySetMixin
 from pfx.pfxcore.shortcuts import f, get_bool, get_int, get_object
 from pfx.pfxcore.storage.s3_storage import StorageException
 
-from . import parameters
-from .fields import VF
-from .fields import FieldType as FT
-from .fields import ViewField
+from .fields import VF, ViewField
 
 logger = logging.getLogger(__name__)
 
 
 # HTTP 404 handler
 def resource_not_found(request, exception):
     return NotFoundError().response
@@ -128,47 +121,31 @@
                 obj.delete()
         except IntegrityError as e:
             logger.debug("IntegrityError: %s", e)
             raise APIError(f(_(
                 "{obj} cannot be deleted because "
                 "it is referenced by other objects."), obj=obj))
 
-    @classmethod
-    def get_apidoc_tags(cls):
-        return cls.tags or [
-            Tag(str(cls.model._meta.verbose_name))]
-
 
 class ModelResponseMixin(ModelMixin):
     def serialize_object(self, obj, **fields):
-        if isinstance(obj, JSONReprMixin):
-            vals = obj.json_repr()
-        else:
-            vals = dict(
-                pk=obj.pk,
-                resource_name=str(obj))
+        vals = obj.json_repr()
         vals.update(fields)
         return vals
 
     def response(self, o, **meta):
         return JsonResponse(self.serialize_object(o, **{
             f.alias: f.to_json(o, self.format_date)
             for f in self.get_fields().values()}, meta=meta))
 
     def validate(self, obj, created=False, **kwargs):
         obj.full_clean(**kwargs)
 
-    def is_valid(self, obj, created=False, rel_data=None):
-        if rel_data:
-            with transaction.atomic():
-                obj.save()
-                for k, v in rel_data.items():
-                    getattr(obj, k).set(v)
-        else:
-            obj.save()
+    def is_valid(self, obj, created=False):
+        obj.save()
         message = (
                 created and
                 _("{model} {obj} created.") or
                 _("{model} {obj} updated."))
         object = self.get_object(pk=obj.pk)
         return self.response(
             object, message=f(
@@ -183,23 +160,14 @@
         if get_bool(self.request.GET, 'fields', defaults.get('fields')):
             meta['fields'] = {
                 n: f.meta() for n, f in self.get_fields().items()}
         return meta
 
     @rest_api("/meta", method="get")
     def get_meta(self, *args, **kwargs):
-        """Retrieve the model metadata.
-        ---
-        get:
-            summary: Get {model} metadata
-            responses:
-                200:
-                content:
-                    application/json
-        """
         return JsonResponse(self.object_meta())
 
 
 class BodyMixin:
     def deserialize_body(self):
         try:
             return json.loads(self.request.body)
@@ -217,24 +185,18 @@
             if fields[fname].is_readonly(created=created):
                 logger.warning(
                     "Field %s is ignored because it is readonly on view %s",
                     fname, self.__class__.__name__)
                 return False
             return True
 
-        res = {}
-        res_rel = {}
-        for k, v in data.items():
-            if can_write(k):
-                mk, mv = fields[k].to_model_value(v, self.get_related_queryset)
-                if fields[k].field_type == FT.ModelObjectList:
-                    res_rel[mk] = mv
-                else:
-                    res[mk] = mv
-        return res, res_rel
+        return dict(
+            fields[k].to_model_value(v, self.get_related_queryset)
+            for k, v in data.items()
+            if can_write(k))
 
     def set_values(self, obj, **values):
         for fname, value in values.items():
             setattr(obj, fname, value)
 
 
 class ListRestViewMixin(ModelResponseMixin):
@@ -276,26 +238,16 @@
                 n: f.meta() for n, f in self.get_list_fields().items()}
         if get_bool(self.request.GET, 'filters', default_all):
             meta['filters'] = [f.meta for f in self.filters]
         if get_bool(self.request.GET, 'orders', default_all):
             meta['orders'] = list(self.orderable_fields(self.model))
         return meta
 
-    @rest_api("/meta/list", method="get", parameters=[
-        parameters.groups.MetaList])
+    @rest_api("/meta/list", method="get")
     def get_meta_list(self, *args, **kwargs):
-        """Retrieve the model list metadata.
-        ---
-        get:
-            summary: Get {models} list metadata
-            responses:
-                200:
-                content:
-                    application/json
-        """
         return JsonResponse(self.object_meta_list())
 
     def apply_view_filter(self, qs):
         for filter in self.filters:
             qs = qs.filter(filter.query(self.request.GET))
         return qs
 
@@ -312,15 +264,15 @@
         return qs
 
     def get_list_queryset(self):
         qs = super().get_list_queryset()
         qs = self.apply_view_filter(qs)
         qs = self.apply_view_search(qs)
         qs = self.apply_view_order(qs)
-        return qs.distinct()
+        return qs
 
     def get_list_result(self, qs):
         for o in qs:
             yield self.serialize_object(o, **{
                 f.alias: f.to_json(o, self.format_date)
                 for f in self.get_list_fields().values()})
 
@@ -357,26 +309,16 @@
         qs = qs.all()[offset:offset + limit]
         return qs, dict(
             count=count,
             page_count=page_count,
             limit=limit,
             offset=offset)
 
-    @rest_api("", method="get", parameters=[
-        parameters.groups.List], filters=True)
+    @rest_api("", method="get")
     def get_list(self, *args, **kwargs):
-        """Retrieve a list of model.
-        ---
-        get:
-            summary: Get {models} list
-            responses:
-                200:
-                content:
-                    application/json
-        """
         res = {}
         meta = {}
         qs = self.get_list_queryset()
         subset = self.request.GET.get('subset', self.Subset.NONE)
         if get_bool(self.request.GET, 'count'):
             meta['count'] = qs.count()
         if subset == self.Subset.PAGINATION:
@@ -386,66 +328,30 @@
         elif settings.PFX_MAX_LIST_RESULT_SIZE:
             qs = qs.all()[:settings.PFX_MAX_LIST_RESULT_SIZE]
         else:
             qs = qs.all()
         if meta:
             res['meta'] = meta
         if get_bool(self.request.GET, 'items', 'count' not in meta):
-            if self.request.GET.get('mode', 'list') == 'select':
-                res['items'] = list(self.get_short_list_result(qs))
-            else:
-                res['items'] = list(self.get_list_result(qs))
+            res['items'] = list(self.get_list_result(qs))
         return JsonResponse(res)
 
-    def get_short_list_result(self, qs):
-        for o in qs:
-            if isinstance(o, JSONReprMixin):
-                yield o.json_repr()
-            else:
-                yield dict(
-                    pk=o.pk,
-                    resource_name=str(o))
-
 
 class DetailRestViewMixin(ModelResponseMixin):
-    @rest_api("/<int:id>", method="get", parameters=[
-        parameters.groups.ModelSerialization])
+    @rest_api("/<int:id>", method="get")
     def get(self, id, *args, **kwargs):
-        """Retrieve the model by pk.
-        ---
-        get:
-            summary: Get {model}
-            responses:
-                200:
-                content:
-                    application/json
-            parameters extras:
-                id: the {model} pk
-        """
         obj = self.get_object(pk=id)
         return self.response(obj)
 
 
 class SlugDetailRestViewMixin(ModelResponseMixin):
     SLUG_FIELD = "slug"
 
-    @rest_api("/slug/<slug:slug>", method="get", parameters=[
-        parameters.groups.ModelSerialization])
+    @rest_api("/slug/<slug:slug>", method="get")
     def get_by_slug(self, slug, *args, **kwargs):
-        """Retrieve the model by slug.
-        ---
-        get:
-            summary: Get {model} by slug
-            responses:
-                200:
-                content:
-                    application/json
-            parameters extras:
-                slug: the {model} slug name
-        """
         obj = self.get_object(**{self.SLUG_FIELD: slug})
         return self.response(obj)
 
 
 class CreateRestViewMixin(ModelBodyMixin, ModelResponseMixin):
     default_values = {}
 
@@ -456,77 +362,53 @@
         return self.model(**self.get_default_values())
 
     def object_create_perm(self, data):
         return True
 
     def _post(self, *args, **kwargs):
         obj = self.new_object()
-        data, rel_data = self.get_model_data(
-            obj, self.deserialize_body(), created=True)
+        data = self.get_model_data(obj, self.deserialize_body(), created=True)
         forbidden = False
         if not self.object_create_perm(data):
             forbidden = True
         self.set_values(obj, **data)
         try:
             self.validate(obj, created=True)
             if forbidden:
                 raise ForbiddenError
-            return self.is_valid(obj, created=True, rel_data=rel_data)
+            return self.is_valid(obj, created=True)
         except ValidationError as e:
             return self.is_invalid(obj, errors=e)
 
-    @rest_api("", method="post", parameters=[
-        parameters.groups.ModelSerialization])
+    @rest_api("", method="post")
     def post(self, *args, **kwargs):
-        """Create the model.
-        ---
-        post:
-            summary: Create {model}
-            responses:
-                200:
-                content:
-                    application/json
-        """
         return self._post(*args, **kwargs)
 
 
 class UpdateRestViewMixin(ModelBodyMixin, ModelResponseMixin):
     def object_update_perm(self, obj, data):
         return True
 
     def _put(self, id, *args, **kwargs):
         obj = self.get_object(pk=id)
-        data, rel_data = self.get_model_data(
-            obj, self.deserialize_body(), created=False)
+        data = self.get_model_data(obj, self.deserialize_body(), created=False)
         forbidden = False
         if not self.object_update_perm(obj, data):
             forbidden = True
         self.set_values(obj, **data)
         try:
             self.validate(obj, created=False)
             if forbidden:
                 raise ForbiddenError
-            return self.is_valid(obj, created=False, rel_data=rel_data)
+            return self.is_valid(obj, created=False)
         except ValidationError as e:
             return self.is_invalid(obj, errors=e)
 
-    @rest_api("/<int:id>", method="put", parameters=[
-        parameters.groups.ModelSerialization])
+    @rest_api("/<int:id>", method="put")
     def put(self, id, *args, **kwargs):
-        """Update the model by pk.
-        ---
-        put:
-            summary: Update {model}
-            responses:
-                200:
-                content:
-                    application/json
-            parameters extras:
-                id: the {model} pk
-        """
         return self._put(id, *args, **kwargs)
 
 
 class DeleteRestViewMixin(ModelMixin):
     def object_delete_perm(self, obj):
         return True
 
@@ -536,25 +418,14 @@
             raise ForbiddenError()
         self.delete_object(obj)
         return self.message_response(f(
             _("{model} {obj} deleted."), model=self.model_name, obj=obj))
 
     @rest_api("/<int:id>", method="delete")
     def delete(self, id, *args, **kwargs):
-        """Delete the model by pk.
-        ---
-        delete:
-            summary: Delete {model}
-            responses:
-                200:
-                content:
-                    application/json
-            parameters extras:
-                id: the {model} pk
-        """
         return self._delete(id, *args, **kwargs)
 
 
 class MediaRestViewMixin(ModelMixin):
     def _get_model_field(self, field):
         try:
             model_field = self.model._meta.get_field(field)
@@ -562,62 +433,34 @@
                 raise NotFoundError  # pragma: no cover
         except FieldDoesNotExist:  # pragma: no cover
             raise NotFoundError
         return model_field
 
     @rest_api("/<int:pk>/<str:field>/upload-url/<str:filename>", method="get")
     def field_media_upload_url(self, pk, field, filename, *args, **kwargs):
-        """Get upload URL for a media field.
-        ---
-        get:
-            summary: Get upload URL
-            description: Get upload URL for a file field.
-            responses:
-                200:
-                content:
-                    application/json
-            parameters extras:
-                pk: the {model} pk
-                field: the {model} field name
-                filename: the desired filename
-        """
         obj = self.get_object(pk=pk)
         try:
             res = self._get_model_field(field).get_upload_url(
                 self.request, obj, filename)
         except StorageException as e:  # pragma: no cover
             logger.exception(e)
             raise APIError(_("Unexpected storage error", status=500))
         return JsonResponse(res)
 
-    @rest_api("/<int:pk>/<str:field>", method="get", parameters=[
-        parameters.MediaRedirect])
+    @rest_api("/<int:pk>/<str:field>", method="get")
     def field_media_get(self, pk, field, *args, **kwargs):
-        """Get the URL for a media field file.
-        ---
-        get:
-            summary: Get {model} file
-            description: Get the URL for a media field file.
-            responses:
-                200:
-                content:
-                    application/json
-            parameters extras:
-                pk: the {model} pk
-                field: the {model} field name
-        """
         obj = self.get_object(pk=pk)
         try:
             url = self._get_model_field(field).get_url(self.request, obj)
         except StorageException as e:  # pragma: no cover
             logger.exception(e)
             raise APIError(_("Unexpected storage error", status=500))
-        if get_bool(self.request.GET, 'redirect'):
-            return redirect(url)
-        return JsonResponse(dict(url=url))
+        if self.request.GET.get('redirect', '0').lower() in ['0', 'false']:
+            return JsonResponse(dict(url=url))
+        return redirect(url)
 
 
 class SecuredRestViewMixin(View):
     default_public = False
 
     def perm(self):
         return True
@@ -639,82 +482,15 @@
             raise ForbiddenError()
         fperm = f'{func_name}_perm'
         if hasattr(self, fperm) and not getattr(self, fperm)(*args, **kwargs):
             raise ForbiddenError()
 
 
 class BaseRestView(SecuredRestViewMixin, View):
-    pfx_methods = None
-    rest_view_path = {}
-    rest_doc = {}
-    tags = None
-
-    def dispatch(self, request, *args, **kwargs):
-        # Try to dispatch to the right method; if a method doesn't exist,
-        # defer to the error handler. Also defer to the error handler if the
-        # request method isn't on the approved list.
-        if request.method.lower() in self.http_method_names:
-            handler = getattr(
-                self, self.pfx_methods.get(
-                    request.method.lower(), 'http_method_not_allowed'),
-                self.http_method_not_allowed)
-        else:
-            handler = self.http_method_not_allowed
-        return handler(request, *args, **kwargs)
-
-    @staticmethod
-    def _path_order(path, methods):
-        def process(e):
-            e = re.sub(r'<path:.*>', '!01', e)
-            e = re.sub(r'<int:.*>', '!03', e)
-            e = re.sub(r'<uuid:.*>', '!04', e)
-            e = re.sub(r'<slug:.*>', '!05', e)
-            e = re.sub(r'<str:.*>', '!06', e)
-            e = re.sub(r'<.*>', '!02', e)
-            return e
-
-        return methods.get('priority', 0), *map(
-            process, path.lstrip('/').split('/'))
-
-    @classmethod
-    def get_urls(cls, as_pattern=False):
-        def fullpath(p2):
-            res = f'{cls.rest_view_path[cls]}{p2}'.lstrip('/')
-            return res if as_pattern else f'/{res}'
-
-        paths = {}
-        for name in dir(cls):
-            m = getattr(cls, name, None)
-            if m and callable(m) and hasattr(m, 'rest_api_method'):
-                methods = paths.setdefault(m.rest_api_path, dict(priority=0))
-                methods[m.rest_api_method] = name
-                if m.rest_api_priority != 0:
-                    if methods['priority'] not in (0, m.rest_api_priority):
-                        raise Exception(
-                            f"Path {fullpath(m.rest_api_path)}: "
-                            "you cannot set different priority for same path")
-                    methods['priority'] = m.rest_api_priority
-        return [
-            path(fullpath(p), cls.as_view(pfx_methods=ms)) if as_pattern
-            else dict(path=fullpath(p), methods={
-                k: v for k, v in ms.items() if k != 'priority'})
-            for p, ms in sorted(
-                paths.items(), key=lambda e:
-                    cls._path_order(*e) if as_pattern else e[0],
-                reverse=True)]
-
-    @classmethod
-    def as_urlpatterns(cls):
-        if cls not in __PFX_VIEWS__:
-            __PFX_VIEWS__.append(cls)
-        return cls.get_urls(as_pattern=True)
-
-    @classmethod
-    def get_apidoc_tags(cls):
-        return cls.tags or [Tag(str(cls.__name__))]
+    pass
 
 
 class RestView(
         ListRestViewMixin,
         DetailRestViewMixin,
         CreateRestViewMixin,
         UpdateRestViewMixin,
```

### Comparing `django-pfx-1.2.dev60/setup.cfg` & `django-pfx-1.2.dev8/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 
 [options]
 packages = find_namespace:
 include_package_data = true
 install_requires = 
 	django>=3.2,<4.0
 	django-cors-headers
+	django_request_mapping
 	django_json_widget
 	pyjwt>=2.1
 	Babel
 	boto3
-	apispec
 
 [options.packages.find]
 exclude = 
 	tests*
 	venv*
 	img*
```

### Comparing `django-pfx-1.2.dev60/tests/models.py` & `django-pfx-1.2.dev8/tests/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 from django.utils.functional import cached_property
 
 from pfx.pfxcore.decorator import rest_property
 from pfx.pfxcore.fields import MediaField, MinutesDurationField
 from pfx.pfxcore.models import (
     CacheableMixin,
     CacheDependsMixin,
-    NotNullCharField,
-    NotNullURLField,
     PFXModelMixin,
     UniqueConstraint,
 )
+from pfx.pfxcore.models.not_null_fields import NotNullCharField
 from pfx.pfxcore.models.pfx_models import JSONReprMixin
 from pfx.pfxcore.models.user_filtered_queryset_mixin import (
     UserFilteredQuerySetMixin,
 )
 
 
 class UserManager(BaseUserManager):
@@ -116,18 +115,14 @@
         ('male', "Male"), ('female', "Female")], default='male')
     science_fiction = models.BooleanField("Science Fiction", default=False)
     created_at = models.DateField("Created at", auto_now_add=True)
     create_comment = NotNullCharField(
         "Create comment", max_length=255, blank=True)
     update_comment = NotNullCharField(
         "Update comment", max_length=255, blank=True)
-    website = NotNullURLField("Website", max_length=255, blank=True)
-    types = models.ManyToManyField(
-        'tests.BookType', related_name='authors',
-        verbose_name="Types")
 
     objects = models.QuerySet.as_manager()
     bad_user_objects = BadUserAuthorQuerySet.as_manager()
     user_objects = UserAuthorQuerySet.as_manager()
 
     class Meta:
         verbose_name = "Author"
```

### Comparing `django-pfx-1.2.dev60/tests/settings/common.py` & `django-pfx-1.2.dev8/tests/settings/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 ]
 
 DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
 
 AUTH_USER_MODEL = 'tests.User'
 
 PFX_SECRET_KEY = "fake-secret-key"
+PFX_TOKEN_VALIDITY = None
 PFX_COOKIE_DOMAIN = None
+PFX_COOKIE_SECURE = None  # Default True
+PFX_COOKIE_SAMESITE = None  # Default None
 
 PFX_MAX_LIST_RESULT_SIZE = 0
 
 ROOT_URLCONF = 'tests.urls'
 APPEND_SLASH = False
 
 EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
```

### Comparing `django-pfx-1.2.dev60/tests/settings/dev_custom_example.py` & `django-pfx-1.2.dev8/tests/settings/dev_custom_example.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/tests/tests/__init__.py` & `django-pfx-1.2.dev8/tests/tests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from .basic_api_errors import BasicAPIErrorTest
 from .basic_api_test import BasicAPITest
-from .test_api_doc import ApiDocTest
 from .test_auth_api import AuthAPITest
 from .test_cache import TestCache
 from .test_fields import FieldsTest
 from .test_filters import FiltersTest
 from .test_locale_api import LocaleAPITest
 from .test_perm_tests import PermTestsTest
 from .test_perms_api import PermsAPITest
 from .test_shortcuts import ShortcutTest
 from .test_timezone_middleware import TimezoneMiddlewareTest
 from .test_user_queryset import TestUserQuerySet
-from .test_view_decorators import ViewDecoratorTest
 from .test_view_fields import ViewFieldTest
```

### Comparing `django-pfx-1.2.dev60/tests/tests/basic_api_errors.py` & `django-pfx-1.2.dev8/tests/tests/basic_api_errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from unittest.mock import MagicMock, patch
+from unittest.mock import patch
 
 from django.test import TestCase
 from django.test.utils import override_settings
 
 from pfx.pfxcore.test import APIClient, TestAssertMixin
 from tests.models import User
 
@@ -18,16 +18,16 @@
 
     @override_settings(DEBUG=False)
     def test_resource_not_found(self):
         response = self.client.get('/api/error/404')
         self.assertRC(response, 404)
 
     @override_settings(DEBUG=False)
-    @patch('pfx.pfxcore.decorator.rest.logger', MagicMock())
-    def test_error500(self):
+    @patch('builtins.print')
+    def test_error500(self, mock_print):
         response = self.client.get('/api/error/500')
         self.assertRC(response, 500)
 
     def test_malformed_json(self):
         response = self.client.post(
             '/api/authors', '''{
                 "first_name": "Arthur Charles",
```

### Comparing `django-pfx-1.2.dev60/tests/tests/basic_api_test.py` & `django-pfx-1.2.dev8/tests/tests/basic_api_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,72 +13,65 @@
     def setUp(self):
         self.client = APIClient(default_locale='en')
         with connection.cursor() as cursor:
             cursor.execute("create extension if not exists unaccent;")
 
     @classmethod
     def setUpTestData(cls):
-        cls.type_sf = BookType.objects.create(
-            name="Science fiction", slug="sf")
-        cls.type_fantastique = BookType.objects.create(
-            name="Fantastique", slug="fantastique")
-        cls.type_fantasy = BookType.objects.create(
-            name="Fantastique", slug="fantastique")
-        cls.type_romance = BookType.objects.create(
-            name="Romance", slug="romance")
-
         cls.author1 = Author.objects.create(
             first_name='John Ronald Reuel',
             last_name='Tolkien',
             slug='jrr-tolkien')
         cls.author1_book1 = Book.objects.create(
             author=cls.author1,
             name="The Hobbit",
-            pub_date=date(1937, 1, 1))
+            pub_date=date(1937, 1, 1)
+        )
         cls.author1_book2 = Book.objects.create(
             author=cls.author1,
             name="The Fellowship of the Ring",
-            pub_date=date(1954, 1, 1))
+            pub_date=date(1954, 1, 1)
+        )
         cls.author1_book3 = Book.objects.create(
             author=cls.author1,
             name="The Two Towers",
-            pub_date=date(1954, 1, 1))
+            pub_date=date(1954, 1, 1)
+        )
         cls.author1_book4 = Book.objects.create(
             author=cls.author1,
             name="The Return of the King",
-            pub_date=date(1955, 1, 1))
-
+            pub_date=date(1955, 1, 1)
+        )
         cls.author2 = Author.objects.create(
             first_name='Philip Kindred',
             last_name='Dick',
             science_fiction=True,
             slug='philip-k-dick')
-        cls.author2.types.set([cls.type_sf, cls.type_fantastique])
-
         cls.author3 = Author.objects.create(
             first_name='Isaac',
             last_name='Asimov',
             science_fiction=True,
             slug='isaac-asimov')
-        cls.author3.types.set([cls.type_sf])
         cls.author3_book1 = Book.objects.create(
             author=cls.author3,
             name="The Caves of Steel",
             pub_date=date(1954, 1, 1),
             pages=224,
-            rating=4.6)
+            rating=4.6,
+        )
         cls.author3_book2 = Book.objects.create(
             author=cls.author3,
             name="The Naked Sun",
-            pub_date=date(1957, 1, 1))
+            pub_date=date(1957, 1, 1),
+        )
         cls.author3_book3 = Book.objects.create(
             author=cls.author3,
             name="The Robots of Dawn",
-            pub_date=date(1983, 1, 1))
-
+            pub_date=date(1983, 1, 1),
+        )
         cls.author4 = Author.objects.create(
             first_name='Joanne',
             last_name='Rowling',
             science_fiction=False,
             gender='female',
             slug='j-k-rowling')
 
@@ -152,87 +145,16 @@
         self.assertJE(response, 'items.@0.gender.value', 'male')
         self.assertJE(response, 'items.@0.gender.label', 'Male')
 
     def test_meta_list(self):
         response = self.client.get('/api/authors/meta/list')
         self.assertRC(response, 200)
         self.assertJE(response, 'filters.@0.name', 'book_type')
-        self.assertJE(response, 'filters.@0.items', [
-            {
-                "is_group": False,
-                "label": "Science Fiction",
-                "name": "science_fiction",
-                "technical": True,
-                "type": "BooleanField"
-            },
-            {
-                "label": "Heroic Fantasy",
-                "name": "heroic_fantasy",
-                "technical": False,
-                "type": "BooleanField"
-            },
-            {
-                "is_group": False,
-                "label": "Types",
-                "name": "types",
-                "related_model": "BookType",
-                "technical": False,
-                "type": "ModelObject"
-            }
-        ])
-        self.assertJE(response, 'filters.@1.name', 'custom')
-        self.assertJE(response, 'filters.@1.items', [
-            {
-                "is_group": False,
-                "label": "Last Name",
-                "name": "last_name",
-                "technical": False,
-                "type": "BooleanField"
-            },
-            {
-                "is_group": False,
-                "label": "First Name",
-                "name": "first_name",
-                "technical": False,
-                "type": "CharField"
-            },
-            {
-                "choices": [
-                    {
-                        "label": "Male",
-                        "value": "male"
-                    },
-                    {
-                        "label": "Female",
-                        "value": "female"
-                    }
-                ],
-                "is_group": False,
-                "label": "Gender",
-                "name": "gender",
-                "technical": False,
-                "type": "CharField"
-            },
-            {
-                "choices": [
-                    {
-                        "label": "Tolkien",
-                        "value": "Tolkien"
-                    },
-                    {
-                        "label": "Asimov",
-                        "value": "Asimov"
-                    }
-                ],
-                "label": "Tolkien or Asimov",
-                "name": "last_name_choices",
-                "technical": False,
-                "type": "CharField"
-            }
-        ])
+        self.assertJE(response, 'filters.@0.items.@0.name', 'science_fiction')
+        self.assertJE(response, 'filters.@0.items.@0.technical', True)
 
         response = self.client.get('/api/books/meta/list')
         self.assertRC(response, 200)
         self.assertJIn(response, 'orders', 'pk')
         self.assertJIn(response, 'orders', 'name')
         self.assertJIn(response, 'orders', 'author')
         self.assertJIn(response, 'orders', 'author__pk')
@@ -301,49 +223,14 @@
     def test_model_filter_date(self):
         response = self.client.get(
             '/api/books?pub_date=1954-01-01&items=1&count=1')
 
         self.assertRC(response, 200)
         self.assertJE(response, 'meta.count', 3)
 
-    def test_model_filter_manytomany(self):
-        response = self.client.get(
-            f'/api/authors?types={self.type_romance.pk}&items=1&count=1')
-        self.assertRC(response, 200)
-        self.assertJE(response, 'meta.count', 0)
-
-        response = self.client.get(
-            f'/api/authors?types={self.type_fantastique.pk}&items=1&count=1')
-        self.assertRC(response, 200)
-        self.assertJE(response, 'meta.count', 1)
-        self.assertJE(response, 'items.@0.pk', self.author2.pk)
-
-        response = self.client.get(
-            f'/api/authors?types={self.type_sf.pk}&items=1&count=1')
-        self.assertRC(response, 200)
-        self.assertJE(response, 'meta.count', 2)
-        self.assertJE(response, 'items.@0.pk', self.author2.pk)
-        self.assertJE(response, 'items.@1.pk', self.author3.pk)
-
-        # Check multiple values filtered with OR condition.
-        response = self.client.get(
-            f'/api/authors?types={self.type_fantastique.pk}'
-            f'&types={self.type_romance.pk}&items=1&count=1')
-        self.assertRC(response, 200)
-        self.assertJE(response, 'meta.count', 1)
-        self.assertJE(response, 'items.@0.pk', self.author2.pk)
-
-        response = self.client.get(
-            f'/api/authors?types={self.type_fantastique.pk}'
-            f'&types={self.type_sf.pk}&items=1&count=1')
-        self.assertRC(response, 200)
-        self.assertJE(response, 'meta.count', 2)
-        self.assertJE(response, 'items.@0.pk', self.author2.pk)
-        self.assertJE(response, 'items.@1.pk', self.author3.pk)
-
     def test_model_filter_decimal(self):
         # TODO: Wait Decimal implementation
         pass
 
     def test_model_filter_foreign_key(self):
         response = self.client.get(
             f'/api/books?author={self.author3.pk}&items=1&count=1')
@@ -429,49 +316,27 @@
             '/api/authors?subset=offset&offset=3&limit=5')
         self.assertRC(response, 200)
         # With offset 3 the first item must be the same as the 4th
         # in the request with offest 0.
         self.assertJE(response, 'items.@0.pk', item4_pk)
         self.assertJE(response, 'meta.subset.count', 14)
 
-    def test_select_list(self):
-        response = self.client.get(
-            '/api/authors?mode=select&items=true&limit=10')
-        self.assertRC(response, 200)
-        self.assertSize(response, 'items', 4)
-
-    def test_select_list_search(self):
-        response = self.client.get(
-            '/api/authors?mode=select&subset=offset&limit=10&search=Isaac')
-        self.assertRC(response, 200)
-        self.assertJE(response, 'meta.subset.count', 1)
-        self.assertJE(response, 'items.@0.resource_name', "Isaac Asimov")
-
-    def test_select_list_max(self):
-        response = self.client.get(
-            '/api/authors?mode=select&subset=offset&items=true&limit=3')
-        self.assertRC(response, 200)
-        self.assertJE(response, 'meta.subset.count', 4)
-        self.assertSize(response, 'items', 3)
-
     def test_meta_service(self):
         response = self.client.get('/api/authors/meta')
         self.assertRC(response, 200)
         self.assertJE(response, 'fields.first_name.type', 'CharField')
         self.assertJE(response, 'fields.first_name.name', 'First Name')
         self.assertJE(response, 'fields.last_name.type', 'CharField')
         self.assertJE(response, 'fields.last_name.name', 'Last Name')
         self.assertJE(response, 'fields.books.type', 'ModelObjectList')
         self.assertJE(response, 'fields.books.name', 'Books')
         self.assertJE(response, 'fields.created_at.type', 'DateField')
         self.assertJE(response, 'fields.created_at.name', 'Created at')
         self.assertJE(response, 'fields.name_length.type', 'IntegerField')
         self.assertJE(response, 'fields.name_length.name', 'Name Length')
-        self.assertJE(response, 'fields.types.type', 'ModelObjectList')
-        self.assertJE(response, 'fields.types.name', 'Types')
         response = self.client.get('/api/books/meta')
         self.assertJE(
             response, 'fields.read_time.type', 'MinutesDurationField')
         self.assertJE(response, 'fields.read_time.name', 'Read Time')
 
     def test_get_detail_by_id(self):
         response = self.client.get(f'/api/authors/{self.author1.pk}')
@@ -523,62 +388,40 @@
         self.assertRC(response, 200)
         self.assertJE(response, 'author.pk', self.author3.pk)
         self.assertJE(response, 'author.resource_name', "Isaac Asimov")
         self.assertJE(response, 'author.resource_slug', "isaac-asimov")
         self.assertJE(response, 'author.hello', "World")
         self.assertJE(response, 'author.last_name', "Asimov")
 
-    def test_get_detail_manytomany(self):
-        response = self.client.get(f'/api/authors/{self.author1.pk}')
-        self.assertRC(response, 200)
-        self.assertSize(response, 'types', 0)
-
-        response = self.client.get(f'/api/authors/{self.author2.pk}')
-        self.assertRC(response, 200)
-        self.assertSize(response, 'types', 2)
-        self.assertJE(response, 'types.@0.pk', self.type_sf.pk)
-        self.assertJE(response, 'types.@1.pk', self.type_fantastique.pk)
-
-        response = self.client.get(f'/api/authors/{self.author3.pk}')
-        self.assertRC(response, 200)
-        self.assertSize(response, 'types', 1)
-        self.assertJE(response, 'types.@0.pk', self.type_sf.pk)
-
     def test_get_non_existant_record(self):
         response = self.client.get('/api/authors/999999')
         self.assertRC(response, 404)
 
     def test_get_non_existant_record_by_slug(self):
         response = self.client.get('/api/authors/slug/not-existent')
         self.assertRC(response, 404)
 
     def test_create(self):
         response = self.client.post(
-            '/api/authors', dict(
-                first_name='Arthur Charles',
-                last_name='Clarke',
-                name_length=1,
-                gender='male',
-                create_comment='CREATE COMMENT',
-                update_comment='UPDATE COMMENT',
-                website=None,
-                slug='arthur-c-clarke',
-                types=[self.type_sf.pk, dict(pk=self.type_fantastique.pk)]))
+            '/api/authors', {
+                'first_name': 'Arthur Charles',
+                'last_name': 'Clarke',
+                'name_length': 1,
+                'gender': 'male',
+                'create_comment': 'CREATE COMMENT',
+                'update_comment': 'UPDATE COMMENT',
+                'slug': 'arthur-c-clarke'})
 
         self.assertRC(response, 200)
         self.assertJE(response, 'first_name', 'Arthur Charles')
         self.assertJE(response, 'last_name', 'Clarke')
         self.assertJE(response, 'gender.value', 'male')
         self.assertJE(response, 'gender.label', 'Male')
         self.assertJE(response, 'create_comment', 'CREATE COMMENT')
         self.assertNJE(response, 'update_comment', 'UPDATE COMMENT')
-        self.assertJE(response, 'website', '')
-        self.assertSize(response, 'types', 2)
-        self.assertJE(response, 'types.@0.pk', self.type_sf.pk)
-        self.assertJE(response, 'types.@1.pk', self.type_fantastique.pk)
 
     def test_create_null_values(self):
         response = self.client.post(
             '/api/books', dict(
                 name="Test Book",
                 author=self.author1.pk,
                 type=None,
@@ -654,31 +497,14 @@
 
         response = self.client.put(
             f'/api/authors/{self.author1.pk}', {'gender': {'value': 'male'}})
         self.assertRC(response, 200)
         self.author1.refresh_from_db()
         self.assertEqual(self.author1.gender, 'male')
 
-    def test_update_manytomny(self):
-        self.assertEqual(self.author1.types.count(), 0)
-
-        response = self.client.put(
-            f'/api/authors/{self.author1.pk}', dict(
-                types=[self.type_fantasy.pk]))
-        self.assertRC(response, 200)
-        self.author1.refresh_from_db()
-        self.assertEqual(self.author1.types.count(), 1)
-        self.assertEqual(self.author1.types.all()[0].pk, self.type_fantasy.pk)
-
-        response = self.client.put(
-            f'/api/authors/{self.author1.pk}', dict(types=[]))
-        self.assertRC(response, 200)
-        self.author1.refresh_from_db()
-        self.assertEqual(self.author1.types.count(), 0)
-
     def test_update_enum_bad_value(self):
         response = self.client.put(
             f'/api/authors/{self.author1.pk}', {
                 'gender': {'value': 'writer'}})
 
         self.assertRC(response, 422)
         self.assertJE(
@@ -953,15 +779,15 @@
         response = self.client.get(
             f'/api/books/{self.author1_book1.pk}/cover?redirect=false')
         self.assertRC(response, 200)
         self.assertJE(
             response, 'url', "http://dragonfly.fake/Book/1/cover.png")
 
         response = self.client.get(
-            f'/api/books/{self.author1_book1.pk}/cover?redirect=true')
+            f'/api/books/{self.author1_book1.pk}/cover?redirect')
         self.assertRedirects(
             response, "http://dragonfly.fake/Book/1/cover.png",
             fetch_redirect_response=False)
 
         with patch.object(
                 MockBoto3Client, 'delete_object',
                 return_value=None) as mock_delete:
```

### Comparing `django-pfx-1.2.dev60/tests/tests/test_auth_api.py` & `django-pfx-1.2.dev8/tests/tests/test_auth_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from django.contrib.auth.tokens import default_token_generator
 from django.core import mail
 from django.test import TransactionTestCase, modify_settings, override_settings
 from django.utils.encoding import force_bytes
 from django.utils.http import urlsafe_base64_encode
 
 import jwt
-from freezegun import freeze_time
 
 from pfx.pfxcore.test import APIClient, TestAssertMixin, get_auth_cookie
 from tests.models import User
 
 logger = logging.getLogger(__name__)
 
 
@@ -40,119 +39,43 @@
         self.assertRC(response, 401)
 
     def test_emtpy_login(self):
         response = self.client.post(
             '/api/auth/login', {})
         self.assertRC(response, 401)
 
-    @override_settings(PFX_TOKEN_SHORT_VALIDITY={'minutes': 30})
     def test_valid_login(self):
         response = self.client.post(
             '/api/auth/login', {
                 'username': 'jrr.tolkien',
                 'password': 'RIGHT PASSWORD'})
 
         self.assertRC(response, 200)
         decoded = jwt.decode(
             response.json_content['token'], settings.PFX_SECRET_KEY,
             algorithms="HS256")
         self.assertEqual(decoded['pfx_user_pk'], self.user1.pk)
-        self.assertTrue(
-            datetime.utcnow() + timedelta(minutes=25) <
-            datetime.utcfromtimestamp(decoded['exp'])
-            < datetime.utcnow() + timedelta(minutes=35))
-
-    @override_settings(PFX_TOKEN_LONG_VALIDITY={'minutes': 60})
-    def test_valid_login_remember_me(self):
-        response = self.client.post(
-            '/api/auth/login', {
-                'username': 'jrr.tolkien',
-                'password': 'RIGHT PASSWORD',
-                'remember_me': True})
-
-        self.assertRC(response, 200)
-        decoded = jwt.decode(
-            response.json_content['token'], settings.PFX_SECRET_KEY,
-            algorithms="HS256")
-        self.assertEqual(decoded['pfx_user_pk'], self.user1.pk)
-        self.assertTrue(
-            datetime.utcnow() + timedelta(minutes=55) <
-            datetime.utcfromtimestamp(decoded['exp'])
-            < datetime.utcnow() + timedelta(minutes=65))
 
-    @override_settings(PFX_TOKEN_SHORT_VALIDITY={'minutes': 30})
     def test_valid_login_with_cookie(self):
         response = self.client.post(
             '/api/auth/login?mode=cookie', {
                 'username': 'jrr.tolkien',
                 'password': 'RIGHT PASSWORD'})
 
-        cookie = get_auth_cookie(response)
-        regex = r".*token=([\w\._-]*);.*"
-        token = re.findall(regex, str(cookie))[0]
-
-        # The cookie should be a session cookie
-        # (removed when browser is closed)
-        regex = r".*expires=([^;]*);.*"
-        expires = re.findall(regex, str(cookie))
-        regex = r".*Max-Age=([^;]*);.*"
-        max_age = re.findall(regex, str(cookie))
-        self.assertEqual(len(expires), 0)
-        self.assertEqual(len(max_age), 0)
-
-        self.assertRC(response, 200)
-        decoded = jwt.decode(
-            token, settings.PFX_SECRET_KEY,
-            algorithms="HS256")
-        self.assertEqual(decoded['pfx_user_pk'], self.user1.pk)
-
-        # token expires in 30 minutes +/- 5 minutes.
-        self.assertTrue(
-            datetime.utcnow() + timedelta(minutes=25) <
-            datetime.utcfromtimestamp(decoded['exp'])
-            < datetime.utcnow() + timedelta(minutes=35))
-
-    @override_settings(PFX_TOKEN_LONG_VALIDITY={'minutes': 60})
-    def test_valid_login_with_cookie_remember_me(self):
-        response = self.client.post(
-            '/api/auth/login?mode=cookie', {
-                'username': 'jrr.tolkien',
-                'password': 'RIGHT PASSWORD',
-                'remember_me': 'true'})
-
-        cookie = get_auth_cookie(response)
-
+        cookie = [v for k, v in response.client.cookies.items()
+                  if k == 'token'][0]
         regex = r".*token=([\w\._-]*);.*"
         token = re.findall(regex, str(cookie))[0]
 
-        regex = r".*expires=([^;]*);.*"
-        expires = re.findall(regex, str(cookie))[0]
-        d = datetime.strptime(expires, '%a, %d %b %Y %H:%M:%S %Z')
-
-        regex = r".*Max-Age=([^;]*);.*"
-        max_age = re.findall(regex, str(cookie))[0]
-
-        # cookie expires in 60 minutes +/- 5 minutes.
-        self.assertTrue(
-            datetime.utcnow() + timedelta(minutes=55) <
-            d < datetime.utcnow() + timedelta(minutes=65))
-        self.assertEqual(int(max_age), 3600)
-
         self.assertRC(response, 200)
         decoded = jwt.decode(
             token, settings.PFX_SECRET_KEY,
             algorithms="HS256")
         self.assertEqual(decoded['pfx_user_pk'], self.user1.pk)
 
-        # token expires in 60 minutes +/- 5 minutes.
-        self.assertTrue(
-            datetime.utcnow() + timedelta(minutes=55) <
-            datetime.utcfromtimestamp(decoded['exp'])
-            < datetime.utcnow() + timedelta(minutes=65))
-
     def test_logout(self):
         self.client.login(
             username='jrr.tolkien',
             password='RIGHT PASSWORD')
         response = self.client.get('/api/auth/logout')
         self.assertRC(response, 200)
         cookie = [v for k, v in response.client.cookies.items()
@@ -280,17 +203,48 @@
             '/api/auth/change-password', {
                 'old_password': 'RIGHT PASSWORD',
                 'new_password': None})
         self.assertRC(response, 422)
         self.assertJE(
             response, "new_password.@0", "Empty password is not allowed")
 
+    @override_settings(PFX_TOKEN_VALIDITY={'minutes': 30})
+    def test_valid_token_with_expiration(self):
+        self.client.login(
+            username='jrr.tolkien',
+            password='RIGHT PASSWORD')
+        response = self.client.get(
+            '/api/private/authors')
+        self.assertRC(response, 200)
+
+    @override_settings(PFX_TOKEN_VALIDITY={'minutes': 30})
+    def test_valid_cookie_token_with_expiration(self):
+        self.cookie_client.login(
+            username='jrr.tolkien',
+            password='RIGHT PASSWORD')
+
+        regex = r".*expires=([^;]*);.*"
+        expires = re.findall(regex, str(self.cookie_client.auth_cookie))[0]
+        d = datetime.strptime(expires, '%a, %d %b %Y %H:%M:%S %Z')
+
+        regex = r".*Max-Age=([^;]*);.*"
+        max_age = re.findall(regex, str(self.cookie_client.auth_cookie))[0]
+
+        # cookie expires in 30 minutes +/- 5 minutes.
+        self.assertTrue(
+            datetime.utcnow() + timedelta(minutes=25) <
+            d < datetime.utcnow() + timedelta(minutes=35))
+        self.assertEqual(int(max_age), 1800)
+
+        response = self.cookie_client.get(
+            '/api/private/authors')
+        self.assertRC(response, 200)
+
     @override_settings(
-        PFX_TOKEN_SHORT_VALIDITY={'minutes': 30},
-        PFX_COOKIE_DOMAIN='example.com')
+        PFX_TOKEN_VALIDITY={'minutes': 30}, PFX_COOKIE_DOMAIN='example.com')
     def test_valid_cookie_token_with_domain(self):
         self.cookie_client.login(
             username='jrr.tolkien',
             password='RIGHT PASSWORD')
 
         regex = r".*Domain=([^;]*);.*"
         domain = re.findall(regex, str(self.cookie_client.auth_cookie))[0]
@@ -305,16 +259,15 @@
         self.assertEqual(samesite, "None")  # default value
 
         response = self.cookie_client.get(
             '/api/private/authors')
         self.assertRC(response, 200)
 
     @override_settings(
-        PFX_COOKIE_DOMAIN='example.com',
-        PFX_COOKIE_SECURE=False,
+        PFX_COOKIE_DOMAIN='example.com', PFX_COOKIE_SECURE=False,
         PFX_COOKIE_SAMESITE='Lax')
     def test_valid_cookie_token_with_domain_same_site_insecure(self):
         self.cookie_client.login(
             username='jrr.tolkien',
             password='RIGHT PASSWORD')
 
         regex = r".*Domain=([^;]*);.*"
@@ -329,41 +282,49 @@
         samesite = re.findall(regex, str(self.cookie_client.auth_cookie))[0]
         self.assertEqual(samesite, "Lax")
 
         response = self.cookie_client.get(
             '/api/private/authors')
         self.assertRC(response, 200)
 
-    @override_settings(PFX_TOKEN_SHORT_VALIDITY={'hours': 4})
+    @override_settings(PFX_TOKEN_VALIDITY={'minutes': -30})
     def test_expired_token(self):
-        with freeze_time("2023-05-01 08:00:00"):
-            self.client.login(
-                username='jrr.tolkien',
-                password='RIGHT PASSWORD')
-        with freeze_time("2023-05-01 12:01:00"):
-            response = self.client.get(
-                '/api/private/authors')
-            self.assertRC(response, 401)
-
-    @override_settings(PFX_TOKEN_LONG_VALIDITY={'days': 2})
-    def test_expired_cookie_with_expired_token(self):
-
-        with freeze_time("2023-05-01 08:00:00"):
-            self.cookie_client.login(
-                username='jrr.tolkien',
-                password='RIGHT PASSWORD',
-                remember_me=True)
-        with freeze_time("2023-05-04 08:00:00"):
-            response = self.cookie_client.get(
-                '/api/private/authors')
-            self.assertRC(response, 401)
-            self.assertEqual(
-                str(get_auth_cookie(response)),
-                'Set-Cookie: token=""; expires=Thu, 01 Jan 1970 00:00:00 GMT; '
-                'Max-Age=0; Path=/; SameSite=None; Secure')
+        self.client.login(
+            username='jrr.tolkien',
+            password='RIGHT PASSWORD')
+
+        response = self.client.get(
+            '/api/private/authors')
+        self.assertRC(response, 401)
+
+    @override_settings(PFX_TOKEN_VALIDITY={'minutes': -30})
+    def test_expired_cookie_token(self):
+        self.cookie_client.login(
+            username='jrr.tolkien',
+            password='RIGHT PASSWORD')
+
+        regex = r".*expires=([^;]*);.*"
+        expires = re.findall(regex, str(self.cookie_client.auth_cookie))[0]
+        d = datetime.strptime(expires, '%a, %d %b %Y %H:%M:%S %Z')
+
+        regex = r".*Max-Age=([^;]*);.*"
+        max_age = re.findall(regex, str(self.cookie_client.auth_cookie))[0]
+
+        # cookie expires now +/- 5 minutes.
+        self.assertTrue(
+            datetime.utcnow() - timedelta(minutes=5) <
+            d < datetime.utcnow() + timedelta(minutes=5))
+        self.assertEqual(int(max_age), 0)
+        response = self.cookie_client.get(
+            '/api/private/authors')
+        self.assertRC(response, 401)
+        self.assertEqual(
+            str(get_auth_cookie(response)),
+            'Set-Cookie: token=""; expires=Thu, 01 Jan 1970 00:00:00 GMT; '
+            'Max-Age=0; Path=/; SameSite=None; Secure')
 
     def test_invalid_auth_header(self):
         logging.disable(logging.CRITICAL)
         response = self.client.get(
             '/api/private/authors',
             HTTP_AUTHORIZATION='Beer here',
             content_type='application/json')
@@ -602,36 +563,14 @@
         response = self.client.post(
             '/api/auth/forgotten-password', {
                 'email': '@bluestar.solutions',
             })
         self.assertRC(response, 422)
         self.assertJE(response, 'email.@0', 'Enter a valid email address.')
 
-    def test_validate_user_token(self):
-        # Try with a wrong token and uid
-        response = self.client.post(
-            '/api/auth/validate-user-token', {
-                'token': 'WRONG TOKEN',
-                'uidb64': 'WRONG UID'
-            })
-
-        self.assertRC(response, 422)
-        self.assertJE(response, '__all__.@0', "User or token is invalid")
-
-        # Then try with a valid token and uid
-        token = default_token_generator.make_token(self.user1)
-        uid = urlsafe_base64_encode(force_bytes(self.user1.pk))
-        response = self.client.post(
-            '/api/auth/validate-user-token', {
-                'token': token,
-                'uidb64': uid
-            })
-        self.assertRC(response, 200)
-        self.assertJE(response, '__all__.@0', "User and token are valid")
-
     def test_set_password(self):
         # Try with a wrong token and uid
         response = self.client.post(
             '/api/auth/set-password', {
                 'token': 'WRONG TOKEN',
                 'uidb64': 'WRONG UID',
                 'password': 'NEW PASSWORD',
```

### Comparing `django-pfx-1.2.dev60/tests/tests/test_cache.py` & `django-pfx-1.2.dev8/tests/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/tests/tests/test_fields.py` & `django-pfx-1.2.dev8/tests/tests/test_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from datetime import date, timedelta
-from unittest.mock import MagicMock, patch
 
 from django.core.exceptions import ValidationError
 from django.db import connection
 from django.test import TestCase
 
 from pfx.pfxcore.fields import MinutesDurationField
 from pfx.pfxcore.test import APIClient, TestAssertMixin
@@ -25,15 +24,14 @@
             slug='jrr-tolkien')
         cls.book = Book.objects.create(
             author=cls.author,
             name="The Hobbit",
             pub_date=date(1937, 1, 1)
         )
 
-    @patch('pfx.pfxcore.fields.logger', MagicMock())
     def test_to_python(self):
         d = MinutesDurationField()
         self.assertIsNone(d.to_python(None))
         self.assertIsNone(d.to_python(''))
         self.assertEqual(d.to_python(0), timedelta(0))
         self.assertEqual(d.to_python('0'), timedelta(0))
         self.assertEqual(
```

### Comparing `django-pfx-1.2.dev60/tests/tests/test_filters.py` & `django-pfx-1.2.dev8/tests/tests/test_filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,37 +15,20 @@
 
 class FiltersTest(TestAssertMixin, TestCase):
     def test_filter_func(self):
         filter = Filter('test', "Test", filter_func=lambda v: Q(test=v))
         q = filter.query(MockParams(test=["A test value"]))
         self.assertEqual(str(q), "(AND: ('test', 'A test value'))")
 
-    def test_filter_func_defaults(self):
-        filter = Filter(
-            'test', "Test", filter_func=lambda v: Q(test=v),
-            defaults=["A default value"])
-        q = filter.query(MockParams(test=[]))
-        self.assertEqual(str(q), "(AND: ('test', 'A default value'))")
-        q = filter.query(MockParams(test=["A test value"]))
-        self.assertEqual(str(q), "(AND: ('test', 'A test value'))")
-
     def test_filter_func_multi(self):
         filter = Filter('test', "Test", filter_func=lambda v: Q(test=v))
         q = filter.query(MockParams(test=["A test value", "another"]))
         self.assertEqual(
             str(q), "(OR: ('test', 'A test value'), ('test', 'another'))")
 
-    def test_filter_func_multi_and(self):
-        filter = Filter(
-            'test', "Test", filter_func=lambda v: Q(test=v),
-            filter_func_and=True)
-        q = filter.query(MockParams(test=["A test value", "another"]))
-        self.assertEqual(
-            str(q), "(AND: ('test', 'A test value'), ('test', 'another'))")
-
     def test_filter_func_multi_list(self):
         filter = Filter(
             'test', "Test", filter_func=lambda v: Q(test=v),
             filter_func_list=True)
         q = filter.query(MockParams(test=["A test value", "another"]))
         self.assertEqual(
             str(q), "(AND: ('test', ['A test value', 'another']))")
```

### Comparing `django-pfx-1.2.dev60/tests/tests/test_locale_api.py` & `django-pfx-1.2.dev8/tests/tests/test_locale_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/tests/tests/test_perm_tests.py` & `django-pfx-1.2.dev8/tests/tests/test_perm_tests.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/tests/tests/test_perms_api.py` & `django-pfx-1.2.dev8/tests/tests/test_perms_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/tests/tests/test_shortcuts.py` & `django-pfx-1.2.dev8/tests/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/tests/tests/test_timezone_middleware.py` & `django-pfx-1.2.dev8/tests/tests/test_timezone_middleware.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/tests/tests/test_tools.py` & `django-pfx-1.2.dev8/tests/tests/test_tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import date
 from unittest.mock import patch
 
 import django
 from django.test import TestCase
 
-from pfx.pfxcore.test import APIClient, TestAssertMixin, get_url
+from pfx.pfxcore.test import APIClient, TestAssertMixin
 from tests.models import Author
 
 
 class TestTools(TestAssertMixin, TestCase):
 
     def setUp(self):
         self.client = APIClient(default_locale='en')
@@ -77,18 +77,7 @@
         self.assertIn('"last_name": "Tolkien",', printed)
         self.assertIn('"name_length": 25,', printed)
         self.assertIn(f'"pk": {self.author1.pk},', printed)
         self.assertIn('"resource_name": "John Ronald Reuel Tolkien",', printed)
         self.assertIn('"slug": "jrr-tolkien",', printed)
         self.assertIn('"update_comment": ""', printed)
         self.assertIn('"meta": {},', printed)
-
-    def test_get_url(self):
-        self.assertEqual(
-            get_url('/test/thing'),
-            '/test/thing')
-        self.assertEqual(
-            get_url('/test/thing', mode="test"),
-            '/test/thing?mode=test')
-        self.assertEqual(
-            get_url('/test/thing', mode="qwertz", uid=12345, other="string"),
-            '/test/thing?mode=qwertz&uid=12345&other=string')
```

### Comparing `django-pfx-1.2.dev60/tests/tests/test_user_queryset.py` & `django-pfx-1.2.dev8/tests/tests/test_user_queryset.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/tests/tests/test_view_fields.py` & `django-pfx-1.2.dev8/tests/tests/test_view_fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev60/tests/views.py` & `django-pfx-1.2.dev8/tests/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 from django.core.exceptions import ImproperlyConfigured
 from django.db.models import Count, Q
 from django.utils.translation import gettext as _
 
-from pfx.pfxcore.decorator import rest_api, rest_doc, rest_view
+from pfx.pfxcore.decorator import rest_api, rest_view
 from pfx.pfxcore.http import JsonResponse
 from pfx.pfxcore.views import (
     VF,
     BaseRestView,
     FieldType,
     Filter,
     FilterGroup,
@@ -22,18 +22,18 @@
 
 logger = logging.getLogger(__name__)
 
 
 class AuthorRestViewMixin():
     model = Author
     fields = [
-        'first_name', 'last_name', 'name_length', 'slug', 'gender', 'types',
+        'first_name', 'last_name', 'name_length', 'slug', 'gender',
         VF('books', readonly=True), VF('created_at', readonly=True),
         VF('create_comment', readonly_update=True),
-        VF('update_comment', readonly_create=True), 'website']
+        VF('update_comment', readonly_create=True)]
     list_fields = ['first_name', 'last_name', 'gender']
 
 
 def heroic_fantasy_filter(value):
     q = Q(last_name="Tolkien")
     return value and q or ~q
 
@@ -59,15 +59,14 @@
     default_public = True
     filters = [
         FilterGroup('book_type', _("Book Type"), [
             ModelFilter(Author, 'science_fiction', technical=True),
             Filter(
                 'heroic_fantasy', _("Heroic Fantasy"),
                 FieldType.BooleanField, heroic_fantasy_filter),
-            ModelFilter(Author, 'types')
         ]),
         FilterGroup('custom', _("Custom"), [
             ModelFilter(
                 Author, 'last_name', type=FieldType.BooleanField,
                 filter_func=last_name_filter),
             ModelFilter(Author, 'first_name'),
             ModelFilter(Author, 'gender'),
@@ -88,48 +87,15 @@
         book = Author.cache_get(id)
         if book:
             return self.response(book, from_cache=True)
         book = self.get_object(pk=id)
         book.cache()
         return self.response(book, from_cache=False)
 
-    @rest_api("/priority/default", method="get")
-    def priority_default(self, *args, **kwargs):
-        return JsonResponse(dict(value='static:default'))
 
-    @rest_api("/priority/<value>", method="get")
-    def priority_param(self, value, *args, **kwargs):
-        return JsonResponse(dict(value=f"untyped:{value}"))
-
-    @rest_api("/priority/<int:value>", method="get")
-    def priority_int(self, value, *args, **kwargs):
-        return JsonResponse(dict(value=f"int:{value}"))
-
-    @rest_api("/priority/<str:value>", method="get")
-    def priority_str(self, value, *args, **kwargs):
-        return JsonResponse(dict(value=f"str:{value}"))
-
-    @rest_api("/priority/<path:value>", method="get")
-    def priority_path(self, value, *args, **kwargs):
-        return JsonResponse(dict(value=f"path:{value}"))
-
-    @rest_api("/priority/default/path", method="get")
-    def priority_default_path(self, *args, **kwargs):
-        return JsonResponse(dict(value="static:default_path"))
-
-    @rest_api("/priority/priority-less", method="get", priority=-1)
-    def priority_test2(self, *args, **kwargs):
-        return JsonResponse(dict(value='static:less'))
-
-    @rest_api("/priority/priority-more", method="get", priority=1)
-    def priority_test3(self, *args, **kwargs):
-        return JsonResponse(dict(value='static:more'))
-
-
-@rest_doc('/<int:id>', 'get', summary="Get custom author")
 @rest_view("/authors-annotate")
 class AuthorAnnotateRestView(AuthorRestView):
     fields = [
         'first_name', 'last_name', 'slug',
         'books_count', 'books_count_annotate', 'books_count_prop']
     list_fields = [
         'first_name', 'last_name', 'slug',
@@ -250,20 +216,7 @@
 @rest_view("/timezone")
 class TestTimezoneView(BaseRestView):
     default_public = True
 
     @rest_api("", method="get")
     def get(self):
         return JsonResponse({'tz': self.request.TIMEZONE})
-
-
-@rest_view("/illegal-priority")
-class IllegalPriorityRestView(BaseRestView):
-    default_public = True
-
-    @rest_api("/test", method="get", priority=1)
-    def get(self, *args, **kwargs):
-        return JsonResponse(dict(value='test'))
-
-    @rest_api("/test", method="put", priority=2)
-    def put(self, *args, **kwargs):
-        return JsonResponse(dict(value='test'))
```

