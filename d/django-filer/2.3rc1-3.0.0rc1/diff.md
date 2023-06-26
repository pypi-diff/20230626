# Comparing `tmp/django-filer-2.3rc1.tar.gz` & `tmp/django-filer-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-filer-2.3rc1.tar", last modified: Fri Jan 20 20:29:04 2023, max compression
+gzip compressed data, was "django-filer-3.0.0rc1.tar", last modified: Mon Jun 26 13:23:51 2023, max compression
```

## Comparing `django-filer-2.3rc1.tar` & `django-filer-3.0.0rc1.tar`

### file list

```diff
@@ -1,399 +1,375 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.600533 django-filer-2.3rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-01-20 20:28:55.000000 django-filer-2.3rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-20 20:28:55.000000 django-filer-2.3rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-01-20 20:29:04.600533 django-filer-2.3rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-01-20 20:28:55.000000 django-filer-2.3rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.548534 django-filer-2.3rc1/django_filer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-01-20 20:29:04.000000 django-filer-2.3rc1/django_filer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-01-20 20:29:04.000000 django-filer-2.3rc1/django_filer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 20:29:04.000000 django-filer-2.3rc1/django_filer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 20:29:04.000000 django-filer-2.3rc1/django_filer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-20 20:29:04.000000 django-filer-2.3rc1/django_filer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-20 20:29:04.000000 django-filer-2.3rc1/django_filer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.548534 django-filer-2.3rc1/filer/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.552534 django-filer-2.3rc1/filer/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/admin/clipboardadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/admin/fileadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)    56125 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/admin/folderadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/admin/imageadmin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.552534 django-filer-2.3rc1/filer/admin/patched/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/admin/patched/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/admin/patched/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/admin/permissionadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/admin/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/admin/thumbnailoptionadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/admin/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/admin/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.552534 django-filer-2.3rc1/filer/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.552534 django-filer-2.3rc1/filer/contrib/django_cms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/contrib/django_cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/contrib/django_cms/cms_toolbars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.552534 django-filer-2.3rc1/filer/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/fields/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/fields/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/fields/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/fields/multistorage_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.552534 django-filer-2.3rc1/filer/locale/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.552534 django-filer-2.3rc1/filer/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26987 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.552534 django-filer-2.3rc1/filer/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26487 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.552534 django-filer-2.3rc1/filer/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.552534 django-filer-2.3rc1/filer/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    27071 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.552534 django-filer-2.3rc1/filer/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18714 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33818 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.552534 django-filer-2.3rc1/filer/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16420 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32184 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.552534 django-filer-2.3rc1/filer/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33463 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.556534 django-filer-2.3rc1/filer/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    27500 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.556534 django-filer-2.3rc1/filer/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30481 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.556534 django-filer-2.3rc1/filer/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26373 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.556534 django-filer-2.3rc1/filer/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17098 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32686 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.556534 django-filer-2.3rc1/filer/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18372 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    34069 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.556534 django-filer-2.3rc1/filer/locale/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    27630 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.556534 django-filer-2.3rc1/filer/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32519 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.556534 django-filer-2.3rc1/filer/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31855 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.556534 django-filer-2.3rc1/filer/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33167 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.540534 django-filer-2.3rc1/filer/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.556534 django-filer-2.3rc1/filer/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17810 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33347 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.556534 django-filer-2.3rc1/filer/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26374 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.556534 django-filer-2.3rc1/filer/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26388 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/ja_JP/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.556534 django-filer-2.3rc1/filer/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33347 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/lt_LT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/lt_LT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/lt_LT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26674 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/lt_LT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31143 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/nl_NL/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/nl_NL/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33623 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/nl_NL/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/nn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/nn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12947 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/nn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31075 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/nn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33701 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15418 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32621 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    21923 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37699 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26616 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29066 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/vi_VN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/vi_VN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/vi_VN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26393 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/vi_VN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26373 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/zh-Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/zh-Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/zh-Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31148 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/zh-Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26387 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26388 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.560534 django-filer-2.3rc1/filer/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.564534 django-filer-2.3rc1/filer/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/management/commands/filer_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/management/commands/generate_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/management/commands/import_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.564534 django-filer-2.3rc1/filer/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0002_auto_20150606_2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0003_thumbnailoption.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0004_auto_20160328_1434.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0005_auto_20160623_1425.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0006_auto_20160623_1627.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0007_auto_20161016_1055.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0008_auto_20171117_1313.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0009_auto_20171220_1635.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0010_auto_20180414_2058.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0011_auto_20190418_0137.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0012_file_mime_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0013_image_width_height_to_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0014_folder_permission_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.568534 django-filer-2.3rc1/filer/models/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/models/clipboardmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/models/filemodels.py
--rw-r--r--   0 runner    (1001) docker     (123)    13324 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/models/foldermodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/models/imagemodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/models/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/models/thumbnailoptionmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/models/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/models/virtualitems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.568534 django-filer-2.3rc1/filer/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.568534 django-filer-2.3rc1/filer/server/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/server/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/server/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/server/backends/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/server/backends/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/server/backends/xsendfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/server/main_server_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/server/thumbnails_server_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/server/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/server/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/static/filer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.572534 django-filer-2.3rc1/filer/static/filer/css/
--rwxr-xr-x   0 runner    (1001) docker     (123)   116820 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/css/admin_filer.css
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/css/admin_folderpermissions.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.572534 django-filer-2.3rc1/filer/static/filer/css/maps/
--rw-r--r--   0 runner    (1001) docker     (123)   243454 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/css/maps/admin_filer.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.572534 django-filer-2.3rc1/filer/static/filer/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   106260 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/fonts/django-filer-iconfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/fonts/django-filer-iconfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/fonts/django-filer-iconfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/fonts/django-filer-iconfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/fonts/django-filer-iconfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    68875 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   355981 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   138204 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    81284 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    64464 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.576534 django-filer-2.3rc1/filer/static/filer/fonts/src/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/fonts/src/check.svg
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/fonts/src/remove.svg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/fonts/src/trash-o.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.576534 django-filer-2.3rc1/filer/static/filer/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/icons/cloud-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/icons/file-zip.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/icons/folder-dropdown.svg
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/icons/folder-root.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/icons/folder-unfiled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/icons/folder.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.580534 django-filer-2.3rc1/filer/static/filer/img/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/img/button-bg.gif
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/img/close.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/img/icon_changelink.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/img/icon_deletelink.gif
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/img/loading_animation.gif
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/img/nav-bg.gif
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/img/select_item-hover.gif
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/img/select_item.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/img/upload_button.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.580534 django-filer-2.3rc1/filer/static/filer/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.580534 django-filer-2.3rc1/filer/static/filer/js/addons/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/addons/copy-move-files.js
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/addons/dropdown-menu.js
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/addons/dropzone.init.js
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/addons/focal-point.js
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/addons/popup_handling.js
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/addons/table-dropzone.js
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/addons/toggler.js
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/addons/tooltip.js
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/addons/upload-button.js
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/addons/widget.js
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.584534 django-filer-2.3rc1/filer/static/filer/js/libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/libs/class.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    34316 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/libs/dropzone.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18574 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/libs/fileuploader.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    31941 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/libs/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/libs/jquery.cookie.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    95957 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/libs/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/static/filer/js/libs/mediator.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.544534 django-filer-2.3rc1/filer/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.584534 django-filer-2.3rc1/filer/templates/admin/filer/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/base_site.html
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/delete_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/delete_selected_files_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/dismiss_popup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.584534 django-filer-2.3rc1/filer/templates/admin/filer/file/
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/file/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.588533 django-filer-2.3rc1/filer/templates/admin/filer/folder/
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/folder/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/folder/choose_copy_destination.html
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/folder/choose_images_resize_options.html
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/folder/choose_move_destination.html
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/folder/choose_rename_format.html
--rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/folder/directory_listing.html
--rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/folder/directory_table_list.html
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/folder/directory_thumbnail_list.html
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/folder/list_type_switcher.html
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/folder/new_folder_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.588533 django-filer-2.3rc1/filer/templates/admin/filer/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/image/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.588533 django-filer-2.3rc1/filer/templates/admin/filer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/templatetags/file_icon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.588533 django-filer-2.3rc1/filer/templates/admin/filer/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.588533 django-filer-2.3rc1/filer/templates/admin/filer/tools/clipboard/
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/tools/clipboard/clipboard.html
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/tools/detail_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/tools/search_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.588533 django-filer-2.3rc1/filer/templates/admin/filer/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/widgets/admin_file.html
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templates/admin/filer/widgets/admin_folder.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.588533 django-filer-2.3rc1/filer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templatetags/filer_admin_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templatetags/filer_image_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/templatetags/filer_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/thumbnail_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.592533 django-filer-2.3rc1/filer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/utils/filer_easy_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/utils/generate_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/utils/model_label.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/utils/pil_exif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/utils/recursive_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/utils/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-01-20 20:28:55.000000 django-filer-2.3rc1/filer/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-01-20 20:29:04.600533 django-filer-2.3rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-01-20 20:28:55.000000 django-filer-2.3rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.596533 django-filer-2.3rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    59990 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/test_filer_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/test_server_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.596533 django-filer-2.3rc1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.596533 django-filer-2.3rc1/tests/utils/custom_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/custom_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/custom_image/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.596533 django-filer-2.3rc1/tests/utils/custom_image/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/custom_image/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/custom_image/migrations/0002_auto_20160621_1510.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/custom_image/migrations/0003_auto_20180414_2059.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/custom_image/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/custom_image/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.596533 django-filer-2.3rc1/tests/utils/extended_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/extended_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/extended_app/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/extended_app/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.596533 django-filer-2.3rc1/tests/utils/extended_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/extended_app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/extended_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/extended_app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.600533 django-filer-2.3rc1/tests/utils/test_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/test_app/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/test_app/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:29:04.600533 django-filer-2.3rc1/tests/utils/test_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/test_app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/test_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/test_app/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-01-20 20:28:55.000000 django-filer-2.3rc1/tests/utils/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.147806 django-filer-3.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-26 13:23:51.147806 django-filer-3.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.099805 django-filer-3.0.0rc1/django_filer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-26 13:23:51.000000 django-filer-3.0.0rc1/django_filer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-06-26 13:23:51.000000 django-filer-3.0.0rc1/django_filer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:23:51.000000 django-filer-3.0.0rc1/django_filer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:23:50.000000 django-filer-3.0.0rc1/django_filer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 13:23:51.000000 django-filer-3.0.0rc1/django_filer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 13:23:51.000000 django-filer-3.0.0rc1/django_filer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.099805 django-filer-3.0.0rc1/filer/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.099805 django-filer-3.0.0rc1/filer/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/clipboardadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/fileadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57162 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/folderadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/imageadmin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.099805 django-filer-3.0.0rc1/filer/admin/patched/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/patched/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/patched/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/permissionadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/thumbnailoptionadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.099805 django-filer-3.0.0rc1/filer/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/contrib/django_cms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/contrib/django_cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/contrib/django_cms/cms_toolbars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/fields/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/fields/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/fields/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/fields/multistorage_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26987 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26487 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    27071 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18714 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33818 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16420 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32184 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33463 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    27500 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30481 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26373 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17098 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32686 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18372 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    34069 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    27630 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32519 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31855 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33167 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17810 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33347 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26374 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26388 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ja_JP/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33347 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/lt_LT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/lt_LT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/lt_LT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26674 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/lt_LT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31143 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/nl_NL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33623 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/nl_NL/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/nn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/nn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12947 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/nn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31075 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/nn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33701 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15418 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32621 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21923 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37699 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26616 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    29066 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/vi_VN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/vi_VN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/vi_VN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26393 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/vi_VN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26373 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/zh-Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/zh-Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh-Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31148 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh-Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.095805 django-filer-3.0.0rc1/filer/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26387 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.095805 django-filer-3.0.0rc1/filer/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26388 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.115805 django-filer-3.0.0rc1/filer/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/management/commands/filer_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/management/commands/generate_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/management/commands/import_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.115805 django-filer-3.0.0rc1/filer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0002_auto_20150606_2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0003_thumbnailoption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0004_auto_20160328_1434.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0005_auto_20160623_1425.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0006_auto_20160623_1627.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0007_auto_20161016_1055.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0008_auto_20171117_1313.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0009_auto_20171220_1635.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0010_auto_20180414_2058.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0011_auto_20190418_0137.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0012_file_mime_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0013_image_width_height_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0014_folder_permission_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0017_image__transparent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.119805 django-filer-3.0.0rc1/filer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/clipboardmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/filemodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/foldermodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/imagemodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/thumbnailoptionmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/virtualitems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.119805 django-filer-3.0.0rc1/filer/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.119805 django-filer-3.0.0rc1/filer/server/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/backends/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/backends/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/backends/xsendfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/main_server_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/thumbnails_server_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.095805 django-filer-3.0.0rc1/filer/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.095805 django-filer-3.0.0rc1/filer/static/filer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.119805 django-filer-3.0.0rc1/filer/static/filer/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/css/admin_filer.cms.icons.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    92632 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/css/admin_filer.css
+-rw-r--r--   0 runner    (1001) docker     (123)    25479 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/css/admin_filer.fa.icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/css/admin_folderpermissions.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.119805 django-filer-3.0.0rc1/filer/static/filer/css/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)    88599 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/css/maps/admin_filer.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.123805 django-filer-3.0.0rc1/filer/static/filer/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   106260 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    68875 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   355981 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   138204 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    81284 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    64464 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.123805 django-filer-3.0.0rc1/filer/static/filer/fonts/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/arrow-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/expand.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/move-to-folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/remove-selection.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/select.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/th-large.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/th-list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/upload.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.127805 django-filer-3.0.0rc1/filer/static/filer/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/cloud-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-zip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/folder-dropdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/folder-root.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/folder-unfiled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/folder.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.127805 django-filer-3.0.0rc1/filer/static/filer/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/button-bg.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/close.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/icon_changelink.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/icon_deletelink.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/loading_animation.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/nav-bg.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/select_item-hover.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/select_item.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/upload_button.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.127805 django-filer-3.0.0rc1/filer/static/filer/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.131805 django-filer-3.0.0rc1/filer/static/filer/js/addons/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/copy-move-files.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/dropdown-menu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/dropzone.init.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/filer_popup_response.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/focal-point.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/popup_handling.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/table-dropzone.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/toggler.js
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/tooltip.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/upload-button.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.135805 django-filer-3.0.0rc1/filer/static/filer/js/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/libs/class.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34316 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/libs/dropzone.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18574 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/libs/fileuploader.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/libs/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/libs/jquery.cookie.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95957 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/libs/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/libs/mediator.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.095805 django-filer-3.0.0rc1/filer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.095805 django-filer-3.0.0rc1/filer/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.135805 django-filer-3.0.0rc1/filer/templates/admin/filer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/delete_selected_files_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/dismiss_popup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.135805 django-filer-3.0.0rc1/filer/templates/admin/filer/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/file/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/file/popup_response.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.139805 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_copy_destination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_images_resize_options.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_move_destination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_rename_format.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/directory_listing.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/directory_table_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/directory_thumbnail_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/list_type_switcher.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/new_folder_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.143806 django-filer-3.0.0rc1/filer/templates/admin/filer/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/image/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.143806 django-filer-3.0.0rc1/filer/templates/admin/filer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/templatetags/file_icon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.143806 django-filer-3.0.0rc1/filer/templates/admin/filer/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.143806 django-filer-3.0.0rc1/filer/templates/admin/filer/tools/clipboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/tools/clipboard/clipboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/tools/detail_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/tools/search_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.143806 django-filer-3.0.0rc1/filer/templates/admin/filer/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/widgets/admin_file.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/widgets/admin_folder.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.143806 django-filer-3.0.0rc1/filer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templatetags/filer_admin_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templatetags/filer_image_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templatetags/filer_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/thumbnail_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.147806 django-filer-3.0.0rc1/filer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/filer_easy_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/generate_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/model_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/pil_exif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/recursive_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-26 13:23:51.147806 django-filer-3.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/setup.py
```

### Comparing `django-filer-2.3rc1/LICENSE` & `django-filer-3.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/PKG-INFO` & `django-filer-3.0.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filer
-Version: 2.3rc1
+Version: 3.0.0rc1
 Summary: A file management application for django that makes handling of files and images a breeze.
 Home-page: https://github.com/django-cms/django-filer
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -22,14 +22,15 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django CMS
 Classifier: Framework :: Django CMS :: 3.6
 Classifier: Framework :: Django CMS :: 3.7
 Classifier: Framework :: Django CMS :: 3.8
 Classifier: Framework :: Django CMS :: 3.9
 Classifier: Framework :: Django CMS :: 3.10
 Classifier: Framework :: Django CMS :: 3.11
@@ -42,15 +43,15 @@
 Requires-Python: >=3.6
 License-File: LICENSE
 
 ============
 Django Filer
 ============
 
-|pypi| |build| |python| |django| |coverage|
+|pypi| |python| |django| |coverage|
 
 **django Filer** is a file management application for django that makes
 handling of files and images a breeze.
 
 .. note::
 
         This project is endorsed by the `django CMS Association <https://www.django-cms.org/en/about-us/>`_.
@@ -92,16 +93,13 @@
 
 Please head over to the separate `documentation <https://django-filer.readthedocs.io/en/latest/index.html>`_
 for all the details on how to install, configure and use django-filer.
 
 
 .. |pypi| image:: https://badge.fury.io/py/django-filer.svg
     :target: http://badge.fury.io/py/django-filer
-.. |build| image:: https://travis-ci.org/django-cms/django-filer.svg?branch=master
-    :target: https://travis-ci.org/django-cms/django-filer
 .. |coverage| image:: https://codecov.io/gh/django-cms/django-filer/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/django-cms/django-filer
-
-.. |python| image:: https://img.shields.io/badge/python-3.7+-blue.svg
+.. |python| image:: https://img.shields.io/badge/python-3.8+-blue.svg
     :target: https://pypi.org/project/django-filer/
-.. |django| image:: https://img.shields.io/badge/django-2.2,%203.2,%204.1-blue.svg
+.. |django| image:: https://img.shields.io/badge/django-3.2+-blue.svg
     :target: https://www.djangoproject.com/
```

### Comparing `django-filer-2.3rc1/README.rst` & `django-filer-3.0.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ============
 Django Filer
 ============
 
-|pypi| |build| |python| |django| |coverage|
+|pypi| |python| |django| |coverage|
 
 **django Filer** is a file management application for django that makes
 handling of files and images a breeze.
 
 .. note::
 
         This project is endorsed by the `django CMS Association <https://www.django-cms.org/en/about-us/>`_.
@@ -48,16 +48,13 @@
 
 Please head over to the separate `documentation <https://django-filer.readthedocs.io/en/latest/index.html>`_
 for all the details on how to install, configure and use django-filer.
 
 
 .. |pypi| image:: https://badge.fury.io/py/django-filer.svg
     :target: http://badge.fury.io/py/django-filer
-.. |build| image:: https://travis-ci.org/django-cms/django-filer.svg?branch=master
-    :target: https://travis-ci.org/django-cms/django-filer
 .. |coverage| image:: https://codecov.io/gh/django-cms/django-filer/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/django-cms/django-filer
-
-.. |python| image:: https://img.shields.io/badge/python-3.7+-blue.svg
+.. |python| image:: https://img.shields.io/badge/python-3.8+-blue.svg
     :target: https://pypi.org/project/django-filer/
-.. |django| image:: https://img.shields.io/badge/django-2.2,%203.2,%204.1-blue.svg
+.. |django| image:: https://img.shields.io/badge/django-3.2+-blue.svg
     :target: https://www.djangoproject.com/
```

### Comparing `django-filer-2.3rc1/django_filer.egg-info/PKG-INFO` & `django-filer-3.0.0rc1/django_filer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filer
-Version: 2.3rc1
+Version: 3.0.0rc1
 Summary: A file management application for django that makes handling of files and images a breeze.
 Home-page: https://github.com/django-cms/django-filer
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -22,14 +22,15 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django CMS
 Classifier: Framework :: Django CMS :: 3.6
 Classifier: Framework :: Django CMS :: 3.7
 Classifier: Framework :: Django CMS :: 3.8
 Classifier: Framework :: Django CMS :: 3.9
 Classifier: Framework :: Django CMS :: 3.10
 Classifier: Framework :: Django CMS :: 3.11
@@ -42,15 +43,15 @@
 Requires-Python: >=3.6
 License-File: LICENSE
 
 ============
 Django Filer
 ============
 
-|pypi| |build| |python| |django| |coverage|
+|pypi| |python| |django| |coverage|
 
 **django Filer** is a file management application for django that makes
 handling of files and images a breeze.
 
 .. note::
 
         This project is endorsed by the `django CMS Association <https://www.django-cms.org/en/about-us/>`_.
@@ -92,16 +93,13 @@
 
 Please head over to the separate `documentation <https://django-filer.readthedocs.io/en/latest/index.html>`_
 for all the details on how to install, configure and use django-filer.
 
 
 .. |pypi| image:: https://badge.fury.io/py/django-filer.svg
     :target: http://badge.fury.io/py/django-filer
-.. |build| image:: https://travis-ci.org/django-cms/django-filer.svg?branch=master
-    :target: https://travis-ci.org/django-cms/django-filer
 .. |coverage| image:: https://codecov.io/gh/django-cms/django-filer/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/django-cms/django-filer
-
-.. |python| image:: https://img.shields.io/badge/python-3.7+-blue.svg
+.. |python| image:: https://img.shields.io/badge/python-3.8+-blue.svg
     :target: https://pypi.org/project/django-filer/
-.. |django| image:: https://img.shields.io/badge/django-2.2,%203.2,%204.1-blue.svg
+.. |django| image:: https://img.shields.io/badge/django-3.2+-blue.svg
     :target: https://www.djangoproject.com/
```

### Comparing `django-filer-2.3rc1/django_filer.egg-info/SOURCES.txt` & `django-filer-3.0.0rc1/django_filer.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 django_filer.egg-info/top_level.txt
 filer/__init__.py
 filer/apps.py
 filer/settings.py
 filer/storage.py
 filer/thumbnail_processors.py
 filer/urls.py
+filer/validation.py
 filer/views.py
 filer/admin/__init__.py
 filer/admin/clipboardadmin.py
 filer/admin/fileadmin.py
 filer/admin/folderadmin.py
 filer/admin/forms.py
 filer/admin/imageadmin.py
@@ -124,14 +125,16 @@
 filer/migrations/0009_auto_20171220_1635.py
 filer/migrations/0010_auto_20180414_2058.py
 filer/migrations/0011_auto_20190418_0137.py
 filer/migrations/0012_file_mime_type.py
 filer/migrations/0013_image_width_height_to_float.py
 filer/migrations/0014_folder_permission_choices.py
 filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py
+filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py
+filer/migrations/0017_image__transparent.py
 filer/migrations/__init__.py
 filer/models/__init__.py
 filer/models/abstract.py
 filer/models/clipboardmodels.py
 filer/models/filemodels.py
 filer/models/foldermodels.py
 filer/models/imagemodels.py
@@ -145,31 +148,43 @@
 filer/server/urls.py
 filer/server/views.py
 filer/server/backends/__init__.py
 filer/server/backends/base.py
 filer/server/backends/default.py
 filer/server/backends/nginx.py
 filer/server/backends/xsendfile.py
+filer/static/filer/css/admin_filer.cms.icons.css
 filer/static/filer/css/admin_filer.css
+filer/static/filer/css/admin_filer.fa.icons.css
 filer/static/filer/css/admin_folderpermissions.css
 filer/static/filer/css/maps/admin_filer.css.map
 filer/static/filer/fonts/FontAwesome.otf
 filer/static/filer/fonts/django-filer-iconfont.eot
 filer/static/filer/fonts/django-filer-iconfont.svg
 filer/static/filer/fonts/django-filer-iconfont.ttf
 filer/static/filer/fonts/django-filer-iconfont.woff
 filer/static/filer/fonts/django-filer-iconfont.woff2
 filer/static/filer/fonts/fontawesome-webfont.eot
 filer/static/filer/fonts/fontawesome-webfont.svg
 filer/static/filer/fonts/fontawesome-webfont.ttf
 filer/static/filer/fonts/fontawesome-webfont.woff
 filer/static/filer/fonts/fontawesome-webfont.woff2
-filer/static/filer/fonts/src/check.svg
-filer/static/filer/fonts/src/remove.svg
-filer/static/filer/fonts/src/trash-o.svg
+filer/static/filer/fonts/src/arrow-down.svg
+filer/static/filer/fonts/src/caret-down.svg
+filer/static/filer/fonts/src/chevron-right.svg
+filer/static/filer/fonts/src/download.svg
+filer/static/filer/fonts/src/expand.svg
+filer/static/filer/fonts/src/link.svg
+filer/static/filer/fonts/src/move-to-folder.svg
+filer/static/filer/fonts/src/picture.svg
+filer/static/filer/fonts/src/remove-selection.svg
+filer/static/filer/fonts/src/select.svg
+filer/static/filer/fonts/src/th-large.svg
+filer/static/filer/fonts/src/th-list.svg
+filer/static/filer/fonts/src/upload.svg
 filer/static/filer/icons/cloud-up.svg
 filer/static/filer/icons/file-audio.svg
 filer/static/filer/icons/file-empty.svg
 filer/static/filer/icons/file-font.svg
 filer/static/filer/icons/file-missing.svg
 filer/static/filer/icons/file-pdf.svg
 filer/static/filer/icons/file-picture.svg
@@ -189,14 +204,15 @@
 filer/static/filer/img/select_item-hover.gif
 filer/static/filer/img/select_item.gif
 filer/static/filer/img/upload_button.png
 filer/static/filer/js/base.js
 filer/static/filer/js/addons/copy-move-files.js
 filer/static/filer/js/addons/dropdown-menu.js
 filer/static/filer/js/addons/dropzone.init.js
+filer/static/filer/js/addons/filer_popup_response.js
 filer/static/filer/js/addons/focal-point.js
 filer/static/filer/js/addons/popup_handling.js
 filer/static/filer/js/addons/table-dropzone.js
 filer/static/filer/js/addons/toggler.js
 filer/static/filer/js/addons/tooltip.js
 filer/static/filer/js/addons/upload-button.js
 filer/static/filer/js/addons/widget.js
@@ -211,14 +227,15 @@
 filer/templates/admin/filer/base_site.html
 filer/templates/admin/filer/breadcrumbs.html
 filer/templates/admin/filer/change_form.html
 filer/templates/admin/filer/delete_confirmation.html
 filer/templates/admin/filer/delete_selected_files_confirmation.html
 filer/templates/admin/filer/dismiss_popup.html
 filer/templates/admin/filer/file/change_form.html
+filer/templates/admin/filer/file/popup_response.html
 filer/templates/admin/filer/folder/change_form.html
 filer/templates/admin/filer/folder/choose_copy_destination.html
 filer/templates/admin/filer/folder/choose_images_resize_options.html
 filer/templates/admin/filer/folder/choose_move_destination.html
 filer/templates/admin/filer/folder/choose_rename_format.html
 filer/templates/admin/filer/folder/directory_listing.html
 filer/templates/admin/filer/folder/directory_table_list.html
@@ -242,41 +259,8 @@
 filer/utils/filer_easy_thumbnails.py
 filer/utils/files.py
 filer/utils/generate_filename.py
 filer/utils/loader.py
 filer/utils/model_label.py
 filer/utils/pil_exif.py
 filer/utils/recursive_dictionary.py
-filer/utils/zip.py
-tests/__init__.py
-tests/helpers.py
-tests/settings.py
-tests/test_admin.py
-tests/test_dump.py
-tests/test_filer_check.py
-tests/test_migrations.py
-tests/test_models.py
-tests/test_permissions.py
-tests/test_server_backends.py
-tests/test_tools.py
-tests/test_utils.py
-tests/utils/__init__.py
-tests/utils/urls.py
-tests/utils/custom_image/__init__.py
-tests/utils/custom_image/apps.py
-tests/utils/custom_image/models.py
-tests/utils/custom_image/migrations/0001_initial.py
-tests/utils/custom_image/migrations/0002_auto_20160621_1510.py
-tests/utils/custom_image/migrations/0003_auto_20180414_2059.py
-tests/utils/custom_image/migrations/__init__.py
-tests/utils/extended_app/__init__.py
-tests/utils/extended_app/admin.py
-tests/utils/extended_app/apps.py
-tests/utils/extended_app/models.py
-tests/utils/extended_app/migrations/0001_initial.py
-tests/utils/extended_app/migrations/__init__.py
-tests/utils/test_app/__init__.py
-tests/utils/test_app/admin.py
-tests/utils/test_app/apps.py
-tests/utils/test_app/models.py
-tests/utils/test_app/migrations/0001_initial.py
-tests/utils/test_app/migrations/__init__.py
+filer/utils/zip.py
```

### Comparing `django-filer-2.3rc1/filer/__init__.py` & `django-filer-3.0.0rc1/filer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,10 +9,10 @@
  5. git push
  6. Assure that all tests pass on https://github.com/django-cms/django-filer/actions
  7. Create a new release on github. Create the new tag against the latest master commit and auto generate
     the release notes https://github.com/django-cms/django-filer/releases/new
  8. Publish the release and it will automatically release to pypi
 """
 
-__version__ = '2.3rc1'
+__version__ = '3.0.0rc1'
 
 default_app_config = 'filer.apps.FilerConfig'
```

### Comparing `django-filer-2.3rc1/filer/admin/__init__.py` & `django-filer-3.0.0rc1/filer/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/admin/clipboardadmin.py` & `django-filer-3.0.0rc1/filer/admin/clipboardadmin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-from django.contrib import admin
+from django.contrib import admin, messages
 from django.forms.models import modelform_factory
 from django.http import JsonResponse
-from django.urls import re_path
+from django.urls import path
+from django.utils.translation import gettext_lazy as _
 from django.views.decorators.csrf import csrf_exempt
 
 from .. import settings as filer_settings
 from ..models import Clipboard, ClipboardItem, Folder
 from ..utils.files import handle_request_files_upload, handle_upload
 from ..utils.loader import load_model
+from ..validation import FileValidationError, validate_upload
 from . import views
 
 
-NO_FOLDER_ERROR = "Can't find folder to upload. Please refresh and try again"
-NO_PERMISSIONS_FOR_FOLDER = (
+NO_PERMISSIONS = _("You do not have permission to upload files.")
+NO_FOLDER_ERROR = _("Can't find folder to upload. Please refresh and try again")
+NO_PERMISSIONS_FOR_FOLDER = _(
     "Can't use this folder, Permission Denied. Please select another folder."
 )
 
 
 Image = load_model(filer_settings.FILER_IMAGE_MODEL)
 
 
@@ -31,29 +34,29 @@
     filter_horizontal = ('files',)
     raw_id_fields = ('user',)
     verbose_name = "DEBUG Clipboard"
     verbose_name_plural = "DEBUG Clipboards"
 
     def get_urls(self):
         return [
-            re_path(r'^operations/paste_clipboard_to_folder/$',
-                    self.admin_site.admin_view(views.paste_clipboard_to_folder),
-                    name='filer-paste_clipboard_to_folder'),
-            re_path(r'^operations/discard_clipboard/$',
-                    self.admin_site.admin_view(views.discard_clipboard),
-                    name='filer-discard_clipboard'),
-            re_path(r'^operations/delete_clipboard/$',
-                    self.admin_site.admin_view(views.delete_clipboard),
-                    name='filer-delete_clipboard'),
-            re_path(r'^operations/upload/(?P<folder_id>[0-9]+)/$',
-                    ajax_upload,
-                    name='filer-ajax_upload'),
-            re_path(r'^operations/upload/no_folder/$',
-                    ajax_upload,
-                    name='filer-ajax_upload'),
+            path('operations/paste_clipboard_to_folder/',
+                 self.admin_site.admin_view(views.paste_clipboard_to_folder),
+                 name='filer-paste_clipboard_to_folder'),
+            path('operations/discard_clipboard/',
+                 self.admin_site.admin_view(views.discard_clipboard),
+                 name='filer-discard_clipboard'),
+            path('operations/delete_clipboard/',
+                 self.admin_site.admin_view(views.delete_clipboard),
+                 name='filer-delete_clipboard'),
+            path('operations/upload/<int:folder_id>/',
+                 ajax_upload,
+                 name='filer-ajax_upload'),
+            path('operations/upload/no_folder/',
+                 ajax_upload,
+                 name='filer-ajax_upload'),
         ] + super().get_urls()
 
     def get_model_perms(self, *args, **kwargs):
         """
         It seems this is only used for the list view. NICE :-)
         """
         return {
@@ -64,29 +67,36 @@
 
 
 @csrf_exempt
 def ajax_upload(request, folder_id=None):
     """
     Receives an upload from the uploader. Receives only one file at a time.
     """
+
+    if not request.user.has_perm("filer.add_file"):
+        messages.error(request, NO_PERMISSIONS)
+        return JsonResponse({'error': NO_PERMISSIONS})
+
     if folder_id:
         try:
             # Get folder
             folder = Folder.objects.get(pk=folder_id)
         except Folder.DoesNotExist:
+            messages.error(request, NO_FOLDER_ERROR)
             return JsonResponse({'error': NO_FOLDER_ERROR})
     else:
         folder = Folder.objects.filter(pk=request.session.get('filer_last_folder_id', 0)).first()
 
     # check permissions
     if folder and not folder.has_add_children_permission(request):
+        messages.error(request, NO_PERMISSIONS_FOR_FOLDER)
         return JsonResponse({'error': NO_PERMISSIONS_FOR_FOLDER})
 
     if len(request.FILES) == 1:
-        # dont check if request is ajax or not, just grab the file
+        # don't check if request is ajax or not, just grab the file
         upload, filename, is_raw, mime_type = handle_request_files_upload(request)
     else:
         # else process the request as usual
         upload, filename, is_raw, mime_type = handle_upload(request)
     # TODO: Deprecated/refactor
     # Get clipboad
     # clipboard = Clipboard.objects.get_or_create(user=request.user)[0]
@@ -101,14 +111,21 @@
                 fields=('original_filename', 'owner', 'file')
             )
             break
     uploadform = FileForm({'original_filename': filename, 'owner': request.user.pk},
                           {'file': upload})
     uploadform.instance.mime_type = mime_type
     if uploadform.is_valid():
+        try:
+            validate_upload(filename, upload, request.user, mime_type)
+        except FileValidationError as error:
+            from django.contrib.messages import ERROR, add_message
+            message = str(error)
+            add_message(request, ERROR, message)
+            return JsonResponse({'error': message})
         file_obj = uploadform.save(commit=False)
         # Enforce the FILER_IS_PUBLIC_DEFAULT
         file_obj.is_public = filer_settings.FILER_IS_PUBLIC_DEFAULT
         file_obj.folder = folder
         file_obj.save()
         # TODO: Deprecated/refactor
         # clipboard_item = ClipboardItem(
@@ -131,13 +148,13 @@
             }
             thumbnail_180 = file_obj.file.get_thumbnail(
                 thumbnail_180_options)
             data['thumbnail_180'] = thumbnail_180.url
             data['original_image'] = file_obj.url
         return JsonResponse(data)
     else:
-        form_errors = '; '.join(['%s: %s' % (
+        form_errors = '; '.join(['{}: {}'.format(
             field,
             ', '.join(errors)) for field, errors in list(
                 uploadform.errors.items())
         ])
         return JsonResponse({'message': str(form_errors)}, status=422)
```

### Comparing `django-filer-2.3rc1/filer/admin/folderadmin.py` & `django-filer-3.0.0rc1/filer/admin/folderadmin.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,26 +9,29 @@
 from django.conf import settings as django_settings
 from django.contrib import messages
 from django.contrib.admin import helpers
 from django.contrib.admin.utils import capfirst, quote, unquote
 from django.core.exceptions import PermissionDenied, ValidationError
 from django.core.paginator import EmptyPage, PageNotAnInteger, Paginator
 from django.db import models, router
+from django.db.models import F, OuterRef, Subquery
 from django.http import HttpResponse, HttpResponseRedirect
 from django.shortcuts import get_object_or_404, render
-from django.urls import re_path, reverse
+from django.urls import path, reverse
 from django.utils.encoding import force_str
 from django.utils.html import escape, format_html
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 from django.utils.translation import ngettext_lazy
 
+from easy_thumbnails.models import Thumbnail
+
 from .. import settings
 from ..models import File, Folder, FolderPermission, FolderRoot, ImagesWithMissingData, UnsortedImages, tools
-from ..settings import FILER_IMAGE_MODEL, FILER_PAGINATE_BY
+from ..settings import FILER_IMAGE_MODEL, FILER_PAGINATE_BY, TABLE_LIST_TYPE
 from ..thumbnail_processors import normalize_subject_location
 from ..utils.compatibility import get_delete_permission
 from ..utils.filer_easy_thumbnails import FilerActionThumbnailer
 from ..utils.loader import load_model
 from . import views
 from .forms import CopyFilesAndFoldersForm, RenameFilesForm, ResizeImagesForm
 from .patched.admin_utils import get_deleted_objects
@@ -50,15 +53,15 @@
         model = Folder
         fields = ('name',)
 
 
 class FolderAdmin(PrimitivePermissionAwareModelAdmin):
     list_display = ('name',)
     exclude = ('parent',)
-    list_per_page = 20
+    list_per_page = 100
     list_filter = ('owner',)
     search_fields = ['name']
     autocomplete_fields = ['owner']
     save_as = True  # see ImageAdmin
     actions = ['delete_files_or_folders', 'move_files_and_folders',
                'copy_files_and_folders', 'resize_images', 'rename_files']
 
@@ -124,15 +127,15 @@
         ):
 
             if obj.parent:
                 url = reverse('admin:filer-directory_listing',
                               kwargs={'folder_id': obj.parent.id})
             else:
                 url = reverse('admin:filer-directory_listing-root')
-            url = "{0}{1}".format(
+            url = "{}{}".format(
                 url,
                 admin_url_params_encoded(request),
             )
             return HttpResponseRedirect(url)
         return super().response_change(request, obj)
 
     def render_change_form(self, request, context, add=False, change=False,
@@ -177,15 +180,15 @@
                 folders_queryset=self.get_queryset(request).filter(id=object_id)
             )
             if parent_folder:
                 url = reverse('admin:filer-directory_listing',
                               kwargs={'folder_id': parent_folder.id})
             else:
                 url = reverse('admin:filer-directory_listing-root')
-            url = "{0}{1}".format(
+            url = "{}{}".format(
                 url,
                 admin_url_params_encoded(request),
             )
             return HttpResponseRedirect(url)
 
         return self.delete_files_or_folders(
             request,
@@ -197,69 +200,81 @@
         return format_html('<img src="filer/icons/folder.svg" alt="Folder Icon" />', django_settings.STATIC_ROOT)
     icon_img.allow_tags = True
 
     def get_urls(self):
         return [
             # we override the default list view with our own directory listing
             # of the root directories
-            re_path(r'^$',
-                    self.admin_site.admin_view(self.directory_listing),
-                    name='filer-directory_listing-root'),
-
-            re_path(r'^last/$',
-                    self.admin_site.admin_view(self.directory_listing),
-                    {'viewtype': 'last'},
-                    name='filer-directory_listing-last'),
-
-            re_path(r'^(?P<folder_id>\d+)/list/$',
-                    self.admin_site.admin_view(self.directory_listing),
-                    name='filer-directory_listing'),
-
-            re_path(r'^(?P<folder_id>\d+)/make_folder/$',
-                    self.admin_site.admin_view(views.make_folder),
-                    name='filer-directory_listing-make_folder'),
-            re_path(r'^make_folder/$',
-                    self.admin_site.admin_view(views.make_folder),
-                    name='filer-directory_listing-make_root_folder'),
-
-            re_path(r'^images_with_missing_data/$',
-                    self.admin_site.admin_view(self.directory_listing),
-                    {'viewtype': 'images_with_missing_data'},
-                    name='filer-directory_listing-images_with_missing_data'),
-
-            re_path(r'^unfiled_images/$',
-                    self.admin_site.admin_view(self.directory_listing),
-                    {'viewtype': 'unfiled_images'},
-                    name='filer-directory_listing-unfiled_images'),
+            path('',
+                 self.admin_site.admin_view(self.directory_listing),
+                 name='filer-directory_listing-root'),
+
+            path('last/',
+                 self.admin_site.admin_view(self.directory_listing),
+                 {'viewtype': 'last'},
+                 name='filer-directory_listing-last'),
+
+            path('<int:folder_id>/list/',
+                 self.admin_site.admin_view(self.directory_listing),
+                 name='filer-directory_listing'),
+
+            path('<int:folder_id>/make_folder/',
+                 self.admin_site.admin_view(views.make_folder),
+                 name='filer-directory_listing-make_folder'),
+            path('make_folder/',
+                 self.admin_site.admin_view(views.make_folder),
+                 name='filer-directory_listing-make_root_folder'),
+
+            path('images_with_missing_data/',
+                 self.admin_site.admin_view(self.directory_listing),
+                 {'viewtype': 'images_with_missing_data'},
+                 name='filer-directory_listing-images_with_missing_data'),
+
+            path('unfiled_images/',
+                 self.admin_site.admin_view(self.directory_listing),
+                 {'viewtype': 'unfiled_images'},
+                 name='filer-directory_listing-unfiled_images'),
         ] + super().get_urls()
 
     # custom views
     def directory_listing(self, request, folder_id=None, viewtype=None):
+        if not request.user.has_perm("filer.can_use_directory_listing"):
+            raise PermissionDenied()
         clipboard = tools.get_user_clipboard(request.user)
         if viewtype == 'images_with_missing_data':
             folder = ImagesWithMissingData()
         elif viewtype == 'unfiled_images':
-            folder = UnsortedImages()
+            # pass user in the class invocation, so that we can get
+            # access to the current user instance in the class
+            folder = UnsortedImages(user=request.user)
         elif viewtype == 'last':
             last_folder_id = request.session.get('filer_last_folder_id')
             try:
                 self.get_queryset(request).get(id=last_folder_id)
             except self.model.DoesNotExist:
                 url = reverse('admin:filer-directory_listing-root')
-                url = "%s%s" % (url, admin_url_params_encoded(request))
+                url = "{}{}".format(url, admin_url_params_encoded(request))
             else:
                 url = reverse('admin:filer-directory_listing', kwargs={'folder_id': last_folder_id})
-                url = "%s%s" % (url, admin_url_params_encoded(request))
+                url = "{}{}".format(url, admin_url_params_encoded(request))
             return HttpResponseRedirect(url)
         elif folder_id is None:
             folder = FolderRoot()
         else:
             folder = get_object_or_404(self.get_queryset(request), id=folder_id)
         request.session['filer_last_folder_id'] = folder_id
 
+        list_type = get_directory_listing_type(request) or settings.FILER_FOLDER_ADMIN_DEFAULT_LIST_TYPE
+        if list_type == TABLE_LIST_TYPE:
+            size = "40x40"  # Prefetch thumbnails for listing
+            size_x2 = "80x80"
+        else:
+            size = "160x160"  # Prefetch thumbnails for thumbnail view
+            size_x2 = "320x320"
+
         # Check actions to see if any are available on this changelist
         actions = self.get_actions(request)
 
         # Remove action checkboxes if there aren't any actions available.
         list_display = list(self.list_display)
         if not actions:
             try:
@@ -278,43 +293,42 @@
             search_mode = False
         # Limit search results to current folder.
         limit_search_to_folder = request.GET.get('limit_search_to_folder',
                                                  False) in (True, 'on')
 
         if len(search_terms) > 0:
             if folder and limit_search_to_folder and not folder.is_root:
+                desc_folder_ids = folder.get_descendants_ids()
                 # Do not include current folder itself in search results.
-                folder_qs = folder.get_descendants(include_self=False)
+                folder_qs = Folder.objects.filter(pk__in=desc_folder_ids)
                 # Limit search results to files in the current folder or any
                 # nested folder.
-                file_qs = File.objects.filter(
-                    folder__in=folder.get_descendants(include_self=True))
+                file_qs = File.objects.filter(folder_id__in=desc_folder_ids + [folder.pk])
             else:
                 folder_qs = self.get_queryset(request)
                 file_qs = File.objects.all()
-            folder_qs = self.filter_folder(folder_qs, search_terms)
+            folder_qs = self.filter_folder(folder_qs, search_terms).prefetch_related("children", "all_files")
             file_qs = self.filter_file(file_qs, search_terms)
 
             show_result_count = True
         else:
             folder_qs = folder.children.all()
             file_qs = folder.files.all()
             show_result_count = False
 
-        folder_qs = folder_qs.order_by('name')
+        folder_qs = folder_qs.order_by('name').select_related("owner")
         order_by = request.GET.get('order_by', None)
-        if order_by is not None:
-            order_by = order_by.split(',')
-            order_by = [field for field in order_by
-                        if re.sub(r'^-', '', field) in self.order_by_file_fields]
-            if len(order_by) > 0:
-                file_qs = file_qs.order_by(*order_by)
+        if order_by is None:
+            order_by = "file"
+        order_by = order_by.split(',')
+        order_by = [field for field in order_by
+                    if re.sub(r'^-', '', field) in self.order_by_file_fields]
+        if len(order_by) > 0:
+            file_qs = file_qs.order_by(*order_by)
 
-        folder_children = []
-        folder_files = []
         if folder.is_root and not search_mode:
             virtual_items = folder.virtual_folders
         else:
             virtual_items = []
 
         perms = FolderPermission.objects.get_read_id_list(request.user)
         if perms != 'All':
@@ -326,37 +340,46 @@
             folder_qs = folder_qs.filter(models.Q(id__in=perms) | models.Q(owner=request.user))
             root_exclude_kwargs = {'parent__isnull': False, 'parent__id__in': perms}
         else:
             root_exclude_kwargs = {'parent__isnull': False}
         if folder.is_root:
             folder_qs = folder_qs.exclude(**root_exclude_kwargs)
 
-        folder_children += folder_qs
-        folder_files += file_qs
+        # Annotate thumbnail status
+        thumbnail_qs = (
+            Thumbnail.objects
+            .filter(
+                source__name=OuterRef("file"),
+                modified__gte=F("source__modified"),
+            )
+            .exclude(name__contains="upscale")  # TODO: Check WHY not used by directory listing
+            .order_by("-modified")
+        )
+        file_qs = file_qs.annotate(
+            thumbnail_name=Subquery(thumbnail_qs.filter(name__contains=f"__{size}_").values_list("name")[:1]),
+            thumbnailx2_name=Subquery(thumbnail_qs.filter(name__contains=f"__{size_x2}_").values_list("name")[:1])
+        ).select_related("owner")
 
         try:
             permissions = {
                 'has_edit_permission': folder.has_edit_permission(request),
                 'has_read_permission': folder.has_read_permission(request),
                 'has_add_children_permission':
                     folder.has_add_children_permission(request),
             }
         except:  # noqa
             permissions = {}
 
-        if order_by is None or len(order_by) == 0:
-            folder_files.sort()
-
-        items = folder_children + folder_files
+        items = list(itertools.chain(folder_qs, file_qs))
         paginator = Paginator(items, FILER_PAGINATE_BY)
 
         # Are we moving to clipboard?
         if request.method == 'POST' and '_save' not in request.POST:
             # TODO: Refactor/remove clipboard parts
-            for f in folder_files:
+            for f in folder_qs:
                 if "move-to-clipboard-%d" % (f.id,) in request.POST:
                     clipboard = tools.get_user_clipboard(request.user)
                     if f.has_edit_permission(request):
                         tools.move_file_to_clipboard([f], clipboard)
                         return HttpResponseRedirect(request.get_full_path())
                     else:
                         raise PermissionDenied
@@ -403,34 +426,35 @@
         try:
             paginated_items = paginator.page(request.GET.get('page', 1))
         except PageNotAnInteger:
             paginated_items = paginator.page(1)
         except EmptyPage:
             paginated_items = paginator.page(paginator.num_pages)
 
-        list_type = get_directory_listing_type(request) or settings.FILER_FOLDER_ADMIN_DEFAULT_LIST_TYPE
         context = self.admin_site.each_context(request)
         context.update({
             'folder': folder,
             'clipboard_files': File.objects.filter(
                 in_clipboards__clipboarditem__clipboard__user=request.user
             ).distinct(),
             'paginator': paginator,
             'paginated_items': paginated_items,
             'virtual_items': virtual_items,
             'uploader_connections': settings.FILER_UPLOADER_CONNECTIONS,
+            'max_files': settings.FILER_UPLOADER_MAX_FILES,
+            'max_filesize': settings.FILER_UPLOADER_MAX_FILE_SIZE,
             'permissions': permissions,
             'permstest': userperms_for_request(folder, request),
             'current_url': request.path,
             'title': _('Directory listing for %(folder_name)s') % {'folder_name': folder.name},
             'search_string': ' '.join(search_terms),
             'q': urlquote(q),
             'show_result_count': show_result_count,
-            'folder_children': folder_children,
-            'folder_files': folder_files,
+            'folder_children': folder_qs,
+            'folder_files': file_qs,
             'limit_search_to_folder': limit_search_to_folder,
             'is_popup': popup_status(request),
             'filer_admin_context': AdminContext(request),
             # needed in the admin/base.html template for logout links
             'root_path': reverse('admin:index'),
             'action_form': action_form,
             'actions_on_top': self.actions_on_top,
@@ -490,15 +514,15 @@
         return [
             field.name for field in User._meta.fields
             if isinstance(field, models.CharField) and field.name != 'password'
         ]
 
     def get_owner_filter_lookups(self):
         return [
-            'owner__{field}__icontains'.format(field=field)
+            f'owner__{field}__icontains'
             for field in self.owner_search_fields
         ]
 
     def response_action(self, request, files_queryset, folders_queryset):
         """
         Handle an admin action. This is called if a request is POSTed to the
         changelist; it returns an HttpResponse if the action was handled, and
@@ -738,16 +762,15 @@
                 # delete all files in all selected folders and their children
                 # This would happen automatically by ways of the delete
                 # cascade, but then the individual .delete() methods won't be
                 # called and the files won't be deleted from the filesystem.
                 folder_ids = set()
                 for folder in folders_queryset:
                     folder_ids.add(folder.id)
-                    folder_ids.update(
-                        folder.get_descendants().values_list('id', flat=True))
+                    folder_ids.update(folder.get_descendants_ids())
                 for f in File.objects.filter(folder__in=folder_ids):
                     self.log_deletion(request, f, force_str(f))
                     f.delete()
                 # delete all folders
                 for f in folders_queryset:
                     self.log_deletion(request, f, force_str(f))
                     f.delete()
@@ -801,15 +824,15 @@
             if not user.has_perm(p):
                 perms_needed.add(opts.verbose_name)
             # Display a link to the admin page.
             return format_html('{}: <a href="{}">{}</a>', escape(capfirst(opts.verbose_name)), admin_url, escape(obj))
         else:
             # Don't display link to edit, because it either has no
             # admin or is edited inline.
-            return '%s: %s' % (capfirst(opts.verbose_name), force_str(obj))
+            return '{}: {}'.format(capfirst(opts.verbose_name), force_str(obj))
 
     def _check_copy_perms(self, request, files_queryset, folders_queryset):
         try:
             check_files_read_permissions(request, files_queryset)
             check_folder_read_permissions(request, folders_queryset)
         except PermissionDenied:
             return True
@@ -855,28 +878,23 @@
 
             if not fo.has_read_permission(request):
                 continue
 
             # We do not allow copying/moving back to the folder itself
             enabled = (allow_self or fo != current_folder) and fo.has_add_children_permission(request)
             yield (fo, (mark_safe(("&nbsp;&nbsp;" * level) + force_str(fo)), enabled))
-            for c in self._list_all_destination_folders_recursive(request, folders_queryset, current_folder, fo.children.all(), allow_self, level + 1):
-                yield c
+            yield from self._list_all_destination_folders_recursive(request, folders_queryset, current_folder, fo.children.all(), allow_self, level + 1)
 
     def _list_all_destination_folders(self, request, folders_queryset, current_folder, allow_self):
         root_folders = self.get_queryset(request).filter(parent__isnull=True).order_by('name')
         return list(self._list_all_destination_folders_recursive(request, folders_queryset, current_folder, root_folders, allow_self, 0))
 
     def _move_files_and_folders_impl(self, files_queryset, folders_queryset, destination):
-        for f in files_queryset:
-            f.folder = destination
-            f.save()
-        for f in folders_queryset:
-            f.move_to(destination, 'last-child')
-            f.save()
+        files_queryset.update(folder=destination)
+        folders_queryset.update(parent=destination)
 
     def move_files_and_folders(self, request, files_queryset, folders_queryset):
         opts = self.model._meta
         app_label = opts.app_label
 
         current_folder = self._get_current_action_folder(request, files_queryset, folders_queryset)
         perms_needed = self._check_move_perms(request, files_queryset, folders_queryset)
@@ -1039,15 +1057,15 @@
             self._copy_file(f, destination, suffix, overwrite)
         return len(files)
 
     def _get_available_name(self, destination, name):
         count = itertools.count(1)
         original = name
         while destination.contains_folder(name):
-            name = "%s_%s" % (original, next(count))
+            name = "{}_{}".format(original, next(count))
         return name
 
     def _copy_folder(self, folder, destination, suffix, overwrite):
         if overwrite:
             # Not yet implemented as we have to find a portable (for different storage backends) way to overwrite files
             raise NotImplementedError
```

### Comparing `django-filer-2.3rc1/filer/admin/forms.py` & `django-filer-3.0.0rc1/filer/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/admin/imageadmin.py` & `django-filer-3.0.0rc1/filer/admin/imageadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/admin/patched/admin_utils.py` & `django-filer-3.0.0rc1/filer/admin/patched/admin_utils.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/admin/permissionadmin.py` & `django-filer-3.0.0rc1/filer/admin/permissionadmin.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     search_fields = ['user__username', 'group__name', 'folder__name']
     autocomplete_fields = ['user', 'group', 'folder']
 
     class Media:
         css = {'all': ['filer/css/admin_folderpermissions.css']}
 
     def get_queryset(self, request):
-        qs = super(PermissionAdmin, self).get_queryset(request)
+        qs = super().get_queryset(request)
         return qs.prefetch_related("group", "folder")
 
     def get_model_perms(self, request):
         # don't display the permissions admin if permissions are disabled.
         # This method is easier for testing than not registering the admin at all at import time
         enable_permissions = settings.FILER_ENABLE_PERMISSIONS and request.user.has_perm('filer.add_folderpermission')
         return {
```

### Comparing `django-filer-2.3rc1/filer/admin/permissions.py` & `django-filer-3.0.0rc1/filer/admin/permissions.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/admin/tools.py` & `django-filer-3.0.0rc1/filer/admin/tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,14 +62,18 @@
     # (injection attacks)
     pick_type = request.GET.get('_pick', request.POST.get('_pick'))
     if pick_type in ALLOWED_PICK_TYPES:
         return pick_type
     return None
 
 
+def edit_from_widget(request):
+    return request.GET.get('_edit_from_widget') == '1'
+
+
 def get_directory_listing_type(request):
     list_type = request.GET.get('_list_type', None)
     if list_type not in settings.FILER_FOLDER_ADMIN_LIST_TYPE_CHOICES:
         return
     return list_type
 
 
@@ -80,28 +84,30 @@
     """
     params = params or {}
     if popup_status(request):
         params[IS_POPUP_VAR] = '1'
     pick_type = popup_pick_type(request)
     if pick_type:
         params['_pick'] = pick_type
+    if edit_from_widget(request):
+        params['_edit_from_widget'] = '1'
     list_type = get_directory_listing_type(request)
     if list_type and '_list_type' not in params.keys():
         params['_list_type'] = list_type
     return params
 
 
 def admin_url_params_encoded(request, first_separator='?', params=None):
     # sorted to make testing easier
     params = urlencode(
         sorted(admin_url_params(request, params=params).items())
     )
     if not params:
         return ''
-    return '{0}{1}'.format(first_separator, params)
+    return f'{first_separator}{params}'
 
 
 class AdminContext(dict):
     def __init__(self, request):
         super().__init__()
         self.update(admin_url_params(request))
```

### Comparing `django-filer-2.3rc1/filer/admin/views.py` & `django-filer-3.0.0rc1/filer/admin/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             tools.discard_clipboard(clipboard)
         else:
             raise PermissionDenied
     redirect = request.GET.get('redirect_to', '')
     if not redirect:
         redirect = request.POST.get('redirect_to', '')
     return HttpResponseRedirect(
-        '{0}?order_by=-modified_at{1}'.format(
+        '{}?order_by=-modified_at{}'.format(
             redirect,
             admin_url_params_encoded(request, first_separator='&'),
         )
     )
 
 
 @login_required
@@ -103,15 +103,15 @@
         # TODO: cleanly remove Clipboard code if it is no longer needed
         return HttpResponseBadRequest('not implemented anymore')
 
     if request.method == 'POST':
         clipboard = Clipboard.objects.get(id=request.POST.get('clipboard_id'))
         tools.discard_clipboard(clipboard)
     return HttpResponseRedirect(
-        '{0}{1}'.format(
+        '{}{}'.format(
             request.POST.get('redirect_to', ''),
             admin_url_params_encoded(request, first_separator='&'),
         )
     )
 
 
 @login_required
@@ -120,12 +120,12 @@
         # TODO: cleanly remove Clipboard code if it is no longer needed
         return HttpResponseBadRequest('not implemented anymore')
 
     if request.method == 'POST':
         clipboard = Clipboard.objects.get(id=request.POST.get('clipboard_id'))
         tools.delete_clipboard(clipboard)
     return HttpResponseRedirect(
-        '{0}{1}'.format(
+        '{}{}'.format(
             request.POST.get('redirect_to', ''),
             admin_url_params_encoded(request, first_separator='&'),
         )
     )
```

### Comparing `django-filer-2.3rc1/filer/contrib/django_cms/cms_toolbars.py` & `django-filer-3.0.0rc1/filer/contrib/django_cms/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/fields/file.py` & `django-filer-3.0.0rc1/filer/fields/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,32 +10,35 @@
 from django.template.loader import render_to_string
 from django.urls import reverse
 from django.utils.http import urlencode
 from django.utils.safestring import mark_safe
 
 from .. import settings as filer_settings
 from ..models import File
+from ..settings import ICON_CSS_LIB
 from ..utils.compatibility import truncate_words
 from ..utils.model_label import get_model_label
 
 
 logger = logging.getLogger(__name__)
 
 
 class AdminFileWidget(ForeignKeyRawIdWidget):
     choices = None
 
     def render(self, name, value, attrs=None, renderer=None):
         obj = self.obj_for_value(value)
         css_id = attrs.get('id', 'id_image_x')
         related_url = None
+        change_url = ''
         if value:
             try:
                 file_obj = File.objects.get(pk=value)
                 related_url = file_obj.logical_folder.get_admin_directory_listing_url_path()
+                change_url = file_obj.get_admin_change_url()
             except Exception as e:
                 # catch exception and manage it. We can re-raise it for debugging
                 # purposes and/or just logging it, provided user configured
                 # proper logging configuration
                 if filer_settings.FILER_ENABLE_LOGGING:
                     logger.error('Error while rendering file widget: %s', e)
                 if filer_settings.FILER_DEBUG:
@@ -53,15 +56,16 @@
             attrs['class'] = 'vForeignKeyRawIdAdminField'
         # rendering the super for ForeignKeyRawIdWidget on purpose here because
         # we only need the input and none of the other stuff that
         # ForeignKeyRawIdWidget adds
         hidden_input = super(ForeignKeyRawIdWidget, self).render(name, value, attrs)  # grandparent super
         context = {
             'hidden_input': hidden_input,
-            'lookup_url': '%s%s' % (related_url, lookup_url),
+            'lookup_url': '{}{}'.format(related_url, lookup_url),
+            'change_url': change_url,
             'object': obj,
             'lookup_name': name,
             'id': css_id,
             'admin_icon_delete': ('admin/img/icon-deletelink.svg'),
         }
         html = render_to_string('admin/filer/widgets/admin_file.html', context)
         return mark_safe(html)
@@ -81,17 +85,17 @@
         else:
             obj = None
         return obj
 
     class Media:
         extra = '' if settings.DEBUG else '.min'
         css = {
-            'all': [
+            'all': (
                 'filer/css/admin_filer.css',
-            ]
+            ) + ICON_CSS_LIB,
         }
         js = (
             'admin/js/vendor/jquery/jquery%s.js' % extra,
             'admin/js/jquery.init.js',
             'filer/js/libs/dropzone.min.js',
             'filer/js/addons/dropzone.init.js',
             'filer/js/addons/popup_handling.js',
```

### Comparing `django-filer-2.3rc1/filer/fields/folder.py` & `django-filer-3.0.0rc1/filer/fields/folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         super_attrs = attrs.copy()
         hidden_input = super(ForeignKeyRawIdWidget, self).render(name, value, super_attrs)  # grandparent super
 
         # TODO: "id_" is hard-coded here. This should instead use the correct
         # API to determine the ID dynamically.
         context = {
             'hidden_input': hidden_input,
-            'lookup_url': '%s%s' % (related_url, url),
+            'lookup_url': '{}{}'.format(related_url, url),
             'lookup_name': name,
             'span_id': css_id_description_txt,
             'object': obj,
             'clear_id': '%s_clear' % css_id,
             'descid': css_id_description_txt,
             'noimg': 'filer/icons/nofile_32x32.png',
             'foldid': css_id_folder,
@@ -111,15 +111,15 @@
 
     def __init__(self, **kwargs):
         # We hard-code the `to` argument for ForeignKey.__init__
         dfl = get_model_label(self.default_model_class)
         if "to" in kwargs.keys():  # pragma: no cover
             old_to = get_model_label(kwargs.pop("to"))
             if old_to.lower() != dfl.lower():
-                msg = "%s can only be a ForeignKey to %s; %s passed" % (
+                msg = "{} can only be a ForeignKey to {}; {} passed".format(
                     self.__class__.__name__, dfl, old_to
                 )
                 warnings.warn(msg, SyntaxWarning)
         kwargs['to'] = dfl
         super().__init__(**kwargs)
 
     def formfield(self, **kwargs):
```

### Comparing `django-filer-2.3rc1/filer/fields/multistorage_file.py` & `django-filer-3.0.0rc1/filer/fields/multistorage_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         super().__set__(instance, value)
 
         # To prevent recalculating file data related attributes when we are instantiating
         # an object from the database, update only if the field had a value before this assignment.
         # To prevent recalculating upon reassignment of the same file, update only if value is
         # different than the previous one.
         if prev_assigned and value != previous_file:
-            callback_attr = '{}_data_changed'.format(self.field.name)
+            callback_attr = f'{self.field.name}_data_changed'
             if hasattr(instance, callback_attr):
                 getattr(instance, callback_attr)()
 
 
 class MultiStorageFieldFile(ThumbnailerNameMixin,
                             easy_thumbnails_files.ThumbnailerFieldFile):
     def __init__(self, instance, field, name):
@@ -154,16 +154,16 @@
             sha = hashlib.sha1()
             sha.update(payload_file.read())
             if sha.hexdigest() != obj.sha1:
                 warnings.warn('The checksum for "%s" diverges. Check for file consistency!' % obj.original_filename)
             payload_file.seek(0)
             encoded_string = base64.b64encode(payload_file.read()).decode('utf-8')
             return value, encoded_string
-        except IOError:
-            warnings.warn('The payload for "%s" is missing. No such file on disk: %s!' % (obj.original_filename, self.storage.location))
+        except OSError:
+            warnings.warn('The payload for "{}" is missing. No such file on disk: {}!'.format(obj.original_filename, self.storage.location))
             return value
 
     def to_python(self, value):
         if isinstance(value, list) and len(value) == 2 and isinstance(value[0], str):
             filename, payload = value
             try:
                 payload = base64.b64decode(payload)
```

### Comparing `django-filer-2.3rc1/filer/locale/ar/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/ar/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/bg/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/ca/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/ca/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/cs/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/cs/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/de/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/de/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/en/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/en/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/es/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/es/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/et/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/et/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/eu/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/eu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/eu/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/fa/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/fi/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/fi/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/fr/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/fr/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/gl/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/gl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/gl/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/he/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/he/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/hr/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/hr/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/hu/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/hu/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/it/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/it/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/ja/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/ja_JP/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/lt/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/lt/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/lt_LT/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/lt_LT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/lt_LT/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/lt_LT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/nb/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/nb/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/nl_NL/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/nl_NL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/nl_NL/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/nl_NL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/nn/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/nn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/nn/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/nn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/pl/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/pl/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/pt/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/pt_BR/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/pt_BR/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/ru/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/ru/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/sk/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/tr/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/tr/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/vi_VN/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/vi_VN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/zh/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/zh-Hans/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc1/filer/locale/zh-Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/zh-Hans/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/zh-Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/zh_CN/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/locale/zh_TW/LC_MESSAGES/django.po` & `django-filer-3.0.0rc1/filer/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/management/commands/filer_check.py` & `django-filer-3.0.0rc1/filer/management/commands/filer_check.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/management/commands/generate_thumbnails.py` & `django-filer-3.0.0rc1/filer/management/commands/generate_thumbnails.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/management/commands/import_files.py` & `django-filer-3.0.0rc1/filer/management/commands/import_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """
         Create a File or an Image into the given folder
         """
         try:
             iext = os.path.splitext(file_obj.name)[1].lower()
         except:  # noqa
             iext = ''
-        if iext in ['.jpg', '.jpeg', '.png', '.gif']:
+        if iext in ['.jpg', '.jpeg', '.png', '.gif', '.webp']:
             obj, created = Image.objects.get_or_create(
                 original_filename=file_obj.name,
                 file=file_obj,
                 folder=folder,
                 is_public=FILER_IS_PUBLIC_DEFAULT)
             if created:
                 self.image_created += 1
```

### Comparing `django-filer-2.3rc1/filer/migrations/0001_initial.py` & `django-filer-3.0.0rc1/filer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/migrations/0002_auto_20150606_2003.py` & `django-filer-3.0.0rc1/filer/migrations/0002_auto_20150606_2003.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/migrations/0003_thumbnailoption.py` & `django-filer-3.0.0rc1/filer/migrations/0003_thumbnailoption.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/migrations/0005_auto_20160623_1425.py` & `django-filer-3.0.0rc1/filer/migrations/0005_auto_20160623_1425.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/migrations/0006_auto_20160623_1627.py` & `django-filer-3.0.0rc1/filer/migrations/0006_auto_20160623_1627.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/migrations/0008_auto_20171117_1313.py` & `django-filer-3.0.0rc1/filer/migrations/0008_auto_20171117_1313.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/migrations/0010_auto_20180414_2058.py` & `django-filer-3.0.0rc1/filer/migrations/0010_auto_20180414_2058.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/migrations/0011_auto_20190418_0137.py` & `django-filer-3.0.0rc1/filer/migrations/0011_auto_20190418_0137.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/migrations/0012_file_mime_type.py` & `django-filer-3.0.0rc1/filer/migrations/0012_file_mime_type.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/migrations/0013_image_width_height_to_float.py` & `django-filer-3.0.0rc1/filer/migrations/0013_image_width_height_to_float.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/migrations/0014_folder_permission_choices.py` & `django-filer-3.0.0rc1/filer/migrations/0014_folder_permission_choices.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py` & `django-filer-3.0.0rc1/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.0.3 on 2022-04-12 12:20
+# Generated by Django 4.1.9 on 2023-06-15 20:03
 
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
```

### Comparing `django-filer-2.3rc1/filer/models/abstract.py` & `django-filer-3.0.0rc1/filer/models/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
 from django.db import models
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 
+import easy_thumbnails.utils
 from easy_thumbnails.VIL import Image as VILImage
 
 from .. import settings as filer_settings
 from ..utils.compatibility import PILImage
 from ..utils.filer_easy_thumbnails import FilerThumbnailer
 from ..utils.pil_exif import get_exif_for_file
 from .filemodels import File
@@ -35,14 +36,19 @@
     )
 
     _width = models.FloatField(
         null=True,
         blank=True,
     )
 
+    _transparent = models.BooleanField(
+        null=False,
+        default=False,
+    )
+
     default_alt_text = models.CharField(
         _("default alt text"),
         max_length=255,
         blank=True,
         null=True,
     )
 
@@ -73,37 +79,41 @@
         verbose_name_plural = _("images")
         abstract = True
         default_manager_name = 'objects'
 
     @classmethod
     def matches_file_type(cls, iname, ifile, mime_type):
         # source: https://www.freeformatter.com/mime-types-list.html
-        image_subtypes = ['gif', 'jpeg', 'png', 'x-png', 'svg+xml']
+        image_subtypes = ['gif', 'jpeg', 'png', 'x-png', 'svg+xml', 'webp']
         maintype, subtype = mime_type.split('/')
         return maintype == 'image' and subtype in image_subtypes
 
     def file_data_changed(self, post_init=False):
         attrs_updated = super().file_data_changed(post_init=post_init)
         if attrs_updated:
             try:
                 try:
                     imgfile = self.file.file
                 except ValueError:
                     imgfile = self.file_ptr.file
                 imgfile.seek(0)
                 if self.mime_type == 'image/svg+xml':
                     self._width, self._height = VILImage.load(imgfile).size
+                    self._transparent = True
                 else:
-                    self._width, self._height = PILImage.open(imgfile).size
+                    pil_image = PILImage.open(imgfile)
+                    self._width, self._height = pil_image.size
+                    self._transparent = easy_thumbnails.utils.is_transparent(pil_image)
                 imgfile.seek(0)
             except Exception:
                 if post_init is False:
                     # in case `imgfile` could not be found, unset dimensions
                     # but only if not initialized by loading a fixture file
                     self._width, self._height = None, None
+                    self._transparent = False
         return attrs_updated
 
     def save(self, *args, **kwargs):
         self.has_all_mandatory_data = self._check_validity()
         super().save(*args, **kwargs)
 
     def _check_validity(self):
@@ -180,20 +190,22 @@
                     logger.error('Error while generating thumbnail: %s', e)
                 if filer_settings.FILER_DEBUG:
                     raise
         return _thumbnails
 
     @property
     def icons(self):
-        required_thumbnails = dict(
-            (size, {'size': (int(size), int(size)),
-                    'crop': True,
-                    'upscale': True,
-                    'subject_location': self.subject_location})
-            for size in filer_settings.FILER_ADMIN_ICON_SIZES)
+        required_thumbnails = {
+            size: {
+                'size': (int(size), int(size)),
+                'crop': True,
+                'upscale': True,
+                'subject_location': self.subject_location,
+            }
+            for size in filer_settings.FILER_ADMIN_ICON_SIZES}
         return self._generate_thumbnails(required_thumbnails)
 
     @property
     def thumbnails(self):
         return self._generate_thumbnails(BaseImage.DEFAULT_THUMBNAILS)
 
     @property
```

### Comparing `django-filer-2.3rc1/filer/models/clipboardmodels.py` & `django-filer-3.0.0rc1/filer/models/clipboardmodels.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             return False
         except filemodels.File.DoesNotExist:
             newitem = ClipboardItem(file=file_obj, clipboard=self)
             newitem.save()
             return True
 
     def __str__(self):
-        return "Clipboard %s of %s" % (self.id, self.user)
+        return "Clipboard {} of {}".format(self.id, self.user)
 
 
 class ClipboardItem(models.Model):
     file = models.ForeignKey(
         'File',
         verbose_name=_("file"),
         on_delete=models.CASCADE,
```

### Comparing `django-filer-2.3rc1/filer/models/filemodels.py` & `django-filer-3.0.0rc1/filer/models/filemodels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 import hashlib
 import mimetypes
 import os
-from datetime import datetime
+from datetime import datetime, timezone
 
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.core.files.base import ContentFile
 from django.db import models
 from django.urls import NoReverseMatch, reverse
-from django.utils import timezone
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 
 from polymorphic.managers import PolymorphicManager
 from polymorphic.models import PolymorphicModel
+from polymorphic.query import PolymorphicQuerySet
 
 from .. import settings as filer_settings
 from ..fields.multistorage_file import MultiStorageFileField
 from . import mixins
 from .foldermodels import Folder
 
 
+class FileQuerySet(PolymorphicQuerySet):
+    def only(self, *fields):
+        fields = set(fields)
+        fields.update(["_file_size", "sha1", "is_public"])
+        return super().only(*fields)
+
+
 class FileManager(PolymorphicManager):
+    queryset_class = FileQuerySet
+
     def find_all_duplicates(self):
         r = {}
         for file_obj in self.all():
             if file_obj.sha1:
                 q = self.filter(sha1=file_obj.sha1)
                 if len(q) > 1:
                     r[file_obj.sha1] = q
@@ -145,17 +154,17 @@
     class Meta:
         app_label = 'filer'
         verbose_name = _("file")
         verbose_name_plural = _("files")
 
     def __str__(self):
         if self.name in ('', None):
-            text = "%s" % (self.original_filename,)
+            text = "{}".format(self.original_filename)
         else:
-            text = "%s" % (self.name,)
+            text = "{}".format(self.name)
         return text
 
     @classmethod
     def matches_file_type(cls, iname, ifile, mime_type):
         return True  # I match all files...
 
     def __init__(self, *args, **kwargs):
@@ -289,28 +298,28 @@
 
     @property
     def label(self):
         if self.name in ['', None]:
             text = self.original_filename or 'unnamed file'
         else:
             text = self.name
-        text = "%s" % (text,)
+        text = "{}".format(text)
         return text
 
     def __lt__(self, other):
         return self.label.lower() < other.label.lower()
 
     def has_edit_permission(self, request):
-        return self.has_generic_permission(request, 'edit')
+        return request.user.has_perm("filer.change_file") and self.has_generic_permission(request, 'edit')
 
     def has_read_permission(self, request):
         return self.has_generic_permission(request, 'read')
 
     def has_add_children_permission(self, request):
-        return self.has_generic_permission(request, 'add_children')
+        return request.user.has_perm("filer.add_file") and self.has_generic_permission(request, 'add_children')
 
     def has_generic_permission(self, request, permission_type):
         """
         Return true if the current user has permission on this
         image. Return the string 'ALL' if the user has all rights.
         """
         user = request.user
@@ -323,24 +332,24 @@
         elif self.folder:
             return self.folder.has_generic_permission(request, permission_type)
         else:
             return False
 
     def get_admin_change_url(self):
         return reverse(
-            'admin:{0}_{1}_change'.format(
+            'admin:{}_{}_change'.format(
                 self._meta.app_label,
                 self._meta.model_name,
             ),
             args=(self.pk,)
         )
 
     def get_admin_delete_url(self):
         return reverse(
-            'admin:{0}_{1}_delete'.format(self._meta.app_label, self._meta.model_name),
+            f'admin:{self._meta.app_label}_{self._meta.model_name}_delete',
             args=(self.pk,))
 
     @property
     def url(self):
         """
         to make the model behave like a file field
         """
@@ -404,14 +413,14 @@
     def logical_path(self):
         """
         Gets logical path of the folder in the tree structure.
         Used to generate breadcrumbs
         """
         folder_path = []
         if self.folder:
-            folder_path.extend(self.folder.get_ancestors())
+            folder_path.extend(self.folder.logical_path)
         folder_path.append(self.logical_folder)
         return folder_path
 
     @property
     def duplicates(self):
         return File.objects.find_duplicates(self)
```

### Comparing `django-filer-2.3rc1/filer/models/foldermodels.py` & `django-filer-3.0.0rc1/filer/models/foldermodels.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-import warnings
-from urllib.parse import quote as urlquote
-
 from django.conf import settings
 from django.contrib.auth import models as auth_models
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.db.models import Q
 from django.urls import reverse
 from django.utils.functional import cached_property
 from django.utils.html import format_html, format_html_join
-from django.utils.translation import gettext_lazy as _
-
-import mptt
+from django.utils.translation import gettext as _
 
 from .. import settings as filer_settings
 from . import mixins
 
 
 class FolderPermissionManager(models.Manager):
     """
@@ -38,16 +33,16 @@
     def __get_id_list(self, user, attr):
         if user.is_superuser or not filer_settings.FILER_ENABLE_PERMISSIONS:
             return 'All'
         allow_list = set()
         deny_list = set()
         group_ids = user.groups.all().values_list('id', flat=True)
         q = Q(user=user) | Q(group__in=group_ids) | Q(everybody=True)
-        perms = self.filter(q).order_by('folder__tree_id', 'folder__level',
-                                        'folder__lft')
+        perms = self.filter(q)
+
         for perm in perms:
             p = getattr(perm, attr)
 
             if p is None:
                 # Not allow nor deny, we continue with the next permission
                 continue
 
@@ -66,17 +61,17 @@
             if p == FolderPermission.ALLOW:
                 allow_list.add(folder_id)
             else:
                 deny_list.add(folder_id)
 
             if perm.type in [FolderPermission.ALL, FolderPermission.CHILDREN]:
                 if p == FolderPermission.ALLOW:
-                    allow_list.update(perm.folder.get_descendants().values_list('id', flat=True))
+                    allow_list.update(perm.folder.get_descendants_ids())
                 else:
-                    deny_list.update(perm.folder.get_descendants().values_list('id', flat=True))
+                    deny_list.update(perm.folder.get_descendants_ids())
 
         # Deny has precedence over allow
         return allow_list - deny_list
 
 
 class Folder(models.Model, mixins.IconsMixin):
     """
@@ -89,24 +84,17 @@
     (Duck Type).
     """
     file_type = 'Folder'
     is_root = False
     can_have_subfolders = True
     _icon = 'plainfolder'
 
-    # explicitly define MPTT fields which would otherwise change
-    # and create a migration, depending on django-mptt version
-    # (see: https://github.com/django-mptt/django-mptt/pull/578)
-    level = models.PositiveIntegerField(editable=False)
-    lft = models.PositiveIntegerField(editable=False)
-    rght = models.PositiveIntegerField(editable=False)
-
     parent = models.ForeignKey(
         'self',
-        verbose_name=('parent'),
+        verbose_name=_('parent'),
         null=True,
         blank=True,
         related_name='children',
         on_delete=models.CASCADE,
     )
 
     name = models.CharField(
@@ -135,16 +123,14 @@
 
     modified_at = models.DateTimeField(
         _('modified at'),
         auto_now=True,
     )
 
     class Meta:
-        # see: https://github.com/django-mptt/django-mptt/pull/577
-        index_together = (('tree_id', 'lft'),)
         unique_together = (('parent', 'name'),)
         ordering = ('name',)
         permissions = (("can_use_directory_listing",
                         "Can use directory listing"),)
         app_label = 'filer'
         verbose_name = _("Folder")
         verbose_name_plural = _("Folders")
@@ -179,38 +165,37 @@
     def logical_path(self):
         """
         Gets logical path of the folder in the tree structure.
         Used to generate breadcrumbs
         """
         folder_path = []
         if self.parent:
-            folder_path.extend(self.parent.get_ancestors())
+            folder_path.extend(self.parent.logical_path)
             folder_path.append(self.parent)
         return folder_path
 
+    def get_descendants_ids(self):
+        desc = []
+        for child in self.children.all():
+            desc.append(child.id)
+            desc.extend(child.get_descendants_ids())
+        return desc
+
     @property
     def pretty_logical_path(self):
         return format_html('/{}', format_html_join('/', '{0}', ((f.name,) for f in self.logical_path + [self])))
 
-    @property
-    def quoted_logical_path(self):
-        warnings.warn(
-            'Method filer.foldermodels.Folder.quoted_logical_path is deprecated and will be removed',
-            DeprecationWarning, stacklevel=2,
-        )
-        return urlquote(self.pretty_logical_path)
-
     def has_edit_permission(self, request):
-        return self.has_generic_permission(request, 'edit')
+        return request.user.has_perm("filer.change_folder") and self.has_generic_permission(request, 'edit')
 
     def has_read_permission(self, request):
         return self.has_generic_permission(request, 'read')
 
     def has_add_children_permission(self, request):
-        return self.has_generic_permission(request, 'add_children')
+        return request.user.has_perm("filer.change_folder") and self.has_generic_permission(request, 'add_children')
 
     def has_generic_permission(self, request, permission_type):
         """
         Return true if the current user has permission on this
         folder. Return the string 'ALL' if the user has all rights.
         """
         user = request.user
@@ -258,21 +243,14 @@
         try:
             self.children.get(name=folder_name)
             return True
         except Folder.DoesNotExist:
             return False
 
 
-# MPTT registration
-try:
-    mptt.register(Folder)
-except mptt.AlreadyRegistered:
-    pass
-
-
 class FolderPermission(models.Model):
     ALL = 0
     THIS = 1
     CHILDREN = 2
 
     ALLOW = 1
     DENY = 0
```

### Comparing `django-filer-2.3rc1/filer/models/imagemodels.py` & `django-filer-3.0.0rc1/filer/models/imagemodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/models/mixins.py` & `django-filer-3.0.0rc1/filer/models/mixins.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def icons(self):
         warnings.warn("Method 'icons' is deprecated and will be re moved in future versions",
                       DeprecationWarning)
         r = {}
         if getattr(self, '_icon', False):
             for size in FILER_ADMIN_ICON_SIZES:
                 try:
-                    r[size] = static("filer/icons/%s_%sx%s.png" % (
+                    r[size] = static("filer/icons/{}_{}x{}.png".format(
                         self._icon, size, size))
                 except ValueError:
                     # Do not raise an exception while trying to call static()
                     # on non-existent icon file. This avoids the issue with
                     # rendering parts of the template as empty blocks that
                     # happens on an attempt to access object 'icons' attribute
                     # in template.
```

### Comparing `django-filer-2.3rc1/filer/models/thumbnailoptionmodels.py` & `django-filer-3.0.0rc1/filer/models/thumbnailoptionmodels.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     class Meta:
         app_label = 'filer'
         ordering = ('width', 'height')
         verbose_name = _("thumbnail option")
         verbose_name_plural = _("thumbnail options")
 
     def __str__(self):
-        return '%s -- %s x %s' % (self.name, self.width, self.height)
+        return '{} -- {} x {}'.format(self.name, self.width, self.height)
 
     @property
     def as_dict(self):
         """
         This property returns a dictionary suitable for Thumbnailer.get_thumbnail()
 
         Sample code:
```

### Comparing `django-filer-2.3rc1/filer/models/tools.py` & `django-filer-3.0.0rc1/filer/models/tools.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/models/virtualitems.py` & `django-filer-3.0.0rc1/filer/models/virtualitems.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,16 +44,28 @@
 
 class UnsortedImages(DummyFolder):
     name = _("Unsorted Uploads")
     is_root = True
     is_unsorted_uploads = True
     _icon = "unfiled_folder"
 
+    def __init__(self, user=None):
+        super().__init__()
+        self.user = user
+
     def _files(self):
-        return File.objects.filter(folder__isnull=True)
+        """
+        If the current user is not a superuser, we don't them to see/edit/change
+        file in the unsorted uploads folder that they don't own.
+        """
+        if self.user.is_superuser or not filer_settings.FILER_ENABLE_PERMISSIONS:
+            return File.objects.filter(folder__isnull=True)
+        else:
+            return File.objects.filter(folder__isnull=True, owner=self.user)
+
     files = property(_files)
 
     def get_admin_directory_listing_url_path(self):
         return reverse(
             'admin:filer-directory_listing-unfiled_images')
```

### Comparing `django-filer-2.3rc1/filer/server/backends/base.py` & `django-filer-3.0.0rc1/filer/server/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/server/backends/default.py` & `django-filer-3.0.0rc1/filer/server/backends/default.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/server/backends/nginx.py` & `django-filer-3.0.0rc1/filer/server/backends/nginx.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/server/backends/xsendfile.py` & `django-filer-3.0.0rc1/filer/server/backends/xsendfile.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/server/views.py` & `django-filer-3.0.0rc1/filer/server/views.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/settings.py` & `django-filer-3.0.0rc1/filer/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                              and ('' in settings.LOGGING['loggers']
                              or 'filer' in settings.LOGGING['loggers'])))
 
 FILER_ENABLE_PERMISSIONS = getattr(settings, 'FILER_ENABLE_PERMISSIONS', False)
 FILER_ALLOW_REGULAR_USERS_TO_ADD_ROOT_FOLDERS = getattr(settings, 'FILER_ALLOW_REGULAR_USERS_TO_ADD_ROOT_FOLDERS', False)
 FILER_IS_PUBLIC_DEFAULT = getattr(settings, 'FILER_IS_PUBLIC_DEFAULT', True)
 
-FILER_PAGINATE_BY = getattr(settings, 'FILER_PAGINATE_BY', 20)
+FILER_PAGINATE_BY = getattr(settings, 'FILER_PAGINATE_BY', 100)
 
 _ICON_SIZES = getattr(settings, 'FILER_ADMIN_ICON_SIZES', ('16', '32', '48', '64'))
 if not _ICON_SIZES:
     raise ImproperlyConfigured('Please, configure FILER_ADMIN_ICON_SIZES')
 # Reliably sort by integer value, but keep icon size as string.
 # (There is some code in the wild that depends on this being strings.)
 FILER_ADMIN_ICON_SIZES = [str(i) for i in sorted([int(s) for s in _ICON_SIZES])]
@@ -243,14 +243,19 @@
 # By default limit number of simultaneous uploads if we are using SQLite
 if settings.DATABASES['default']['ENGINE'].endswith('sqlite3'):
     _uploader_connections = 1
 else:
     _uploader_connections = 3
 FILER_UPLOADER_CONNECTIONS = getattr(
     settings, 'FILER_UPLOADER_CONNECTIONS', _uploader_connections)
+FILER_UPLOADER_MAX_FILES = getattr(
+    settings, 'FILER_UPLOADER_MAX_FILES', 100)
+FILER_UPLOADER_MAX_FILE_SIZE = getattr(
+    settings, 'FILER_UPLOADER_MAX_FILE_SIZE', None)
+
 
 FILER_DUMP_PAYLOAD = getattr(settings, 'FILER_DUMP_PAYLOAD', False)  # Whether the filer shall dump the files payload
 
 FILER_CANONICAL_URL = getattr(settings, 'FILER_CANONICAL_URL', 'canonical/')
 
 TABLE_LIST_TYPE = 'tb'
 THUMBNAIL_LIST_TYPE = 'th'
@@ -270,7 +275,45 @@
     },
     THUMBNAIL_LIST_TYPE: {
         'icon': 'th-large',
         'tooltip_text': _('Show thumbnail view'),
         'template': 'admin/filer/folder/directory_thumbnail_list.html',
     },
 }
+
+DEFERRED_THUMBNAIL_SIZES = (40, 80, 160)
+
+FILE_VALIDATORS = {
+    "text/html": ["filer.validation.deny_html"],
+    "image/svg+xml": ["filer.validation.validate_svg"],
+}
+
+remove_mime_types = getattr(settings, "FILER_REMOVE_FILE_VALIDATORS", [])
+for mime_type in remove_mime_types:  # pragma: no cover
+    if mime_type in FILE_VALIDATORS:
+        del FILE_VALIDATORS[mime_type]
+
+for mime_type, validators in getattr(settings, "FILER_ADD_FILE_VALIDATORS", {}).items():  # pragma: no cover
+    if mime_type in FILE_VALIDATORS:
+        FILE_VALIDATORS[mime_type] += list(validators)
+    else:
+        FILE_VALIDATORS[mime_type] = list(validators)
+
+FILER_MIME_TYPE_WHITELIST = getattr(settings, "FILER_MIME_TYPE_WHITELIST", [])
+
+
+# Determine if django CMS is installed and if it comes with its own iconset
+
+ICON_CSS_LIB = ("filer/css/admin_filer.fa.icons.css",)
+if "cms" in settings.INSTALLED_APPS:  # pragma: no cover
+    try:
+        from cms import __version__
+        from cms.utils.urlutils import static_with_version
+
+        if __version__ >= "4":
+            ICON_CSS_LIB = (
+                static_with_version("cms/css/cms.admin.css"),
+                "filer/css/admin_filer.cms.icons.css",
+            )
+    except (ModuleNotFoundError, ImportError):
+        # Import error? No django CMS used: stay with own icons
+        pass
```

### Comparing `django-filer-2.3rc1/filer/static/filer/fonts/FontAwesome.otf` & `django-filer-3.0.0rc1/filer/static/filer/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/fonts/fontawesome-webfont.eot` & `django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/fonts/fontawesome-webfont.svg` & `django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/fonts/fontawesome-webfont.ttf` & `django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/fonts/fontawesome-webfont.woff` & `django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/fonts/fontawesome-webfont.woff2` & `django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/icons/cloud-up.svg` & `django-filer-3.0.0rc1/filer/static/filer/icons/cloud-up.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/icons/file-audio.svg` & `django-filer-3.0.0rc1/filer/static/filer/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/icons/file-empty.svg` & `django-filer-3.0.0rc1/filer/static/filer/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/icons/file-font.svg` & `django-filer-3.0.0rc1/filer/static/filer/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/icons/file-missing.svg` & `django-filer-3.0.0rc1/filer/static/filer/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/icons/file-pdf.svg` & `django-filer-3.0.0rc1/filer/static/filer/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/icons/file-picture.svg` & `django-filer-3.0.0rc1/filer/static/filer/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/icons/file-unknown.svg` & `django-filer-3.0.0rc1/filer/static/filer/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/icons/file-video.svg` & `django-filer-3.0.0rc1/filer/static/filer/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/icons/file-zip.svg` & `django-filer-3.0.0rc1/filer/static/filer/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/icons/folder-dropdown.svg` & `django-filer-3.0.0rc1/filer/static/filer/icons/folder-dropdown.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/icons/folder-root.svg` & `django-filer-3.0.0rc1/filer/static/filer/icons/folder-root.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/icons/folder-unfiled.svg` & `django-filer-3.0.0rc1/filer/static/filer/icons/folder-unfiled.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/icons/folder.svg` & `django-filer-3.0.0rc1/filer/static/filer/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/img/icon_changelink.gif` & `django-filer-3.0.0rc1/filer/static/filer/img/icon_changelink.gif`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/img/icon_deletelink.gif` & `django-filer-3.0.0rc1/filer/static/filer/img/icon_deletelink.gif`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/img/loading_animation.gif` & `django-filer-3.0.0rc1/filer/static/filer/img/loading_animation.gif`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/img/upload_button.png` & `django-filer-3.0.0rc1/filer/static/filer/img/upload_button.png`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/js/addons/copy-move-files.js` & `django-filer-3.0.0rc1/filer/static/filer/js/addons/copy-move-files.js`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/js/addons/dropdown-menu.js` & `django-filer-3.0.0rc1/filer/static/filer/js/addons/dropdown-menu.js`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/js/addons/dropzone.init.js` & `django-filer-3.0.0rc1/filer/static/filer/js/addons/dropzone.init.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -18,14 +18,15 @@
 djQuery(function($) {
     var dropzoneTemplateSelector = '.js-filer-dropzone-template';
     var previewImageSelector = '.js-img-preview';
     var dropzoneSelector = '.js-filer-dropzone';
     var dropzones = $(dropzoneSelector);
     var messageSelector = '.js-filer-dropzone-message';
     var lookupButtonSelector = '.js-related-lookup';
+    var editButtonSelector = '.js-related-edit';
     var progressSelector = '.js-filer-dropzone-progress';
     var previewImageWrapperSelector = '.js-img-wrapper';
     var filerClearerSelector = '.filerClearer';
     var fileChooseSelector = '.js-file-selector';
     var fileIdInputSelector = '.vForeignKeyRawIdAdminField';
     var dragHoverClass = 'dz-drag-hover';
     var hiddenClass = 'hidden';
@@ -52,14 +53,15 @@
 
     var createDropzone = function() {
         var dropzone = $(this);
         var dropzoneUrl = dropzone.data('url');
         var inputId = dropzone.find(fileIdInputSelector);
         var isImage = inputId.is('[name="image"]');
         var lookupButton = dropzone.find(lookupButtonSelector);
+        var editButton = dropzone.find(editButtonSelector);
         var message = dropzone.find(messageSelector);
         var clearButton = dropzone.find(filerClearerSelector);
         var fileChoose = dropzone.find(fileChooseSelector);
 
         if (this.dropzone) {
             return;
         }
@@ -68,16 +70,15 @@
             checkMinWidth(dropzone);
         });
 
         new Dropzone(this, {
             url: dropzoneUrl,
             paramName: 'file',
             maxFiles: 1,
-            // for now disabled as we don't have the correct file size limit
-            // maxFilesize: dropzone.data(dataMaxFileSize) || 20, // MB
+            maxFilesize: this.dataset.maxFilesize,
             previewTemplate: $(dropzoneTemplateSelector).html(),
             clickable: false,
             addRemoveLinks: false,
             init: function() {
                 checkMinWidth(dropzone);
                 this.on('removedfile', function() {
                     fileChoose.show();
@@ -96,14 +97,15 @@
             maxfilesexceeded: function() {
                 this.removeAllFiles(true);
             },
             drop: function() {
                 this.removeAllFiles(true);
                 fileChoose.hide();
                 lookupButton.addClass('related-lookup-change');
+                editButton.addClass('related-lookup-change');
                 message.addClass(hiddenClass);
                 dropzone.removeClass(dragHoverClass);
                 dropzone.addClass(objectAttachedClass);
             },
             success: function(file, response) {
                 $(progressSelector).addClass(hiddenClass);
                 if (file && file.status === 'success' && response) {
@@ -143,14 +145,15 @@
                     $(previewImageSelector).css({
                         'background-image': 'none'
                     });
                 }
                 dropzone.removeClass(objectAttachedClass);
                 inputId.val('');
                 lookupButton.removeClass('related-lookup-change');
+                editButton.removeClass('related-lookup-change');
                 message.removeClass(hiddenClass);
                 inputId.trigger('change');
             }
         });
     };
 
     if (dropzones.length && Dropzone) {
```

### Comparing `django-filer-2.3rc1/filer/static/filer/js/addons/focal-point.js` & `django-filer-3.0.0rc1/filer/static/filer/js/addons/focal-point.js`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/js/addons/popup_handling.js` & `django-filer-3.0.0rc1/filer/static/filer/js/addons/popup_handling.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -15,32 +15,45 @@
         return text.split('__')[0];
     }
 
     window.dismissPopupAndReload = function(win) {
         document.location.reload();
         win.close();
     };
-    window.dismissRelatedImageLookupPopup = function(win, chosenId, chosenThumbnailUrl, chosenDescriptionTxt) {
+    window.dismissRelatedImageLookupPopup = function(
+        win,
+        chosenId,
+        chosenThumbnailUrl,
+        chosenDescriptionTxt,
+        chosenAdminChangeUrl
+    ) {
         var id = windowname_to_id(win.name);
         var lookup = $('#' + id);
         var container = lookup.closest('.filerFile');
+        var edit = container.find('.edit');
         var image = container.find('.thumbnail_img');
         var descriptionText = container.find('.description_text');
         var clearer = container.find('.filerClearer');
         var dropzoneMessage = container.siblings('.dz-message');
         var element = container.find(':input');
         var oldId = element.value;
 
         element.val(chosenId);
         element.closest('.js-filer-dropzone').addClass('js-object-attached');
-        image.attr('src', chosenThumbnailUrl).removeClass('hidden');
-        image.removeAttr('srcset'); // would be nicer, but much more complicate to also replace 'srcset'
+        if (chosenThumbnailUrl) {
+            image.attr('src', chosenThumbnailUrl).removeClass('hidden');
+            image.removeAttr('srcset'); // would be nicer, but much more complicate to also replace 'srcset'
+        }
         descriptionText.text(chosenDescriptionTxt);
         clearer.removeClass('hidden');
         lookup.addClass('related-lookup-change');
+        edit.addClass('related-lookup-change');
+        if (chosenAdminChangeUrl) {
+            edit.attr('href', chosenAdminChangeUrl + '?_edit_from_widget=1');
+        }
         dropzoneMessage.addClass('hidden');
 
         if (oldId !== chosenId) {
             element.trigger('change');
         }
         win.close();
     };
```

### Comparing `django-filer-2.3rc1/filer/static/filer/js/addons/table-dropzone.js` & `django-filer-3.0.0rc1/filer/static/filer/js/addons/table-dropzone.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -61,32 +61,36 @@
             ));
         };
 
         if (dropzoneBase && dropzoneBase.length) {
             baseUrl = dropzoneBase.data('url');
             baseFolderTitle = dropzoneBase.data('folder-name');
 
-            $('body').data('url', baseUrl).data('folder-name', baseFolderTitle).addClass('js-filer-dropzone');
+            $('body')
+                .data('url', baseUrl)
+                .data('folder-name', baseFolderTitle)
+                .data('max-files', dropzoneBase.data('max-files'))
+                .data('max-filesize', dropzoneBase.data('max-files'))
+                .addClass('js-filer-dropzone');
         }
 
         Cl.mediator.subscribe('filer-upload-in-progress', destroyDropzones);
 
         dropzones = $(dropzoneSelector);
 
         if (dropzones.length && Dropzone) {
             Dropzone.autoDiscover = false;
             dropzones.each(function() {
                 var dropzone = $(this);
                 var dropzoneUrl = $(this).data('url');
                 var dropzoneInstance = new Dropzone(this, {
                     url: dropzoneUrl,
                     paramName: 'file',
-                    maxFiles: 100,
-                    // for now disabled as we don't have the correct file size limit
-                    // maxFilesize: dropzone.data(dataMaxFileSize) || 20, // MB
+                    maxFiles: parseInt(dropzone.data('max-files')) || 100,
+                    maxFilesize: parseInt(dropzone.data('max-filesize')), // no default
                     previewTemplate: '<div></div>',
                     clickable: false,
                     addRemoveLinks: false,
                     parallelUploads: dropzone.data(dataUploaderConnections) || 3,
                     accept: function(file, done) {
                         var uploadInfoClone;
```

### Comparing `django-filer-2.3rc1/filer/static/filer/js/addons/toggler.js` & `django-filer-3.0.0rc1/filer/static/filer/js/addons/toggler.js`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/js/addons/tooltip.js` & `django-filer-3.0.0rc1/filer/static/filer/js/addons/tooltip.js`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/js/addons/upload-button.js` & `django-filer-3.0.0rc1/filer/static/filer/js/addons/upload-button.js`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/js/base.js` & `django-filer-3.0.0rc1/filer/static/filer/js/base.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -79,28 +79,34 @@
                     $(containerSelector).removeClass('search-is-focused');
                 });
             }
         }());
 
         // show counter if file is selected
         (function() {
-            var navigatorTable = $('.navigator-table, .navigator-list').find('tr, .list-item');
+            var navigatorTable = $('.navigator-table tr, .navigator-list .list-item');
             var actionList = $('.actions-wrapper');
             var actionSelect = $(
                 '.action-select, #action-toggle, #files-action-toggle, #folders-action-toggle, .actions .clear a'
             );
 
             // timeout is needed to wait until table row has class selected.
             setTimeout(function() {
                 if (navigatorTable.hasClass('selected')) {
                     actionList.addClass('action-selected');
                 }
             }, 100);
 
             actionSelect.on('change', function() {
+                // Mark element selected (for table view this is done by Django admin js - we do it ourselves
+                if ($(this).prop('checked')) {
+                    $(this).closest('.list-item').addClass('selected');
+                } else {
+                    $(this).closest('.list-item').removeClass('selected');
+                }
                 // setTimeout makes sure that change event fires before click event which is reliable to admin
                 setTimeout(function() {
                     if (navigatorTable.hasClass('selected')) {
                         actionList.addClass('action-selected');
                     } else {
                         actionList.removeClass('action-selected');
                     }
@@ -118,15 +124,15 @@
             var html = '';
             var actionDelete = $('.js-action-delete');
             var actionCopy = $('.js-action-copy');
             var actionMove = $('.js-action-move');
             var valueDelete = 'delete_files_or_folders';
             var valueCopy = 'copy_files_and_folders';
             var valueMove = 'move_files_and_folders';
-            var navigatorTable = $('.navigator-table, .navigator-list').find('tr, .list-item');
+            var navigatorTable = $('.navigator-table tr, .navigator-list .list-item');
 
             // triggers delete copy and move actions on separate buttons
             function actionsButton(optionValue, actionButton) {
                 actionsSelectOptions.each(function() {
                     if (this.value === optionValue) {
                         actionButton.show();
                         actionButton.on('click', function(e) {
@@ -206,59 +212,51 @@
                 headerWidth = header.outerWidth();
                 breadcrumbSizeHandler();
             });
 
         }());
         // thumbnail folder admin view
         (function() {
-            $(document).ready(function() {
-                var $actionEls = $('.navigator-list .list-item input.action-select'),
-                    foldersActionCheckboxes = '.navigator-list .navigator-folders-body .list-item input.action-select',
-                    filesActionCheckboxes = '.navigator-list .navigator-files-body .list-item input.action-select',
-                    $allFilesToggle = $('#files-action-toggle'),
-                    $allFoldersToggle = $('#folders-action-toggle');
-
-                if ($actionEls.length > 0) {
-                    $actionEls.actions({
-                        allToggle: '#all-items-action-toggle'
-                    });
-                }
-
-                $allFoldersToggle.on('click', function() {
-                    if (!!$(this).prop('checked')) {
-                        $(foldersActionCheckboxes).filter(':not(:checked)').trigger('click');
-                    } else {
-                        $(foldersActionCheckboxes).filter(':checked').trigger('click');
+            var $actionEls = $('.navigator-list .list-item input.action-select'),
+                foldersActionCheckboxes = '.navigator-list .navigator-folders-body .list-item input.action-select',
+                filesActionCheckboxes = '.navigator-list .navigator-files-body .list-item input.action-select',
+                $allFilesToggle = $('#files-action-toggle'),
+                $allFoldersToggle = $('#folders-action-toggle');
+
+            $allFoldersToggle.on('click', function() {
+                if (!!$(this).prop('checked')) {
+                    $(foldersActionCheckboxes).filter(':not(:checked)').trigger('click');
+                } else {
+                    $(foldersActionCheckboxes).filter(':checked').trigger('click');
+                }
+            });
+            $allFilesToggle.on('click', function() {
+                if (!!$(this).prop('checked')) {
+                    $(filesActionCheckboxes).filter(':not(:checked)').trigger('click');
+                } else {
+                    $(filesActionCheckboxes).filter(':checked').trigger('click');
+                }
+            });
+            $actionEls.on('click', function() {
+                if (!$(this).prop('checked')) {
+                    if (!!$(filesActionCheckboxes).filter(':not(:checked)').length) {
+                        $allFilesToggle.prop('checked', false);
                     }
-                });
-                $allFilesToggle.on('click', function() {
-                    if (!!$(this).prop('checked')) {
-                        $(filesActionCheckboxes).filter(':not(:checked)').trigger('click');
-                    } else {
-                        $(filesActionCheckboxes).filter(':checked').trigger('click');
+                    if (!!$(foldersActionCheckboxes).filter(':not(:checked)').length) {
+                        $allFoldersToggle.prop('checked', false);
                     }
-                });
-                $actionEls.on('click', function() {
-                    if (!$(this).prop('checked')) {
-                        if (!!$(filesActionCheckboxes).filter(':not(:checked)').length) {
-                            $allFilesToggle.prop('checked', false);
-                        }
-                        if (!!$(foldersActionCheckboxes).filter(':not(:checked)').length) {
-                            $allFoldersToggle.prop('checked', false);
-                        }
-                    } else {
-                        if (!$(filesActionCheckboxes).filter(':not(:checked)').length) {
-                            $allFilesToggle.prop('checked', true);
-                        }
-                        if (!$(foldersActionCheckboxes).filter(':not(:checked)').length) {
-                            $allFoldersToggle.prop('checked', true);
-                        }
+                } else {
+                    if (!$(filesActionCheckboxes).filter(':not(:checked)').length) {
+                        $allFilesToggle.prop('checked', true);
                     }
-                });
-                $('.navigator .actions .clear a').on('click', function() {
-                    $allFoldersToggle.prop('checked', false);
-                    $allFilesToggle.prop('checked', false);
-                });
+                    if (!$(foldersActionCheckboxes).filter(':not(:checked)').length) {
+                        $allFoldersToggle.prop('checked', true);
+                    }
+                }
+            });
+            $('.navigator .actions .clear a').on('click', function() {
+                $allFoldersToggle.prop('checked', false);
+                $allFilesToggle.prop('checked', false);
             });
         })();
     });
 })(djQuery);
```

### Comparing `django-filer-2.3rc1/filer/static/filer/js/libs/class.min.js` & `django-filer-3.0.0rc1/filer/static/filer/js/libs/class.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/js/libs/dropzone.min.js` & `django-filer-3.0.0rc1/filer/static/filer/js/libs/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/js/libs/fileuploader.min.js` & `django-filer-3.0.0rc1/filer/static/filer/js/libs/fileuploader.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/js/libs/jquery.cookie.min.js` & `django-filer-3.0.0rc1/filer/static/filer/js/libs/jquery.cookie.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/js/libs/jquery.min.js` & `django-filer-3.0.0rc1/filer/static/filer/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/static/filer/js/libs/mediator.min.js` & `django-filer-3.0.0rc1/filer/static/filer/js/libs/mediator.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/storage.py` & `django-filer-3.0.0rc1/filer/storage.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/actions.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/actions.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 {% load i18n %}
 
 <div class="actions hidden">
     {% for field in action_form %}{% if field.label %}<label>{{ field.label }} {% endif %}{{ field }}{% if field.label %}</label>{% endif %}{% endfor %}
-    <button type="submit" class="button" title="{% trans 'Run the selected action' %}" name="index" value="{{ action_index|default:0 }}">{% trans "Go" %}</button>
+    <button type="submit" class="button" title="{% translate 'Run the selected action' %}" name="index" value="{{ action_index|default:0 }}">{% translate "Go" %}</button>
     {% if actions_selection_counter %}
         <script type="text/javascript">
             var _actions_icnt="{{ paginated_items.object_list|length|default:'0' }}";
         </script>
         <span class="action-counter" data-actions-icnt="{{ paginated_items.object_list|length|default:'0' }}">{{ selection_note }}</span>
         {% if paginator.count != paginated_items.object_list|length %}
             <span class="all">{{ selection_note_all }}</span>
             <span class="question">
-                <a href="javascript:;" title="{% trans 'Click here to select the objects across all pages' %}">{% blocktrans with paginator.count as total_count %}Select all {{ total_count }} files and/or folders{% endblocktrans %}</a>
+                <a href="javascript:;" title="{% translate 'Click here to select the objects across all pages' %}">{% blocktrans with paginator.count as total_count %}Select all {{ total_count }} files and/or folders{% endblocktrans %}</a>
             </span>
-            <span class="clear"><a href="javascript:;">{% trans "Clear selection" %}</a></span>
+            <span class="clear"><a href="javascript:;">{% translate "Clear selection" %}</a></span>
         {% endif %}
     {% endif %}
 </div>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% load i18n %}
 {% for field in action_form %}{% if field.label %}{{ field.label }} {% endif %}
-{{ field }}{% if field.label %}{% endif %}{% endfor %} {% trans "Go" %} {% if
-actions_selection_counter %}
+{{ field }}{% if field.label %}{% endif %}{% endfor %} {% translate "Go" %} {%
+if actions_selection_counter %}
  {{ selection_note }} {% if paginator.count !=
 paginated_items.object_list|length %} {{ selection_note_all }}  {%_blocktrans
 with_paginator.count_as_total_count_%}Select_all_{{_total_count_}}_files_and/or
-folders{%_endblocktrans_%}  {%_trans_"Clear_selection"_%} {% endif %} {% endif
-%}
+folders{%_endblocktrans_%}  {%_translate_"Clear_selection"_%} {% endif %} {%
+endif %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/base_site.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/base_site.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends "admin/base_site.html" %}
-{% load i18n static %}
+{% load i18n static filer_admin_tags %}
 
 {% block extrastyle %}
     {{ block.super }}
-
     <link rel="stylesheet" type="text/css" href="{% static 'filer/css/admin_filer.css' %}">
+    {% icon_css_library %}
 {% endblock %}
 
 {% block extrahead %}
     {{ block.super }}
 
     {# upload stuff #}
     {{ media.js }}
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
-{% extends "admin/base_site.html" %} {% load i18n static %} {% block extrastyle
-%} {{ block.super }}
- {% endblock %} {% block extrahead %} {{ block.super }} {# upload stuff #} {
-{ media.js }}
+{% extends "admin/base_site.html" %} {% load i18n static filer_admin_tags %} {%
+block extrastyle %} {{ block.super }}
+ {% icon_css_library %} {% endblock %} {% block extrahead %} {{ block.super }}
+{# upload stuff #} {{ media.js }}
  {% endblock %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/breadcrumbs.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/breadcrumbs.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-{% load i18n %}
+{% load i18n filer_admin_tags %}
 
 <div class="breadcrumbs">
-    <a href="{% url 'admin:index' %}" title="{% trans 'Go back to admin homepage' %}">{% trans "Home" %}</a>
-    &rsaquo; <a href="{% url 'admin:app_list' app_label='filer' %}" title="{% trans 'Go back to Filer app' %}"> {% trans "Filer" %}</a>
+    <a href="{% url 'admin:index' %}" title="{% translate 'Go back to admin homepage' %}">{% translate "Home" %}</a>
+    &rsaquo; <a href="{% url 'admin:app_list' app_label='filer' %}" title="{% translate 'Go back to Filer app' %}"> {% translate "Filer" %}</a>
     {% if not instance.is_root and instance.is_smart_folder %}
-        &rsaquo; <a href="{% url 'admin:filer-directory_listing-root' %}" title="{% trans 'Go back to root folder' %}">{% trans "root" %}</a>
+        &rsaquo; <a href="{% url 'admin:filer-directory_listing-root' %}{% filer_admin_context_url_params %}" title="{% translate 'Go back to root folder' %}">{% translate "root" %}</a>
     {% endif %}
     {% for ancestor_folder in instance.logical_path %}
-        &rsaquo; <a href="{{ ancestor_folder.get_admin_directory_listing_url_path }}" title="{% blocktrans with ancestor_folder.name as folder_name %}Go back to '{{ folder_name }}' folder{% endblocktrans %}">
+        &rsaquo; <a href="{{ ancestor_folder.get_admin_directory_listing_url_path }}{% filer_admin_context_url_params %}" title="{% blocktrans with ancestor_folder.name as folder_name %}Go back to '{{ folder_name }}' folder{% endblocktrans %}">
             {% if ancestor_folder.label %}
                 {{ ancestor_folder.label }}
             {% else %}
                 {{ ancestor_folder.name }}
             {% endif %}
         </a>
     {% endfor %}
     {% if breadcrumbs_action %}
         {% if instance.label or instance.name %}
-            &rsaquo; <a href="{{ instance.get_admin_directory_listing_url_path }}" title="{% blocktrans with instance.name as folder_name %}Go back to '{{ folder_name }}' folder{% endblocktrans %}">{% if instance.label %}{{ instance.label }}{% else %}{{ instance.name }}{% endif %}</a>
+            &rsaquo; <a href="{{ instance.get_admin_directory_listing_url_path }}{% filer_admin_context_url_params %}" title="{% blocktrans with instance.name as folder_name %}Go back to '{{ folder_name }}' folder{% endblocktrans %}">{% if instance.label %}{{ instance.label }}{% else %}{{ instance.name }}{% endif %}</a>
         {% endif %}
         &rsaquo; {{ breadcrumbs_action }}
     {% else %}
         &rsaquo; {% if instance.label %}{{ instance.label }}{% else %}{{ instance.name }}{% endif %}
     {% endif %}
 </div>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{% load i18n %}
-{%_trans_"Home"_%} › {%_trans_"Filer"_%} {% if not instance.is_root and
-instance.is_smart_folder %} › {%_trans_"root"_%} {% endif %} {% for
+{% load i18n filer_admin_tags %}
+{%_translate_"Home"_%} › {%_translate_"Filer"_%} {% if not instance.is_root and
+instance.is_smart_folder %} › {%_translate_"root"_%} {% endif %} {% for
 ancestor_folder in instance.logical_path %} › {%_if_ancestor_folder.label_%}_{
 {_ancestor_folder.label_}}_{%_else_%}_{{_ancestor_folder.name_}}_{%_endif_%} {%
 endfor %} {% if breadcrumbs_action %} {% if instance.label or instance.name %}
 › {%_if_instance.label_%}{{_instance.label_}}{%_else_%}{{_instance.name_}}{%
 endif_%} {% endif %} › {{ breadcrumbs_action }} {% else %} › {% if
 instance.label %}{{ instance.label }}{% else %}{{ instance.name }}{% endif %}
 {% endif %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/change_form.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/change_form.html`

 * *Files 21% similar despite different names*

```diff
@@ -6,27 +6,28 @@
         {% include "admin/filer/breadcrumbs.html" %}
     {% endwith %}
 {% endblock %}
 
 {% block extrastyle %}
     {{ block.super }}
     <link rel="stylesheet" type="text/css" href="{% static 'filer/css/admin_filer.css' %}">
+    {% icon_css_library %}
 {% endblock %}
 
 
 {% block after_field_sets %}
     {% filer_admin_context_hidden_formfields %}
 {% endblock %}
 
 {% block sidebar %}
     {% block file_sidebar %}
         {% with original.duplicates as duplicates %}
             {% if duplicates %}
                 <div class="file-duplicates">
-                    <h3>{% trans "Duplicates" %}</h3>
+                    <h3>{% translate "Duplicates" %}</h3>
                     <ul>
                         {% for duplicate in duplicates %}
                             <li><a href="{{ duplicate.get_admin_change_url }}">{{ duplicate }}</a></li>
                         {% endfor %}
                     </ul>
                 </div>
             {% endif %}
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% extends "admin/change_form.html" %} {% load i18n admin_modify static
 filer_admin_tags %} {% block breadcrumbs %} {% with original as instance %} {%
 include "admin/filer/breadcrumbs.html" %} {% endwith %} {% endblock %} {% block
 extrastyle %} {{ block.super }}
- {% endblock %} {% block after_field_sets %} {%
+ {% icon_css_library %} {% endblock %} {% block after_field_sets %} {%
 filer_admin_context_hidden_formfields %} {% endblock %} {% block sidebar %} {%
 block file_sidebar %} {% with original.duplicates as duplicates %} {% if
 duplicates %}
-**** {% trans "Duplicates" %} ****
+**** {% translate "Duplicates" %} ****
     * {% for duplicate in duplicates %}
     * {{_duplicate_}}
     * {% endfor %}
 {% endif %} {% endwith %} {% endblock %} {% endblock %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/delete_selected_files_confirmation.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/delete_selected_files_confirmation.html`

 * *Files 9% similar despite different names*

```diff
@@ -28,24 +28,24 @@
         {% for deletable_object in deletable_objects %}
             <ul>{{ deletable_object|unordered_list }}</ul>
         {% endfor %}
         <form action="" method="post">
             {% csrf_token %}
             <div>
                 {% for f in files_queryset %}
-                    <input type="hidden" name="{{ action_checkbox_name }}" value="file-{{ f.pk }}">
+                    <input type="hidden" name="{{ action_checkbox_name }}" value="file-{{ f.pk|safe }}">
                 {% endfor %}
                 {% for f in folders_queryset %}
-                    <input type="hidden" name="{{ action_checkbox_name }}" value="folder-{{ f.pk }}">
+                    <input type="hidden" name="{{ action_checkbox_name }}" value="folder-{{ f.pk|safe }}">
                 {% endfor %}
                 {% if is_popup %}
                     <input type="hidden" name="_popup" value="1">
                     {% if select_folder %}<input type="hidden" name="select_folder" value="1">{% endif %}
                 {% endif %}
                 <input type="hidden" name="action" value="delete_files_or_folders">
                 <input type="hidden" name="post" value="yes">
-                <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% trans "No, take me back" %}</a>
-                <input type="submit" value="{% trans 'Yes, I&#39;m sure' %}">
+                <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% translate "No, take me back" %}</a>
+                <input type="submit" value="{% translate 'Yes, I&#39;m sure' %}">
             </div>
         </form>
     {% endif %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -19,9 +19,9 @@
 {% endblocktrans %}
 {% for deletable_object in deletable_objects %}
     * {{ deletable_object|unordered_list }}
 {% endfor %}
 {% csrf_token %}
 {% for f in files_queryset %}  {% endfor %} {% for f in folders_queryset %}  {%
 endfor %} {% if is_popup %}  {% if select_folder %}{% endif %} {% endif %}   {%
-trans_"No,_take_me_back"_%} [{% trans 'Yes, I&#39;m sure' %}]
+translate_"No,_take_me_back"_%} [{% translate 'Yes, I&#39;m sure' %}]
 {% endif %} {% endblock %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/file/change_form.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/file/change_form.html`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     </script>
 {% endblock %}
 
 
 {% block object-tools %}
     {% if change and not is_popup %}
         <ul class="object-tools">
-            <li><a href="{% url history_url object_id %}" class="historylink">{% trans "History" %}</a></li>
+            <li><a href="{% url history_url object_id %}" class="historylink">{% translate "History" %}</a></li>
             {% if has_absolute_url %}
-                <li><a href="../../../r/{{ content_type_id }}/{{ object_id }}/" class="viewsitelink">{% trans "View on site" %}</a></li>
+                <li><a href="../../../r/{{ content_type_id }}/{{ object_id }}/" class="viewsitelink">{% translate "View on site" %}</a></li>
             {% endif%}
         </ul>
     {% endif %}
     {% include "admin/filer/tools/detail_info.html" %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 {% extends "admin/filer/change_form.html" %} {% load i18n admin_modify static
 %} {% block extrahead %} {{ block.super }} {# upload stuff #}
  {% endblock %} {% block object-tools %} {% if change and not is_popup %}
-    * {%_trans_"History"_%}
+    * {%_translate_"History"_%}
     * {% if has_absolute_url %}
-    * {%_trans_"View_on_site"_%}
+    * {%_translate_"View_on_site"_%}
     * {% endif%}
 {% endif %} {% include "admin/filer/tools/detail_info.html" %} {% endblock %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/folder/change_form.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/change_form.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 {% extends "admin/change_form.html" %}
 {% load i18n admin_modify static filer_admin_tags %}
 
 {% block breadcrumbs %}
     <div class="breadcrumbs">
-        <a href="{% url 'admin:index' %}" title="{% trans 'Go back to' %} {% trans 'admin homepage' %}">{% trans "Home" %}</a>
-        &rsaquo; <a href="{% url 'admin:app_list' app_label='filer' %}" title="{% trans 'Go back to' %} {% trans 'Filer' %}"> {% trans "Filer" %}</a>
-        &rsaquo; <a href="{% url 'admin:filer-directory_listing-root' %}" title="{% trans 'Go back to' %} '{% trans 'root'|title %}' {% trans 'folder' %}">{% trans "root"|title %}</a>
-        {% for ancestor_folder in original.get_ancestors %}
+        <a href="{% url 'admin:index' %}" title="{% translate 'Go back to' %} {% translate 'admin homepage' %}">{% translate "Home" %}</a>
+        &rsaquo; <a href="{% url 'admin:app_list' app_label='filer' %}" title="{% translate 'Go back to' %} {% translate 'Filer' %}"> {% translate "Filer" %}</a>
+        &rsaquo; <a href="{% url 'admin:filer-directory_listing-root' %}" title="{% translate 'Go back to' %} '{% translate 'root'|title %}' {% translate 'folder' %}">{% translate "root"|title %}</a>
+        {% for ancestor_folder in original.logical_path %}
             &rsaquo; <a href="{% url 'admin:filer-directory_listing' ancestor_folder.id %}" title="{% blocktrans with ancestor_folder.name as folder_name %}Go back to '{{ folder_name }}' folder{% endblocktrans %}">{{ ancestor_folder.name }}</a>
         {% endfor %}
         &rsaquo; {{ original.name }}
     </div>
 {% endblock %}
 
 {% block coltype %}{% if is_popup %}colM{% else %}colMS{% endif %}{% endblock %}
 
 {% block object-tools %}
     {% if change and not is_popup %}
         <ul class="object-tools">
-            <li><a href="{% url history_url object_id %}" class="historylink">{% trans "History" %}</a></li>
+            <li><a href="{% url history_url object_id %}" class="historylink">{% translate "History" %}</a></li>
             {% if has_absolute_url %}
-                <li><a href="../../../r/{{ content_type_id }}/{{ object_id }}/" class="viewsitelink">{% trans "View on site" %}</a></li>
+                <li><a href="../../../r/{{ content_type_id }}/{{ object_id }}/" class="viewsitelink">{% translate "View on site" %}</a></li>
             {% endif%}
         </ul>
     {% endif %}
 {% endblock %}
 
 {% block after_field_sets %}
     {% filer_admin_context_hidden_formfields %}
 {% endblock %}
 
 {% block sidebar %}
     {% if not is_popup %}
         <div id="content-related">
             <div id="navcontainer">
-                <img src="{% static 'filer/icons/folder.svg' %}" alt="{% trans 'Folder Icon' %}" width="128" height="128" />
+                <img src="{% static 'filer/icons/folder.svg' %}" alt="{% translate 'Folder Icon' %}" width="128" height="128" />
             </div>
         </div>
     {% endif %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 {% extends "admin/change_form.html" %} {% load i18n admin_modify static
 filer_admin_tags %} {% block breadcrumbs %}
-{%_trans_"Home"_%} › {%_trans_"Filer"_%} › {%_trans_"root"|title_%} {% for
-ancestor_folder in original.get_ancestors %} › {{_ancestor_folder.name_}} {%
-endfor %} › {{ original.name }}
+{%_translate_"Home"_%} › {%_translate_"Filer"_%} › {%_translate_"root"|title_%}
+{% for ancestor_folder in original.logical_path %} › {{_ancestor_folder.name_}}
+{% endfor %} › {{ original.name }}
 {% endblock %} {% block coltype %}{% if is_popup %}colM{% else %}colMS{% endif
 %}{% endblock %} {% block object-tools %} {% if change and not is_popup %}
-    * {%_trans_"History"_%}
+    * {%_translate_"History"_%}
     * {% if has_absolute_url %}
-    * {%_trans_"View_on_site"_%}
+    * {%_translate_"View_on_site"_%}
     * {% endif%}
 {% endif %} {% endblock %} {% block after_field_sets %} {%
 filer_admin_context_hidden_formfields %} {% endblock %} {% block sidebar %} {%
 if not is_popup %}
-[{% trans 'Folder Icon' %}]
+[{% translate 'Folder Icon' %}]
 {% endif %} {% endblock %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/folder/choose_copy_destination.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_copy_destination.html`

 * *Files 9% similar despite different names*

```diff
@@ -9,80 +9,67 @@
     {{ block.super }}
     <link rel="stylesheet" type="text/css" href="{% static 'admin/css/forms.css' %}">
     <link rel="stylesheet" type="text/css" href="{% static 'filer/css/admin_filer.css' %}">
 {% endblock %}
 
 {% block extrahead %}
     {{ block.super }}
-    <script src="{% static 'filer/js/libs/jquery.min.js' %}"></script>
     <script src="{% static 'admin/js/jquery.init.js' %}"></script>
-    <script type="text/javascript">
-        var __jQuery = django.jQuery;
-        window.jQuery = (__jQuery) ? __jQuery : window.jQuery || undefined;
-        window.$ = window.jQuery;
-    </script>
     <script src="{% static 'filer/js/addons/tooltip.js' %}"></script>
     <script src="{% static 'filer/js/addons/copy-move-files.js' %}"></script>
-    <script type="text/javascript">
-        var __jQuery;
-        var __$;
-        // reassign jQuery if jQuery is already loaded
-        __jQuery = (window.jQuery) ? window.jQuery.noConflict(true) : undefined;
-        __$ = __jQuery;
-    </script>
 {% endblock %}
 
 {% block content %}
     {% if perms_lacking %}
         <p>{% blocktrans %}Your account doesn't have permissions to copy all of the selected files and/or folders.{% endblocktrans %}</p>
         <div class="text-right clearfix">
-            <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% trans "Take me back" %}</a>
+            <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% translate "Take me back" %}</a>
         </div>
     {% else %}
         {% if not destination_folders %}
             <p>{% blocktrans %}There are no destination folders available.{% endblocktrans %}</p>
             <div class="text-right clearfix">
-                <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% trans "Take me back" %}</a>
+                <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% translate "Take me back" %}</a>
             </div>
         {% else %}
             {% if not to_copy %}
                 <p>{% blocktrans %}There are no files and/or folders available to copy.{% endblocktrans %}</p>
                 <div class="text-right clearfix">
-                    <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% trans "Take me back" %}</a>
+                    <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% translate "Take me back" %}</a>
                 </div>
             {% else %}
                 <p>{% blocktrans %}The following files and/or folders will be copied to a destination folder (retaining their tree structure):{% endblocktrans %}</p>
                 <ul>{{ to_copy|unordered_list }}</ul>
                 <form action="" method="post">
                     {% csrf_token %}
                     <div>
                         {% for f in files_queryset %}
-                            <input type="hidden" name="{{ action_checkbox_name }}" value="file-{{ f.pk }}">
+                            <input type="hidden" name="{{ action_checkbox_name }}" value="file-{{ f.pk|safe }}">
                         {% endfor %}
                         {% for f in folders_queryset %}
-                            <input type="hidden" name="{{ action_checkbox_name }}" value="folder-{{ f.pk }}">
+                            <input type="hidden" name="{{ action_checkbox_name }}" value="folder-{{ f.pk|safe }}">
                         {% endfor %}
                         <input type="hidden" name="action" value="copy_files_and_folders">
                         <input type="hidden" name="post" value="yes">
                         <p>
                             <label for="destination">{% blocktrans %}Destination folder:{% endblocktrans %}</label>
                             <select name="destination" id="destination">
                                 {% for folder, name_and_enabled in destination_folders %}
-                                    <option value="{{ folder.pk }}"{% if not name_and_enabled.1 %} disabled="disabled"{% endif %}{% if selected_destination_folder and folder.pk == selected_destination_folder %} selected="selected"{% endif %}>{{ name_and_enabled.0 }}</option>
+                                    <option value="{{ folder.pk|safe }}"{% if not name_and_enabled.1 %} disabled="disabled"{% endif %}{% if selected_destination_folder and folder.pk == selected_destination_folder %} selected="selected"{% endif %}>{{ name_and_enabled.0 }}</option>
                                 {% endfor %}
                             </select>
                         </p>
                         {{ copy_form.as_p_with_help }}
 
                         <div class="text-right clearfix">
-                            <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% trans "No, take me back" %}</a>
-                            <input type="submit" value="{% trans 'Copy' %}" class="default js-submit-copy-move">
+                            <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% translate "No, take me back" %}</a>
+                            <input type="submit" value="{% translate 'Copy' %}" class="default js-submit-copy-move">
                             <span class="js-disabled-btn-tooltip disabled-btn-tooltip js-filer-tooltip filer-tooltip-wrapper"
-                                title="{% trans 'It is not allowed to copy files into same folder' %}" tabindex="-1">
-                                <a class="default navigator-button" disabled>{% trans 'Copy' %}</a>
+                                title="{% translate 'It is not allowed to copy files into same folder' %}" tabindex="-1">
+                                <a class="default navigator-button" disabled>{% translate 'Copy' %}</a>
                             </span>
                         </div>
                     </div>
                 </form>
             {% endif %}
         {% endif %}
     {% endif %}
```

#### html2text {}

```diff
@@ -2,29 +2,30 @@
 breadcrumbs %} {% include "admin/filer/breadcrumbs.html" %} {% endblock %} {%
 block extrastyle %} {{ block.super }}
 
  {% endblock %} {% block extrahead %} {{ block.super }}
  {% endblock %} {% block content %} {% if perms_lacking %}
 {% blocktrans %}Your account doesn't have permissions to copy all of the
 selected files and/or folders.{% endblocktrans %}
-{%_trans_"Take_me_back"_%}
+{%_translate_"Take_me_back"_%}
 {% else %} {% if not destination_folders %}
 {% blocktrans %}There are no destination folders available.{% endblocktrans %}
-{%_trans_"Take_me_back"_%}
+{%_translate_"Take_me_back"_%}
 {% else %} {% if not to_copy %}
 {% blocktrans %}There are no files and/or folders available to copy.{%
 endblocktrans %}
-{%_trans_"Take_me_back"_%}
+{%_translate_"Take_me_back"_%}
 {% else %}
 {% blocktrans %}The following files and/or folders will be copied to a
 destination folder (retaining their tree structure):{% endblocktrans %}
     * {{ to_copy|unordered_list }}
 {% csrf_token %}
 {% for f in files_queryset %}  {% endfor %} {% for f in folders_queryset %}  {%
 endfor %}
 {% for folder, name_and_enabled in destination_folders %} % if not
 name_and_enabled.1 %} disabled="disabled"{% endif %}{% if
 selected_destination_folder and folder.pk == selected_destination_folder %}
 selected="selected"{% endif %}>{{ name_and_enabled.0 }}{% endfor %}
 {{ copy_form.as_p_with_help }}
-{%_trans_"No,_take_me_back"_%} [{% trans 'Copy' %}]  {% trans 'Copy' %}
+{%_translate_"No,_take_me_back"_%} [{% translate 'Copy' %}]  {% translate
+'Copy' %}
 {% endif %} {% endif %} {% endif %} {% endblock %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/folder/choose_images_resize_options.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_images_resize_options.html`

 * *Files 3% similar despite different names*

```diff
@@ -18,30 +18,30 @@
             <p>{% blocktrans %}There are no images available to resize.{% endblocktrans %}</p>
         {% else %}
             <p>{% blocktrans %}The following images will be resized:{% endblocktrans %}</p>
             <ul>{{ to_resize|unordered_list }}</ul>
             <form action="" method="post">{% csrf_token %}
                 <div>
                     {% for f in files_queryset %}
-                        <input type="hidden" name="{{ action_checkbox_name }}" value="file-{{ f.pk }}">
+                        <input type="hidden" name="{{ action_checkbox_name }}" value="file-{{ f.pk|safe }}">
                     {% endfor %}
                     {% for f in folders_queryset %}
-                        <input type="hidden" name="{{ action_checkbox_name }}" value="folder-{{ f.pk }}">
+                        <input type="hidden" name="{{ action_checkbox_name }}" value="folder-{{ f.pk|safe }}">
                     {% endfor %}
                     <input type="hidden" name="action" value="resize_images">
                     <input type="hidden" name="post" value="yes">
                     {% if cmsplugin_enabled %}
                         <p>{% blocktrans %}Choose an existing thumbnail option or enter resize parameters:{% endblocktrans %}</p>
                     {% else %}
                         <p>{% blocktrans %}Choose resize parameters:{% endblocktrans %}</p>
                     {% endif %}
                     {{ resize_form.as_p_with_help }}
                     <p>{% blocktrans %}Warning: Images will be resized in-place and originals will be lost. Maybe first make a copy of them to retain the originals.{% endblocktrans %}</p>
 
                     <div class="text-right clearfix">
-                        <input type="submit" value="{% trans 'Resize' %}" class="default">
+                        <input type="submit" value="{% translate 'Resize' %}" class="default">
                     </div>
                 </div>
             </form>
         {% endif %}
     {% endif %}
 {% endblock %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/folder/choose_move_destination.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_move_destination.html`

 * *Files 21% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 {% block breadcrumbs %}
     {% include "admin/filer/breadcrumbs.html" %}
 {% endblock %}
 
 {% block extrastyle %}
     {{ block.super }}
     <link rel="stylesheet" type="text/css" href="{% static 'admin/css/forms.css' %}">
+    <link rel="stylesheet" type="text/css" href="{% static 'filer/css/admin_filer.icons.css' %}">
     <link rel="stylesheet" type="text/css" href="{% static 'filer/css/admin_filer.css' %}">
 {% endblock %}
 
 {% block extrahead %}
     {{ block.super }}
-    <script src="{% static 'filer/js/libs/jquery.min.js' %}"></script>
     <script src="{% static 'admin/js/jquery.init.js' %}"></script>
     <script type="text/javascript">
         var __jQuery = django.jQuery;
         window.jQuery = (__jQuery) ? __jQuery : window.jQuery || undefined;
         window.$ = window.jQuery;
     </script>
     <script src="{% static 'filer/js/addons/tooltip.js' %}"></script>
@@ -31,54 +31,54 @@
     </script>
 {% endblock %}
 
 {% block content %}
     {% if perms_lacking %}
         <p>{% blocktrans %}Your account doesn't have permissions to move all of the selected files and/or folders.{% endblocktrans %}</p>
         <div class="text-right clearfix">
-            <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% trans "Take me back" %}</a>
+            <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% translate "Take me back" %}</a>
         </div>
     {% else %}
         {% if not destination_folders %}
             <p>{% blocktrans %}There are no destination folders available.{% endblocktrans %}</p>
-            <div class="text-right clearfix">
-                <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% trans "Take me back" %}</a>
+            <div class="text-right clearfix submit-row">
+                <a href="#" onclick="window.history.back(); return false;" class="closelink">{% translate "Take me back" %}</a>
             </div>
         {% else %}
             {% if not to_move %}
                 <p>{% blocktrans %}There are no files and/or folders available to move.{% endblocktrans %}</p>
-                <div class="text-right clearfix">
-                    <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% trans "Take me back" %}</a>
+                <div class="text-right clearfix submit-row">
+                    <a href="#" onclick="window.history.back(); return false;" class="closelink">{% translate "Take me back" %}</a>
                 </div>
             {% else %}
                 <p>{% blocktrans %}The following files and/or folders will be moved to a destination folder (retaining their tree structure):{% endblocktrans %}</p>
                 <ul>{{ to_move|unordered_list }}</ul>
                 <form action="" method="post">{% csrf_token %}
                     <div>
                         {% for f in files_queryset %}
-                            <input type="hidden" name="{{ action_checkbox_name }}" value="file-{{ f.pk }}">
+                            <input type="hidden" name="{{ action_checkbox_name }}" value="file-{{ f.pk|safe }}">
                         {% endfor %}
                         {% for f in folders_queryset %}
-                            <input type="hidden" name="{{ action_checkbox_name }}" value="folder-{{ f.pk }}">
+                            <input type="hidden" name="{{ action_checkbox_name }}" value="folder-{{ f.pk|safe }}">
                         {% endfor %}
                         <input type="hidden" name="action" value="move_files_and_folders">
                         <input type="hidden" name="post" value="yes">
                         <p><label for="destination">{% blocktrans %}Destination folder:{% endblocktrans %}</label>
                         <select name="destination" id="destination">
                             {% for folder, name_and_enabled in destination_folders %}
-                                <option value="{{ folder.pk }}"{% if not name_and_enabled.1 %} disabled="disabled"{% endif %}>{{ name_and_enabled.0 }}</option>
+                                <option value="{{ folder.pk|safe }}"{% if not name_and_enabled.1 %} disabled="disabled"{% endif %}>{{ name_and_enabled.0 }}</option>
                             {% endfor %}
                         </select></p>
 
-                       <div class="text-right clearfix">
-                            <a href="#" onclick="window.history.back(); return false;" class="button cancel-link">{% trans "No, take me back" %}</a>
-                            <input type="submit" value="{% trans 'Move' %}" class="default js-submit-copy-move">
+                       <div class="text-right clearfix submit-row">
+                            <a href="#" onclick="window.history.back(); return false;" class="closelink">{% translate "No, take me back" %}</a>
+                            <input type="submit" value="{% translate 'Move' %}" class="default js-submit-copy-move">
                             <span class="js-disabled-btn-tooltip disabled-btn-tooltip js-filer-tooltip filer-tooltip-wrapper"
-                                title="{% trans 'It is not allowed to move files into same folder' %}" tabindex="-1">
-                                <a class="default navigator-button" disabled>{% trans 'Move' %}</a>
+                                title="{% translate 'It is not allowed to move files into same folder' %}" tabindex="-1">
+                                <a class="default navigator-button" disabled>{% translate 'Move' %}</a>
                             </span>
                         </div>
                     </div>
                 </form>
             {% endif %}
         {% endif %}
     {% endif %}
```

#### html2text {}

```diff
@@ -1,28 +1,30 @@
 {% extends "admin/base_site.html" %} {% load i18n static %} {% block
 breadcrumbs %} {% include "admin/filer/breadcrumbs.html" %} {% endblock %} {%
 block extrastyle %} {{ block.super }}
 
+
  {% endblock %} {% block extrahead %} {{ block.super }}
  {% endblock %} {% block content %} {% if perms_lacking %}
 {% blocktrans %}Your account doesn't have permissions to move all of the
 selected files and/or folders.{% endblocktrans %}
-{%_trans_"Take_me_back"_%}
+{%_translate_"Take_me_back"_%}
 {% else %} {% if not destination_folders %}
 {% blocktrans %}There are no destination folders available.{% endblocktrans %}
-{%_trans_"Take_me_back"_%}
+{%_translate_"Take_me_back"_%}
 {% else %} {% if not to_move %}
 {% blocktrans %}There are no files and/or folders available to move.{%
 endblocktrans %}
-{%_trans_"Take_me_back"_%}
+{%_translate_"Take_me_back"_%}
 {% else %}
 {% blocktrans %}The following files and/or folders will be moved to a
 destination folder (retaining their tree structure):{% endblocktrans %}
     * {{ to_move|unordered_list }}
 {% csrf_token %}
 {% for f in files_queryset %}  {% endfor %} {% for f in folders_queryset %}  {%
 endfor %}
 {% for folder, name_and_enabled in destination_folders %} % if not
 name_and_enabled.1 %} disabled="disabled"{% endif %}>{{ name_and_enabled.0 }}{%
 endfor %}
-{%_trans_"No,_take_me_back"_%} [{% trans 'Move' %}]  {% trans 'Move' %}
+{%_translate_"No,_take_me_back"_%} [{% translate 'Move' %}]  {% translate
+'Move' %}
 {% endif %} {% endif %} {% endif %} {% endblock %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/folder/choose_rename_format.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_rename_format.html`

 * *Files 6% similar despite different names*

```diff
@@ -19,18 +19,18 @@
         {% else %}
             <p>{% blocktrans %}The following files will be renamed (they will stay in their folders and keep original filename, only displayed filename will be changed):{% endblocktrans %}</p>
             <ul>{{ to_rename|unordered_list }}</ul>
             <form action="" method="post">
                 {% csrf_token %}
                 <div>
                     {% for f in files_queryset %}
-                        <input type="hidden" name="{{ action_checkbox_name }}" value="file-{{ f.pk }}">
+                        <input type="hidden" name="{{ action_checkbox_name }}" value="file-{{ f.pk|safe }}">
                     {% endfor %}
                     {% for f in folders_queryset %}
-                        <input type="hidden" name="{{ action_checkbox_name }}" value="folder-{{ f.pk }}">
+                        <input type="hidden" name="{{ action_checkbox_name }}" value="folder-{{ f.pk|safe }}">
                     {% endfor %}
                     <input type="hidden" name="action" value="rename_files">
                     <input type="hidden" name="post" value="yes">
                     {{ rename_form.as_p_with_help }}
                     <div class="help">
                         <p>Rename format is in <a href="http://docs.python.org/library/stdtypes.html#string-formatting-operations">Python % operator format</a> using dictionary of possible values:</p>
                         <dl>
@@ -52,14 +52,14 @@
                         <p>Examples:</p>
                         <ul>
                             <li><code>Prefix %(current_filename)s</code></li>
                             <li><code>Image %(counter)03d</code></li>
                         </ul>
                     </div>
                     <p>
-                        <input type="submit" value="{% trans 'Rename' %}">
+                        <input type="submit" value="{% translate 'Rename' %}">
                     </p>
                 </div>
             </form>
         {% endif %}
     {% endif %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -29,9 +29,9 @@
   counter
       Renaming sequence counter in the current folder (1-based).
   global_counter
       Renaming squence counter for all files currently renaming (1-based).
 Examples:
     * Prefix %(current_filename)s
     * Image %(counter)03d
-[{% trans 'Rename' %}]
+[{% translate 'Rename' %}]
 {% endif %} {% endif %} {% endblock %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/folder/directory_listing.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/directory_listing.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,938 +1,971 @@
 00000000: 7b25 2065 7874 656e 6473 2022 6164 6d69  {% extends "admi
 00000010: 6e2f 6669 6c65 722f 6261 7365 5f73 6974  n/filer/base_sit
 00000020: 652e 6874 6d6c 2220 257d 0a7b 2520 6c6f  e.html" %}.{% lo
 00000030: 6164 2069 3138 6e20 7374 6174 6963 2066  ad i18n static f
 00000040: 696c 6572 5f61 646d 696e 5f74 6167 7320  iler_admin_tags 
-00000050: 257d 0a0a 7b25 2062 6c6f 636b 2065 7874  %}..{% block ext
-00000060: 7261 6865 6164 2025 7d0a 2020 2020 7b7b  rahead %}.    {{
-00000070: 2062 6c6f 636b 2e73 7570 6572 207d 7d0a   block.super }}.
-00000080: 0a20 2020 207b 2520 6966 2061 6374 696f  .    {% if actio
-00000090: 6e5f 666f 726d 2061 6e64 2061 6374 696f  n_form and actio
-000000a0: 6e73 5f6f 6e5f 746f 7020 6f72 2061 6374  ns_on_top or act
-000000b0: 696f 6e73 5f6f 6e5f 626f 7474 6f6d 2025  ions_on_bottom %
-000000c0: 7d0a 2020 2020 2020 2020 3c73 6372 6970  }.        <scrip
-000000d0: 7420 7479 7065 3d22 7465 7874 2f6a 6176  t type="text/jav
-000000e0: 6173 6372 6970 7422 3e0a 2020 2020 2020  ascript">.      
-000000f0: 2020 2020 2020 2866 756e 6374 696f 6e28        (function(
-00000100: 2429 207b 0a20 2020 2020 2020 2020 2020  $) {.           
-00000110: 2020 2020 2024 2864 6f63 756d 656e 7429       $(document)
-00000120: 2e72 6561 6479 2866 756e 6374 696f 6e28  .ready(function(
-00000130: 2429 207b 0a20 2020 2020 2020 2020 2020  $) {.           
-00000140: 2020 2020 2020 2020 2024 2827 7472 2069           $('tr i
-00000150: 6e70 7574 2e61 6374 696f 6e2d 7365 6c65  nput.action-sele
-00000160: 6374 2729 2e61 6374 696f 6e73 2829 3b0a  ct').actions();.
-00000170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000180: 7d29 3b0a 2020 2020 2020 2020 2020 2020  });.            
-00000190: 7d29 2864 6a61 6e67 6f2e 6a51 7565 7279  })(django.jQuery
-000001a0: 293b 0a20 2020 2020 2020 203c 2f73 6372  );.        </scr
-000001b0: 6970 743e 0a20 2020 207b 2520 656e 6469  ipt>.    {% endi
-000001c0: 6620 257d 0a7b 2520 656e 6462 6c6f 636b  f %}.{% endblock
-000001d0: 2025 7d0a 0a7b 2520 626c 6f63 6b20 636f   %}..{% block co
-000001e0: 6c74 7970 6520 257d 7b25 2065 6e64 626c  ltype %}{% endbl
-000001f0: 6f63 6b20 257d 0a7b 2520 626c 6f63 6b20  ock %}.{% block 
-00000200: 626f 6479 636c 6173 7320 257d 7b7b 2062  bodyclass %}{{ b
-00000210: 6c6f 636b 2e73 7570 6572 207d 7d20 6368  lock.super }} ch
-00000220: 616e 6765 2d6c 6973 7420 6669 6c65 6272  ange-list filebr
-00000230: 6f77 7365 727b 2520 656e 6462 6c6f 636b  owser{% endblock
-00000240: 2025 7d0a 0a0a 7b25 2062 6c6f 636b 2065   %}...{% block e
-00000250: 7874 7261 7374 796c 6520 257d 0a20 2020  xtrastyle %}.   
-00000260: 207b 7b20 626c 6f63 6b2e 7375 7065 7220   {{ block.super 
-00000270: 7d7d 0a0a 2020 2020 7b7b 206d 6564 6961  }}..    {{ media
-00000280: 2e63 7373 207d 7d0a 2020 2020 7b25 2069  .css }}.    {% i
-00000290: 6620 6163 7469 6f6e 5f66 6f72 6d20 257d  f action_form %}
-000002a0: 0a20 2020 2020 2020 207b 2520 7572 6c20  .        {% url 
-000002b0: 2761 646d 696e 3a6a 7369 3138 6e27 2061  'admin:jsi18n' a
-000002c0: 7320 6a73 6931 386e 7572 6c20 257d 0a20  s jsi18nurl %}. 
-000002d0: 2020 2020 2020 203c 7363 7269 7074 2074         <script t
-000002e0: 7970 653d 2274 6578 742f 6a61 7661 7363  ype="text/javasc
-000002f0: 7269 7074 2220 7372 633d 227b 7b20 6a73  ript" src="{{ js
-00000300: 6931 386e 7572 6c7c 6465 6661 756c 743a  i18nurl|default:
-00000310: 272e 2e2f 2e2e 2f6a 7369 3138 6e2f 2720  '../../jsi18n/' 
-00000320: 7d7d 223e 3c2f 7363 7269 7074 3e0a 2020  }}"></script>.  
-00000330: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
-00000340: 2020 7b25 2069 6620 7175 6572 792e 706f    {% if query.po
-00000350: 7020 257d 0a20 2020 2020 2020 203c 7374  p %}.        <st
-00000360: 796c 6520 7479 7065 3d22 7465 7874 2f63  yle type="text/c
-00000370: 7373 223e 0a20 2020 2020 2020 2020 2020  ss">.           
-00000380: 2023 6865 6164 6572 207b 0a20 2020 2020   #header {.     
-00000390: 2020 2020 2020 2020 2020 2064 6973 706c             displ
-000003a0: 6179 3a20 6e6f 6e65 3b0a 2020 2020 2020  ay: none;.      
-000003b0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-000003c0: 3c2f 7374 796c 653e 0a20 2020 207b 2520  </style>.    {% 
-000003d0: 656e 6469 6620 257d 0a7b 2520 656e 6462  endif %}.{% endb
-000003e0: 6c6f 636b 2025 7d0a 0a7b 2520 626c 6f63  lock %}..{% bloc
-000003f0: 6b20 6272 6561 6463 7275 6d62 7320 257d  k breadcrumbs %}
-00000400: 0a20 2020 7b25 2069 6620 6e6f 7420 6973  .   {% if not is
-00000410: 5f70 6f70 7570 2025 7d0a 2020 2020 2020  _popup %}.      
-00000420: 2020 3c64 6976 2063 6c61 7373 3d22 6272    <div class="br
-00000430: 6561 6463 7275 6d62 7322 3e0a 2020 2020  eadcrumbs">.    
-00000440: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
-00000450: 227b 2520 7572 6c20 2761 646d 696e 3a69  "{% url 'admin:i
-00000460: 6e64 6578 2720 257d 2220 7469 746c 653d  ndex' %}" title=
-00000470: 227b 2520 7472 616e 7320 2747 6f20 6261  "{% trans 'Go ba
-00000480: 636b 2074 6f20 6164 6d69 6e20 686f 6d65  ck to admin home
-00000490: 7061 6765 2720 257d 223e 0a20 2020 2020  page' %}">.     
-000004a0: 2020 2020 2020 2020 2020 207b 2520 7472             {% tr
-000004b0: 616e 7320 2248 6f6d 6522 2025 7d0a 2020  ans "Home" %}.  
-000004c0: 2020 2020 2020 2020 2020 3c2f 613e 0a20            </a>. 
-000004d0: 2020 2020 2020 2020 2020 2026 7273 6171             &rsaq
-000004e0: 756f 3b0a 2020 2020 2020 2020 2020 2020  uo;.            
-000004f0: 3c61 2068 7265 663d 227b 2520 7572 6c20  <a href="{% url 
-00000500: 2761 646d 696e 3a61 7070 5f6c 6973 7427  'admin:app_list'
-00000510: 2061 7070 5f6c 6162 656c 3d27 6669 6c65   app_label='file
-00000520: 7227 2025 7d22 2074 6974 6c65 3d22 7b25  r' %}" title="{%
-00000530: 2074 7261 6e73 2027 476f 2062 6163 6b20   trans 'Go back 
-00000540: 746f 2046 696c 6572 2061 7070 2720 257d  to Filer app' %}
-00000550: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00000560: 2020 207b 2520 7472 616e 7320 2246 696c     {% trans "Fil
-00000570: 6572 2220 257d 0a20 2020 2020 2020 2020  er" %}.         
-00000580: 2020 203c 2f61 3e0a 2020 2020 2020 2020     </a>.        
-00000590: 2020 2020 7b25 2069 6620 6e6f 7420 696e      {% if not in
-000005a0: 7374 616e 6365 2e69 735f 726f 6f74 2061  stance.is_root a
-000005b0: 6e64 2069 6e73 7461 6e63 652e 6973 5f73  nd instance.is_s
-000005c0: 6d61 7274 5f66 6f6c 6465 7220 257d 0a20  mart_folder %}. 
-000005d0: 2020 2020 2020 2020 2020 2020 2020 2026                 &
-000005e0: 7273 6171 756f 3b0a 2020 2020 2020 2020  rsaquo;.        
-000005f0: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
-00000600: 227b 2520 7572 6c20 2761 646d 696e 3a66  "{% url 'admin:f
-00000610: 696c 6572 2d64 6972 6563 746f 7279 5f6c  iler-directory_l
-00000620: 6973 7469 6e67 2d72 6f6f 7427 2025 7d22  isting-root' %}"
-00000630: 2074 6974 6c65 3d22 7b25 2074 7261 6e73   title="{% trans
-00000640: 2027 476f 2062 6163 6b20 746f 2072 6f6f   'Go back to roo
-00000650: 7420 666f 6c64 6572 2720 257d 223e 7b25  t folder' %}">{%
-00000660: 2074 7261 6e73 2022 726f 6f74 2220 257d   trans "root" %}
-00000670: 3c2f 613e 0a20 2020 2020 2020 2020 2020  </a>.           
-00000680: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
-00000690: 2020 2020 2020 2020 207b 2520 666f 7220           {% for 
-000006a0: 616e 6365 7374 6f72 5f66 6f6c 6465 7220  ancestor_folder 
-000006b0: 696e 2069 6e73 7461 6e63 652e 6c6f 6769  in instance.logi
-000006c0: 6361 6c5f 7061 7468 2025 7d0a 2020 2020  cal_path %}.    
-000006d0: 2020 2020 2020 2020 2020 2020 2672 7361              &rsa
-000006e0: 7175 6f3b 0a20 2020 2020 2020 2020 2020  quo;.           
-000006f0: 2020 2020 203c 6120 6872 6566 3d22 7b7b       <a href="{{
-00000700: 2061 6e63 6573 746f 725f 666f 6c64 6572   ancestor_folder
-00000710: 2e67 6574 5f61 646d 696e 5f64 6972 6563  .get_admin_direc
-00000720: 746f 7279 5f6c 6973 7469 6e67 5f75 726c  tory_listing_url
-00000730: 5f70 6174 6820 7d7d 220a 2020 2020 2020  _path }}".      
-00000740: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00000750: 746c 653d 227b 2520 626c 6f63 6b74 7261  tle="{% blocktra
-00000760: 6e73 2077 6974 6820 616e 6365 7374 6f72  ns with ancestor
-00000770: 5f66 6f6c 6465 722e 6e61 6d65 2061 7320  _folder.name as 
-00000780: 666f 6c64 6572 5f6e 616d 6520 257d 476f  folder_name %}Go
-00000790: 2062 6163 6b20 746f 2027 7b7b 2066 6f6c   back to '{{ fol
-000007a0: 6465 725f 6e61 6d65 207d 7d27 2066 6f6c  der_name }}' fol
-000007b0: 6465 727b 2520 656e 6462 6c6f 636b 7472  der{% endblocktr
-000007c0: 616e 7320 257d 223e 0a20 2020 2020 2020  ans %}">.       
-000007d0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-000007e0: 6966 2061 6e63 6573 746f 725f 666f 6c64  if ancestor_fold
-000007f0: 6572 2e6c 6162 656c 2025 7d7b 7b20 616e  er.label %}{{ an
-00000800: 6365 7374 6f72 5f66 6f6c 6465 722e 6c61  cestor_folder.la
-00000810: 6265 6c20 7d7d 7b25 2065 6c73 6520 257d  bel }}{% else %}
-00000820: 7b7b 2061 6e63 6573 746f 725f 666f 6c64  {{ ancestor_fold
-00000830: 6572 2e6e 616d 6520 7d7d 7b25 2065 6e64  er.name }}{% end
-00000840: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
-00000850: 2020 2020 2020 3c2f 613e 0a20 2020 2020        </a>.     
-00000860: 2020 2020 2020 207b 2520 656e 6466 6f72         {% endfor
-00000870: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00000880: 7b25 2069 6620 6272 6561 6463 7275 6d62  {% if breadcrumb
-00000890: 735f 6163 7469 6f6e 2025 7d0a 2020 2020  s_action %}.    
-000008a0: 2020 2020 2020 2020 2020 2020 2672 7361              &rsa
-000008b0: 7175 6f3b 0a20 2020 2020 2020 2020 2020  quo;.           
-000008c0: 2020 2020 203c 6120 6872 6566 3d22 7b7b       <a href="{{
-000008d0: 2069 6e73 7461 6e63 652e 6765 745f 6164   instance.get_ad
-000008e0: 6d69 6e5f 6469 7265 6374 6f72 795f 6c69  min_directory_li
-000008f0: 7374 696e 675f 7572 6c5f 7061 7468 207d  sting_url_path }
-00000900: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-00000910: 2020 2020 2020 2074 6974 6c65 3d22 7b25         title="{%
-00000920: 2062 6c6f 636b 7472 616e 7320 7769 7468   blocktrans with
-00000930: 2069 6e73 7461 6e63 652e 6e61 6d65 2061   instance.name a
-00000940: 7320 666f 6c64 6572 5f6e 616d 6520 257d  s folder_name %}
-00000950: 476f 2062 6163 6b20 746f 2027 7b7b 2066  Go back to '{{ f
-00000960: 6f6c 6465 725f 6e61 6d65 207d 7d27 2066  older_name }}' f
-00000970: 6f6c 6465 727b 2520 656e 6462 6c6f 636b  older{% endblock
-00000980: 7472 616e 7320 257d 223e 0a20 2020 2020  trans %}">.     
-00000990: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000009a0: 2520 6966 2069 6e73 7461 6e63 652e 6c61  % if instance.la
-000009b0: 6265 6c20 257d 0a20 2020 2020 2020 2020  bel %}.         
-000009c0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000009d0: 7b20 696e 7374 616e 6365 2e6c 6162 656c  { instance.label
-000009e0: 207d 7d0a 2020 2020 2020 2020 2020 2020   }}.            
-000009f0: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
-00000a00: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00000a10: 2020 2020 2020 2020 2020 207b 7b20 696e             {{ in
-00000a20: 7374 616e 6365 2e6e 616d 6520 7d7d 0a20  stance.name }}. 
-00000a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a40: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
-00000a50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000a60: 2f61 3e0a 2020 2020 2020 2020 2020 2020  /a>.            
-00000a70: 2020 2020 2672 7361 7175 6f3b 0a20 2020      &rsaquo;.   
-00000a80: 2020 2020 2020 2020 2020 2020 207b 7b20               {{ 
-00000a90: 6272 6561 6463 7275 6d62 735f 6163 7469  breadcrumbs_acti
-00000aa0: 6f6e 207d 7d0a 2020 2020 2020 2020 2020  on }}.          
-00000ab0: 2020 7b25 2065 6c73 6520 257d 0a20 2020    {% else %}.   
-00000ac0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00000ad0: 6966 206e 6f74 2069 6e73 7461 6e63 652e  if not instance.
-00000ae0: 6973 5f72 6f6f 7420 616e 6420 696e 7374  is_root and inst
-00000af0: 616e 6365 2e69 735f 736d 6172 745f 666f  ance.is_smart_fo
-00000b00: 6c64 6572 2025 7d0a 2020 2020 2020 2020  lder %}.        
-00000b10: 2020 2020 2020 2020 2020 2020 2672 7361              &rsa
-00000b20: 7175 6f3b 0a20 2020 2020 2020 2020 2020  quo;.           
-00000b30: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-00000b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000b50: 207b 2520 6966 2069 6e73 7461 6e63 652e   {% if instance.
-00000b60: 6c61 6265 6c20 257d 0a20 2020 2020 2020  label %}.       
-00000b70: 2020 2020 2020 2020 2020 2020 207b 7b20               {{ 
-00000b80: 696e 7374 616e 6365 2e6c 6162 656c 207d  instance.label }
-00000b90: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00000ba0: 2020 7b25 2065 6c73 6520 257d 0a20 2020    {% else %}.   
-00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bc0: 207b 7b20 696e 7374 616e 6365 2e6e 616d   {{ instance.nam
-00000bd0: 6520 7d7d 0a20 2020 2020 2020 2020 2020  e }}.           
-00000be0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-00000bf0: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
-00000c00: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
-00000c10: 203c 2f64 6976 3e0a 2020 2020 7b25 2065   </div>.    {% e
-00000c20: 6e64 6966 2025 7d0a 7b25 2065 6e64 626c  ndif %}.{% endbl
-00000c30: 6f63 6b20 257d 0a0a 7b25 2062 6c6f 636b  ock %}..{% block
-00000c40: 2073 6964 6562 6172 2025 7d7b 2520 656e   sidebar %}{% en
-00000c50: 6462 6c6f 636b 2025 7d0a 0a7b 2520 626c  dblock %}..{% bl
-00000c60: 6f63 6b20 636f 6e74 656e 745f 7469 746c  ock content_titl
-00000c70: 6520 257d 0a20 2020 203c 6832 3e26 6e62  e %}.    <h2>&nb
-00000c80: 7370 3b3c 2f68 323e 0a7b 2520 656e 6462  sp;</h2>.{% endb
-00000c90: 6c6f 636b 2025 7d0a 0a7b 2520 626c 6f63  lock %}..{% bloc
-00000ca0: 6b20 636f 6e74 656e 7420 257d 0a20 2020  k content %}.   
-00000cb0: 203c 6469 7620 636c 6173 733d 226e 6176   <div class="nav
-00000cc0: 6967 6174 6f72 2d74 6f70 2d6e 6176 2063  igator-top-nav c
-00000cd0: 6c65 6172 6669 7822 3e0a 2020 2020 2020  learfix">.      
-00000ce0: 2020 3c64 6976 2063 6c61 7373 3d22 6272    <div class="br
-00000cf0: 6561 6463 7275 6d62 732d 636f 6e74 6169  eadcrumbs-contai
-00000d00: 6e65 722d 7772 6170 7065 7222 3e0a 2020  ner-wrapper">.  
-00000d10: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00000d20: 6c61 7373 3d22 6272 6561 6463 7275 6d62  lass="breadcrumb
-00000d30: 732d 636f 6e74 6169 6e65 7222 3e0a 2020  s-container">.  
-00000d40: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00000d50: 6976 2063 6c61 7373 3d22 6272 6561 6463  iv class="breadc
-00000d60: 7275 6d62 732d 636f 6e74 6169 6e65 722d  rumbs-container-
-00000d70: 696e 6e65 7222 3e0a 2020 2020 2020 2020  inner">.        
-00000d80: 2020 2020 2020 2020 2020 2020 7b25 2066              {% f
-00000d90: 6f72 2061 6e63 6573 746f 725f 666f 6c64  or ancestor_fold
-00000da0: 6572 2069 6e20 696e 7374 616e 6365 2e6c  er in instance.l
-00000db0: 6f67 6963 616c 5f70 6174 6820 257d 0a20  ogical_path %}. 
-00000dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000dd0: 2020 2020 2020 207b 7b20 616e 6365 7374         {{ ancest
-00000de0: 6f72 5f66 6f6c 6465 7220 7d7d 0a20 2020  or_folder }}.   
-00000df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e00: 207b 2520 656e 6466 6f72 2025 7d0a 0a20   {% endfor %}.. 
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2020 203c 6469 7620 636c 6173 733d 226e     <div class="n
-00000e30: 6176 6967 6174 6f72 2d62 7265 6164 6372  avigator-breadcr
-00000e40: 756d 6273 223e 0a20 2020 2020 2020 2020  umbs">.         
-00000e50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000e60: 6469 7620 636c 6173 733d 2266 696c 6572  div class="filer
-00000e70: 2d6e 6176 6967 6174 6f72 2d62 7265 6164  -navigator-bread
-00000e80: 6372 756d 6273 2d64 726f 7064 6f77 6e2d  crumbs-dropdown-
-00000e90: 636f 6e74 6169 6e65 7220 6669 6c65 722d  container filer-
-00000ea0: 6472 6f70 646f 776e 2d63 6f6e 7461 696e  dropdown-contain
-00000eb0: 6572 223e 0a20 2020 2020 2020 2020 2020  er">.           
+00000050: 257d 0a0a 7b25 2062 6c6f 636b 2063 6f6c  %}..{% block col
+00000060: 7479 7065 2025 7d7b 2520 656e 6462 6c6f  type %}{% endblo
+00000070: 636b 2025 7d0a 7b25 2062 6c6f 636b 2062  ck %}.{% block b
+00000080: 6f64 7963 6c61 7373 2025 7d7b 7b20 626c  odyclass %}{{ bl
+00000090: 6f63 6b2e 7375 7065 7220 7d7d 2063 6861  ock.super }} cha
+000000a0: 6e67 652d 6c69 7374 2066 696c 6562 726f  nge-list filebro
+000000b0: 7773 6572 7b25 2065 6e64 626c 6f63 6b20  wser{% endblock 
+000000c0: 257d 0a0a 0a7b 2520 626c 6f63 6b20 6578  %}...{% block ex
+000000d0: 7472 6173 7479 6c65 2025 7d0a 2020 2020  trastyle %}.    
+000000e0: 7b7b 2062 6c6f 636b 2e73 7570 6572 207d  {{ block.super }
+000000f0: 7d0a 0a20 2020 207b 7b20 6d65 6469 612e  }..    {{ media.
+00000100: 6373 7320 7d7d 0a20 2020 207b 2520 6966  css }}.    {% if
+00000110: 2061 6374 696f 6e5f 666f 726d 2025 7d0a   action_form %}.
+00000120: 2020 2020 2020 2020 7b25 2075 726c 2027          {% url '
+00000130: 6164 6d69 6e3a 6a73 6931 386e 2720 6173  admin:jsi18n' as
+00000140: 206a 7369 3138 6e75 726c 2025 7d0a 2020   jsi18nurl %}.  
+00000150: 2020 2020 2020 3c73 6372 6970 7420 7479        <script ty
+00000160: 7065 3d22 7465 7874 2f6a 6176 6173 6372  pe="text/javascr
+00000170: 6970 7422 2073 7263 3d22 7b7b 206a 7369  ipt" src="{{ jsi
+00000180: 3138 6e75 726c 7c64 6566 6175 6c74 3a27  18nurl|default:'
+00000190: 2e2e 2f2e 2e2f 6a73 6931 386e 2f27 207d  ../../jsi18n/' }
+000001a0: 7d22 3e3c 2f73 6372 6970 743e 0a20 2020  }"></script>.   
+000001b0: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
+000001c0: 207b 2520 6966 2071 7565 7279 2e70 6f70   {% if query.pop
+000001d0: 2025 7d0a 2020 2020 2020 2020 3c73 7479   %}.        <sty
+000001e0: 6c65 2074 7970 653d 2274 6578 742f 6373  le type="text/cs
+000001f0: 7322 3e0a 2020 2020 2020 2020 2020 2020  s">.            
+00000200: 2368 6561 6465 7220 7b0a 2020 2020 2020  #header {.      
+00000210: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+00000220: 793a 206e 6f6e 653b 0a20 2020 2020 2020  y: none;.       
+00000230: 2020 2020 207d 0a20 2020 2020 2020 203c       }.        <
+00000240: 2f73 7479 6c65 3e0a 2020 2020 7b25 2065  /style>.    {% e
+00000250: 6e64 6966 2025 7d0a 7b25 2065 6e64 626c  ndif %}.{% endbl
+00000260: 6f63 6b20 257d 0a0a 7b25 2062 6c6f 636b  ock %}..{% block
+00000270: 2062 7265 6164 6372 756d 6273 2025 7d0a   breadcrumbs %}.
+00000280: 2020 207b 2520 6966 206e 6f74 2069 735f     {% if not is_
+00000290: 706f 7075 7020 257d 0a20 2020 2020 2020  popup %}.       
+000002a0: 203c 6469 7620 636c 6173 733d 2262 7265   <div class="bre
+000002b0: 6164 6372 756d 6273 223e 0a20 2020 2020  adcrumbs">.     
+000002c0: 2020 2020 2020 203c 6120 6872 6566 3d22         <a href="
+000002d0: 7b25 2075 726c 2027 6164 6d69 6e3a 696e  {% url 'admin:in
+000002e0: 6465 7827 2025 7d22 2074 6974 6c65 3d22  dex' %}" title="
+000002f0: 7b25 2074 7261 6e73 2027 476f 2062 6163  {% trans 'Go bac
+00000300: 6b20 746f 2061 646d 696e 2068 6f6d 6570  k to admin homep
+00000310: 6167 6527 2025 7d22 3e0a 2020 2020 2020  age' %}">.      
+00000320: 2020 2020 2020 2020 2020 7b25 2074 7261            {% tra
+00000330: 6e73 2022 486f 6d65 2220 257d 0a20 2020  ns "Home" %}.   
+00000340: 2020 2020 2020 2020 203c 2f61 3e0a 2020           </a>.  
+00000350: 2020 2020 2020 2020 2020 2672 7361 7175            &rsaqu
+00000360: 6f3b 0a20 2020 2020 2020 2020 2020 203c  o;.            <
+00000370: 6120 6872 6566 3d22 7b25 2075 726c 2027  a href="{% url '
+00000380: 6164 6d69 6e3a 6170 705f 6c69 7374 2720  admin:app_list' 
+00000390: 6170 705f 6c61 6265 6c3d 2766 696c 6572  app_label='filer
+000003a0: 2720 257d 2220 7469 746c 653d 227b 2520  ' %}" title="{% 
+000003b0: 7472 616e 7320 2747 6f20 6261 636b 2074  trans 'Go back t
+000003c0: 6f20 4669 6c65 7220 6170 7027 2025 7d22  o Filer app' %}"
+000003d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000003e0: 2020 7b25 2074 7261 6e73 2022 4669 6c65    {% trans "File
+000003f0: 7222 2025 7d0a 2020 2020 2020 2020 2020  r" %}.          
+00000400: 2020 3c2f 613e 0a20 2020 2020 2020 2020    </a>.         
+00000410: 2020 207b 2520 6966 206e 6f74 2066 6f6c     {% if not fol
+00000420: 6465 722e 6973 5f72 6f6f 7420 616e 6420  der.is_root and 
+00000430: 666f 6c64 6572 2e69 735f 736d 6172 745f  folder.is_smart_
+00000440: 666f 6c64 6572 2025 7d0a 2020 2020 2020  folder %}.      
+00000450: 2020 2020 2020 2020 2020 2672 7361 7175            &rsaqu
+00000460: 6f3b 0a20 2020 2020 2020 2020 2020 2020  o;.             
+00000470: 2020 203c 6120 6872 6566 3d22 7b25 2075     <a href="{% u
+00000480: 726c 2027 6164 6d69 6e3a 6669 6c65 722d  rl 'admin:filer-
+00000490: 6469 7265 6374 6f72 795f 6c69 7374 696e  directory_listin
+000004a0: 672d 726f 6f74 2720 257d 7b25 2066 696c  g-root' %}{% fil
+000004b0: 6572 5f61 646d 696e 5f63 6f6e 7465 7874  er_admin_context
+000004c0: 5f75 726c 5f70 6172 616d 7320 257d 2220  _url_params %}" 
+000004d0: 7469 746c 653d 227b 2520 7472 616e 7320  title="{% trans 
+000004e0: 2747 6f20 6261 636b 2074 6f20 726f 6f74  'Go back to root
+000004f0: 2066 6f6c 6465 7227 2025 7d22 3e7b 2520   folder' %}">{% 
+00000500: 7472 616e 7320 2272 6f6f 7422 2025 7d3c  trans "root" %}<
+00000510: 2f61 3e0a 2020 2020 2020 2020 2020 2020  /a>.            
+00000520: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00000530: 2020 2020 2020 2020 7b25 2066 6f72 2061          {% for a
+00000540: 6e63 6573 746f 725f 666f 6c64 6572 2069  ncestor_folder i
+00000550: 6e20 666f 6c64 6572 2e6c 6f67 6963 616c  n folder.logical
+00000560: 5f70 6174 6820 257d 0a20 2020 2020 2020  _path %}.       
+00000570: 2020 2020 2020 2020 2026 7273 6171 756f           &rsaquo
+00000580: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00000590: 2020 3c61 2068 7265 663d 227b 7b20 616e    <a href="{{ an
+000005a0: 6365 7374 6f72 5f66 6f6c 6465 722e 6765  cestor_folder.ge
+000005b0: 745f 6164 6d69 6e5f 6469 7265 6374 6f72  t_admin_director
+000005c0: 795f 6c69 7374 696e 675f 7572 6c5f 7061  y_listing_url_pa
+000005d0: 7468 207d 7d7b 2520 6669 6c65 725f 6164  th }}{% filer_ad
+000005e0: 6d69 6e5f 636f 6e74 6578 745f 7572 6c5f  min_context_url_
+000005f0: 7061 7261 6d73 2025 7d22 0a20 2020 2020  params %}".     
+00000600: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00000610: 6974 6c65 3d22 7b25 2062 6c6f 636b 7472  itle="{% blocktr
+00000620: 616e 7320 7769 7468 2061 6e63 6573 746f  ans with ancesto
+00000630: 725f 666f 6c64 6572 2e6e 616d 6520 6173  r_folder.name as
+00000640: 2066 6f6c 6465 725f 6e61 6d65 2025 7d47   folder_name %}G
+00000650: 6f20 6261 636b 2074 6f20 277b 7b20 666f  o back to '{{ fo
+00000660: 6c64 6572 5f6e 616d 6520 7d7d 2720 666f  lder_name }}' fo
+00000670: 6c64 6572 7b25 2065 6e64 626c 6f63 6b74  lder{% endblockt
+00000680: 7261 6e73 2025 7d22 3e0a 2020 2020 2020  rans %}">.      
+00000690: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000006a0: 2069 6620 616e 6365 7374 6f72 5f66 6f6c   if ancestor_fol
+000006b0: 6465 722e 6c61 6265 6c20 257d 7b7b 2061  der.label %}{{ a
+000006c0: 6e63 6573 746f 725f 666f 6c64 6572 2e6c  ncestor_folder.l
+000006d0: 6162 656c 207d 7d7b 2520 656c 7365 2025  abel }}{% else %
+000006e0: 7d7b 7b20 616e 6365 7374 6f72 5f66 6f6c  }{{ ancestor_fol
+000006f0: 6465 722e 6e61 6d65 207d 7d7b 2520 656e  der.name }}{% en
+00000700: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
+00000710: 2020 2020 2020 203c 2f61 3e0a 2020 2020         </a>.    
+00000720: 2020 2020 2020 2020 7b25 2065 6e64 666f          {% endfo
+00000730: 7220 257d 0a20 2020 2020 2020 2020 2020  r %}.           
+00000740: 207b 2520 6966 2062 7265 6164 6372 756d   {% if breadcrum
+00000750: 6273 5f61 6374 696f 6e20 257d 0a20 2020  bs_action %}.   
+00000760: 2020 2020 2020 2020 2020 2020 2026 7273               &rs
+00000770: 6171 756f 3b0a 2020 2020 2020 2020 2020  aquo;.          
+00000780: 2020 2020 2020 3c61 2068 7265 663d 227b        <a href="{
+00000790: 7b20 666f 6c64 6572 2e67 6574 5f61 646d  { folder.get_adm
+000007a0: 696e 5f64 6972 6563 746f 7279 5f6c 6973  in_directory_lis
+000007b0: 7469 6e67 5f75 726c 5f70 6174 6820 7d7d  ting_url_path }}
+000007c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000007d0: 2020 2020 2020 7469 746c 653d 227b 2520        title="{% 
+000007e0: 626c 6f63 6b74 7261 6e73 2077 6974 6820  blocktrans with 
+000007f0: 666f 6c64 6572 2e6e 616d 6520 6173 2066  folder.name as f
+00000800: 6f6c 6465 725f 6e61 6d65 2025 7d47 6f20  older_name %}Go 
+00000810: 6261 636b 2074 6f20 277b 7b20 666f 6c64  back to '{{ fold
+00000820: 6572 5f6e 616d 6520 7d7d 2720 666f 6c64  er_name }}' fold
+00000830: 6572 7b25 2065 6e64 626c 6f63 6b74 7261  er{% endblocktra
+00000840: 6e73 2025 7d22 3e0a 2020 2020 2020 2020  ns %}">.        
+00000850: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
+00000860: 6620 666f 6c64 6572 2e6c 6162 656c 2025  f folder.label %
+00000870: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00000880: 2020 2020 2020 2020 2020 7b7b 2066 6f6c            {{ fol
+00000890: 6465 722e 6c61 6265 6c20 7d7d 0a20 2020  der.label }}.   
+000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008b0: 207b 2520 656c 7365 2025 7d0a 2020 2020   {% else %}.    
+000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008d0: 2020 2020 7b7b 2066 6f6c 6465 722e 6e61      {{ folder.na
+000008e0: 6d65 207d 7d0a 2020 2020 2020 2020 2020  me }}.          
+000008f0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+00000900: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+00000910: 2020 2020 2020 3c2f 613e 0a20 2020 2020        </a>.     
+00000920: 2020 2020 2020 2020 2020 2026 7273 6171             &rsaq
+00000930: 756f 3b0a 2020 2020 2020 2020 2020 2020  uo;.            
+00000940: 2020 2020 7b7b 2062 7265 6164 6372 756d      {{ breadcrum
+00000950: 6273 5f61 6374 696f 6e20 7d7d 0a20 2020  bs_action }}.   
+00000960: 2020 2020 2020 2020 207b 2520 656c 7365           {% else
+00000970: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00000980: 2020 2020 7b25 2069 6620 6e6f 7420 696e      {% if not in
+00000990: 7374 616e 6365 2e69 735f 726f 6f74 2061  stance.is_root a
+000009a0: 6e64 2069 6e73 7461 6e63 652e 6973 5f73  nd instance.is_s
+000009b0: 6d61 7274 5f66 6f6c 6465 7220 257d 0a20  mart_folder %}. 
+000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009d0: 2020 2026 7273 6171 756f 3b0a 2020 2020     &rsaquo;.    
+000009e0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+000009f0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+00000a00: 2020 2020 2020 2020 7b25 2069 6620 696e          {% if in
+00000a10: 7374 616e 6365 2e6c 6162 656c 2025 7d0a  stance.label %}.
+00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a30: 2020 2020 7b7b 2069 6e73 7461 6e63 652e      {{ instance.
+00000a40: 6c61 6265 6c20 7d7d 0a20 2020 2020 2020  label }}.       
+00000a50: 2020 2020 2020 2020 207b 2520 656c 7365           {% else
+00000a60: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00000a70: 2020 2020 2020 2020 7b7b 2069 6e73 7461          {{ insta
+00000a80: 6e63 652e 6e61 6d65 207d 7d0a 2020 2020  nce.name }}.    
+00000a90: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00000aa0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+00000ab0: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
+00000ac0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00000ad0: 2020 207b 2520 656e 6469 6620 257d 0a7b     {% endif %}.{
+00000ae0: 2520 656e 6462 6c6f 636b 2025 7d0a 0a7b  % endblock %}..{
+00000af0: 2520 626c 6f63 6b20 7369 6465 6261 7220  % block sidebar 
+00000b00: 257d 7b25 2065 6e64 626c 6f63 6b20 257d  %}{% endblock %}
+00000b10: 0a0a 7b25 2062 6c6f 636b 2063 6f6e 7465  ..{% block conte
+00000b20: 6e74 5f74 6974 6c65 2025 7d0a 2020 2020  nt_title %}.    
+00000b30: 3c68 323e 266e 6273 703b 3c2f 6832 3e0a  <h2>&nbsp;</h2>.
+00000b40: 7b25 2065 6e64 626c 6f63 6b20 257d 0a0a  {% endblock %}..
+00000b50: 7b25 2062 6c6f 636b 2063 6f6e 7465 6e74  {% block content
+00000b60: 2025 7d0a 2020 2020 3c64 6976 2063 6c61   %}.    <div cla
+00000b70: 7373 3d22 6e61 7669 6761 746f 722d 746f  ss="navigator-to
+00000b80: 702d 6e61 7620 636c 6561 7266 6978 223e  p-nav clearfix">
+00000b90: 0a20 2020 2020 2020 203c 6469 7620 636c  .        <div cl
+00000ba0: 6173 733d 2262 7265 6164 6372 756d 6273  ass="breadcrumbs
+00000bb0: 2d63 6f6e 7461 696e 6572 2d77 7261 7070  -container-wrapp
+00000bc0: 6572 223e 0a20 2020 2020 2020 2020 2020  er">.           
+00000bd0: 203c 6469 7620 636c 6173 733d 2262 7265   <div class="bre
+00000be0: 6164 6372 756d 6273 2d63 6f6e 7461 696e  adcrumbs-contain
+00000bf0: 6572 223e 0a20 2020 2020 2020 2020 2020  er">.           
+00000c00: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00000c10: 2262 7265 6164 6372 756d 6273 2d63 6f6e  "breadcrumbs-con
+00000c20: 7461 696e 6572 2d69 6e6e 6572 223e 0a20  tainer-inner">. 
+00000c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c40: 2020 207b 2520 666f 7220 616e 6365 7374     {% for ancest
+00000c50: 6f72 5f66 6f6c 6465 7220 696e 2069 6e73  or_folder in ins
+00000c60: 7461 6e63 652e 6c6f 6769 6361 6c5f 7061  tance.logical_pa
+00000c70: 7468 2025 7d0a 2020 2020 2020 2020 2020  th %}.          
+00000c80: 2020 2020 2020 2020 2020 2020 2020 7b7b                {{
+00000c90: 2061 6e63 6573 746f 725f 666f 6c64 6572   ancestor_folder
+00000ca0: 207d 7d0a 2020 2020 2020 2020 2020 2020   }}.            
+00000cb0: 2020 2020 2020 2020 7b25 2065 6e64 666f          {% endfo
+00000cc0: 7220 257d 0a0a 2020 2020 2020 2020 2020  r %}..          
+00000cd0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00000ce0: 6c61 7373 3d22 6e61 7669 6761 746f 722d  lass="navigator-
+00000cf0: 6272 6561 6463 7275 6d62 7322 3e0a 2020  breadcrumbs">.  
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d10: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000d20: 3d22 6669 6c65 722d 6e61 7669 6761 746f  ="filer-navigato
+00000d30: 722d 6272 6561 6463 7275 6d62 732d 6472  r-breadcrumbs-dr
+00000d40: 6f70 646f 776e 2d63 6f6e 7461 696e 6572  opdown-container
+00000d50: 2066 696c 6572 2d64 726f 7064 6f77 6e2d   filer-dropdown-
+00000d60: 636f 6e74 6169 6e65 7222 3e0a 2020 2020  container">.    
+00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d80: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
+00000d90: 2223 2220 6461 7461 2d74 6f67 676c 653d  "#" data-toggle=
+00000da0: 2266 696c 6572 2d64 726f 7064 6f77 6e22  "filer-dropdown"
+00000db0: 2061 7269 612d 6578 7061 6e64 6564 3d22   aria-expanded="
+00000dc0: 6661 6c73 6522 3e0a 2020 2020 2020 2020  false">.        
+00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000de0: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000df0: 3d22 7b25 2073 7461 7469 6320 2766 696c  ="{% static 'fil
+00000e00: 6572 2f69 636f 6e73 2f66 6f6c 6465 722d  er/icons/folder-
+00000e10: 6472 6f70 646f 776e 2e73 7667 2720 257d  dropdown.svg' %}
+00000e20: 2220 616c 743d 2222 2077 6964 7468 3d22  " alt="" width="
+00000e30: 3238 2220 6865 6967 6874 3d22 3238 223e  28" height="28">
+00000e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e50: 2020 2020 2020 2020 2020 2020 203c 2f61               </a
+00000e60: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000e70: 2020 2020 2020 2020 2020 2020 2020 3c75                <u
+00000e80: 6c20 636c 6173 733d 2266 696c 6572 2d64  l class="filer-d
+00000e90: 726f 7064 6f77 6e2d 6d65 6e75 206e 6176  ropdown-menu nav
+00000ea0: 6967 6174 6f72 2d62 7265 6164 6372 756d  igator-breadcrum
+00000eb0: 6273 2d64 726f 7064 6f77 6e22 3e0a 2020  bs-dropdown">.  
 00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ed0: 203c 6120 6872 6566 3d22 2322 2064 6174   <a href="#" dat
-00000ee0: 612d 746f 6767 6c65 3d22 6669 6c65 722d  a-toggle="filer-
-00000ef0: 6472 6f70 646f 776e 2220 6172 6961 2d65  dropdown" aria-e
-00000f00: 7870 616e 6465 643d 2266 616c 7365 223e  xpanded="false">
-00000f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ed0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00000ee0: 2066 6f72 2066 6f6c 6465 7220 696e 2066   for folder in f
+00000ef0: 6f6c 6465 722e 6c6f 6769 6361 6c5f 7061  older.logical_pa
+00000f00: 7468 2072 6576 6572 7365 6420 257d 0a20  th reversed %}. 
+00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f30: 203c 696d 6720 7372 633d 227b 2520 7374   <img src="{% st
-00000f40: 6174 6963 2027 6669 6c65 722f 6963 6f6e  atic 'filer/icon
-00000f50: 732f 666f 6c64 6572 2d64 726f 7064 6f77  s/folder-dropdow
-00000f60: 6e2e 7376 6727 2025 7d22 2061 6c74 3d22  n.svg' %}" alt="
-00000f70: 2220 7769 6474 683d 2232 3822 2068 6569  " width="28" hei
-00000f80: 6768 743d 2232 3822 3e0a 2020 2020 2020  ght="28">.      
-00000f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fa0: 2020 2020 2020 3c2f 613e 0a20 2020 2020        </a>.     
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 2020 2020 203c 756c 2063 6c61 7373         <ul class
-00000fd0: 3d22 6669 6c65 722d 6472 6f70 646f 776e  ="filer-dropdown
-00000fe0: 2d6d 656e 7520 6e61 7669 6761 746f 722d  -menu navigator-
-00000ff0: 6272 6561 6463 7275 6d62 732d 6472 6f70  breadcrumbs-drop
-00001000: 646f 776e 223e 0a20 2020 2020 2020 2020  down">.         
-00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001020: 2020 2020 2020 207b 2520 666f 7220 666f         {% for fo
-00001030: 6c64 6572 2069 6e20 666f 6c64 6572 2e6c  lder in folder.l
-00001040: 6f67 6963 616c 5f70 6174 6820 257d 0a20  ogical_path %}. 
-00001050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001070: 2020 203c 6c69 3e0a 2020 2020 2020 2020     <li>.        
-00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010a0: 3c61 2068 7265 663d 227b 2520 7572 6c20  <a href="{% url 
-000010b0: 2761 646d 696e 3a66 696c 6572 2d64 6972  'admin:filer-dir
-000010c0: 6563 746f 7279 5f6c 6973 7469 6e67 2720  ectory_listing' 
-000010d0: 666f 6c64 6572 2e69 6420 257d 7b25 2066  folder.id %}{% f
-000010e0: 696c 6572 5f61 646d 696e 5f63 6f6e 7465  iler_admin_conte
-000010f0: 7874 5f75 726c 5f70 6172 616d 7320 257d  xt_url_params %}
-00001100: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00001110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001120: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00001130: 746c 653d 227b 2520 7472 616e 7320 2747  tle="{% trans 'G
-00001140: 6f20 6261 636b 2074 6f20 7468 6520 7061  o back to the pa
-00001150: 7265 6e74 2066 6f6c 6465 7227 2025 7d22  rent folder' %}"
-00001160: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001180: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-00001190: 6d67 2073 7263 3d22 7b25 2073 7461 7469  mg src="{% stati
-000011a0: 6320 2766 696c 6572 2f69 636f 6e73 2f66  c 'filer/icons/f
-000011b0: 6f6c 6465 722e 7376 6727 2025 7d22 2061  older.svg' %}" a
-000011c0: 6c74 3d22 7b25 2074 7261 6e73 2027 466f  lt="{% trans 'Fo
-000011d0: 6c64 6572 2049 636f 6e27 2025 7d22 2077  lder Icon' %}" w
-000011e0: 6964 7468 3d22 3238 2220 6865 6967 6874  idth="28" height
-000011f0: 3d22 3238 223e 0a20 2020 2020 2020 2020  ="28">.         
-00001200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001220: 2020 207b 7b20 666f 6c64 6572 2e6e 616d     {{ folder.nam
-00001230: 6520 7d7d 0a20 2020 2020 2020 2020 2020  e }}.           
-00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001250: 2020 2020 2020 2020 2020 2020 203c 2f61               </a
-00001260: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001280: 2020 2020 2020 3c2f 6c69 3e0a 2020 2020        </li>.    
-00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012a0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-000012b0: 6e64 666f 7220 257d 0a20 2020 2020 2020  ndfor %}.       
-000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012d0: 2020 2020 2020 2020 203c 6c69 3e0a 2020           <li>.  
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001300: 2020 3c61 2068 7265 663d 227b 2520 7572    <a href="{% ur
-00001310: 6c20 2761 646d 696e 3a66 696c 6572 2d64  l 'admin:filer-d
-00001320: 6972 6563 746f 7279 5f6c 6973 7469 6e67  irectory_listing
-00001330: 2d72 6f6f 7427 2025 7d7b 2520 6669 6c65  -root' %}{% file
-00001340: 725f 6164 6d69 6e5f 636f 6e74 6578 745f  r_admin_context_
-00001350: 7572 6c5f 7061 7261 6d73 2025 7d22 0a20  url_params %}". 
+00000f30: 2020 203c 6c69 3e0a 2020 2020 2020 2020     <li>.        
+00000f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f60: 3c61 2068 7265 663d 227b 2520 7572 6c20  <a href="{% url 
+00000f70: 2761 646d 696e 3a66 696c 6572 2d64 6972  'admin:filer-dir
+00000f80: 6563 746f 7279 5f6c 6973 7469 6e67 2720  ectory_listing' 
+00000f90: 666f 6c64 6572 2e69 6420 257d 7b25 2066  folder.id %}{% f
+00000fa0: 696c 6572 5f61 646d 696e 5f63 6f6e 7465  iler_admin_conte
+00000fb0: 7874 5f75 726c 5f70 6172 616d 7320 257d  xt_url_params %}
+00000fc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fe0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00000ff0: 746c 653d 227b 2520 7472 616e 7320 2747  tle="{% trans 'G
+00001000: 6f20 6261 636b 2074 6f20 7468 6520 7061  o back to the pa
+00001010: 7265 6e74 2066 6f6c 6465 7227 2025 7d22  rent folder' %}"
+00001020: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001040: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
+00001050: 6d67 2073 7263 3d22 7b25 2073 7461 7469  mg src="{% stati
+00001060: 6320 2766 696c 6572 2f69 636f 6e73 2f66  c 'filer/icons/f
+00001070: 6f6c 6465 722e 7376 6727 2025 7d22 2061  older.svg' %}" a
+00001080: 6c74 3d22 7b25 2074 7261 6e73 2027 466f  lt="{% trans 'Fo
+00001090: 6c64 6572 2049 636f 6e27 2025 7d22 2077  lder Icon' %}" w
+000010a0: 6964 7468 3d22 3238 2220 6865 6967 6874  idth="28" height
+000010b0: 3d22 3238 223e 0a20 2020 2020 2020 2020  ="28">.         
+000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010e0: 2020 207b 7b20 666f 6c64 6572 2e6e 616d     {{ folder.nam
+000010f0: 6520 7d7d 0a20 2020 2020 2020 2020 2020  e }}.           
+00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001110: 2020 2020 2020 2020 2020 2020 203c 2f61               </a
+00001120: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001140: 2020 2020 2020 3c2f 6c69 3e0a 2020 2020        </li>.    
+00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001160: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00001170: 6e64 666f 7220 257d 0a20 2020 2020 2020  ndfor %}.       
+00001180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001190: 2020 2020 2020 2020 203c 6c69 3e0a 2020           <li>.  
+000011a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011c0: 2020 3c61 2068 7265 663d 227b 2520 7572    <a href="{% ur
+000011d0: 6c20 2761 646d 696e 3a66 696c 6572 2d64  l 'admin:filer-d
+000011e0: 6972 6563 746f 7279 5f6c 6973 7469 6e67  irectory_listing
+000011f0: 2d72 6f6f 7427 2025 7d7b 2520 6669 6c65  -root' %}{% file
+00001200: 725f 6164 6d69 6e5f 636f 6e74 6578 745f  r_admin_context_
+00001210: 7572 6c5f 7061 7261 6d73 2025 7d22 0a20  url_params %}". 
+00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001240: 2020 2020 2020 2074 6974 6c65 3d22 7b25         title="{%
+00001250: 2074 7261 6e73 2027 476f 2062 6163 6b20   trans 'Go back 
+00001260: 746f 2720 257d 207b 2520 7472 616e 7320  to' %} {% trans 
+00001270: 2772 6f6f 7427 7c74 6974 6c65 2025 7d20  'root'|title %} 
+00001280: 7b25 2074 7261 6e73 2027 666f 6c64 6572  {% trans 'folder
+00001290: 2720 257d 223e 0a20 2020 2020 2020 2020  ' %}">.         
+000012a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000012c0: 696d 6720 7372 633d 227b 2520 7374 6174  img src="{% stat
+000012d0: 6963 2027 6669 6c65 722f 6963 6f6e 732f  ic 'filer/icons/
+000012e0: 666f 6c64 6572 2d72 6f6f 742e 7376 6727  folder-root.svg'
+000012f0: 2025 7d22 2061 6c74 3d22 7b25 2074 7261   %}" alt="{% tra
+00001300: 6e73 2027 466f 6c64 6572 2049 636f 6e27  ns 'Folder Icon'
+00001310: 2025 7d22 2077 6964 7468 3d22 3238 2220   %}" width="28" 
+00001320: 6865 6967 6874 3d22 3238 223e 0a20 2020  height="28">.   
+00001330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001350: 2020 2020 2052 6f6f 740a 2020 2020 2020       Root.      
 00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001380: 2020 2020 2020 2074 6974 6c65 3d22 7b25         title="{%
-00001390: 2074 7261 6e73 2027 476f 2062 6163 6b20   trans 'Go back 
-000013a0: 746f 2720 257d 207b 2520 7472 616e 7320  to' %} {% trans 
-000013b0: 2772 6f6f 7427 7c74 6974 6c65 2025 7d20  'root'|title %} 
-000013c0: 7b25 2074 7261 6e73 2027 666f 6c64 6572  {% trans 'folder
-000013d0: 2720 257d 223e 0a20 2020 2020 2020 2020  ' %}">.         
-000013e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001400: 696d 6720 7372 633d 227b 2520 7374 6174  img src="{% stat
-00001410: 6963 2027 6669 6c65 722f 6963 6f6e 732f  ic 'filer/icons/
-00001420: 666f 6c64 6572 2d72 6f6f 742e 7376 6727  folder-root.svg'
-00001430: 2025 7d22 2061 6c74 3d22 7b25 2074 7261   %}" alt="{% tra
-00001440: 6e73 2027 466f 6c64 6572 2049 636f 6e27  ns 'Folder Icon'
-00001450: 2025 7d22 2077 6964 7468 3d22 3238 2220   %}" width="28" 
-00001460: 6865 6967 6874 3d22 3238 223e 0a20 2020  height="28">.   
-00001470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001490: 2020 2020 2052 6f6f 740a 2020 2020 2020       Root.      
-000014a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014b0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000014c0: 613e 0a20 2020 2020 2020 2020 2020 2020  a>.             
-000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014e0: 2020 203c 2f6c 693e 0a20 2020 2020 2020     </li>.       
-000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001500: 2020 2020 203c 2f75 6c3e 0a20 2020 2020       </ul>.     
-00001510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001520: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001540: 2020 7b25 2069 6620 6e6f 7420 666f 6c64    {% if not fold
-00001550: 6572 2e69 735f 726f 6f74 206f 7220 666f  er.is_root or fo
-00001560: 6c64 6572 2e69 735f 736d 6172 745f 666f  lder.is_smart_fo
-00001570: 6c64 6572 2025 7d0a 2020 2020 2020 2020  lder %}.        
-00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001590: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
-000015a0: 2269 636f 6e20 6661 2066 612d 6368 6576  "icon fa fa-chev
-000015b0: 726f 6e2d 7269 6768 7422 3e3c 2f73 7061  ron-right"></spa
-000015c0: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
-000015d0: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-000015e0: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
-000015f0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-00001600: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001610: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00001620: 3d22 6e61 7669 6761 746f 722d 6272 6561  ="navigator-brea
-00001630: 6463 7275 6d62 732d 6e61 6d65 2d64 726f  dcrumbs-name-dro
-00001640: 7064 6f77 6e2d 7772 6170 7065 7222 3e0a  pdown-wrapper">.
-00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001660: 2020 2020 2020 2020 7b25 2069 6620 6e6f          {% if no
-00001670: 7420 666f 6c64 6572 2e69 735f 726f 6f74  t folder.is_root
-00001680: 206f 7220 666f 6c64 6572 2e69 735f 736d   or folder.is_sm
-00001690: 6172 745f 666f 6c64 6572 2025 7d0a 0a20  art_folder %}.. 
-000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016b0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-000016c0: 636c 6173 733d 226e 6176 6967 6174 6f72  class="navigator
-000016d0: 2d62 7265 6164 6372 756d 6273 2d66 6f6c  -breadcrumbs-fol
-000016e0: 6465 722d 6e61 6d65 2d77 7261 7070 6572  der-name-wrapper
-000016f0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001710: 2020 203c 7370 616e 2063 6c61 7373 3d22     <span class="
-00001720: 6e61 7669 6761 746f 722d 6272 6561 6463  navigator-breadc
-00001730: 7275 6d62 732d 666f 6c64 6572 2d6e 616d  rumbs-folder-nam
-00001740: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
-00001750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001760: 2020 2020 2020 2020 3c73 7061 6e20 636c          <span cl
-00001770: 6173 733d 226e 6176 6967 6174 6f72 2d62  ass="navigator-b
-00001780: 7265 6164 6372 756d 6273 2d66 6f6c 6465  readcrumbs-folde
-00001790: 722d 6e61 6d65 2d69 6e6e 6572 223e 0a20  r-name-inner">. 
+00001370: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00001380: 613e 0a20 2020 2020 2020 2020 2020 2020  a>.             
+00001390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013a0: 2020 203c 2f6c 693e 0a20 2020 2020 2020     </li>.       
+000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013c0: 2020 2020 203c 2f75 6c3e 0a20 2020 2020       </ul>.     
+000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013e0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001400: 2020 7b25 2069 6620 6e6f 7420 666f 6c64    {% if not fold
+00001410: 6572 2e69 735f 726f 6f74 206f 7220 666f  er.is_root or fo
+00001420: 6c64 6572 2e69 735f 736d 6172 745f 666f  lder.is_smart_fo
+00001430: 6c64 6572 2025 7d0a 2020 2020 2020 2020  lder %}.        
+00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001450: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
+00001460: 2269 636f 6e20 6669 6c65 722d 6963 6f6e  "icon filer-icon
+00001470: 2066 696c 6572 2d69 636f 6e2d 6368 6576   filer-icon-chev
+00001480: 726f 6e2d 7269 6768 7420 6661 2066 612d  ron-right fa fa-
+00001490: 6368 6576 726f 6e2d 7269 6768 7422 3e3c  chevron-right"><
+000014a0: 2f73 7061 6e3e 0a20 2020 2020 2020 2020  /span>.         
+000014b0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+000014c0: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+000014d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000014e0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+000014f0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00001500: 6c61 7373 3d22 6e61 7669 6761 746f 722d  lass="navigator-
+00001510: 6272 6561 6463 7275 6d62 732d 6e61 6d65  breadcrumbs-name
+00001520: 2d64 726f 7064 6f77 6e2d 7772 6170 7065  -dropdown-wrappe
+00001530: 7222 3e0a 2020 2020 2020 2020 2020 2020  r">.            
+00001540: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
+00001550: 6620 6e6f 7420 666f 6c64 6572 2e69 735f  f not folder.is_
+00001560: 726f 6f74 206f 7220 666f 6c64 6572 2e69  root or folder.i
+00001570: 735f 736d 6172 745f 666f 6c64 6572 2025  s_smart_folder %
+00001580: 7d0a 0a20 2020 2020 2020 2020 2020 2020  }..             
+00001590: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000015a0: 6469 7620 636c 6173 733d 226e 6176 6967  div class="navig
+000015b0: 6174 6f72 2d62 7265 6164 6372 756d 6273  ator-breadcrumbs
+000015c0: 2d66 6f6c 6465 722d 6e61 6d65 2d77 7261  -folder-name-wra
+000015d0: 7070 6572 223e 0a20 2020 2020 2020 2020  pper">.         
+000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015f0: 2020 2020 2020 203c 7370 616e 2063 6c61         <span cla
+00001600: 7373 3d22 6e61 7669 6761 746f 722d 6272  ss="navigator-br
+00001610: 6561 6463 7275 6d62 732d 666f 6c64 6572  eadcrumbs-folder
+00001620: 2d6e 616d 6522 3e0a 2020 2020 2020 2020  -name">.        
+00001630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001640: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
+00001650: 6e20 636c 6173 733d 226e 6176 6967 6174  n class="navigat
+00001660: 6f72 2d62 7265 6164 6372 756d 6273 2d66  or-breadcrumbs-f
+00001670: 6f6c 6465 722d 6e61 6d65 2d69 6e6e 6572  older-name-inner
+00001680: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00001690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016a0: 2020 2020 2020 2020 2020 207b 7b20 666f             {{ fo
+000016b0: 6c64 6572 2e6e 616d 6520 7d7d 0a20 2020  lder.name }}.   
+000016c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016e0: 203c 2f73 7061 6e3e 0a20 2020 2020 2020   </span>.       
+000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001700: 2020 2020 2020 2020 203c 2f73 7061 6e3e           </span>
+00001710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001720: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00001730: 6976 3e0a 0a20 2020 2020 2020 2020 2020  iv>..           
+00001740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001750: 203c 6469 7620 636c 6173 733d 2266 696c   <div class="fil
+00001760: 6572 2d64 726f 7064 6f77 6e2d 636f 6e74  er-dropdown-cont
+00001770: 6169 6e65 7220 6669 6c65 722d 6472 6f70  ainer filer-drop
+00001780: 646f 776e 2d63 6f6e 7461 696e 6572 2d64  down-container-d
+00001790: 6f77 6e22 3e0a 2020 2020 2020 2020 2020  own">.          
 000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017c0: 2020 2020 2020 207b 7b20 666f 6c64 6572         {{ folder
-000017d0: 2e6e 616d 6520 7d7d 0a20 2020 2020 2020  .name }}.       
-000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017f0: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
-00001800: 7061 6e3e 0a20 2020 2020 2020 2020 2020  pan>.           
-00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001820: 2020 2020 203c 2f73 7061 6e3e 0a20 2020       </span>.   
-00001830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001840: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00001850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001860: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00001870: 7620 636c 6173 733d 2266 696c 6572 2d64  v class="filer-d
-00001880: 726f 7064 6f77 6e2d 636f 6e74 6169 6e65  ropdown-containe
-00001890: 7220 6669 6c65 722d 6472 6f70 646f 776e  r filer-dropdown
-000018a0: 2d63 6f6e 7461 696e 6572 2d64 6f77 6e22  -container-down"
-000018b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018d0: 2020 7b25 2069 6620 6e6f 7420 6973 5f70    {% if not is_p
-000018e0: 6f70 7570 2061 6e64 2066 6f6c 6465 722e  opup and folder.
-000018f0: 6669 6c65 5f74 7970 6520 3d3d 2027 466f  file_type == 'Fo
-00001900: 6c64 6572 2720 616e 6420 7065 726d 6973  lder' and permis
-00001910: 7369 6f6e 732e 6861 735f 6564 6974 5f70  sions.has_edit_p
-00001920: 6572 6d69 7373 696f 6e20 257d 0a20 2020  ermission %}.   
-00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001950: 203c 6120 6872 6566 3d22 2322 2064 6174   <a href="#" dat
-00001960: 612d 746f 6767 6c65 3d22 6669 6c65 722d  a-toggle="filer-
-00001970: 6472 6f70 646f 776e 2220 6172 6961 2d65  dropdown" aria-e
-00001980: 7870 616e 6465 643d 2266 616c 7365 223e  xpanded="false">
-00001990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019b0: 2020 2020 2020 2020 203c 7370 616e 2063           <span c
-000019c0: 6c61 7373 3d22 6661 2066 612d 6361 7265  lass="fa fa-care
-000019d0: 742d 646f 776e 223e 3c2f 7370 616e 3e0a  t-down"></span>.
-000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a00: 2020 2020 3c2f 613e 0a20 2020 2020 2020      </a>.       
-00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a20: 2020 2020 2020 2020 2020 2020 203c 756c               <ul
-00001a30: 2063 6c61 7373 3d22 6669 6c65 722d 6472   class="filer-dr
-00001a40: 6f70 646f 776e 2d6d 656e 7522 3e0a 2020  opdown-menu">.  
-00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017b0: 2020 2020 2020 7b25 2069 6620 6e6f 7420        {% if not 
+000017c0: 6973 5f70 6f70 7570 2061 6e64 2066 6f6c  is_popup and fol
+000017d0: 6465 722e 6669 6c65 5f74 7970 6520 3d3d  der.file_type ==
+000017e0: 2027 466f 6c64 6572 2720 616e 6420 7065   'Folder' and pe
+000017f0: 726d 6973 7369 6f6e 732e 6861 735f 6564  rmissions.has_ed
+00001800: 6974 5f70 6572 6d69 7373 696f 6e20 257d  it_permission %}
+00001810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001830: 2020 2020 203c 6120 6872 6566 3d22 2322       <a href="#"
+00001840: 2064 6174 612d 746f 6767 6c65 3d22 6669   data-toggle="fi
+00001850: 6c65 722d 6472 6f70 646f 776e 2220 6172  ler-dropdown" ar
+00001860: 6961 2d65 7870 616e 6465 643d 2266 616c  ia-expanded="fal
+00001870: 7365 223e 0a20 2020 2020 2020 2020 2020  se">.           
+00001880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001890: 2020 2020 2020 2020 2020 2020 203c 7370               <sp
+000018a0: 616e 2063 6c61 7373 3d22 6669 6c65 722d  an class="filer-
+000018b0: 6963 6f6e 2066 696c 6572 2d69 636f 6e2d  icon filer-icon-
+000018c0: 6361 7265 742d 646f 776e 2066 6120 6661  caret-down fa fa
+000018d0: 2d63 6172 6574 2d64 6f77 6e22 3e3c 2f73  -caret-down"></s
+000018e0: 7061 6e3e 0a20 2020 2020 2020 2020 2020  pan>.           
+000018f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001900: 2020 2020 2020 2020 203c 2f61 3e0a 2020           </a>.  
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001930: 2020 3c75 6c20 636c 6173 733d 2266 696c    <ul class="fil
+00001940: 6572 2d64 726f 7064 6f77 6e2d 6d65 6e75  er-dropdown-menu
+00001950: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001970: 2020 2020 2020 2020 2020 203c 6c69 3e0a             <li>.
+00001980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019a0: 2020 2020 2020 2020 2020 2020 3c61 2068              <a h
+000019b0: 7265 663d 227b 2520 7572 6c20 2761 646d  ref="{% url 'adm
+000019c0: 696e 3a66 696c 6572 5f66 6f6c 6465 725f  in:filer_folder_
+000019d0: 6368 616e 6765 2720 666f 6c64 6572 2e69  change' folder.i
+000019e0: 6420 257d 7b25 2066 696c 6572 5f61 646d  d %}{% filer_adm
+000019f0: 696e 5f63 6f6e 7465 7874 5f75 726c 5f70  in_context_url_p
+00001a00: 6172 616d 7320 257d 2220 7469 746c 653d  arams %}" title=
+00001a10: 227b 2520 7472 616e 7320 2743 6861 6e67  "{% trans 'Chang
+00001a20: 6520 6375 7272 656e 7420 666f 6c64 6572  e current folder
+00001a30: 2064 6574 6169 6c73 2720 257d 223e 7b25   details' %}">{%
+00001a40: 2074 7261 6e73 2022 4368 616e 6765 2220   trans "Change" 
+00001a50: 257d 3c2f 613e 0a20 2020 2020 2020 2020  %}</a>.         
 00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a70: 2020 2020 2020 3c6c 693e 0a20 2020 2020        <li>.     
-00001a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a70: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001a80: 2f6c 693e 0a20 2020 2020 2020 2020 2020  /li>.           
 00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001aa0: 2020 2020 2020 203c 6120 6872 6566 3d22         <a href="
-00001ab0: 7b25 2075 726c 2027 6164 6d69 6e3a 6669  {% url 'admin:fi
-00001ac0: 6c65 725f 666f 6c64 6572 5f63 6861 6e67  ler_folder_chang
-00001ad0: 6527 2066 6f6c 6465 722e 6964 2025 7d7b  e' folder.id %}{
-00001ae0: 2520 6669 6c65 725f 6164 6d69 6e5f 636f  % filer_admin_co
-00001af0: 6e74 6578 745f 7572 6c5f 7061 7261 6d73  ntext_url_params
-00001b00: 2025 7d22 2074 6974 6c65 3d22 7b25 2074   %}" title="{% t
-00001b10: 7261 6e73 2027 4368 616e 6765 2063 7572  rans 'Change cur
-00001b20: 7265 6e74 2066 6f6c 6465 7220 6465 7461  rent folder deta
-00001b30: 696c 7327 2025 7d22 3e7b 2520 7472 616e  ils' %}">{% tran
-00001b40: 7320 2243 6861 6e67 6522 2025 7d3c 2f61  s "Change" %}</a
-00001b50: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b70: 2020 2020 2020 2020 2020 3c2f 6c69 3e0a            </li>.
-00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ba0: 2020 2020 3c2f 756c 3e0a 2020 2020 2020      </ul>.      
-00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bc0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-00001bd0: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
-00001be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bf0: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c10: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
-00001c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c30: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00001c40: 2265 6d70 7479 2d66 696c 6572 2d68 6561  "empty-filer-hea
-00001c50: 6465 722d 6365 6c6c 223e 3c2f 6469 763e  der-cell"></div>
-00001c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001c70: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c90: 3c66 6f72 6d20 636c 6173 733d 2266 696c  <form class="fil
-00001ca0: 7465 722d 6669 6c65 732d 636f 6e74 6169  ter-files-contai
-00001cb0: 6e65 7220 6a73 2d66 696c 7465 722d 6669  ner js-filter-fi
-00001cc0: 6c65 732d 636f 6e74 6169 6e65 7222 2061  les-container" a
-00001cd0: 6374 696f 6e3d 222e 2220 6d65 7468 6f64  ction="." method
-00001ce0: 3d22 6765 7422 2063 6c61 7373 3d22 6a73  ="get" class="js
-00001cf0: 2d66 696c 6572 2d73 6561 7263 682d 666f  -filer-search-fo
-00001d00: 726d 223e 0a20 2020 2020 2020 2020 2020  rm">.           
-00001d10: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00001d20: 7620 636c 6173 733d 2266 696c 7465 722d  v class="filter-
-00001d30: 6669 6c65 7273 2d63 6f6e 7461 696e 6572  filers-container
-00001d40: 2d69 6e6e 6572 223e 0a20 2020 2020 2020  -inner">.       
-00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d60: 2020 2020 203c 6275 7474 6f6e 2063 6c61       <button cla
-00001d70: 7373 3d22 6e61 7669 6761 746f 722d 6275  ss="navigator-bu
-00001d80: 7474 6f6e 2066 696c 7465 722d 6669 6c65  tton filter-file
-00001d90: 732d 6275 7474 6f6e 2220 7469 746c 653d  s-button" title=
-00001da0: 227b 2520 7472 616e 7320 2743 6c69 636b  "{% trans 'Click
-00001db0: 2068 6572 6520 746f 2072 756e 2073 6561   here to run sea
-00001dc0: 7263 6820 666f 7220 656e 7465 7265 6420  rch for entered 
-00001dd0: 7068 7261 7365 2720 257d 223e 3c73 7061  phrase' %}"><spa
-00001de0: 6e20 636c 6173 733d 2269 636f 6e20 6661  n class="icon fa
-00001df0: 2066 612d 7365 6172 6368 223e 3c2f 7370   fa-search"></sp
-00001e00: 616e 3e3c 2f62 7574 746f 6e3e 0a20 2020  an></button>.   
-00001e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e20: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00001e30: 6173 733d 2266 696c 7465 722d 7365 6172  ass="filter-sear
-00001e40: 6368 2d77 7261 7070 6572 223e 0a20 2020  ch-wrapper">.   
-00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e60: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00001e70: 6669 6c65 725f 6164 6d69 6e5f 636f 6e74  filer_admin_cont
-00001e80: 6578 745f 6869 6464 656e 5f66 6f72 6d66  ext_hidden_formf
-00001e90: 6965 6c64 7320 257d 0a20 2020 2020 2020  ields %}.       
-00001ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001eb0: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
-00001ec0: 7479 7065 3d22 7465 7874 2220 706c 6163  type="text" plac
-00001ed0: 6568 6f6c 6465 723d 227b 2520 7472 616e  eholder="{% tran
-00001ee0: 7320 2753 6561 7263 6827 2025 7d22 2063  s 'Search' %}" c
-00001ef0: 6c61 7373 3d22 6669 6c74 6572 2d66 696c  lass="filter-fil
-00001f00: 6573 2d66 6965 6c64 206a 732d 6669 6c74  es-field js-filt
-00001f10: 6572 2d66 696c 6573 2220 7661 6c75 653d  er-files" value=
-00001f20: 227b 7b20 7365 6172 6368 5f73 7472 696e  "{{ search_strin
-00001f30: 6720 7d7d 2220 6e61 6d65 3d22 7122 3e0a  g }}" name="q">.
-00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f60: 3c64 6976 2063 6c61 7373 3d22 6669 6c65  <div class="file
-00001f70: 722d 6472 6f70 646f 776e 2d63 6f6e 7461  r-dropdown-conta
-00001f80: 696e 6572 2066 696c 6572 2d64 726f 7064  iner filer-dropd
-00001f90: 6f77 6e2d 636f 6e74 6169 6e65 722d 646f  own-container-do
-00001fa0: 776e 223e 0a20 2020 2020 2020 2020 2020  wn">.           
-00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fc0: 2020 2020 2020 2020 203c 6120 6872 6566           <a href
-00001fd0: 3d22 2322 2064 6174 612d 746f 6767 6c65  ="#" data-toggle
-00001fe0: 3d22 6669 6c65 722d 6472 6f70 646f 776e  ="filer-dropdown
-00001ff0: 2220 6172 6961 2d65 7870 616e 6465 643d  " aria-expanded=
-00002000: 2266 616c 7365 223e 0a20 2020 2020 2020  "false">.       
-00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002030: 203c 7370 616e 2063 6c61 7373 3d22 6661   <span class="fa
-00002040: 2066 612d 6361 7265 742d 646f 776e 223e   fa-caret-down">
-00002050: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
-00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002070: 2020 2020 2020 2020 2020 2020 3c2f 613e              </a>
-00002080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020a0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020c0: 2020 2020 2020 2020 3c75 6c20 636c 6173          <ul clas
-000020d0: 733d 2266 696c 6572 2d64 726f 7064 6f77  s="filer-dropdow
-000020e0: 6e2d 6d65 6e75 2066 696c 6572 2d64 726f  n-menu filer-dro
-000020f0: 7064 6f77 6e2d 6d65 6e75 2d63 6865 636b  pdown-menu-check
-00002100: 626f 7865 7322 3e0a 2020 2020 2020 2020  boxes">.        
-00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002120: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
-00002130: 6e20 636c 6173 733d 2266 6120 6661 2d63  n class="fa fa-c
-00002140: 6c6f 7365 206a 732d 636c 6f73 652d 6472  lose js-close-dr
-00002150: 6f70 646f 776e 2d6d 656e 752d 6368 6563  opdown-menu-chec
-00002160: 6b62 6f78 6573 223e 3c73 7061 6e20 636c  kboxes"><span cl
-00002170: 6173 733d 2273 722d 6f6e 6c79 223e 7b25  ass="sr-only">{%
-00002180: 2074 7261 6e73 2022 436c 6f73 6522 2025   trans "Close" %
-00002190: 7d3c 2f73 7061 6e3e 3c2f 7370 616e 3e0a  }</span></span>.
+00001aa0: 2020 2020 2020 2020 203c 2f75 6c3e 0a20           </ul>. 
+00001ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00001ad0: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001af0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00001b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b10: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00001b20: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00001b30: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00001b40: 6c61 7373 3d22 656d 7074 792d 6669 6c65  lass="empty-file
+00001b50: 722d 6865 6164 6572 2d63 656c 6c22 3e3c  r-header-cell"><
+00001b60: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00001b70: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00001b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b90: 2020 2020 203c 666f 726d 2063 6c61 7373       <form class
+00001ba0: 3d22 6669 6c74 6572 2d66 696c 6573 2d63  ="filter-files-c
+00001bb0: 6f6e 7461 696e 6572 206a 732d 6669 6c74  ontainer js-filt
+00001bc0: 6572 2d66 696c 6573 2d63 6f6e 7461 696e  er-files-contain
+00001bd0: 6572 2220 6163 7469 6f6e 3d22 2e22 206d  er" action="." m
+00001be0: 6574 686f 643d 2267 6574 2220 636c 6173  ethod="get" clas
+00001bf0: 733d 226a 732d 6669 6c65 722d 7365 6172  s="js-filer-sear
+00001c00: 6368 2d66 6f72 6d22 3e0a 2020 2020 2020  ch-form">.      
+00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c20: 2020 3c64 6976 2063 6c61 7373 3d22 6669    <div class="fi
+00001c30: 6c74 6572 2d66 696c 6572 732d 636f 6e74  lter-filers-cont
+00001c40: 6169 6e65 722d 696e 6e65 7222 3e0a 2020  ainer-inner">.  
+00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c60: 2020 2020 2020 2020 2020 3c62 7574 746f            <butto
+00001c70: 6e20 636c 6173 733d 226e 6176 6967 6174  n class="navigat
+00001c80: 6f72 2d62 7574 746f 6e20 6669 6c74 6572  or-button filter
+00001c90: 2d66 696c 6573 2d62 7574 746f 6e22 2074  -files-button" t
+00001ca0: 6974 6c65 3d22 7b25 2074 7261 6e73 2027  itle="{% trans '
+00001cb0: 436c 6963 6b20 6865 7265 2074 6f20 7275  Click here to ru
+00001cc0: 6e20 7365 6172 6368 2066 6f72 2065 6e74  n search for ent
+00001cd0: 6572 6564 2070 6872 6173 6527 2025 7d22  ered phrase' %}"
+00001ce0: 3e3c 7370 616e 2063 6c61 7373 3d22 6963  ><span class="ic
+00001cf0: 6f6e 2066 6120 6661 2d73 6561 7263 6820  on fa fa-search 
+00001d00: 636d 732d 6963 6f6e 2063 6d73 2d69 636f  cms-icon cms-ico
+00001d10: 6e2d 7365 6172 6368 223e 3c2f 7370 616e  n-search"></span
+00001d20: 3e3c 2f62 7574 746f 6e3e 0a20 2020 2020  ></button>.     
+00001d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d40: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00001d50: 733d 2266 696c 7465 722d 7365 6172 6368  s="filter-search
+00001d60: 2d77 7261 7070 6572 223e 0a20 2020 2020  -wrapper">.     
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d80: 2020 2020 2020 2020 2020 207b 2520 6669             {% fi
+00001d90: 6c65 725f 6164 6d69 6e5f 636f 6e74 6578  ler_admin_contex
+00001da0: 745f 6869 6464 656e 5f66 6f72 6d66 6965  t_hidden_formfie
+00001db0: 6c64 7320 257d 0a20 2020 2020 2020 2020  lds %}.         
+00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dd0: 2020 2020 2020 203c 696e 7075 7420 7479         <input ty
+00001de0: 7065 3d22 7465 7874 2220 706c 6163 6568  pe="text" placeh
+00001df0: 6f6c 6465 723d 227b 2520 7472 616e 7320  older="{% trans 
+00001e00: 2753 6561 7263 6827 2025 7d22 2063 6c61  'Search' %}" cla
+00001e10: 7373 3d22 6669 6c74 6572 2d66 696c 6573  ss="filter-files
+00001e20: 2d66 6965 6c64 206a 732d 6669 6c74 6572  -field js-filter
+00001e30: 2d66 696c 6573 2220 7661 6c75 653d 227b  -files" value="{
+00001e40: 7b20 7365 6172 6368 5f73 7472 696e 6720  { search_string 
+00001e50: 7d7d 2220 6e61 6d65 3d22 7122 3e0a 2020  }}" name="q">.  
+00001e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e70: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00001e80: 6976 2063 6c61 7373 3d22 6669 6c65 722d  iv class="filer-
+00001e90: 6472 6f70 646f 776e 2d63 6f6e 7461 696e  dropdown-contain
+00001ea0: 6572 2066 696c 6572 2d64 726f 7064 6f77  er filer-dropdow
+00001eb0: 6e2d 636f 6e74 6169 6e65 722d 646f 776e  n-container-down
+00001ec0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ee0: 2020 2020 2020 203c 6120 6872 6566 3d22         <a href="
+00001ef0: 2322 2064 6174 612d 746f 6767 6c65 3d22  #" data-toggle="
+00001f00: 6669 6c65 722d 6472 6f70 646f 776e 2220  filer-dropdown" 
+00001f10: 6172 6961 2d65 7870 616e 6465 643d 2266  aria-expanded="f
+00001f20: 616c 7365 223e 0a20 2020 2020 2020 2020  alse">.         
+00001f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f40: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001f50: 7370 616e 2063 6c61 7373 3d22 6669 6c65  span class="file
+00001f60: 722d 6963 6f6e 2066 696c 6572 2d69 636f  r-icon filer-ico
+00001f70: 6e2d 6361 7265 742d 646f 776e 2066 6120  n-caret-down fa 
+00001f80: 6661 2d63 6172 6574 2d64 6f77 6e22 3e3c  fa-caret-down"><
+00001f90: 2f73 7061 6e3e 0a20 2020 2020 2020 2020  /span>.         
+00001fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fb0: 2020 2020 2020 2020 2020 203c 2f61 3e0a             </a>.
+00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fe0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00001ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002000: 2020 2020 2020 203c 756c 2063 6c61 7373         <ul class
+00002010: 3d22 6669 6c65 722d 6472 6f70 646f 776e  ="filer-dropdown
+00002020: 2d6d 656e 7520 6669 6c65 722d 6472 6f70  -menu filer-drop
+00002030: 646f 776e 2d6d 656e 752d 6368 6563 6b62  down-menu-checkb
+00002040: 6f78 6573 223e 0a20 2020 2020 2020 2020  oxes">.         
+00002050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002060: 2020 2020 2020 2020 2020 203c 7370 616e             <span
+00002070: 2063 6c61 7373 3d22 6661 2066 612d 636c   class="fa fa-cl
+00002080: 6f73 6520 636d 732d 6963 6f6e 2063 6d73  ose cms-icon cms
+00002090: 2d69 636f 6e2d 636c 6f73 6520 6a73 2d63  -icon-close js-c
+000020a0: 6c6f 7365 2d64 726f 7064 6f77 6e2d 6d65  lose-dropdown-me
+000020b0: 6e75 2d63 6865 636b 626f 7865 7322 3e3c  nu-checkboxes"><
+000020c0: 7370 616e 2063 6c61 7373 3d22 7372 2d6f  span class="sr-o
+000020d0: 6e6c 7922 3e7b 2520 7472 616e 7320 2243  nly">{% trans "C
+000020e0: 6c6f 7365 2220 257d 3c2f 7370 616e 3e3c  lose" %}</span><
+000020f0: 2f73 7061 6e3e 0a20 2020 2020 2020 2020  /span>.         
+00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002110: 2020 2020 2020 2020 2020 203c 6c69 3e0a             <li>.
+00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002140: 2020 2020 2020 2020 3c70 3e7b 2520 7472          <p>{% tr
+00002150: 616e 7320 224c 696d 6974 2220 257d 3c2f  ans "Limit" %}</
+00002160: 703e 0a20 2020 2020 2020 2020 2020 2020  p>.             
+00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002180: 2020 2020 2020 2020 2020 203c 6c61 6265             <labe
+00002190: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
 000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021c0: 2020 2020 3c6c 693e 0a20 2020 2020 2020      <li>.       
-000021d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021f0: 203c 703e 7b25 2074 7261 6e73 2022 4c69   <p>{% trans "Li
-00002200: 6d69 7422 2025 7d3c 2f70 3e0a 2020 2020  mit" %}</p>.    
+000021b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000021c0: 696e 7075 7420 7479 7065 3d22 6368 6563  input type="chec
+000021d0: 6b62 6f78 2220 6964 3d22 6c69 6d69 745f  kbox" id="limit_
+000021e0: 7365 6172 6368 5f74 6f5f 666f 6c64 6572  search_to_folder
+000021f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00002200: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002230: 2020 2020 3c6c 6162 656c 3e0a 2020 2020      <label>.    
+00002220: 206e 616d 653d 226c 696d 6974 5f73 6561   name="limit_sea
+00002230: 7263 685f 746f 5f66 6f6c 6465 7222 0a20  rch_to_folder". 
 00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002260: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
-00002270: 7970 653d 2263 6865 636b 626f 7822 2069  ype="checkbox" i
-00002280: 643d 226c 696d 6974 5f73 6561 7263 685f  d="limit_search_
-00002290: 746f 5f66 6f6c 6465 7222 0a20 2020 2020  to_folder".     
-000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002260: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00002270: 2069 6620 6c69 6d69 745f 7365 6172 6368   if limit_search
+00002280: 5f74 6f5f 666f 6c64 6572 2025 7d63 6865  _to_folder %}che
+00002290: 636b 6564 3d22 6368 6563 6b65 6422 7b25  cked="checked"{%
+000022a0: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
 000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022c0: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
-000022d0: 6c69 6d69 745f 7365 6172 6368 5f74 6f5f  limit_search_to_
-000022e0: 666f 6c64 6572 220a 2020 2020 2020 2020  folder".        
-000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002310: 2020 2020 2020 207b 2520 6966 206c 696d         {% if lim
-00002320: 6974 5f73 6561 7263 685f 746f 5f66 6f6c  it_search_to_fol
-00002330: 6465 7220 257d 6368 6563 6b65 643d 2263  der %}checked="c
-00002340: 6865 636b 6564 227b 2520 656e 6469 6620  hecked"{% endif 
-00002350: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002380: 2020 7469 746c 653d 227b 2520 7472 616e    title="{% tran
-00002390: 7320 2743 6865 636b 2069 7420 746f 206c  s 'Check it to l
-000023a0: 696d 6974 2074 6865 2073 6561 7263 6820  imit the search 
-000023b0: 746f 2063 7572 7265 6e74 2066 6f6c 6465  to current folde
-000023c0: 7227 2025 7d22 3e0a 2020 2020 2020 2020  r' %}">.        
-000023d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022d0: 2020 2020 2020 2020 2074 6974 6c65 3d22           title="
+000022e0: 7b25 2074 7261 6e73 2027 4368 6563 6b20  {% trans 'Check 
+000022f0: 6974 2074 6f20 6c69 6d69 7420 7468 6520  it to limit the 
+00002300: 7365 6172 6368 2074 6f20 6375 7272 656e  search to curren
+00002310: 7420 666f 6c64 6572 2720 257d 223e 0a20  t folder' %}">. 
+00002320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002340: 2020 2020 2020 2020 2020 207b 2520 7472             {% tr
+00002350: 616e 7320 224c 696d 6974 2074 6865 2073  ans "Limit the s
+00002360: 6561 7263 6820 746f 2063 7572 7265 6e74  earch to current
+00002370: 2066 6f6c 6465 7222 2025 7d0a 2020 2020   folder" %}.    
+00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023a0: 2020 2020 3c2f 6c61 6265 6c3e 0a20 2020      </label>.   
+000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023d0: 203c 2f6c 693e 0a20 2020 2020 2020 2020   </li>.         
 000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023f0: 2020 2020 7b25 2074 7261 6e73 2022 4c69      {% trans "Li
-00002400: 6d69 7420 7468 6520 7365 6172 6368 2074  mit the search t
-00002410: 6f20 6375 7272 656e 7420 666f 6c64 6572  o current folder
-00002420: 2220 257d 0a20 2020 2020 2020 2020 2020  " %}.           
-00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002440: 2020 2020 2020 2020 2020 2020 203c 2f6c               </l
-00002450: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
-00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002470: 2020 2020 2020 2020 2020 3c2f 6c69 3e0a            </li>.
-00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024a0: 3c2f 756c 3e0a 2020 2020 2020 2020 2020  </ul>.          
-000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024c0: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024e0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-000024f0: 2020 2020 2020 2020 3c2f 666f 726d 3e0a          </form>.
-00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002510: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00002520: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00002530: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00002540: 3d22 746f 6f6c 732d 636f 6e74 6169 6e65  ="tools-containe
-00002550: 7222 3e0a 2020 2020 2020 2020 2020 2020  r">.            
-00002560: 2020 2020 7b25 2062 6c6f 636b 206f 626a      {% block obj
-00002570: 6563 742d 746f 6f6c 7320 257d 0a20 2020  ect-tools %}.   
-00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002590: 203c 6469 7620 636c 6173 733d 226e 6176   <div class="nav
-000025a0: 6967 6174 6f72 2d74 6f6f 6c73 223e 0a20  igator-tools">. 
-000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025c0: 2020 2020 2020 207b 2520 6966 206e 6f74         {% if not
-000025d0: 2069 735f 706f 7075 7020 257d 0a20 2020   is_popup %}.   
+000023f0: 2020 2020 2020 203c 2f75 6c3e 0a20 2020         </ul>.   
+00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002410: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002430: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00002440: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002450: 2f66 6f72 6d3e 0a20 2020 2020 2020 2020  /form>.         
+00002460: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00002470: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00002480: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
+00002490: 7620 636c 6173 733d 2274 6f6f 6c73 2d63  v class="tools-c
+000024a0: 6f6e 7461 696e 6572 223e 0a20 2020 2020  ontainer">.     
+000024b0: 2020 2020 2020 2020 2020 207b 2520 626c             {% bl
+000024c0: 6f63 6b20 6f62 6a65 6374 2d74 6f6f 6c73  ock object-tools
+000024d0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000024e0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000024f0: 7373 3d22 6e61 7669 6761 746f 722d 746f  ss="navigator-to
+00002500: 6f6c 7322 3e0a 2020 2020 2020 2020 2020  ols">.          
+00002510: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00002520: 2069 6620 6e6f 7420 6973 5f70 6f70 7570   if not is_popup
+00002530: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002550: 3c64 6976 2063 6c61 7373 3d22 6163 7469  <div class="acti
+00002560: 6f6e 732d 7772 6170 7065 7222 3e0a 2020  ons-wrapper">.  
+00002570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002580: 2020 2020 2020 2020 2020 2020 2020 3c75                <u
+00002590: 6c20 636c 6173 733d 2261 6374 696f 6e73  l class="actions
+000025a0: 2d73 6570 6172 6174 6564 2d6c 6973 7422  -separated-list"
+000025b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025d0: 2020 2020 2020 3c6c 693e 0a20 2020 2020        <li>.     
 000025e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025f0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00002600: 6173 733d 2261 6374 696f 6e73 2d77 7261  ass="actions-wra
-00002610: 7070 6572 223e 0a20 2020 2020 2020 2020  pper">.         
-00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002630: 2020 2020 2020 203c 756c 2063 6c61 7373         <ul class
-00002640: 3d22 6163 7469 6f6e 732d 7365 7061 7261  ="actions-separa
-00002650: 7465 642d 6c69 7374 223e 0a20 2020 2020  ted-list">.     
-00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002670: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002680: 6c69 3e0a 2020 2020 2020 2020 2020 2020  li>.            
+000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002600: 2020 203c 6120 6872 6566 3d22 2322 2063     <a href="#" c
+00002610: 6c61 7373 3d22 6a73 2d61 6374 696f 6e2d  lass="js-action-
+00002620: 6465 6c65 7465 2220 7469 746c 653d 227b  delete" title="{
+00002630: 2520 7472 616e 7320 2744 656c 6574 6527  % trans 'Delete'
+00002640: 2025 7d22 3e3c 7370 616e 2063 6c61 7373   %}"><span class
+00002650: 3d22 6661 2066 612d 7472 6173 6820 636d  ="fa fa-trash cm
+00002660: 732d 6963 6f6e 2063 6d73 2d69 636f 6e2d  s-icon cms-icon-
+00002670: 6269 6e22 3e3c 2f73 7061 6e3e 3c2f 613e  bin"></span></a>
+00002680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00002690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026a0: 2020 2020 2020 2020 2020 2020 3c61 2068              <a h
-000026b0: 7265 663d 2223 2220 636c 6173 733d 226a  ref="#" class="j
-000026c0: 732d 6163 7469 6f6e 2d64 656c 6574 6522  s-action-delete"
-000026d0: 2074 6974 6c65 3d22 7b25 2074 7261 6e73   title="{% trans
-000026e0: 2027 4465 6c65 7465 2720 257d 223e 3c73   'Delete' %}"><s
-000026f0: 7061 6e20 636c 6173 733d 2266 6120 6661  pan class="fa fa
-00002700: 2d74 7261 7368 223e 3c2f 7370 616e 3e3c  -trash"></span><
-00002710: 2f61 3e0a 2020 2020 2020 2020 2020 2020  /a>.            
-00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002730: 2020 2020 2020 2020 3c2f 6c69 3e0a 2020          </li>.  
-00002740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002760: 2020 3c6c 693e 0a20 2020 2020 2020 2020    <li>.         
-00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002780: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002790: 6120 6872 6566 3d22 2322 2063 6c61 7373  a href="#" class
-000027a0: 3d22 6a73 2d61 6374 696f 6e2d 636f 7079  ="js-action-copy
-000027b0: 2220 7469 746c 653d 227b 2520 7472 616e  " title="{% tran
-000027c0: 7320 2743 6f70 7927 2025 7d22 3e3c 7370  s 'Copy' %}"><sp
-000027d0: 616e 2063 6c61 7373 3d22 6661 2066 612d  an class="fa fa-
-000027e0: 636f 7079 223e 3c2f 7370 616e 3e3c 2f61  copy"></span></a
-000027f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002810: 2020 2020 2020 3c2f 6c69 3e0a 2020 2020        </li>.    
-00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002840: 3c6c 693e 0a20 2020 2020 2020 2020 2020  <li>.           
-00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002860: 2020 2020 2020 2020 2020 2020 203c 6120               <a 
-00002870: 6872 6566 3d22 2322 2063 6c61 7373 3d22  href="#" class="
-00002880: 6a73 2d61 6374 696f 6e2d 6d6f 7665 2220  js-action-move" 
-00002890: 7469 746c 653d 227b 2520 7472 616e 7320  title="{% trans 
-000028a0: 274d 6f76 6527 2025 7d22 3e3c 7370 616e  'Move' %}"><span
-000028b0: 2063 6c61 7373 3d22 6661 2066 612d 6375   class="fa fa-cu
-000028c0: 7422 3e3c 2f73 7061 6e3e 3c2f 613e 0a20  t"></span></a>. 
-000028d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026a0: 2020 2020 203c 2f6c 693e 0a20 2020 2020       </li>.     
+000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000026d0: 6c69 3e0a 2020 2020 2020 2020 2020 2020  li>.            
+000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026f0: 2020 2020 2020 2020 2020 2020 3c61 2068              <a h
+00002700: 7265 663d 2223 2220 636c 6173 733d 226a  ref="#" class="j
+00002710: 732d 6163 7469 6f6e 2d63 6f70 7922 2074  s-action-copy" t
+00002720: 6974 6c65 3d22 7b25 2074 7261 6e73 2027  itle="{% trans '
+00002730: 436f 7079 2720 257d 223e 3c73 7061 6e20  Copy' %}"><span 
+00002740: 636c 6173 733d 2266 6120 6661 2d63 6f70  class="fa fa-cop
+00002750: 7920 636d 732d 6963 6f6e 2063 6d73 2d69  y cms-icon cms-i
+00002760: 636f 6e2d 636f 7079 2066 6120 6661 2d63  con-copy fa fa-c
+00002770: 6f70 7922 3e3c 2f73 7061 6e3e 3c2f 613e  opy"></span></a>
+00002780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027a0: 2020 2020 203c 2f6c 693e 0a20 2020 2020       </li>.     
+000027b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000027d0: 6c69 3e0a 2020 2020 2020 2020 2020 2020  li>.            
+000027e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027f0: 2020 2020 2020 2020 2020 2020 3c61 2068              <a h
+00002800: 7265 663d 2223 2220 636c 6173 733d 226a  ref="#" class="j
+00002810: 732d 6163 7469 6f6e 2d6d 6f76 6522 2074  s-action-move" t
+00002820: 6974 6c65 3d22 7b25 2074 7261 6e73 2027  itle="{% trans '
+00002830: 4d6f 7665 2720 257d 223e 3c73 7061 6e20  Move' %}"><span 
+00002840: 636c 6173 733d 2266 6120 6661 2d66 6f6c  class="fa fa-fol
+00002850: 6465 7220 6669 6c65 722d 6963 6f6e 2066  der filer-icon f
+00002860: 696c 6572 2d69 636f 6e2d 6d6f 7665 2d74  iler-icon-move-t
+00002870: 6f2d 666f 6c64 6572 2066 6120 6661 2d63  o-folder fa fa-c
+00002880: 7574 223e 3c2f 7370 616e 3e3c 2f61 3e0a  ut"></span></a>.
+00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028b0: 2020 2020 3c2f 6c69 3e0a 2020 2020 2020      </li>.      
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 2020 2020 2020 2020 2020 3c2f 756c 3e0a            </ul>.
 000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028f0: 2020 203c 2f6c 693e 0a20 2020 2020 2020     </li>.       
-00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002910: 2020 2020 2020 2020 203c 2f75 6c3e 0a20           </ul>. 
-00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002930: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002940: 6469 7620 636c 6173 733d 2266 696c 6572  div class="filer
-00002950: 2d64 726f 7064 6f77 6e2d 636f 6e74 6169  -dropdown-contai
-00002960: 6e65 7220 6a73 2d61 6374 696f 6e73 2d6d  ner js-actions-m
-00002970: 656e 7522 3e0a 2020 2020 2020 2020 2020  enu">.          
-00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002990: 2020 2020 2020 2020 2020 3c61 2068 7265            <a hre
-000029a0: 663d 2223 2220 6461 7461 2d74 6f67 676c  f="#" data-toggl
-000029b0: 653d 2266 696c 6572 2d64 726f 7064 6f77  e="filer-dropdow
-000029c0: 6e22 2061 7269 612d 6578 7061 6e64 6564  n" aria-expanded
-000029d0: 3d22 6661 6c73 6522 2063 6c61 7373 3d22  ="false" class="
-000029e0: 6e61 762d 6275 7474 6f6e 206e 6176 2d62  nav-button nav-b
-000029f0: 7574 746f 6e2d 646f 7473 223e 0a20 2020  utton-dots">.   
-00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a20: 2020 2020 203c 7370 616e 2063 6c61 7373       <span class
-00002a30: 3d22 6661 2066 612d 656c 6c69 7073 6973  ="fa fa-ellipsis
-00002a40: 2d68 223e 3c2f 7370 616e 3e0a 2020 2020  -h"></span>.    
+000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002900: 3c64 6976 2063 6c61 7373 3d22 6669 6c65  <div class="file
+00002910: 722d 6472 6f70 646f 776e 2d63 6f6e 7461  r-dropdown-conta
+00002920: 696e 6572 206a 732d 6163 7469 6f6e 732d  iner js-actions-
+00002930: 6d65 6e75 223e 0a20 2020 2020 2020 2020  menu">.         
+00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002950: 2020 2020 2020 2020 2020 203c 6120 6872             <a hr
+00002960: 6566 3d22 2322 2064 6174 612d 746f 6767  ef="#" data-togg
+00002970: 6c65 3d22 6669 6c65 722d 6472 6f70 646f  le="filer-dropdo
+00002980: 776e 2220 6172 6961 2d65 7870 616e 6465  wn" aria-expande
+00002990: 643d 2266 616c 7365 2220 636c 6173 733d  d="false" class=
+000029a0: 226e 6176 2d62 7574 746f 6e20 6e61 762d  "nav-button nav-
+000029b0: 6275 7474 6f6e 2d64 6f74 7322 3e0a 2020  button-dots">.  
+000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029e0: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
+000029f0: 733d 2266 6120 6661 2d65 6c6c 6970 7369  s="fa fa-ellipsi
+00002a00: 732d 6820 636d 732d 6963 6f6e 2063 6d73  s-h cms-icon cms
+00002a10: 2d69 636f 6e2d 6d65 6e75 223e 3c2f 7370  -icon-menu"></sp
+00002a20: 616e 3e0a 2020 2020 2020 2020 2020 2020  an>.            
+00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a40: 2020 2020 2020 2020 3c2f 613e 0a20 2020          </a>.   
 00002a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 3c2f 613e 0a20 2020 2020 2020 2020 2020  </a>.           
-00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a90: 2020 2020 2020 2020 203c 756c 2063 6c61           <ul cla
-00002aa0: 7373 3d22 6372 6561 7465 2d6d 656e 752d  ss="create-menu-
-00002ab0: 6472 6f70 646f 776e 2066 696c 6572 2d64  dropdown filer-d
-00002ac0: 726f 7064 6f77 6e2d 6d65 6e75 223e 0a20  ropdown-menu">. 
-00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002af0: 2020 2020 2020 207b 2320 5468 6973 206c         {# This l
-00002b00: 6973 7420 6973 2070 6f70 756c 6174 6564  ist is populated
-00002b10: 2069 6e20 6a61 7661 7363 7269 7074 2023   in javascript #
-00002b20: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00002a70: 203c 756c 2063 6c61 7373 3d22 6372 6561   <ul class="crea
+00002a80: 7465 2d6d 656e 752d 6472 6f70 646f 776e  te-menu-dropdown
+00002a90: 2066 696c 6572 2d64 726f 7064 6f77 6e2d   filer-dropdown-
+00002aa0: 6d65 6e75 223e 0a20 2020 2020 2020 2020  menu">.         
+00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00002ad0: 2320 5468 6973 206c 6973 7420 6973 2070  # This list is p
+00002ae0: 6f70 756c 6174 6564 2069 6e20 6a61 7661  opulated in java
+00002af0: 7363 7269 7074 2023 7d0a 2020 2020 2020  script #}.      
+00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b10: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00002b20: 756c 3e0a 2020 2020 2020 2020 2020 2020  ul>.            
 00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b40: 2020 2020 2020 3c2f 756c 3e0a 2020 2020        </ul>.    
+00002b40: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
 00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b60: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00002b70: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00002b80: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002b90: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00002ba0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00002bb0: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bd0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00002be0: 3d22 6669 6c65 722d 6c69 7374 2d74 7970  ="filer-list-typ
-00002bf0: 652d 7377 6974 6368 6572 2d77 7261 7070  e-switcher-wrapp
-00002c00: 6572 223e 0a20 2020 2020 2020 2020 2020  er">.           
-00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c20: 2020 207b 2520 6669 6c65 725f 666f 6c64     {% filer_fold
-00002c30: 6572 5f6c 6973 745f 7479 7065 5f73 7769  er_list_type_swi
-00002c40: 7463 6865 7220 257d 0a20 2020 2020 2020  tcher %}.       
-00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c60: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00002b60: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00002b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b80: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00002b90: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00002ba0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00002bb0: 6c61 7373 3d22 6669 6c65 722d 6c69 7374  lass="filer-list
+00002bc0: 2d74 7970 652d 7377 6974 6368 6572 2d77  -type-switcher-w
+00002bd0: 7261 7070 6572 223e 0a20 2020 2020 2020  rapper">.       
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bf0: 2020 2020 203c 756c 2063 6c61 7373 3d22       <ul class="
+00002c00: 6163 7469 6f6e 732d 7365 7061 7261 7465  actions-separate
+00002c10: 642d 6c69 7374 223e 0a20 2020 2020 2020  d-list">.       
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c30: 2020 2020 2020 2020 203c 6c69 3e7b 2520           <li>{% 
+00002c40: 6669 6c65 725f 666f 6c64 6572 5f6c 6973  filer_folder_lis
+00002c50: 745f 7479 7065 5f73 7769 7463 6865 7220  t_type_switcher 
+00002c60: 257d 3c2f 6c69 3e0a 2020 2020 2020 2020  %}</li>.        
 00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c80: 2020 2020 7b25 2062 6c6f 636b 206f 626a      {% block obj
-00002c90: 6563 742d 746f 6f6c 732d 6974 656d 7320  ect-tools-items 
-00002ca0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00002cb0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002cc0: 6469 7620 636c 6173 733d 226e 6176 6967  div class="navig
-00002cd0: 6174 6f72 2d62 7574 746f 6e2d 7772 6170  ator-button-wrap
-00002ce0: 7065 7222 3e0a 2020 2020 2020 2020 2020  per">.          
-00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d00: 2020 2020 2020 7b25 2069 6620 666f 6c64        {% if fold
-00002d10: 6572 2e63 616e 5f68 6176 655f 7375 6266  er.can_have_subf
-00002d20: 6f6c 6465 7273 2061 6e64 2063 616e 5f6d  olders and can_m
-00002d30: 616b 655f 666f 6c64 6572 2025 7d0a 2020  ake_folder %}.  
-00002d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d60: 2020 3c61 2068 7265 663d 227b 2520 7572    <a href="{% ur
-00002d70: 6c20 2761 646d 696e 3a66 696c 6572 2d64  l 'admin:filer-d
-00002d80: 6972 6563 746f 7279 5f6c 6973 7469 6e67  irectory_listing
-00002d90: 2d6d 616b 655f 726f 6f74 5f66 6f6c 6465  -make_root_folde
-00002da0: 7227 2025 7d3f 7061 7265 6e74 5f69 643d  r' %}?parent_id=
-00002db0: 7b7b 2066 6f6c 6465 722e 6964 207d 7d7b  {{ folder.id }}{
-00002dc0: 2520 6966 2069 735f 706f 7075 7020 257d  % if is_popup %}
-00002dd0: 2661 6d70 3b5f 706f 7075 703d 317b 2520  &amp;_popup=1{% 
-00002de0: 656e 6469 6620 257d 220a 2020 2020 2020  endif %}".      
-00002df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e10: 2020 7469 746c 653d 227b 2520 7472 616e    title="{% tran
-00002e20: 7320 2741 6464 7320 6120 6e65 7720 466f  s 'Adds a new Fo
-00002e30: 6c64 6572 2720 257d 220a 2020 2020 2020  lder' %}".      
+00002c80: 2020 2020 3c2f 756c 3e0a 2020 2020 2020      </ul>.      
+00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ca0: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cc0: 207b 2520 626c 6f63 6b20 6f62 6a65 6374   {% block object
+00002cd0: 2d74 6f6f 6c73 2d69 7465 6d73 2025 7d0a  -tools-items %}.
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cf0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00002d00: 2063 6c61 7373 3d22 6e61 7669 6761 746f   class="navigato
+00002d10: 722d 6275 7474 6f6e 2d77 7261 7070 6572  r-button-wrapper
+00002d20: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d40: 2020 207b 2520 6966 2066 6f6c 6465 722e     {% if folder.
+00002d50: 6361 6e5f 6861 7665 5f73 7562 666f 6c64  can_have_subfold
+00002d60: 6572 7320 616e 6420 6361 6e5f 6d61 6b65  ers and can_make
+00002d70: 5f66 6f6c 6465 7220 257d 0a20 2020 2020  _folder %}.     
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d90: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002da0: 6120 6872 6566 3d22 7b25 2075 726c 2027  a href="{% url '
+00002db0: 6164 6d69 6e3a 6669 6c65 722d 6469 7265  admin:filer-dire
+00002dc0: 6374 6f72 795f 6c69 7374 696e 672d 6d61  ctory_listing-ma
+00002dd0: 6b65 5f72 6f6f 745f 666f 6c64 6572 2720  ke_root_folder' 
+00002de0: 257d 3f70 6172 656e 745f 6964 3d7b 7b20  %}?parent_id={{ 
+00002df0: 666f 6c64 6572 2e70 6b7c 7361 6665 207d  folder.pk|safe }
+00002e00: 7d7b 2520 6966 2069 735f 706f 7075 7020  }{% if is_popup 
+00002e10: 257d 2661 6d70 3b5f 706f 7075 703d 317b  %}&amp;_popup=1{
+00002e20: 2520 656e 6469 6620 257d 220a 2020 2020  % endif %}".    
+00002e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e60: 2020 636c 6173 733d 226e 6176 6967 6174    class="navigat
-00002e70: 6f72 2d62 7574 746f 6e22 0a20 2020 2020  or-button".     
+00002e50: 2020 2020 7469 746c 653d 227b 2520 7472      title="{% tr
+00002e60: 616e 7320 2741 6464 7320 6120 6e65 7720  ans 'Adds a new 
+00002e70: 466f 6c64 6572 2720 257d 220a 2020 2020  Folder' %}".    
 00002e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ea0: 2020 206f 6e63 6c69 636b 3d22 7265 7475     onclick="retu
-00002eb0: 726e 2073 686f 7741 6464 416e 6f74 6865  rn showAddAnothe
-00002ec0: 7250 6f70 7570 2874 6869 7329 3b22 3e0a  rPopup(this);">.
+00002ea0: 2020 2020 636c 6173 733d 226e 6176 6967      class="navig
+00002eb0: 6174 6f72 2d62 7574 746f 6e22 0a20 2020  ator-button".   
+00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ef0: 2020 2020 2020 2020 7b25 2074 7261 6e73          {% trans
-00002f00: 2022 4e65 7720 466f 6c64 6572 2220 257d   "New Folder" %}
-00002f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002ee0: 2020 2020 206f 6e63 6c69 636b 3d22 7265       onclick="re
+00002ef0: 7475 726e 2073 686f 7741 6464 416e 6f74  turn showAddAnot
+00002f00: 6865 7250 6f70 7570 2874 6869 7329 3b22  herPopup(this);"
+00002f10: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
 00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f30: 2020 2020 203c 2f61 3e0a 2020 2020 2020       </a>.      
-00002f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f50: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-00002f60: 6966 2025 7d0a 0a20 2020 2020 2020 2020  if %}..         
-00002f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f80: 2020 2020 2020 207b 2520 6966 2070 6572         {% if per
-00002f90: 6d69 7373 696f 6e73 2e68 6173 5f61 6464  missions.has_add
-00002fa0: 5f63 6869 6c64 7265 6e5f 7065 726d 6973  _children_permis
-00002fb0: 7369 6f6e 2061 6e64 206e 6f74 2066 6f6c  sion and not fol
-00002fc0: 6465 722e 6973 5f72 6f6f 7420 257d 0a20  der.is_root %}. 
-00002fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ff0: 2020 203c 6120 6872 6566 3d22 2322 2069     <a href="#" i
-00003000: 643d 2269 645f 7570 6c6f 6164 5f62 7574  d="id_upload_but
-00003010: 746f 6e22 2074 6974 6c65 3d22 7b25 2074  ton" title="{% t
-00003020: 7261 6e73 2027 5570 6c6f 6164 2046 696c  rans 'Upload Fil
-00003030: 6573 2720 257d 220a 2020 2020 2020 2020  es' %}".        
-00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003050: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003060: 6c61 7373 3d22 6e61 7669 6761 746f 722d  lass="navigator-
-00003070: 6275 7474 6f6e 206e 6176 6967 6174 6f72  button navigator
-00003080: 2d62 7574 746f 6e2d 7570 6c6f 6164 206a  -button-upload j
-00003090: 732d 7570 6c6f 6164 2d62 7574 746f 6e22  s-upload-button"
-000030a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030c0: 2020 2020 2020 2020 6461 7461 2d75 726c          data-url
-000030d0: 3d22 7b25 2075 726c 2027 6164 6d69 6e3a  ="{% url 'admin:
-000030e0: 6669 6c65 722d 616a 6178 5f75 706c 6f61  filer-ajax_uploa
-000030f0: 6427 2066 6f6c 6465 725f 6964 3d66 6f6c  d' folder_id=fol
-00003100: 6465 722e 6964 2025 7d22 0a20 2020 2020  der.id %}".     
-00003110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003130: 2020 6461 7461 2d6d 6178 2d75 706c 6f61    data-max-uploa
-00003140: 6465 722d 636f 6e6e 6563 7469 6f6e 733d  der-connections=
-00003150: 227b 7b20 7570 6c6f 6164 6572 5f63 6f6e  "{{ uploader_con
-00003160: 6e65 6374 696f 6e73 207d 7d22 3e0a 2020  nections }}">.  
-00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003190: 2020 2020 2020 7b25 2074 7261 6e73 2022        {% trans "
-000031a0: 5570 6c6f 6164 2046 696c 6573 2220 257d  Upload Files" %}
-000031b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002f30: 2020 2020 2020 2020 2020 7b25 2074 7261            {% tra
+00002f40: 6e73 2022 4e65 7720 466f 6c64 6572 2220  ns "New Folder" 
+00002f50: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00002f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f70: 2020 2020 2020 203c 2f61 3e0a 2020 2020         </a>.    
+00002f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f90: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00002fa0: 6e64 6966 2025 7d0a 0a20 2020 2020 2020  ndif %}..       
+00002fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fc0: 2020 2020 2020 2020 207b 2520 6966 2070           {% if p
+00002fd0: 6572 6d69 7373 696f 6e73 2e68 6173 5f61  ermissions.has_a
+00002fe0: 6464 5f63 6869 6c64 7265 6e5f 7065 726d  dd_children_perm
+00002ff0: 6973 7369 6f6e 2061 6e64 206e 6f74 2066  ission and not f
+00003000: 6f6c 6465 722e 6973 5f72 6f6f 7420 257d  older.is_root %}
+00003010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003030: 2020 2020 203c 6120 6872 6566 3d22 2322       <a href="#"
+00003040: 2069 643d 2269 645f 7570 6c6f 6164 5f62   id="id_upload_b
+00003050: 7574 746f 6e22 2074 6974 6c65 3d22 7b25  utton" title="{%
+00003060: 2074 7261 6e73 2027 5570 6c6f 6164 2046   trans 'Upload F
+00003070: 696c 6573 2720 257d 220a 2020 2020 2020  iles' %}".      
+00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030a0: 2063 6c61 7373 3d22 6e61 7669 6761 746f   class="navigato
+000030b0: 722d 6275 7474 6f6e 206e 6176 6967 6174  r-button navigat
+000030c0: 6f72 2d62 7574 746f 6e2d 7570 6c6f 6164  or-button-upload
+000030d0: 206a 732d 7570 6c6f 6164 2d62 7574 746f   js-upload-butto
+000030e0: 6e22 0a20 2020 2020 2020 2020 2020 2020  n".             
+000030f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003100: 2020 2020 2020 2020 2020 6461 7461 2d75            data-u
+00003110: 726c 3d22 7b25 2075 726c 2027 6164 6d69  rl="{% url 'admi
+00003120: 6e3a 6669 6c65 722d 616a 6178 5f75 706c  n:filer-ajax_upl
+00003130: 6f61 6427 2066 6f6c 6465 725f 6964 3d66  oad' folder_id=f
+00003140: 6f6c 6465 722e 6964 2025 7d22 0a20 2020  older.id %}".   
+00003150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003170: 2020 2020 6461 7461 2d6d 6178 2d75 706c      data-max-upl
+00003180: 6f61 6465 722d 636f 6e6e 6563 7469 6f6e  oader-connection
+00003190: 733d 227b 7b20 7570 6c6f 6164 6572 5f63  s="{{ uploader_c
+000031a0: 6f6e 6e65 6374 696f 6e73 207d 7d22 0a20  onnections }}". 
+000031b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031d0: 2020 2020 203c 2f61 3e0a 2020 2020 2020       </a>.      
-000031e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031f0: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
-00003200: 6620 666f 6c64 6572 2e69 735f 756e 736f  f folder.is_unso
-00003210: 7274 6564 5f75 706c 6f61 6473 2025 7d0a  rted_uploads %}.
-00003220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003240: 2020 2020 3c61 2068 7265 663d 2223 2220      <a href="#" 
-00003250: 6964 3d22 6964 5f75 706c 6f61 645f 6275  id="id_upload_bu
-00003260: 7474 6f6e 2220 7469 746c 653d 227b 2520  tton" title="{% 
-00003270: 7472 616e 7320 2755 706c 6f61 6420 4669  trans 'Upload Fi
-00003280: 6c65 7327 2025 7d22 0a20 2020 2020 2020  les' %}".       
-00003290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031d0: 2020 2020 2020 6461 7461 2d6d 6178 2d66        data-max-f
+000031e0: 696c 6573 3d22 7b7b 206d 6178 5f66 696c  iles="{{ max_fil
+000031f0: 6573 7c73 6166 6520 7d7d 220a 2020 2020  es|safe }}".    
+00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003220: 2020 207b 2520 6966 206d 6178 5f66 696c     {% if max_fil
+00003230: 6573 697a 6520 257d 7d64 6174 612d 6d61  esize %}}data-ma
+00003240: 782d 6669 6c65 7369 7a65 3d22 7b7b 206d  x-filesize="{{ m
+00003250: 6178 5f66 696c 6573 697a 657c 7361 6665  ax_filesize|safe
+00003260: 207d 7d22 7b25 2065 6e64 6966 2025 7d0a   }}"{% endif %}.
+00003270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003290: 2020 2020 3e0a 2020 2020 2020 2020 2020      >.          
 000032a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032b0: 636c 6173 733d 226e 6176 6967 6174 6f72  class="navigator
-000032c0: 2d62 7574 746f 6e20 6e61 7669 6761 746f  -button navigato
-000032d0: 722d 6275 7474 6f6e 2d75 706c 6f61 6420  r-button-upload 
-000032e0: 6a73 2d75 706c 6f61 642d 6275 7474 6f6e  js-upload-button
-000032f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00003300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003310: 2020 2020 2020 2020 2064 6174 612d 7572           data-ur
-00003320: 6c3d 227b 2520 7572 6c20 2761 646d 696e  l="{% url 'admin
-00003330: 3a66 696c 6572 2d61 6a61 785f 7570 6c6f  :filer-ajax_uplo
-00003340: 6164 2720 257d 220a 2020 2020 2020 2020  ad' %}".        
+000032b0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000032c0: 2074 7261 6e73 2022 5570 6c6f 6164 2046   trans "Upload F
+000032d0: 696c 6573 2220 257d 0a20 2020 2020 2020  iles" %}.       
+000032e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032f0: 2020 2020 2020 2020 2020 2020 203c 2f61               </a
+00003300: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00003310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003320: 2020 7b25 2065 6c69 6620 666f 6c64 6572    {% elif folder
+00003330: 2e69 735f 756e 736f 7274 6564 5f75 706c  .is_unsorted_upl
+00003340: 6f61 6473 2025 7d0a 2020 2020 2020 2020  oads %}.        
 00003350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003360: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00003370: 6174 612d 6d61 782d 7570 6c6f 6164 6572  ata-max-uploader
-00003380: 2d63 6f6e 6e65 6374 696f 6e73 3d22 7b7b  -connections="{{
-00003390: 2075 706c 6f61 6465 725f 636f 6e6e 6563   uploader_connec
-000033a0: 7469 6f6e 7320 7d7d 223e 0a20 2020 2020  tions }}">.     
-000033b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003360: 2020 2020 2020 2020 2020 2020 3c61 2068              <a h
+00003370: 7265 663d 2223 2220 6964 3d22 6964 5f75  ref="#" id="id_u
+00003380: 706c 6f61 645f 6275 7474 6f6e 2220 7469  pload_button" ti
+00003390: 746c 653d 227b 2520 7472 616e 7320 2755  tle="{% trans 'U
+000033a0: 706c 6f61 6420 4669 6c65 7327 2025 7d22  pload Files' %}"
+000033b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000033c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033d0: 2020 207b 2520 7472 616e 7320 2255 706c     {% trans "Upl
-000033e0: 6f61 6420 4669 6c65 7322 2025 7d0a 2020  oad Files" %}.  
-000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003410: 2020 3c2f 613e 0a20 2020 2020 2020 2020    </a>.         
+000033d0: 2020 2020 2020 2020 636c 6173 733d 226e          class="n
+000033e0: 6176 6967 6174 6f72 2d62 7574 746f 6e20  avigator-button 
+000033f0: 6e61 7669 6761 746f 722d 6275 7474 6f6e  navigator-button
+00003400: 2d75 706c 6f61 6420 6a73 2d75 706c 6f61  -upload js-uploa
+00003410: 642d 6275 7474 6f6e 220a 2020 2020 2020  d-button".      
 00003420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003430: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-00003440: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00003450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003460: 2020 207b 2520 6966 2066 6f6c 6465 722e     {% if folder.
-00003470: 6973 5f72 6f6f 7420 616e 6420 6e6f 7420  is_root and not 
-00003480: 666f 6c64 6572 2e69 735f 756e 736f 7274  folder.is_unsort
-00003490: 6564 5f75 706c 6f61 6473 2025 7d0a 2020  ed_uploads %}.  
-000034a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034c0: 2020 3c73 7061 6e20 636c 6173 733d 226a    <span class="j
-000034d0: 732d 7570 6c6f 6164 2d62 7574 746f 6e2d  s-upload-button-
-000034e0: 6469 7361 626c 6564 2075 706c 6f61 642d  disabled upload-
-000034f0: 6275 7474 6f6e 2d64 6973 6162 6c65 6420  button-disabled 
-00003500: 6a73 2d66 696c 6572 2d74 6f6f 6c74 6970  js-filer-tooltip
-00003510: 2066 696c 6572 2d74 6f6f 6c74 6970 2d77   filer-tooltip-w
-00003520: 7261 7070 6572 220a 2020 2020 2020 2020  rapper".        
+00003430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003440: 2064 6174 612d 7572 6c3d 227b 2520 7572   data-url="{% ur
+00003450: 6c20 2761 646d 696e 3a66 696c 6572 2d61  l 'admin:filer-a
+00003460: 6a61 785f 7570 6c6f 6164 2720 257d 220a  jax_upload' %}".
+00003470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003490: 2020 2020 2020 2064 6174 612d 6d61 782d         data-max-
+000034a0: 7570 6c6f 6164 6572 2d63 6f6e 6e65 6374  uploader-connect
+000034b0: 696f 6e73 3d22 7b7b 2075 706c 6f61 6465  ions="{{ uploade
+000034c0: 725f 636f 6e6e 6563 7469 6f6e 7320 7d7d  r_connections }}
+000034d0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034f0: 2020 2020 2020 2020 2064 6174 612d 6d61           data-ma
+00003500: 782d 6669 6c65 733d 227b 7b20 6d61 785f  x-files="{{ max_
+00003510: 6669 6c65 737c 7361 6665 207d 7d22 0a20  files|safe }}". 
+00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003550: 2020 7469 746c 653d 227b 2520 7472 616e    title="{% tran
-00003560: 7320 2759 6f75 2068 6176 6520 746f 2073  s 'You have to s
-00003570: 656c 6563 7420 6120 666f 6c64 6572 2066  elect a folder f
-00003580: 6972 7374 2720 257d 223e 0a20 2020 2020  irst' %}">.     
-00003590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003540: 2020 2020 2020 7b25 2069 6620 6d61 785f        {% if max_
+00003550: 6669 6c65 7369 7a65 2025 7d7d 6461 7461  filesize %}}data
+00003560: 2d6d 6178 2d66 696c 6573 697a 653d 227b  -max-filesize="{
+00003570: 7b20 6d61 785f 6669 6c65 7369 7a65 7c73  { max_filesize|s
+00003580: 6166 6520 7d7d 227b 2520 656e 6469 6620  afe }}"{% endif 
+00003590: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
 000035a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035b0: 2020 203c 6120 6872 6566 3d22 2322 2063     <a href="#" c
-000035c0: 6c61 7373 3d22 6e61 7669 6761 746f 722d  lass="navigator-
-000035d0: 6275 7474 6f6e 206e 6176 6967 6174 6f72  button navigator
-000035e0: 2d62 7574 746f 6e2d 7570 6c6f 6164 2220  -button-upload" 
-000035f0: 6469 7361 626c 6564 3e0a 2020 2020 2020  disabled>.      
+000035b0: 2020 2020 2020 203e 0a20 2020 2020 2020         >.       
+000035c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035e0: 207b 2520 7472 616e 7320 2255 706c 6f61   {% trans "Uploa
+000035f0: 6420 4669 6c65 7322 2025 7d0a 2020 2020  d Files" %}.    
 00003600: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003620: 2020 2020 2020 7b25 2074 7261 6e73 2022        {% trans "
-00003630: 5570 6c6f 6164 2046 696c 6573 2220 257d  Upload Files" %}
-00003640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003660: 2020 2020 2020 2020 203c 2f61 3e0a 2020           </a>.  
-00003670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003690: 2020 3c2f 7370 616e 3e0a 2020 2020 2020    </span>.      
-000036a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036b0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-000036c0: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
-000036d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036e0: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-000036f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003700: 207b 2520 656e 6462 6c6f 636b 2025 7d0a   {% endblock %}.
-00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003720: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00003730: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-00003740: 6462 6c6f 636b 2025 7d0a 2020 2020 2020  dblock %}.      
-00003750: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00003760: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00003770: 3c2f 6469 763e 0a20 2020 203c 6469 7620  </div>.    <div 
-00003780: 6964 3d22 636f 6e74 656e 742d 6d61 696e  id="content-main
-00003790: 223e 0a20 2020 2020 2020 207b 2520 696e  ">.        {% in
-000037a0: 636c 7564 6520 2261 646d 696e 2f66 696c  clude "admin/fil
-000037b0: 6572 2f74 6f6f 6c73 2f73 6561 7263 685f  er/tools/search_
-000037c0: 666f 726d 2e68 746d 6c22 2025 7d0a 2020  form.html" %}.  
-000037d0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000037e0: 3d22 6a73 2d6e 6176 6967 6174 6f72 206e  ="js-navigator n
-000037f0: 6176 6967 6174 6f72 7b25 2069 6620 6e6f  avigator{% if no
-00003800: 7420 6163 7469 6f6e 735f 6f6e 5f74 6f70  t actions_on_top
-00003810: 2061 6e64 206e 6f74 2061 6374 696f 6e73   and not actions
-00003820: 5f6f 6e5f 626f 7474 6f6d 2025 7d6e 6176  _on_bottom %}nav
-00003830: 6967 6174 6f72 2d6e 6f2d 6163 7469 6f6e  igator-no-action
-00003840: 737b 2520 656e 6469 6620 257d 223e 0a20  s{% endif %}">. 
-00003850: 2020 2020 2020 2020 2020 203c 666f 726d             <form
-00003860: 2063 6c61 7373 3d22 6a73 2d6e 6176 6967   class="js-navig
-00003870: 6174 6f72 2d66 6f72 6d22 206d 6574 686f  ator-form" metho
-00003880: 643d 2270 6f73 7422 3e0a 2020 2020 2020  d="post">.      
-00003890: 2020 2020 2020 2020 2020 7b25 2063 7372            {% csr
-000038a0: 665f 746f 6b65 6e20 257d 0a20 2020 2020  f_token %}.     
-000038b0: 2020 2020 2020 2020 2020 207b 2520 6669             {% fi
-000038c0: 6c65 725f 6164 6d69 6e5f 636f 6e74 6578  ler_admin_contex
-000038d0: 745f 6869 6464 656e 5f66 6f72 6d66 6965  t_hidden_formfie
-000038e0: 6c64 7320 257d 0a20 2020 2020 2020 2020  lds %}.         
-000038f0: 2020 2020 2020 207b 2520 6966 2061 6374         {% if act
-00003900: 696f 6e5f 666f 726d 2061 6e64 2061 6374  ion_form and act
-00003910: 696f 6e73 5f6f 6e5f 746f 7020 616e 6420  ions_on_top and 
-00003920: 7061 6769 6e61 746f 722e 636f 756e 7420  paginator.count 
-00003930: 616e 6420 6e6f 7420 6973 5f70 6f70 7570  and not is_popup
-00003940: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00003950: 2020 2020 2020 2020 7b25 2066 696c 6572          {% filer
-00003960: 5f61 6374 696f 6e73 2025 7d0a 2020 2020  _actions %}.    
-00003970: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-00003980: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
-00003990: 2020 2020 2020 2020 7b25 2069 6e63 6c75          {% inclu
-000039a0: 6465 206c 6973 745f 7479 7065 5f74 656d  de list_type_tem
-000039b0: 706c 6174 6520 257d 0a20 2020 2020 2020  plate %}.       
-000039c0: 2020 2020 2020 2020 207b 2520 6966 2061           {% if a
-000039d0: 6374 696f 6e5f 666f 726d 2061 6e64 2061  ction_form and a
-000039e0: 6374 696f 6e73 5f6f 6e5f 626f 7474 6f6d  ctions_on_bottom
-000039f0: 2061 6e64 2070 6167 696e 6174 6f72 2e63   and paginator.c
-00003a00: 6f75 6e74 2061 6e64 206e 6f74 2069 735f  ount and not is_
-00003a10: 706f 7075 7020 257d 0a20 2020 2020 2020  popup %}.       
-00003a20: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00003a30: 6669 6c65 725f 6163 7469 6f6e 7320 257d  filer_actions %}
-00003a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003a50: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
-00003a60: 2020 2020 2020 2020 203c 2f66 6f72 6d3e           </form>
-00003a70: 0a20 2020 2020 2020 203c 2f64 6976 3e0a  .        </div>.
-00003a80: 2020 2020 3c2f 6469 763e 0a7b 2520 656e      </div>.{% en
-00003a90: 6462 6c6f 636b 2025 7d0a                 dblock %}.
+00003620: 3c2f 613e 0a20 2020 2020 2020 2020 2020  </a>.           
+00003630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003640: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+00003650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003670: 207b 2520 6966 2066 6f6c 6465 722e 6973   {% if folder.is
+00003680: 5f72 6f6f 7420 616e 6420 6e6f 7420 666f  _root and not fo
+00003690: 6c64 6572 2e69 735f 756e 736f 7274 6564  lder.is_unsorted
+000036a0: 5f75 706c 6f61 6473 2025 7d0a 2020 2020  _uploads %}.    
+000036b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036d0: 3c73 7061 6e20 636c 6173 733d 226a 732d  <span class="js-
+000036e0: 7570 6c6f 6164 2d62 7574 746f 6e2d 6469  upload-button-di
+000036f0: 7361 626c 6564 2075 706c 6f61 642d 6275  sabled upload-bu
+00003700: 7474 6f6e 2d64 6973 6162 6c65 6420 6a73  tton-disabled js
+00003710: 2d66 696c 6572 2d74 6f6f 6c74 6970 2066  -filer-tooltip f
+00003720: 696c 6572 2d74 6f6f 6c74 6970 2d77 7261  iler-tooltip-wra
+00003730: 7070 6572 220a 2020 2020 2020 2020 2020  pper".          
+00003740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003760: 7469 746c 653d 227b 2520 7472 616e 7320  title="{% trans 
+00003770: 2759 6f75 2068 6176 6520 746f 2073 656c  'You have to sel
+00003780: 6563 7420 6120 666f 6c64 6572 2066 6972  ect a folder fir
+00003790: 7374 2720 257d 223e 0a20 2020 2020 2020  st' %}">.       
+000037a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037c0: 203c 6120 6872 6566 3d22 2322 2063 6c61   <a href="#" cla
+000037d0: 7373 3d22 6e61 7669 6761 746f 722d 6275  ss="navigator-bu
+000037e0: 7474 6f6e 206e 6176 6967 6174 6f72 2d62  tton navigator-b
+000037f0: 7574 746f 6e2d 7570 6c6f 6164 2220 6469  utton-upload" di
+00003800: 7361 626c 6564 3e0a 2020 2020 2020 2020  sabled>.        
+00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003830: 2020 2020 7b25 2074 7261 6e73 2022 5570      {% trans "Up
+00003840: 6c6f 6164 2046 696c 6573 2220 257d 0a20  load Files" %}. 
+00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003870: 2020 2020 2020 203c 2f61 3e0a 2020 2020         </a>.    
+00003880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038a0: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
+000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038c0: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+000038d0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038f0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00003900: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00003910: 2520 656e 6462 6c6f 636b 2025 7d0a 2020  % endblock %}.  
+00003920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003930: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00003940: 2020 2020 2020 2020 207b 2520 656e 6462           {% endb
+00003950: 6c6f 636b 2025 7d0a 2020 2020 2020 2020  lock %}.        
+00003960: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+00003970: 2020 203c 2f64 6976 3e0a 2020 2020 3c2f     </div>.    </
+00003980: 6469 763e 0a20 2020 203c 6469 7620 6964  div>.    <div id
+00003990: 3d22 636f 6e74 656e 742d 6d61 696e 223e  ="content-main">
+000039a0: 0a20 2020 2020 2020 207b 2520 696e 636c  .        {% incl
+000039b0: 7564 6520 2261 646d 696e 2f66 696c 6572  ude "admin/filer
+000039c0: 2f74 6f6f 6c73 2f73 6561 7263 685f 666f  /tools/search_fo
+000039d0: 726d 2e68 746d 6c22 2025 7d0a 2020 2020  rm.html" %}.    
+000039e0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+000039f0: 6a73 2d6e 6176 6967 6174 6f72 206e 6176  js-navigator nav
+00003a00: 6967 6174 6f72 7b25 2069 6620 6e6f 7420  igator{% if not 
+00003a10: 6163 7469 6f6e 735f 6f6e 5f74 6f70 2061  actions_on_top a
+00003a20: 6e64 206e 6f74 2061 6374 696f 6e73 5f6f  nd not actions_o
+00003a30: 6e5f 626f 7474 6f6d 2025 7d6e 6176 6967  n_bottom %}navig
+00003a40: 6174 6f72 2d6e 6f2d 6163 7469 6f6e 737b  ator-no-actions{
+00003a50: 2520 656e 6469 6620 257d 223e 0a20 2020  % endif %}">.   
+00003a60: 2020 2020 2020 2020 203c 666f 726d 2063           <form c
+00003a70: 6c61 7373 3d22 6a73 2d6e 6176 6967 6174  lass="js-navigat
+00003a80: 6f72 2d66 6f72 6d22 206d 6574 686f 643d  or-form" method=
+00003a90: 2270 6f73 7422 3e0a 2020 2020 2020 2020  "post">.        
+00003aa0: 2020 2020 2020 2020 7b25 2063 7372 665f          {% csrf_
+00003ab0: 746f 6b65 6e20 257d 0a20 2020 2020 2020  token %}.       
+00003ac0: 2020 2020 2020 2020 207b 2520 6669 6c65           {% file
+00003ad0: 725f 6164 6d69 6e5f 636f 6e74 6578 745f  r_admin_context_
+00003ae0: 6869 6464 656e 5f66 6f72 6d66 6965 6c64  hidden_formfield
+00003af0: 7320 257d 0a20 2020 2020 2020 2020 2020  s %}.           
+00003b00: 2020 2020 207b 2520 6966 2061 6374 696f       {% if actio
+00003b10: 6e5f 666f 726d 2061 6e64 2061 6374 696f  n_form and actio
+00003b20: 6e73 5f6f 6e5f 746f 7020 616e 6420 7061  ns_on_top and pa
+00003b30: 6769 6e61 746f 722e 636f 756e 7420 616e  ginator.count an
+00003b40: 6420 6e6f 7420 6973 5f70 6f70 7570 2025  d not is_popup %
+00003b50: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00003b60: 2020 2020 2020 7b25 2066 696c 6572 5f61        {% filer_a
+00003b70: 6374 696f 6e73 2025 7d0a 2020 2020 2020  ctions %}.      
+00003b80: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+00003b90: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+00003ba0: 2020 2020 2020 7b25 2069 6e63 6c75 6465        {% include
+00003bb0: 206c 6973 745f 7479 7065 5f74 656d 706c   list_type_templ
+00003bc0: 6174 6520 257d 0a20 2020 2020 2020 2020  ate %}.         
+00003bd0: 2020 2020 2020 207b 2520 6966 2061 6374         {% if act
+00003be0: 696f 6e5f 666f 726d 2061 6e64 2061 6374  ion_form and act
+00003bf0: 696f 6e73 5f6f 6e5f 626f 7474 6f6d 2061  ions_on_bottom a
+00003c00: 6e64 2070 6167 696e 6174 6f72 2e63 6f75  nd paginator.cou
+00003c10: 6e74 2061 6e64 206e 6f74 2069 735f 706f  nt and not is_po
+00003c20: 7075 7020 257d 0a20 2020 2020 2020 2020  pup %}.         
+00003c30: 2020 2020 2020 2020 2020 207b 2520 6669             {% fi
+00003c40: 6c65 725f 6163 7469 6f6e 7320 257d 0a20  ler_actions %}. 
+00003c50: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00003c60: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00003c70: 2020 2020 2020 203c 2f66 6f72 6d3e 0a20         </form>. 
+00003c80: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00003c90: 2020 3c2f 6469 763e 0a7b 2520 656e 6462    </div>.{% endb
+00003ca0: 6c6f 636b 2025 7d0a                      lock %}.
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/folder/directory_table_list.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/directory_table_list.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 {% load i18n l10n admin_list filer_tags filer_admin_tags static thumbnail %}
 <div class="drag-hover-border"></div>
 <section class="navigator{% if is_popup %} navigator-popup{% endif %}">
-    <table class="js-filer-dropzone js-filer-dropzone-base navigator-table" id="result_list" data-url="{% if folder.id %}{% url 'admin:filer-ajax_upload' folder_id=folder.id %}{% else %}{% url 'admin:filer-ajax_upload' %}{% endif %}" data-folder-name="{% if folder.is_root %}{% trans 'Unsorted Uploads' %}{% else %}{{ folder.name }}{% endif %}" data-max-uploader-connections="{{ uploader_connections }}" data-max-file-size="20">
+    <table class="js-filer-dropzone js-filer-dropzone-base navigator-table" id="result_list" data-url="{% if folder.id %}{% url 'admin:filer-ajax_upload' folder_id=folder.id %}{% else %}{% url 'admin:filer-ajax_upload' %}{% endif %}" data-folder-name="{% if folder.is_root %}{% translate 'Unsorted Uploads' %}{% else %}{{ folder.name }}{% endif %}"
+           data-max-uploader-connections="{{ uploader_connections }}"
+           data-max-files="{{ max_files|safe }}"
+           {% if max_filesize %}}data-max-filesize="{{ max_filesize|safe }}"{% endif %}>
         <thead>
             <tr>
                 <th class="column-checkbox">
                     {% if paginator.count and not is_popup %}
                         <input type="checkbox" id="action-toggle">
                     {% endif %}
                 </th>
                 <th class="column-icon">&nbsp;</th>
-                <th class="column-name">{% trans "Name" %}</th>
-                <th class="column-owner">{% trans "Owner" %}</th>
-                <th class="column-size">{% trans "Size" %}</th>
-                <th class="column-action">{% trans "Action" %}</th>
+                <th class="column-name">{% translate "Name" %}</th>
+                <th class="column-owner">{% translate "Owner" %}</th>
+                <th class="column-size">{% translate "Size" %}</th>
+                <th class="column-action">{% translate "Action" %}</th>
             </tr>
         </thead>
         <tbody>
             {% for item in virtual_items %}
                 <tr class="unfiled">
                     <td class="column-checkbox">&nbsp;</td>
                     <td class="column-icon">
                         <a href="{{ item.get_admin_directory_listing_url_path }}{% filer_admin_context_url_params %}"
                             title="{% blocktrans with item.name as item_label %}Change '{{ item_label }}' folder details{% endblocktrans %}">
-                            <img src="{% static 'filer/icons/folder-unfiled.svg' %}" alt="{% trans 'Folder Icon' %}" width="28" height="28">
+                            <img src="{% static 'filer/icons/folder-unfiled.svg' %}" alt="{% translate 'Folder Icon' %}" width="28" height="28">
                         </a>
                     </td>
                     <td class="column-name" colspan="4">
                         <div>
                             <a href="{{ item.get_admin_directory_listing_url_path }}{% filer_admin_context_url_params %}"
                                 title="{% blocktrans with item.name as item_label %}Change '{{ item_label }}' folder details{% endblocktrans %}">
                                 {{ item.name }}
@@ -35,29 +38,29 @@
                         </div>
                     </td>
                 </tr>
             {% endfor %}
             {% for item in paginated_items.object_list %}
                 {% if item.file_type == "Folder" %}
                     {% with item as subfolder %}
-                        <tr class="js-filer-dropzone js-filer-dropzone-folder" data-url="{% url 'admin:filer-ajax_upload' folder_id=subfolder.id %}" data-folder-name="{{ subfolder.name }}" data-max-uploader-connections="{{ uploader_connections }}" data-max-file-size="20">
+                        <tr class="js-filer-dropzone js-filer-dropzone-folder" data-url="{% url 'admin:filer-ajax_upload' folder_id=subfolder.id %}" data-folder-name="{{ subfolder.name }}" data-max-uploader-connections="{{ uploader_connections }}" data-max-files="{{ max_files|safe }}" data-max-filesize="{{ max_filesize|safe }}">
                             <td class="column-checkbox">
                                 {% if filer_admin_context.pick_folder and item.file_type == 'Folder' %}
                                     <a class="insertlink insertlinkButton"
-                                        href="#" onclick="opener.dismissRelatedFolderLookupPopup(window, {{ subfolder.id }}, '{{ subfolder.quoted_logical_path }}'); return false;" >
-                                        &nbsp;
+                                        href="#" onclick="opener.dismissRelatedFolderLookupPopup(window, '{{ subfolder.pk|safe }}', '{{ subfolder.quoted_logical_path }}'); return false;" >
+                                        <span class="fa fa-arrow-left filer-icon cms-icon-select"></span>
                                     </a>
                                 {% elif action_form and item.pk and not is_popup %}
-                                    <input type="checkbox" class="action-select" value="folder-{{ item.pk }}" name="_selected_action">
+                                    <input type="checkbox" class="action-select" value="folder-{{ item.pk|safe }}" name="_selected_action">
                                 {% endif %}
                             </td>
                             <td class="column-icon">
                                 <a href="{{ subfolder.get_admin_directory_listing_url_path }}{% filer_admin_context_url_params %}"
                                     title="{% blocktrans with subfolder.name as item_label %}Change '{{ item_label }}' folder details{% endblocktrans %}">
-                                    <img src="{% static 'filer/icons/folder.svg' %}" alt="{% trans 'Folder Icon' %}" width="28" height="28">
+                                    <img src="{% static 'filer/icons/folder.svg' %}" alt="{% translate 'Folder Icon' %}" width="28" height="28">
                                 </a>
                             </td>
                             <td class="column-name">
                                 <div>
                                     <a href="{{ subfolder.get_admin_directory_listing_url_path }}{% filer_admin_context_url_params %}"
                                         title="{% blocktrans with subfolder.name as item_label %}Change '{{ item_label }}' folder details{% endblocktrans %}">
                                         {{ subfolder.name }}
@@ -73,93 +76,104 @@
                                         ({% blocktrans count subfolder.children_count as counter %}{{ counter }} folder{% plural %}{{ counter }} folders{% endblocktrans %},
                                         {% blocktrans count subfolder.file_count as counter %}{{ counter }} file{% plural %}{{ counter }} files{% endblocktrans %})
                                     </span>
                                 {% endif %}
                             </td>
                             <td class="column-action">
                                 {% if subfolder.file_type == "Folder" %}
-                                    <a href="{% url 'admin:filer_folder_change' subfolder.id %}{% filer_admin_context_url_params %}" title="{% trans 'Change folder details' %}" class="action-button"><span class="fa fa-pencil"></span></a>
-                                    <a href="{{ subfolder.get_admin_delete_url }}{% filer_admin_context_url_params %}" class="action-button" title="{% trans 'Remove folder' %}"><span class="fa fa-trash"></span></a>
+                                    <a href="{% url 'admin:filer_folder_change' subfolder.id %}{% filer_admin_context_url_params %}" title="{% translate 'Change folder details' %}" class="action-button"><span class="fa fa-pencil cms-icon cms-icon-settings"></span></a>
+                                    <a href="{{ subfolder.get_admin_delete_url }}{% filer_admin_context_url_params %}" class="action-button" title="{% translate 'Remove folder' %}"><span class="fa fa-trash cms-icon cms-icon-bin"></span></a>
                                 {% endif %}
                             </td>
                         </tr>
                     {% endwith %}
                 {% else %}
                     {% with item as file %}
                         {% filer_has_permission item 'edit' as has_change_permission %}
                         <tr>
                             <td class="column-checkbox">
                                 {% if is_popup and filer_admin_context.pick_file %}
-                                    <a class="insertlink insertlinkButton" href="#" onclick="opener.dismissRelatedImageLookupPopup(window, {{ file.id|unlocalize }}, '{% file_icon_url file %}', '{{ file.label|escapejs }}'); return false;"
-                                        title="{% trans 'Select this file' %}">&nbsp;</a>
+                                    <a class="insertlink insertlinkButton" href="#" onclick="opener.dismissRelatedImageLookupPopup(window, '{{ file.id|unlocalize }}', '{% file_icon_url file %}', '{{ file.label|escapejs }}', '{{ file.get_admin_change_url }}'); return false;"
+                                        title="{% translate 'Select this file' %}"><span class="fa fa-arrow-left filer-icon filer-icon-select"></span></a>
                                 {% elif action_form and not is_popup %}
-                                    <input type="checkbox" class="action-select" value="file-{{ item.pk }}" name="_selected_action">
+                                    <input type="checkbox" class="action-select" value="file-{{ item.pk|safe }}" name="_selected_action">
                                 {% endif %}
                             </td>
                             <td class="column-icon">
                                 {% if is_popup and filer_admin_context.pick_file %}
-                                    <a href="#" onclick="opener.dismissRelatedImageLookupPopup(window, {{ file.id|unlocalize }}, '{% file_icon_url file %}', '{{ file.label|escapejs }}'); return false;"
-                                        title="{% trans 'Select this file' %}">
+                                    <a href="#" onclick="opener.dismissRelatedImageLookupPopup(window, {{ file.id|unlocalize }}, '{% file_icon_url file %}', '{{ file.label|escapejs }}', '{{ file.get_admin_change_url }}'); return false;"
+                                        title="{% translate 'Select this file' %}">
                                 {% elif has_change_permission %}
                                     <a href="{{ file.get_admin_change_url }}{% filer_admin_context_url_params %}"
                                             title="{% blocktrans with file.label as item_label %}Change '{{ item_label }}' details{% endblocktrans %}">
                                 {% endif %}
                                 {% file_icon file %}
                                 {% if has_change_permission or is_popup and filer_admin_context.pick_file %}
                                     </a>
                                 {% endif %}
                             </td>
                             <td class="column-name">
                                 <div>
                                     <strong>
                                         {% if is_popup and filer_admin_context.pick_file %}
-                                            <a href="#" onclick="opener.dismissRelatedImageLookupPopup(window, {{ file.id|unlocalize }}, '{% file_icon_url file %}', '{{ file.label|escapejs }}'); return false;"
-                                                title="{% trans 'Select this file' %}">
+                                            <a href="#" onclick="opener.dismissRelatedImageLookupPopup(window, {{ file.id|unlocalize }}, '{% file_icon_url file %}', '{{ file.label|escapejs }}', '{{ file.get_admin_change_url }}'); return false;"
+                                                title="{% translate 'Select this file' %}">
                                         {% elif has_change_permission %}
                                             <a href="{{ file.get_admin_change_url }}{% filer_admin_context_url_params %}"
                                                 title="{% blocktrans with file.label as item_label %}Change '{{ item_label }}' details{% endblocktrans %}">
                                         {% endif %}
                                         {{ file.label }}
                                         {% if has_change_permission or is_popup and filer_admin_context.pick_file %}
                                             </a>
                                         {% endif %}
                                     </strong>
                                 </div>
                                 {% if enable_permissions %}
-                                    <div>{% trans "Permissions" %}: {% if file.is_public %}{% trans "disabled" %}{% else %}{% trans "enabled" %}{% endif %}</div>
+                                    <div>{% translate "Permissions" %}: {% if file.is_public %}{% translate "disabled" %}{% else %}{% translate "enabled" %}{% endif %}</div>
                                 {% endif %}
                             </td>
                             <td class="column-owner">
                                 {{ file.owner|default:"n/a" }}
                             </td>
                             <td class="column-size">
                                 <span class="tiny"> ({{ file.size|filesize:"auto1000long" }}{% if file.file_type == "Image" and file.width > 0.0 and file.height > 0.0 %}, {{ file.width|floatformat }}x{{ file.height|floatformat }} px{% endif %})</span>
                             </td>
                             <td class="column-action">
-                                <a href="{{ file.canonical_url }}"
-                                    title="{% blocktrans with file.label as item_label %}Canonical url '{{ item_label }}'{% endblocktrans %}" class="action-button" target="_blank"><span class="fa fa-link"></span></a>
-                                <a href="{{ file.url }}" target="_blank"
-                                    title="{% blocktrans with file.label as item_label %}Download '{{ item_label }}'{% endblocktrans %}" class="action-button"><span class="fa fa-download"></span></a>
-                                <a href="{{ file.get_admin_change_url }}{% filer_admin_context_url_params %}"
-                                    title="{% blocktrans with file.label as item_label %}Change '{{ item_label }}' details{% endblocktrans %}" class="action-button"><span class="fa fa-pencil"></span></a>
-                                <a href="{{ file.get_admin_delete_url }}{% filer_admin_context_url_params %}" title="{% trans 'Remove file' %}" class="action-button"><span class="fa fa-trash"></span></a>
+                                {% if file.canonical_url %}
+                                    <a href="{{ file.canonical_url }}" rel="noopener noreferrer"
+                                       download="{{ file.original_filename }}"
+                                       title="{% blocktrans with file.label as item_label %}Canonical url '{{ item_label }}'{% endblocktrans %}" class="action-button" target="_blank"><span class="fa fa-link filer-icon filer-icon-link"></span></a>
+                                {% endif %}
+                                <a href="{{ file.url }}" target="_blank" rel="noopener noreferrer"
+                                   download="{{ file.original_filename }}"
+                                   title="{% blocktrans with file.label as item_label %}Download '{{ item_label }}'{% endblocktrans %}" class="action-button"><span class="fa fa-download filer-icon filer-icon-download"></span></a>
+                                {% if has_change_permission %}
+                                    <a href="{{ file.get_admin_change_url }}{% filer_admin_context_url_params %}"
+                                        title="{% blocktrans with file.label as item_label %}Change '{{ item_label }}' details{% endblocktrans %}" class="action-button"><span class="fa fa-pencil cms-icon cms-icon-settings"></span></a>
+                                    <a href="{{ file.get_admin_delete_url }}{% filer_admin_context_url_params %}" title="{% translate 'Remove file' %}" class="action-button"><span class="fa fa-trash cms-icon cms-icon-bin"></span></a>
+                                {% endif %}
                             </td>
                             {% endwith %}
                         </tr>
                 {% endif %}
             {% empty %}
                 <tr>
-                    <td colspan="6" class="no-files"><span class="fa fa-arrow-down"></span>{% trans 'Drop files here or use the "Upload Files" button' %}</td>
+                    <td colspan="6" class="no-files"><span class="fa fa-arrow-down filer-icon filer-arrow-down"></span>{% trans 'Drop files here or use the "Upload Files" button' %}</td>
                 </tr>
             {% endfor %}
         </tbody>
     </table>
 
-    <div class="filer-dropzone-info-message js-filer-dropzone js-filer-dropzone-info-message hidden" data-url="{% if folder.id %}{% url 'admin:filer-ajax_upload' folder_id=folder.id %}{% else %}{% url 'admin:filer-ajax_upload' %}{% endif %}" data-folder-name="{% if folder.is_root %}{% trans 'Unsorted Uploads' %}{% else %}{{ folder.name }}{% endif %}" data-max-uploader-connections="{{ uploader_connections }}" data-max-file-size="20">
-        <div class="icon"><span class="fa fa-cloud-upload"></span></div>
+  <div class="filer-dropzone-info-message js-filer-dropzone js-filer-dropzone-info-message hidden" data-url="{% if folder.id %}{% url 'admin:filer-ajax_upload' folder_id=folder.id %}{% else %}{% url 'admin:filer-ajax_upload' %}{% endif %}"
+         data-folder-name="{% if folder.is_root %}{% trans 'Unsorted Uploads' %}{% else %}{{ folder.name }}{% endif %}"
+         data-max-uploader-connections="{{ uploader_connections }}"
+         data-max-files="{{ max_files|safe }}"
+         {% if max_filesize %}}data-max-filesize="{{ max_filesize|safe }}"{% endif %}>
+
+        <div class="icon"><span class="filer-icon filer-upload fa fa-cloud-upload"></span></div>
 
         <div class="filer-dropzone-upload-welcome js-filer-dropzone-upload-welcome">
             <div class="text">{% trans "Drop your file to upload into:" %}</div>
             <div class="folder">
                 <div class="folder-inner">
                     <img src="{% static 'filer/icons/folder.svg' %}" alt="{% trans 'Folder Icon' %}" width="18" height="18">
                     <span class="js-filer-dropzone-folder-name"></span>
```

#### html2text {}

```diff
@@ -1,42 +1,60 @@
 {% load i18n l10n admin_list filer_tags filer_admin_tags static thumbnail %}
-{% if paginator.count and not is_popup %} ⁰ {% endif %}                                              {% trans "Name" %}            {% trans "Owner" %}      {% trans "Size" %}       {% trans "Action"
-                                                                                                                                                                                        %}
-                                                                         [{%_trans_'Folder_Icon'_%}]   {{_item.name_}}
-                                                                                                                                                               {% if not
-                                                                                                                                                               subfolder.is_root %}  (
-                                                                                                                                                               {% blocktrans count
-                                                                                                                                                               subfolder.children_count
-                                                                                                                                                               as counter %}{{ counter
-                                                                                                                                      {                        }} folder{% plural %}{   {% if
-{% if filer_admin_context.pick_folder and item.file_type == 'Folder' %}                                                              {                        { counter }} folders{%   subfolder.file_type
-{% elif action_form and item.pk and not is_popup %} ⁰ {% endif %}       [{%_trans_'Folder_Icon'_%}]   {{_subfolder.name_}}          subfolder.owner|default: endblocktrans %}, {%     == "Folder" %}   {%
-                                                                                                                                      "n/a" }}                 blocktrans count         endif %}
-                                                                                                                                                               subfolder.file_count as
-                                                                                                                                                               counter %}{{ counter }}
-                                                                                                                                                               file{% plural %}{
-                                                                                                                                                               { counter }} files{%
-                                                                                                                                                               endblocktrans %})  {%
-                                                                                                                                                               endif %}
-                                                                                                        {% if is_popup and
-                                                                                                        filer_admin_context.pick_file
-                                                                                                        %} {%_elif                                              ({{ file.size|filesize:
-                                                                          {% if is_popup and            has_change_permission_%}_{%                            "auto1000long" }}{% if
-                                                                          filer_admin_context.pick_file endif_%}_{{_file.label_}}_{%                           file.file_type ==
-                                                                          %} {%_elif                    if_has_change_permission_or                            "Image" and file.width >
-{% if is_popup and filer_admin_context.pick_file %}   {% elif action_formhas_change_permission_%}_{%   is_popup_and                  {{ file.owner|default:   0.0 and file.height >
-and not is_popup %} ⁰ {% endif %}                                       endif_%}_{%_file_icon_file_%} filer_admin_context.pick_file "n/a" }}                 0.0 %}, {
-                                                                          {%_if_has_change_permission   %}_{%_endif_%}                                         { file.width|floatformat
-                                                                          or_is_popup_and               {% if enable_permissions %}                            }}x{
-                                                                          filer_admin_context.pick_file {% trans "Permissions" %}: {%                          {
-                                                                          %}_{%_endif_%}                if file.is_public %}{% trans                           file.height|floatformat
-                                                                                                        "disabled" %}{% else %}{%                              }} px{% endif %})
-                                                                                                        trans "enabled" %}{% endif %}
-                                                                                                        {% endif %}
+
+% if max_filesize %}}data-max-filesize="{{ max_filesize|safe }}"{% endif %}>
+{% if paginator.count and not is_popup %} ⁰ {% endif %}
+ 
+{% translate "Name" %}
+{% translate "Owner" %}
+{% translate "Size" %}
+{% translate "Action" %}
+  {% for item in virtual_items %}
+ 
+[{%_translate_'Folder_Icon'_%}]
+{{_item.name_}}
+{% endfor %} {% for item in paginated_items.object_list %} {% if item.file_type
+== "Folder" %} {% with item as subfolder %}
+{% if filer_admin_context.pick_folder and item.file_type == 'Folder' %}  {%
+elif action_form and item.pk and not is_popup %} ⁰ {% endif %}
+[{%_translate_'Folder_Icon'_%}]
+{{_subfolder.name_}}
+{{ subfolder.owner|default:"n/a" }}
+{% if not subfolder.is_root %}  ({% blocktrans count subfolder.children_count
+as counter %}{{ counter }} folder{% plural %}{{ counter }} folders{%
+endblocktrans %}, {% blocktrans count subfolder.file_count as counter %}{
+{ counter }} file{% plural %}{{ counter }} files{% endblocktrans %})  {% endif
+%}
+{% if subfolder.file_type == "Folder" %}   {% endif %}
+{% endwith %} {% else %} {% with item as file %} {% filer_has_permission item
+'edit' as has_change_permission %}
+{% if is_popup and filer_admin_context.pick_file %}  {% elif action_form and
+not is_popup %} ⁰ {% endif %}
+{% if is_popup and filer_admin_context.pick_file %} {%_elif
+has_change_permission_%}_{%_endif_%}_{%_file_icon_file_%}_{%_if
+has_change_permission_or_is_popup_and_filer_admin_context.pick_file_%}_{%_endif
+%}
+{% if is_popup and filer_admin_context.pick_file %} {%_elif
+has_change_permission_%}_{%_endif_%}_{{_file.label_}}_{%_if
+has_change_permission_or_is_popup_and_filer_admin_context.pick_file_%}_{%_endif
+%}
+{% if enable_permissions %}
+{% translate "Permissions" %}: {% if file.is_public %}{% translate "disabled"
+%}{% else %}{% translate "enabled" %}{% endif %}
+{% endif %}
+{{ file.owner|default:"n/a" }}
+ ({{ file.size|filesize:"auto1000long" }}{% if file.file_type == "Image" and
+file.width > 0.0 and file.height > 0.0 %}, {{ file.width|floatformat }}x{
+{ file.height|floatformat }} px{% endif %})
+{% if file.canonical_url %}  {% endif %}  {% if has_change_permission %}   {%
+endif %}
+{% endwith %}
+{% endif %} {% empty %}
 {% trans 'Drop files here or use the "Upload Files" button' %}
+{% endfor %}
+% if max_filesize %}}data-max-filesize="{{ max_filesize|safe }}"{% endif %}>
 {% trans "Drop your file to upload into:" %}
 [{% trans 'Folder Icon' %}]
 {% trans "Upload" %}
 {%_trans_"cancel"_%}
 {% trans "Upload success!" %}
 {% trans "Upload canceled!" %}
 {% if paginated_items.has_previous %} {%_trans_"previous"_%} {% endif %}  {%
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/folder/directory_thumbnail_list.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/directory_thumbnail_list.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,59 +1,68 @@
 {% load i18n l10n admin_list filer_tags filer_admin_tags static thumbnail %}
 <div class="drag-hover-border thumbnail-drag-hover-border"></div>
 <section class="navigator{% if is_popup %} navigator-popup{% endif %} navigator-thumbnail-list">
 
-    <div class="js-filer-dropzone js-filer-dropzone-base navigator-list" id="result_list" data-url="{% if folder.id %}{% url 'admin:filer-ajax_upload' folder_id=folder.id %}{% else %}{% url 'admin:filer-ajax_upload' %}{% endif %}" data-folder-name="{% if folder.is_root %}{% trans 'Unsorted Uploads' %}{% else %}{{ folder.name }}{% endif %}" data-max-uploader-connections="{{ uploader_connections }}" data-max-file-size="20">
+    <div class="js-filer-dropzone js-filer-dropzone-base navigator-list" id="result_list" data-url="{% if folder.id %}{% url 'admin:filer-ajax_upload' folder_id=folder.id %}{% else %}{% url 'admin:filer-ajax_upload' %}{% endif %}" data-folder-name="{% if folder.is_root %}{% translate 'Unsorted Uploads' %}{% else %}{{ folder.name }}{% endif %}" data-max-uploader-connections="{{ uploader_connections }}"
+         data-max-files="{{ max_files|safe }}"
+         {% if max_filesize %}}data-max-filesize="{{ max_filesize|safe }}"{% endif %}>
+
         <input type="checkbox" id="all-items-action-toggle">
 
         <div class="navigator-thumbnail-list-header navigator-header">
-          <p>{% trans 'Folders' %}</p>
+          <p>{% translate 'Folders' %}</p>
           <span class="navigator-checkbox">
               {% if paginator.count and not is_popup %}
-                  {% trans 'Select all' %}
+                  {% translate 'Select all' %}
                   <input type="checkbox" id="folders-action-toggle">
               {% endif %}
           </span>
         </div>
 
         <div class="navigator-body navigator-folders-body">
         {% for item in virtual_items %}
             <div class="thumbnail-item thumbnail-virtual-item">
                 <div class="item-icon">
                     <a href="{{ item.get_admin_directory_listing_url_path }}{% filer_admin_context_url_params %}"
                         title="{% blocktrans with item.name as item_label %}Change '{{ item_label }}' folder details{% endblocktrans %}">
-                        <img src="{% static 'filer/icons/folder-unfiled.svg' %}" alt="{% trans 'Folder Icon' %}" width="28" height="28">
+                        <img src="{% static 'filer/icons/folder-unfiled.svg' %}" alt="{% translate 'Folder Icon' %}" width="28" height="28">
                     </a>
                 </div>
                 <div class="item-name">
                     <a href="{{ item.get_admin_directory_listing_url_path }}{% filer_admin_context_url_params %}"
                         title="{% blocktrans with item.name as item_label %}Change '{{ item_label }}' folder details{% endblocktrans %}">
                         {{ item.name }}
                     </a>
                 </div>
             </div>
         {% endfor %}
         {% for item in paginated_items.object_list %}
             {% if item.file_type == "Folder" %}
                 {% with item as subfolder %}
-                <div class="js-filer-dropzone js-filer-dropzone-folder list-item thumbnail-item thumbnail-folder-item" data-url="{% url 'admin:filer-ajax_upload' folder_id=subfolder.id %}" data-folder-name="{{ subfolder.name }}" data-max-uploader-connections="{{ uploader_connections }}" data-max-file-size="19">
+                <div class="js-filer-dropzone js-filer-dropzone-folder list-item thumbnail-item thumbnail-folder-item"
+                     data-url="{% url 'admin:filer-ajax_upload' folder_id=subfolder.id %}"
+                     data-folder-name="{{ subfolder.name }}"
+                     data-max-uploader-connections="{{ uploader_connections }}"
+                     data-max-files="{{ max_files|safe }}"
+                     {% if max_filesize %}}data-max-filesize="{{ max_filesize|safe }}"{% endif %}>
+
                     <div class="navigator-checkbox">
                         {% if filer_admin_context.pick_folder and item.file_type == 'Folder' %}
                             <a class="insertlink insertlinkButton"
-                                href="#" onclick="opener.dismissRelatedFolderLookupPopup(window, {{ subfolder.id }}, '{{ subfolder.quoted_logical_path }}'); return false;" >
+                                href="#" onclick="opener.dismissRelatedFolderLookupPopup(window, '{{ subfolder.pk|safe }}', '{{ subfolder.quoted_logical_path }}'); return false;" >
                                 &nbsp;
                             </a>
                         {% elif action_form and item.pk and not is_popup %}
-                            <input type="checkbox" class="action-select" value="folder-{{ item.pk }}" name="_selected_action">
+                            <input type="checkbox" class="action-select" value="folder-{{ item.pk|safe }}" name="_selected_action">
                         {% endif %}
                     </div>
                     <div class="item-icon">
                         <a href="{{ subfolder.get_admin_directory_listing_url_path }}{% filer_admin_context_url_params %}"
                             title="{% blocktrans with subfolder.name as item_label %}Change '{{ item_label }}' folder details{% endblocktrans %}">
-                            <img src="{% static 'filer/icons/folder.svg' %}" alt="{% trans 'Folder Icon' %}" width="28" height="28">
+                            <img src="{% static 'filer/icons/folder.svg' %}" alt="{% translate 'Folder Icon' %}" width="28" height="28">
                         </a>
                     </div>
                     <div class="item-name">
                         <a href="{{ subfolder.get_admin_directory_listing_url_path }}{% filer_admin_context_url_params %}"
                             title="{% blocktrans with subfolder.name as item_label %}Change '{{ item_label }}' folder details{% endblocktrans %}">
                             {{ subfolder.name }}
                         </a>
@@ -61,83 +70,88 @@
                 </div>
                 {% endwith %}
             {% endif %}
         {% endfor %}
         </div>
 
         <div class="navigator-thumbnail-list-header navigator-header">
-          <p>{% trans 'Files' %}</p>
+          <p>{% translate 'Files' %}</p>
           <span class="navigator-checkbox">
               {% if paginator.count and not is_popup %}
-                  {% trans 'Select all' %}
+                  {% translate 'Select all' %}
                   <input type="checkbox" id="files-action-toggle">
               {% endif %}
           </span>
         </div>
 
         <div class="navigator-body navigator-files-body">
             {% for item in paginated_items.object_list %}
                 {% if item.file_type != "Folder" %}
                   {% with item as file %}
                       {% filer_has_permission item 'edit' as has_change_permission %}
                           <div class="list-item thumbnail-item thumbnail-file-item">
                               <div class="navigator-checkbox">
                                   {% if is_popup and filer_admin_context.pick_file %}
-                                      <a class="insertlink insertlinkButton" href="#" onclick="opener.dismissRelatedImageLookupPopup(window, {{ file.id|unlocalize }}, '{% file_icon_url file %}', '{{ file.label|escapejs }}'); return false;"
-                                          title="{% trans 'Select this file' %}">&nbsp;</a>
+                                      <a class="insertlink insertlinkButton" href="#" onclick="opener.dismissRelatedImageLookupPopup(window, '{{ file.id|unlocalize }}', '{% file_icon_url file %}', '{{ file.label|escapejs }}'); return false;"
+                                          title="{% translate 'Select this file' %}">&nbsp;</a>
                                   {% elif action_form and not is_popup %}
-                                      <input type="checkbox" class="action-select" value="file-{{ item.pk }}" name="_selected_action">
+                                      <input type="checkbox" class="action-select" value="file-{{ item.pk|safe }}" name="_selected_action">
                                   {% endif %}
                               </div>
                               <div class="thumbnail-file-item-box">
                                   <div class="item-thumbnail">
                                       {% if is_popup and filer_admin_context.pick_file %}
                                           <a href="#" onclick="opener.dismissRelatedImageLookupPopup(window, {{ file.id|unlocalize }}, '{% file_icon_url file %}', '{{ file.label|escapejs }}'); return false;"
-                                              title="{% trans 'Select this file' %}">
+                                              title="{% translate 'Select this file' %}">
                                       {% elif has_change_permission %}
                                           <a href="{{ file.get_admin_change_url }}{% filer_admin_context_url_params %}"
                                                   title="{% blocktrans with file.label as item_label %}Change '{{ item_label }}' details{% endblocktrans %}">
                                       {% endif %}
                                       {% file_icon file size="160x160" %}
                                       {% if has_change_permission or is_popup and filer_admin_context.pick_file %}
                                           </a>
                                       {% endif %}
                                   </div>
                                </div>
                               <div class="item-name">
                                   <div>
                                       {% if is_popup and filer_admin_context.pick_file %}
                                           <a href="#" onclick="opener.dismissRelatedImageLookupPopup(window, {{ file.id|unlocalize }}, '{% file_icon_url file %}', '{{ file.label|escapejs }}'); return false;"
-                                              title="{% trans 'Select this file' %}">
+                                              title="{% translate 'Select this file' %}">
                                       {% elif has_change_permission %}
                                           <a href="{{ file.get_admin_change_url }}{% filer_admin_context_url_params %}"
                                               title="{% blocktrans with file.label as item_label %}Change '{{ item_label }}' details{% endblocktrans %}">
                                       {% endif %}
                                       {{ file.label }}
                                       {% if has_change_permission or is_popup and filer_admin_context.pick_file %}
                                           </a>
                                       {% endif %}
                                   </div>
                                   {% if enable_permissions %}
-                                      <div>{% trans "Permissions" %}: {% if file.is_public %}{% trans "disabled" %}{% else %}{% trans "enabled" %}{% endif %}</div>
+                                      <div>{% translate "Permissions" %}: {% if file.is_public %}{% trans "disabled" %}{% else %}{% trans "enabled" %}{% endif %}</div>
                                   {% endif %}
                             </div>
                         </div>
                   {% endwith %}
               {% endif %}
           {% empty %}
               <div>
-                  <div class="no-files"><span class="fa fa-arrow-down"></span>{% trans 'Drop files here or use the "Upload Files" button' %}</div>
+                  <div class="no-files"><span class="fa fa-arrow-down filer-icon filer-icon-arrow-down"></span>{% trans 'Drop files here or use the "Upload Files" button' %}</div>
               </div>
           {% endfor %}
       </div>
   </div>
 
-  <div class="filer-dropzone-info-message js-filer-dropzone js-filer-dropzone-info-message hidden" data-url="{% if folder.id %}{% url 'admin:filer-ajax_upload' folder_id=folder.id %}{% else %}{% url 'admin:filer-ajax_upload' %}{% endif %}" data-folder-name="{% if folder.is_root %}{% trans 'Unsorted Uploads' %}{% else %}{{ folder.name }}{% endif %}" data-max-uploader-connections="{{ uploader_connections }}" data-max-file-size="20">
-      <div class="icon"><span class="fa fa-cloud-upload"></span></div>
+  <div class="filer-dropzone-info-message js-filer-dropzone js-filer-dropzone-info-message hidden"
+       data-url="{% if folder.id %}{% url 'admin:filer-ajax_upload' folder_id=folder.id %}{% else %}{% url 'admin:filer-ajax_upload' %}{% endif %}"
+       data-folder-name="{% if folder.is_root %}{% trans 'Unsorted Uploads' %}{% else %}{{ folder.name }}{% endif %}"
+       data-max-uploader-connections="{{ uploader_connections }}"
+       data-max-files="{{ max_files|safe }}"
+       {% if max_filesize %}}data-max-filesize="{{ max_filesize|safe }}"{% endif %}>
+  <div class="icon"><span class="filer-icon filer-icon-upload fa fa-cloud-upload"></span></div>
 
       <div class="filer-dropzone-upload-welcome js-filer-dropzone-upload-welcome">
           <div class="text">{% trans "Drop your file to upload into:" %}</div>
           <div class="folder">
               <div class="folder-inner">
                   <img src="{% static 'filer/icons/folder.svg' %}" alt="{% trans 'Folder Icon' %}" width="18" height="18">
                   <span class="js-filer-dropzone-folder-name"></span>
```

#### html2text {}

```diff
@@ -1,45 +1,48 @@
 {% load i18n l10n admin_list filer_tags filer_admin_tags static thumbnail %}
-⁰
-{% trans 'Folders' %}
- {% if paginator.count and not is_popup %} {% trans 'Select all' %} ⁰ {% endif
-%}
+
+% if max_filesize %}}data-max-filesize="{{ max_filesize|safe }}"{% endif %}> ⁰
+{% translate 'Folders' %}
+ {% if paginator.count and not is_popup %} {% translate 'Select all' %} ⁰ {%
+endif %}
 {% for item in virtual_items %}
-[{%_trans_'Folder_Icon'_%}]
+[{%_translate_'Folder_Icon'_%}]
 {{_item.name_}}
 {% endfor %} {% for item in paginated_items.object_list %} {% if item.file_type
 == "Folder" %} {% with item as subfolder %}
+% if max_filesize %}}data-max-filesize="{{ max_filesize|safe }}"{% endif %}>
 {% if filer_admin_context.pick_folder and item.file_type == 'Folder' %}   {%
 elif action_form and item.pk and not is_popup %} ⁰ {% endif %}
-[{%_trans_'Folder_Icon'_%}]
+[{%_translate_'Folder_Icon'_%}]
 {{_subfolder.name_}}
 {% endwith %} {% endif %} {% endfor %}
-{% trans 'Files' %}
- {% if paginator.count and not is_popup %} {% trans 'Select all' %} ⁰ {% endif
-%}
+{% translate 'Files' %}
+ {% if paginator.count and not is_popup %} {% translate 'Select all' %} ⁰ {%
+endif %}
 {% for item in paginated_items.object_list %} {% if item.file_type != "Folder"
 %} {% with item as file %} {% filer_has_permission item 'edit' as
 has_change_permission %}
 {% if is_popup and filer_admin_context.pick_file %}   {% elif action_form and
 not is_popup %} ⁰ {% endif %}
 {% if is_popup and filer_admin_context.pick_file %} {%_elif
 has_change_permission_%}_{%_endif_%}_{%_file_icon_file_size="160x160"_%}_{%_if
 has_change_permission_or_is_popup_and_filer_admin_context.pick_file_%}_{%_endif
 %}
 {% if is_popup and filer_admin_context.pick_file %} {%_elif
 has_change_permission_%}_{%_endif_%}_{{_file.label_}}_{%_if
 has_change_permission_or_is_popup_and_filer_admin_context.pick_file_%}_{%_endif
 %}
 {% if enable_permissions %}
-{% trans "Permissions" %}: {% if file.is_public %}{% trans "disabled" %}{% else
-%}{% trans "enabled" %}{% endif %}
+{% translate "Permissions" %}: {% if file.is_public %}{% trans "disabled" %}{%
+else %}{% trans "enabled" %}{% endif %}
 {% endif %}
 {% endwith %} {% endif %} {% empty %}
 {% trans 'Drop files here or use the "Upload Files" button' %}
 {% endfor %}
+% if max_filesize %}}data-max-filesize="{{ max_filesize|safe }}"{% endif %}>
 {% trans "Drop your file to upload into:" %}
 [{% trans 'Folder Icon' %}]
 {% trans "Upload" %}
 {%_trans_"cancel"_%}
 {% trans "Upload success!" %}
 {% trans "Upload canceled!" %}
 {% if paginated_items.has_previous %} {%_trans_"previous"_%} {% endif %}  {%
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/folder/new_folder_form.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/new_folder_form.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends "admin/change_form.html" %}
 {% load i18n filer_admin_tags %}
 
-{% block title %}{% trans "Add new" %} {% trans "folder" %} | {{ site_title|default:_('Django site admin') }}{% endblock %}
+{% block title %}{% translate "Add new" %} {% translate "folder" %} | {{ site_title|default:_('Django site admin') }}{% endblock %}
 
 {% block content %}
-    <h1>{% trans "Add new" %} {% trans "folder" %}</h1>
+    <h1>{% translate "Add new" %} {% translate "folder" %}</h1>
     <div id="content-main">
         <form id="folder_form" method="post" action="" enctype="multipart/form-data">
             {% csrf_token %}
             <div>
                 {% filer_admin_context_hidden_formfields %}
                 {% if new_folder_form.errors %}
                     <p class="errornote">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% extends "admin/change_form.html" %} {% load i18n filer_admin_tags %} {%
-block title %}{% trans "Add new" %} {% trans "folder" %} | {
+block title %}{% translate "Add new" %} {% translate "folder" %} | {
 { site_title|default:_('Django site admin') }}{% endblock %} {% block content
 %}
-****** {% trans "Add new" %} {% trans "folder" %} ******
+****** {% translate "Add new" %} {% translate "folder" %} ******
 {% csrf_token %}
 {% filer_admin_context_hidden_formfields %} {% if new_folder_form.errors %}
 {% blocktrans count new_folder_form.errors|length as counter %}Please correct
 the error below.{% plural %}Please correct the errors below.{% endblocktrans %}
 {{ new_folder_form.non_field_errors }} {% endif %}
 {{ new_folder_form.errors.name.as_ul }}
 {% for field in new_folder_form %} {{ field.label }}:{{ field }} {% endfor %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/image/change_form.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/image/change_form.html`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         __$ = __jQuery;
     </script>
 {% endblock %}
 
 {% block object-tools %}
     {% if change and not is_popup %}
         <ul class="object-tools">
-            <li><a href="{% url history_url object_id %}" class="historylink">{% trans "History" %}</a></li>
+            <li><a href="{% url history_url object_id %}" class="historylink">{% translate "History" %}</a></li>
             {% if has_absolute_url %}
-                <li><a href="../../../r/{{ content_type_id }}/{{ object_id }}/" class="viewsitelink">{% trans "View on site" %}</a></li>
+                <li><a href="../../../r/{{ content_type_id }}/{{ object_id }}/" class="viewsitelink">{% translate "View on site" %}</a></li>
             {% endif%}
         </ul>
     {% endif %}
     {% include "admin/filer/tools/detail_info.html" %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 {% extends "admin/filer/change_form.html" %} {% load i18n admin_modify static
 %} {% block extrahead %} {{ block.super }} {# upload stuff #}
  {% endblock %} {% block object-tools %} {% if change and not is_popup %}
-    * {%_trans_"History"_%}
+    * {%_translate_"History"_%}
     * {% if has_absolute_url %}
-    * {%_trans_"View_on_site"_%}
+    * {%_translate_"View_on_site"_%}
     * {% endif%}
 {% endif %} {% include "admin/filer/tools/detail_info.html" %} {% endblock %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/templatetags/file_icon.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/templatetags/file_icon.html`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 {% if sidebar_image_ratio %}
 <div class="image-preview js-focal-point" data-location-selector="#id_subject_location">
 {% endif %}
 {% if download_url %}
     {% if mime_maintype == 'audio' %}
     <audio controls>
         <source src="{{ download_url }}" type="{{ mime_type }}">
-        {% trans 'Your browser does not support audio.' %}
+        {% translate 'Your browser does not support audio.' %}
     </audio>
     {% elif mime_maintype == 'video' %}
     <video width="320" height="240" controls>
         <source src="{{ download_url }}" type="{{ mime_type }}">
-        {% trans 'Your browser does not support video.' %}
+        {% translate 'Your browser does not support video.' %}
     </video>
     {% else %}
-    <img src="{{ icon_url }}" width="{{ width }}" height="{{ height }}"{% if alt_text %} alt="{{ alt_text }}"{% endif %}{% if highres_url %} srcset="{{ icon_url }} 1x, {{ highres_url }} 2x"{% endif %}{% if sidebar_image_ratio %} data-ratio="{{ sidebar_image_ratio }}" class="js-focal-point-image"{% endif %} />
+    <img src="{{ icon_url }}" loading="lazy" width="{{ width }}" height="{{ height }}"{% if alt_text %} alt="{{ alt_text }}"{% endif %}{% if highres_url %} srcset="{{ icon_url }} 1x, {{ highres_url }} 2x"{% endif %}{% if sidebar_image_ratio %} data-ratio="{{ sidebar_image_ratio }}" class="js-focal-point-image"{% endif %} />
     {% endif %}
 {% else %}
-    <img src="{{ icon_url }}" width="{{ width }}" height="{{ height }}"{% if alt_text %} alt="{{ alt_text }}"{% endif %}{% if highres_url %} srcset="{{ icon_url }} 1x, {{ highres_url }} 2x"{% endif %} class="thumbnail_img" />
+    <img src="{{ icon_url }}" loading="lazy" width="{{ width }}" height="{{ height }}"{% if alt_text %} alt="{{ alt_text }}"{% endif %}{% if highres_url %} srcset="{{ icon_url }} 1x, {{ highres_url }} 2x"{% endif %} class="thumbnail_img" />
 {% endif %}
 {% if sidebar_image_ratio %}
     <div class="image-preview-field">
         <div class="js-focal-point-circle image-preview-circle hidden"></div>
     </div>
 </div>
 {% endif %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/tools/clipboard/clipboard.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/tools/clipboard/clipboard.html`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,29 @@
                 </tr>
             </thead>
             <tfoot>
                 <tr>
                     <td colspan="3">
                         <form action="{% url 'admin:filer-paste_clipboard_to_folder' %}" method="post" style="display: inline;">
                             {% csrf_token %}
-                            <input type="hidden" name="folder_id" value="{{ folder.id }}">
-                            <input type="hidden" name="clipboard_id" value="{{ clipboard.id }}">
+                            <input type="hidden" name="folder_id" value="{{ folder.pk|safe }}">
+                            <input type="hidden" name="clipboard_id" value="{{ clipboard.pk|safe }}">
                             <input type="hidden" name="redirect_to" value="{{ current_url }}">
                             {% filer_admin_context_hidden_formfields %}
                             <button class="pastelink" type="submit" {% if folder.is_root or not permissions.has_add_children_permission %} disabled="disabled" style="color: gray;"{% endif %} title="{% trans 'Paste all items here' %}"><span>&lArr;</span>&nbsp;Paste</button>
                         </form>
                         <form action="{% url 'admin:filer-discard_clipboard' %}" method="post" style="display: inline;">{% csrf_token %}
-                            <input type="hidden" name="clipboard_id" value="{{ clipboard.id }}">
+                            <input type="hidden" name="clipboard_id" value="{{ clipboard.pk|safe }}">
                             <input type="hidden" name="redirect_to" value="{{ current_url }}">
                             {% filer_admin_context_hidden_formfields %}
                             <button class="deletelink" type="submit" title="{% trans 'Move all clipboard files to' %} &#39;{% trans 'Unsorted Uploads' %}&#39; {% trans 'folder' %}"><span>{% trans "Empty Clipboard" %}</span></button>
                         </form>
                         {% comment %}
                         <form action="{% url 'admin:filer-delete_clipboard' %}" method="post" style="display: inline;">{% csrf_token %}
-                            <input type="hidden" name="clipboard_id" value="{{ clipboard.id }}">
+                            <input type="hidden" name="clipboard_id" value="{{ clipboard.pk|safe }}">
                             <input type="hidden" name="redirect_to" value="{{ current_url }}">
                             {% if is_popup %}
                                 <input type="hidden" name="_popup" value="1">
                             {% endif %}
                             <button class="deletelink" type="submit" title="{% trans 'Delete all files in the clipboard' %}"><span>{% trans "delete files" %}</span></button>
                         </form>
                         {% endcomment %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
                 <td class="buttons"></td>
             </tr>
         {% endwith %}
     {% endfor %}
 {% else %}
     <tr class="clipboardItem">
         <td class="thumbnail"></td>
-        <td class="label">{% trans "upload failed" %}</td>
+        <td class="label">{% translate "upload failed" %}</td>
         <td class="buttons"></td>
     </tr>
 {% endif %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/tools/detail_info.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/tools/detail_info.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,55 @@
 {% load filer_admin_tags i18n static %}
     <section class="image-info image-info-detail">
-        <div class="image-info-title">
-            <span class="icon fa fa-file{% if original.file_type == 'Image' %}-image-o{% endif %}"></span> {{ original }}
-        </div>
+        <div class="image-info-title"></div>
         <div class="image-details-left">
             <div class="image-preview-container">
                 {% file_icon original detail=True %}
-                <div class="text-left">
+                <div class="text-left button-group">
                 {% if original.file.exists %}
-                    <a href="{{ original.url }}" target="_blank" class="btn" download="{{ original.original_filename }}">
-                        <span class="icon fa fa-download"></span>
-                        &nbsp;<span>{% trans "Download" %}</span>
+                    <a href="{{ original.url }}" target="_blank" class="button" download="{{ original.original_filename }}" rel="noopener noreferrer">
+                        <span class="icon fa fa-download filer-icon filer-icon-download"></span>&nbsp;
+                        <span>{% translate "Download" %}</span>
                     </a>
-                    {% if original.mime_maintype == 'image' %}
-                    <a href="{{ original.url }}" target="_blank" class="btn float-right">
-                        <span>{% trans "Expand" %}</span>&nbsp;
-                        <span class="icon fa fa-expand"></span>
+                    {% if original.mime_maintype == 'image' and "svg" not in original.mime_type %}
+                    <a href="{{ original.url }}" target="_blank" rel="noopener noreferrer" class="button">
+                        <span>{% translate "Expand" %}</span>&nbsp;
+                        <span class="icon filer-icon filer-icon-expand fa fa-expand"></span>
                     </a>
                     {% endif %}
                 {% else %}
-                    <span class="warning">{% trans "File is missing" %}</span>
+                    <span class="warning">{% translate "File is missing" %}</span>
                 {% endif %}
                 </div>
             </div>
         </div>
         <div class="image-details-right">
             {% if original.file_type or original.modified_at or original.uploaded_at or original.width or original.height or original.size %}
                 <dl class="image-details">
                     {% if original.file_type %}
-                        <dt>{% trans "Type" %}</dt>
-                        <dd>{{ original.extension|upper }} {{ original.file_type }}</dd>
+                        <dt>{% translate "Type" %}</dt>
+                        <dd>{{ original.extension|upper }} {{ original.file_type }} ({{ original.mime_type }})</dd>
                     {% endif %}
                     {% if original.width or original.height %}
-                        <dt>{% trans "Size" %}</dt>
+                        <dt>{% translate "Size" %}</dt>
                         <dd>{{ original.width|floatformat }}x{{ original.height|floatformat }} px</dd>
                     {% endif %}
                     {% if original.size %}
-                        <dt>{% trans "File-size" %}</dt>
+                        <dt>{% translate "File-size" %}</dt>
                         <dd>{{ original.size|filesizeformat }}</dd>
                     {% endif %}
                     {% if original.modified_at %}
-                        <dt>{% trans "Modified" %}</dt>
+                        <dt>{% translate "Modified" %}</dt>
                         <dd>{{ original.modified_at }}</dd>
                     {% endif %}
                     {% if original.uploaded_at %}
-                        <dt>{% trans "Created" %}</dt>
+                        <dt>{% translate "Created" %}</dt>
                         <dd>{{ original.uploaded_at }}</dd>
                     {% endif %}
+                    {% if original.owner %}
+                        <dt>{% translate "Owner" %}</dt>
+                        <dd><strong>{{ original.owner }}</strong></dd>
+                    {% endif %}
                 </dl>
-                <div class="image-actions">
-                    <ul class="actions-list">
-                        <li>
-                            <span class="icon fa fa-user"></span>
-                            {% if original.owner %}
-                                <span class="text">{% trans "Owner" %}: <strong>{{ original.owner }}</strong></span>
-                            {% endif %}
-                        </li>
-                    </ul>
-                </div>
             {% endif %}
         </div>
     </section>
```

#### html2text {}

```diff
@@ -1,13 +1,11 @@
 {% load filer_admin_tags i18n static %}
- {{ original }}
 {% file_icon original detail=True %}
-{% if original.file.exists %} _ {%_trans_"Download"_%} {% if
-original.mime_maintype == 'image' %} {%_trans_"Expand"_%} _ {% endif %} {% else
-%} {% trans "File is missing" %} {% endif %}
+{% if original.file.exists %}  _{%_translate_"Download"_%} {% if
+original.mime_maintype == 'image' and "svg" not in original.mime_type %} {%
+translate_"Expand"_%} _ {% endif %} {% else %} {% translate "File is missing"
+%} {% endif %}
 {% if original.file_type or original.modified_at or original.uploaded_at or
 original.width or original.height or original.size %}
 {% if original.file_type %}
-    *  {% if original.owner %} {% trans "Owner" %}: {{ original.owner }} {%
-      endif %}
 {% endif %}
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/widgets/admin_file.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/widgets/admin_file.html`

 * *Files 16% similar despite different names*

```diff
@@ -3,48 +3,57 @@
 {% spaceless %}
     <div class="clearfix"></div>
 
     <div class="dz-preview dz-file-preview hidden js-filer-dropzone-template">
         <span class="filerFile">
             <div class="dz-thumbnail"><img class="quiet" data-dz-thumbnail></div>
             <span data-dz-name class="dz-name"></span>
-            <img class="filerClearer" src="{% static admin_icon_delete %}" width="10" height="10" alt="{% trans 'Clear' %}" title="{% trans 'Clear' %}"
-                 data-dz-remove data-no-icon-file="{% static 'filer/icons/file-unknown.svg' %}">
+            <span class="filerClearer fa fa-close filer-icon filer-icon-remove-selection" title="{% translate 'Clear' %}"
+                 data-dz-remove data-no-icon-file="{% static 'filer/icons/file-unknown.svg' %}"></span>
             <div class="dz-progress js-filer-dropzone-progress"><span class="dz-upload" data-dz-uploadprogress></span></div>
         </span>
     </div>
 
-    <div class="js-filer-dropzone filer-dropzone{% if object %} js-object-attached{% endif %}" data-url="{% url 'admin:filer-ajax_upload' %}" data-max-file-size="20">
+    <div class="js-filer-dropzone filer-dropzone{% if object %} js-object-attached{% endif %}"
+         data-url="{% url 'admin:filer-ajax_upload' %}"
+         data-max-files="1"
+         {% if max_filesize %}}data-max-filesize="{{ max_filesize|safe }}"{% endif %}>
         <div class="z-index-fix"></div>
         <div class="dz-default dz-message js-filer-dropzone-message{% if object %} hidden{% endif %}">
-            <span class="icon fa fa-arrow-down"></span><span>{% trans "or drop your file here" %}</span>
+            <span class="icon filer-icon filer-icon-arrow-down fa fa-arrow-down"></span><span>{% translate "or drop your file here" %}</span>
         </div>
 
         <span class="filerFile js-file-selector">
             {% if object %}
                 {% if object.file.exists %}
                     <a href="{{ object.url }}" target="_blank">{% file_icon object size='80x80' %}</a>
                     &nbsp;<span class="description_text">{{ object.label }}</span>
                 {% else %}
                     {% file_icon object %}
-                    &nbsp;<span class="description_text">{% trans 'File is missing' %}</span>
+                    &nbsp;<span class="description_text">{% translate 'File is missing' %}</span>
                 {% endif %}
             {% else %}
-                <img class="thumbnail_img hidden quiet" alt="{% trans 'no file selected' %}">
+                <img class="thumbnail_img hidden quiet" alt="{% translate 'no file selected' %}">
                 &nbsp;<span class="description_text"></span>
             {% endif %}
 
-            <img class="filerClearer {% if not object %}hidden{% endif %}" src="{% static admin_icon_delete %}"
-                 width="10" height="10" alt="{% trans 'Clear' %}" title="{% trans 'Clear' %}"
-                 data-no-icon-file="{% static 'filer/icons/file-unknown.svg' %}">
+            <a class="filerClearer {% if not object %}hidden{% endif %}" title="{% translate 'Clear' %}"
+                 data-no-icon-file="{% static 'filer/icons/file-unknown.svg' %}" href="#">
+                <span class="fa fa-close filer-icon filer-icon-remove-selection"></span>
+            </a>
+
+            <a href="{{ change_url }}?_edit_from_widget=1" class="js-related-edit related-lookup {% if object %}related-lookup-change{% endif %} edit" id="{{ id }}_change"
+                 title="{% translate 'Edit' %}">
+                  <span class="edit-file"><span class="fa fa-pencil cms-icon cms-icon-settings"></span></span>
+            </a>
 
             <a href="{{ lookup_url }}" class="js-related-lookup related-lookup {% if object %}related-lookup-change{% endif %} lookup" id="{{ id }}_lookup"
-               title="{% trans 'Lookup' %}">
-                <span class="choose-file"><span class="fa fa-picture-o"></span>{% trans 'Choose File' %}</span>
-                <span class="edit-file"><span class="fa fa-pencil"></span></span>
+               title="{% translate 'Lookup' %}">
+                <span class="choose-file"><span class="fa fa-search cms-icon cms-icon-search"></span>{% translate 'Choose File' %}</span>
+                <span class="replace-file"><span class="fa fa-search cms-icon cms-icon-search"></span></span>
             </a>
 
             <br>
 
             <div class="hidden">{{ hidden_input }}</div>
             <script type="text/javascript" id="{{id}}_javascript">
                 django.jQuery(document).ready(function(){
```

### Comparing `django-filer-2.3rc1/filer/templates/admin/filer/widgets/admin_folder.html` & `django-filer-3.0.0rc1/filer/templates/admin/filer/widgets/admin_folder.html`

 * *Files 12% similar despite different names*

```diff
@@ -35,9 +35,7 @@
 
                 clearButton.addClass('hidden');
                 addFolderButton.removeClass('hidden');
             });
         }(django.jQuery));
     </script>
 {% endspaceless %}
-
-<link rel="stylesheet" type="text/css" href="{% static 'filer/css/admin_filer.css' %}">
```

### Comparing `django-filer-2.3rc1/filer/templatetags/filer_admin_tags.py` & `django-filer-3.0.0rc1/filer/templatetags/filer_admin_tags.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from math import ceil
 
 from django.contrib.staticfiles.storage import staticfiles_storage
+from django.core.files.storage import FileSystemStorage, default_storage
 from django.template import Library
+from django.templatetags.static import static
+from django.urls import reverse
 from django.utils.html import escapejs, format_html_join
+from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 
 from easy_thumbnails.files import get_thumbnailer
+from easy_thumbnails.options import ThumbnailOptions
 
 from filer import settings
 from filer.admin.tools import admin_url_params, admin_url_params_encoded
 from filer.models.imagemodels import BaseImage
+from filer.settings import DEFERRED_THUMBNAIL_SIZES
 
 
 register = Library()
 
 assignment_tag = getattr(register, 'assignment_tag', register.simple_tag)
 
 
@@ -33,15 +39,15 @@
 @register.inclusion_tag(
     'admin/filer/folder/list_type_switcher.html',
     takes_context=True,
 )
 def filer_folder_list_type_switcher(context):
     choice_list = settings.FILER_FOLDER_ADMIN_LIST_TYPE_CHOICES
     current_list_type = context['list_type']
-    # This solution is user friendly when there's only 2 choices
+    # This solution is user-friendly when there's only 2 choices
     # If there will be more list types then please change this switcher to more
     # proper widget (like for e.g. select list)
     next_list_type = next(
         iter(choice_list[choice_list.index(current_list_type) + 1:]),
         choice_list[0],
     )
 
@@ -72,27 +78,28 @@
 
 @assignment_tag(takes_context=True)
 def filer_has_permission(context, item, action):
     """Does the current user (taken from the request in the context) have
     permission to do the given action on the given item.
 
     """
-    permission_method_name = 'has_{action}_permission'.format(action=action)
+    permission_method_name = f'has_{action}_permission'
     permission_method = getattr(item, permission_method_name, None)
     request = context.get('request')
 
     if not permission_method or not request:
         return False
     # Call the permission method.
     # This amounts to calling `item.has_X_permission(request)`
     return permission_method(request)
 
 
 def file_icon_context(file, detail, width, height):
-    if not file.file.exists():
+    # Only check on FileSystemStorage if file exists for performance reasons
+    if isinstance(default_storage, FileSystemStorage) and not file.file.exists():
         return {
             'icon_url': staticfiles_storage.url('filer/icons/file-missing.svg'),
             'alt_text': _("File is missing"),
             'width': width,
             'height': height,
         }
     mime_maintype, mime_subtype = file.mime_maintype, file.mime_subtype
@@ -112,23 +119,37 @@
         else:
             if detail:
                 width, height = 210, ceil(210 / file.width * file.height)
                 context['sidebar_image_ratio'] = file.width / 210
                 opts = {'size': (width, height), 'upscale': True}
             else:
                 opts = {'size': (width, height), 'crop': True}
-            icon_url = thumbnailer.get_thumbnail(opts).url
-            context['alt_text'] = file.default_alt_text
-            if mime_subtype != 'svg+xml':
-                opts['size'] = 2 * width, 2 * height
-                context['highres_url'] = thumbnailer.get_thumbnail(opts).url
+            thumbnail_options = ThumbnailOptions(opts)
+            # Optimize directory listing:
+            if not detail and width == height and width in DEFERRED_THUMBNAIL_SIZES and hasattr(file, "thumbnail_name"):
+                # Get name of thumbnail from easy-thumbnail
+                configured_name = thumbnailer.get_thumbnail_name(thumbnail_options, transparent=file._transparent)
+                # If the name was annotated: Thumbnail exists and we can use it
+                if configured_name == file.thumbnail_name:
+                    icon_url = default_storage.url(configured_name)
+                    if mime_subtype != 'svg+xml' and file.thumbnailx2_name:
+                        context['highres_url'] = default_storage.url(file.thumbnailx2_name)
+                else:  # Probably does not exist, defer creation
+                    icon_url = reverse("admin:filer_file_fileicon", args=(file.pk, width))
+                context['alt_text'] = file.default_alt_text
+            else:
+                icon_url = thumbnailer.get_thumbnail(thumbnail_options).url
+                context['alt_text'] = file.default_alt_text
+                if mime_subtype != 'svg+xml':
+                    thumbnail_options['size'] = 2 * width, 2 * height
+                    context['highres_url'] = thumbnailer.get_thumbnail(thumbnail_options).url
     elif mime_maintype in ['audio', 'font', 'video']:
-        icon_url = staticfiles_storage.url('filer/icons/file-{}.svg'.format(mime_maintype))
+        icon_url = staticfiles_storage.url(f'filer/icons/file-{mime_maintype}.svg')
     elif mime_maintype == 'application' and mime_subtype in ['zip', 'pdf']:
-        icon_url = staticfiles_storage.url('filer/icons/file-{}.svg'.format(mime_subtype))
+        icon_url = staticfiles_storage.url(f'filer/icons/file-{mime_subtype}.svg')
     else:
         icon_url = staticfiles_storage.url('filer/icons/file-unknown.svg')
     context.update(width=width, height=height, icon_url=icon_url)
     return context
 
 
 @register.inclusion_tag('admin/filer/templatetags/file_icon.html')
@@ -143,9 +164,20 @@
     else:
         width, height = (75, 75) if detail else (40, 40)
     return file_icon_context(file, detail, width, height)
 
 
 @register.simple_tag
 def file_icon_url(file):
-    context = file_icon_context(file, False, 80, 80)
-    return escapejs(context.get('highres_url', context['icon_url']))
+    # Cache since it is called repeatedly by templates
+    if not hasattr(file, "_file_icon_url_cache"):
+        context = file_icon_context(file, False, 80, 80)
+        file._file_icon_url_cache = escapejs(context.get('highres_url', context['icon_url']))
+    return file._file_icon_url_cache
+
+
+@register.simple_tag
+def icon_css_library():
+    html = ""
+    for lib in settings.ICON_CSS_LIB:
+        html += f'<link rel="stylesheet" type="text/css" href="{static(lib)}">'
+    return mark_safe(html)
```

### Comparing `django-filer-2.3rc1/filer/templatetags/filer_image_tags.py` & `django-filer-3.0.0rc1/filer/templatetags/filer_image_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/templatetags/filer_tags.py` & `django-filer-3.0.0rc1/filer/templatetags/filer_tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,20 +80,20 @@
             bytes = '%.0f' % bytes
         else:
             bytes = '%.1f' % bytes
         if format.endswith('long'):
             unit = filesize_long_formats.get(unit, '')
             if base == 1024 and unit:
                 unit = '%sbi' % unit[:2]
-            unit = '%sbyte%s' % (unit, bytes != '1' and 's' or '')
+            unit = '{}byte{}'.format(unit, bytes != '1' and 's' or '')
         else:
-            unit = '%s%s' % (base == 1024 and unit.upper() or unit,
+            unit = '{}{}'.format(base == 1024 and unit.upper() or unit,
                              base == 1024 and 'iB' or 'B')
 
-        return '%s %s' % (bytes, unit)
+        return '{} {}'.format(bytes, unit)
 
     if bytes == 0:
         return bytes
     base = filesize_formats.index(format[0]) + 1
     # Exact multiple of 1000
     if format_len == 2:
         return bytes / (1000.0 ** base)
```

### Comparing `django-filer-2.3rc1/filer/thumbnail_processors.py` & `django-filer-3.0.0rc1/filer/thumbnail_processors.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 def scale_and_crop_with_subject_location(im, size, subject_location=False,
                                          zoom=None, crop=False, upscale=False,
                                          **kwargs):
     """
     Like ``easy_thumbnails.processors.scale_and_crop``, but will use the
     coordinates in ``subject_location`` to make sure that that part of the
     image is in the center or at least somewhere on the cropped image.
-    Please not that this does *not* work correctly if the image has been
+    Please note that this does *not* work correctly if the image has been
     resized by a previous processor (e.g ``autocrop``).
 
     ``crop`` needs to be set for this to work, but any special cropping
     parameters will be ignored.
     """
     subject_location = normalize_subject_location(subject_location)
     if not (subject_location and crop):
@@ -50,16 +50,16 @@
         return processors.scale_and_crop(im, size, zoom=zoom, crop=crop,
                                          upscale=upscale, **kwargs)
 
     # for here on we have a subject_location and cropping is on
 
     # --snip-- this is a copy and paste of the first few
     #          lines of ``scale_and_crop``
-    source_x, source_y = [float(v) for v in im.size]
-    target_x, target_y = [float(v) for v in size]
+    source_x, source_y = (float(v) for v in im.size)
+    target_x, target_y = (float(v) for v in size)
 
     if crop or not target_x or not target_y:
         scale = max(target_x / source_x, target_y / source_y)
     else:
         scale = min(target_x / source_x, target_y / source_y)
 
     # Handle one-dimensional targets.
@@ -79,15 +79,15 @@
                        resample=Image.ANTIALIAS)
     # --endsnip-- begin real code
 
     # ===============================
     # subject location aware cropping
     # ===============================
     # res_x, res_y: the resolution of the possibly already resized image
-    res_x, res_y = [float(v) for v in im.size]
+    res_x, res_y = (float(v) for v in im.size)
 
     # subj_x, subj_y: the position of the subject (maybe already re-scaled)
     subj_x = res_x * float(subject_location[0]) / source_x
     subj_y = res_y * float(subject_location[1]) / source_y
     ex = (res_x - min(res_x, target_x)) / 2
     ey = (res_y - min(res_y, target_y)) / 2
     fx, fy = res_x - ex, res_y - ey
```

### Comparing `django-filer-2.3rc1/filer/utils/compatibility.py` & `django-filer-3.0.0rc1/filer/utils/compatibility.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 truncate_words = keep_lazy(truncate_words, str)
 
 
 def get_delete_permission(opts):
     from django.contrib.auth import get_permission_codename
-    return '%s.%s' % (opts.app_label, get_permission_codename('delete', opts))
+    return '{}.{}'.format(opts.app_label, get_permission_codename('delete', opts))
 
 
 try:
     from PIL import ExifTags as PILExifTags
     from PIL import Image as PILImage
     from PIL import ImageDraw as PILImageDraw
 except ImportError:
```

### Comparing `django-filer-2.3rc1/filer/utils/filer_easy_thumbnails.py` & `django-filer-3.0.0rc1/filer/utils/filer_easy_thumbnails.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,34 +39,34 @@
             extension = self.thumbnail_transparency_extension
         else:
             extension = self.thumbnail_extension
         extension = extension or 'jpg'
 
         thumbnail_options = thumbnail_options.copy()
         size = tuple(thumbnail_options.pop('size'))
-        initial_opts = ['{0}x{1}'.format(*size)]
+        initial_opts = ['{}x{}'.format(*size)]
         quality = thumbnail_options.pop('quality', self.thumbnail_quality)
         if extension == 'jpg':
-            initial_opts.append('q{}'.format(quality))
+            initial_opts.append(f'q{quality}')
         elif extension == 'svg':
             thumbnail_options.pop('subsampling', None)
             thumbnail_options.pop('upscale', None)
 
         opts = list(thumbnail_options.items())
         opts.sort()   # Sort the options so the file name is consistent.
-        opts = ['{}'.format(v is not True and '{}-{}'.format(k, v) or k)
+        opts = ['{}'.format(v is not True and f'{k}-{v}' or k)
                 for k, v in opts if v]
         all_opts = '_'.join(initial_opts + opts)
 
         basedir = self.thumbnail_basedir
         subdir = self.thumbnail_subdir
 
         # make sure our magic delimiter is not used in all_opts
         all_opts = all_opts.replace('__', '_')
-        filename = '{}__{}.{}'.format(source_filename, all_opts, extension)
+        filename = f'{source_filename}__{all_opts}.{extension}'
 
         return os.path.join(basedir, path, subdir, filename)
 
 
 class ActionThumbnailerMixin:
     thumbnail_basedir = ''
     thumbnail_subdir = ''
```

### Comparing `django-filer-2.3rc1/filer/utils/files.py` & `django-filer-3.0.0rc1/filer/utils/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,31 +2,29 @@
 import os
 
 from django.http.multipartparser import ChunkIter, SkipFile, StopFutureHandlers, StopUpload, exhaust
 from django.template.defaultfilters import slugify as slugify_django
 from django.utils.encoding import force_str
 from django.utils.text import get_valid_filename as get_valid_filename_django
 
-from unidecode import unidecode
-
 
 class UploadException(Exception):
     pass
 
 
 def handle_upload(request):
     if not request.method == 'POST':
         raise UploadException("XMLHttpRequest not valid: must be POST")
     if request.headers.get('x-requested-with') == 'XMLHttpRequest':
         # the file is stored raw in the request
         is_raw = True
         filename = request.GET.get('qqfile', False) or request.GET.get('filename', False) or ''
 
         try:
-            content_length = int(request.META['CONTENT_LENGTH'])
+            content_length = int(request.headers['content-length'])
         except (IndexError, TypeError, ValueError):
             content_length = None
 
         if content_length < 0:
             # This means we shouldn't continue...raise an error.
             raise UploadException("Invalid content length: %r" % content_length)
 
@@ -116,23 +114,23 @@
     if mime_type != 'application/octet-stream' and extensions and iext.lower() not in extensions:
         msg = "MIME-Type '{mimetype}' does not correspond to file extension of {filename}."
         raise UploadException(msg.format(mimetype=mime_type, filename=filename))
     return upload, filename, is_raw, mime_type
 
 
 def slugify(string):
-    return slugify_django(unidecode(force_str(string)))
+    return slugify_django(force_str(string))
 
 
 def get_valid_filename(s):
     """
     like the regular get_valid_filename, but also slugifies away
     umlauts and stuff.
     """
     s = get_valid_filename_django(s)
     filename, ext = os.path.splitext(s)
     filename = slugify(filename)
     ext = slugify(ext)
     if ext:
-        return "%s.%s" % (filename, ext)
+        return "{}.{}".format(filename, ext)
     else:
-        return "%s" % (filename,)
+        return "{}".format(filename)
```

### Comparing `django-filer-2.3rc1/filer/utils/generate_filename.py` & `django-filer-3.0.0rc1/filer/utils/generate_filename.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/utils/loader.py` & `django-filer-3.0.0rc1/filer/utils/loader.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/utils/pil_exif.py` & `django-filer-3.0.0rc1/filer/utils/pil_exif.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from ..utils.compatibility import PILExifTags, PILImage
 
 
 def get_exif(im):
     try:
         exif_raw = im._getexif() or {}
-    except:  # noqa
+    except Exception:
+        # Not available? Return empty dict
         return {}
     ret = {}
     for tag, value in list(exif_raw.items()):
         decoded = PILExifTags.TAGS.get(tag, tag)
         ret[decoded] = value
     return ret
 
@@ -19,10 +20,10 @@
     im = PILImage.open(storage.open(file_obj.name), 'r')
     return get_exif(im)
 
 
 def get_subject_location(exif_data):
     try:
         r = (int(exif_data['SubjectLocation'][0]), int(exif_data['SubjectLocation'][1]),)
-    except:  # noqa
+    except KeyError:
         r = None
     return r
```

### Comparing `django-filer-2.3rc1/filer/utils/recursive_dictionary.py` & `django-filer-3.0.0rc1/filer/utils/recursive_dictionary.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/filer/utils/zip.py` & `django-filer-3.0.0rc1/filer/utils/zip.py`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/setup.cfg` & `django-filer-3.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-filer-2.3rc1/setup.py` & `django-filer-3.0.0rc1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 from setuptools import find_packages, setup
 
 from filer import __version__
 
 
 REQUIREMENTS = [
     'django>=2.2,<5',
-    'django-mptt',
     'django-polymorphic',
     'easy-thumbnails[svg]',
-    'Unidecode>=0.04,<1.2',
 ]
 
 
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
@@ -28,14 +26,15 @@
     'Framework :: Django',
     'Framework :: Django :: 2.2',
     'Framework :: Django :: 3.0',
     'Framework :: Django :: 3.1',
     'Framework :: Django :: 3.2',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
+    'Framework :: Django :: 4.2',
     'Framework :: Django CMS',
     'Framework :: Django CMS :: 3.6',
     'Framework :: Django CMS :: 3.7',
     'Framework :: Django CMS :: 3.8',
     'Framework :: Django CMS :: 3.9',
     'Framework :: Django CMS :: 3.10',
     'Framework :: Django CMS :: 3.11',
```

