# Comparing `tmp/django-listing-0.0.8.tar.gz` & `tmp/django-listing-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-listing-0.0.8.tar", last modified: Wed Jul 15 07:32:21 2020, max compression
+gzip compressed data, was "dist/django-listing-0.0.9.tar", last modified: Tue Nov  9 08:54:01 2021, max compression
```

## Comparing `django-listing-0.0.8.tar` & `django-listing-0.0.9.tar`

### file list

```diff
@@ -1,86 +1,93 @@
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2020-07-15 07:32:21.000000 django-listing-0.0.8/setup.cfg
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    17675 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/filters.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10991 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/record.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    16749 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/views.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    40469 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/columns.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     9878 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/toolbar.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      631 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/exceptions.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1997 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/utils.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      622 2020-07-15 07:20:01.000000 django-listing-0.0.8/django_listing/__init__.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8150 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/listing_form.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    38775 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/listing.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/templates/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/templates/django_listing/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      225 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/empty_listing.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      277 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/selection_overlay.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      693 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/tbi_variations.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      815 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/tbi_dropdown.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1188 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/listing_div.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1557 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/tbi_select.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1405 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/view_object_popup.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      852 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/footer.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      311 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/header.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      202 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/toolbar.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5031 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/listing.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1640 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/actions_buttons.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    12926 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/paginator.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1982 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/filters_form.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2759 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/listing_form.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        9 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templates/django_listing/div_row.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1725 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/html_attributes.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      136 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/apps.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7396 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/aggregations.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    12396 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/actions_buttons_column.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/locale/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/locale/en/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/locale/en/LC_MESSAGES/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5411 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/locale/fr/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5410 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/static/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/static/django_listing/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/static/django_listing/js/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     9067 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/js/django_listing.js
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/static/django_listing/css/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15304 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/css/django_listing-ie7.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15031 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/css/django_listing-ie7-codes.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1857 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/css/animation.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8452 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/css/django_listing-codes.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    31302 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/css/django_listing.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74922 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/css/django_listing-embedded.css
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/static/django_listing/icons/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1137 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/icons/csv.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      989 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/icons/tsv.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1086 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/icons/xlsx.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1171 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/icons/html.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      948 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/icons/xls.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3686 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/icons/ods.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2109 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/icons/json.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1721 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/icons/dbf.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1502 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/icons/pdf.svg
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/static/django_listing/font/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    99231 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/font/django_listing.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74488 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/font/django_listing.eot
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    40228 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/font/django_listing.woff
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74296 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/font/django_listing.ttf
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    32996 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/static/django_listing/font/django_listing.woff2
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8173 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/paginators.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing/templatetags/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8298 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templatetags/django_listing.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/templatetags/__init__.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1226 2020-07-14 05:49:09.000000 django-listing-0.0.8/django_listing/context.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3639 2020-07-15 07:23:10.000000 django-listing-0.0.8/README.rst
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1928 2020-07-14 09:17:58.000000 django-listing-0.0.8/setup.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      215 2020-07-14 05:49:09.000000 django-listing-0.0.8/MANIFEST.in
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      119 2020-07-14 06:51:10.000000 django-listing-0.0.8/CHANGES.rst
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing.egg-info/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2020-07-14 05:54:06.000000 django-listing-0.0.8/django_listing.egg-info/not-zip-safe
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3030 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing.egg-info/SOURCES.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       15 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing.egg-info/top_level.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       55 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing.egg-info/requires.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing.egg-info/dependency_links.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5263 2020-07-15 07:32:21.000000 django-listing-0.0.8/django_listing.egg-info/PKG-INFO
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5263 2020-07-15 07:32:21.000000 django-listing-0.0.8/PKG-INFO
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing.egg-info/
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)        1 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing.egg-info/dependency_links.txt
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)        1 2020-07-24 15:40:15.000000 django-listing-0.0.9/django_listing.egg-info/not-zip-safe
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)       55 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing.egg-info/requires.txt
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)     5410 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing.egg-info/PKG-INFO
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)       15 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing.egg-info/top_level.txt
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)     3341 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing.egg-info/SOURCES.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      234 2021-11-09 08:50:06.000000 django-listing-0.0.9/CHANGES.rst
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2021-11-09 08:54:00.000000 django-listing-0.0.9/setup.cfg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      982 2021-04-01 07:22:20.000000 django-listing-0.0.9/LICENSE.rst
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1928 2020-07-24 13:34:19.000000 django-listing-0.0.9/setup.py
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/locale/
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/locale/fr/
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5410 2020-05-15 07:06:48.000000 django-listing-0.0.9/django_listing/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      379 2020-05-15 07:06:39.000000 django-listing-0.0.9/django_listing/locale/fr/LC_MESSAGES/django.mo
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/locale/en/
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5411 2020-05-15 07:06:44.000000 django-listing-0.0.9/django_listing/locale/en/LC_MESSAGES/django.po
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      380 2020-05-15 07:06:39.000000 django-listing-0.0.9/django_listing/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    17683 2020-07-24 13:34:19.000000 django-listing-0.0.9/django_listing/filters.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10991 2020-05-20 12:15:51.000000 django-listing-0.0.9/django_listing/record.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      622 2021-11-09 08:50:06.000000 django-listing-0.0.9/django_listing/__init__.py
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/templatetags/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/templatetags/__init__.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    11013 2021-02-22 12:43:13.000000 django-listing-0.0.9/django_listing/templatetags/django_listing.py
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/templates/
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/templates/django_listing/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    13292 2021-08-19 06:39:39.000000 django-listing-0.0.9/django_listing/templates/django_listing/paginator.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      815 2020-05-19 13:04:26.000000 django-listing-0.0.9/django_listing/templates/django_listing/tbi_dropdown.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      384 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/templates/django_listing/tbi_update.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2759 2020-05-17 09:45:41.000000 django-listing-0.0.9/django_listing/templates/django_listing/listing_form.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      693 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/templates/django_listing/tbi_variations.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        9 2018-05-13 07:49:23.000000 django-listing-0.0.9/django_listing/templates/django_listing/div_row.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1785 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/templates/django_listing/action_footer.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6309 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/templates/django_listing/listing.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      202 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/templates/django_listing/toolbar.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1843 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/templates/django_listing/footer.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      452 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/templates/django_listing/header.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      226 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/templates/django_listing/empty_listing.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      277 2019-04-09 10:09:14.000000 django-listing-0.0.9/django_listing/templates/django_listing/selection_overlay.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1405 2020-05-29 10:15:29.000000 django-listing-0.0.9/django_listing/templates/django_listing/view_object_popup.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1982 2019-04-09 10:09:14.000000 django-listing-0.0.9/django_listing/templates/django_listing/filters_form.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1188 2018-06-21 08:12:52.000000 django-listing-0.0.9/django_listing/templates/django_listing/listing_div.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1557 2020-05-19 13:04:19.000000 django-listing-0.0.9/django_listing/templates/django_listing/tbi_select.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      824 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/templates/django_listing/action_header.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1750 2021-08-23 13:08:34.000000 django-listing-0.0.9/django_listing/templates/django_listing/actions_buttons.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1226 2018-04-26 06:48:47.000000 django-listing-0.0.9/django_listing/context.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2031 2021-08-20 07:33:53.000000 django-listing-0.0.9/django_listing/utils.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    42360 2021-08-23 15:51:02.000000 django-listing-0.0.9/django_listing/listing.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7396 2018-04-26 06:48:47.000000 django-listing-0.0.9/django_listing/aggregations.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    17977 2021-08-23 15:51:02.000000 django-listing-0.0.9/django_listing/views.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7851 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/listing_form.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    41819 2021-08-20 15:32:45.000000 django-listing-0.0.9/django_listing/columns.py
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/static/
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/static/django_listing/
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/static/django_listing/js/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10551 2021-08-19 14:55:45.000000 django-listing-0.0.9/django_listing/static/django_listing/js/django_listing.js
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1137 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/csv.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2109 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/json.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1086 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/xlsx.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1502 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/pdf.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1721 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/dbf.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      948 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/xls.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      989 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/tsv.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1171 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/html.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3686 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/ods.svg
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/static/django_listing/css/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74922 2019-04-09 10:09:14.000000 django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-embedded.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8452 2019-04-09 10:09:14.000000 django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-codes.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15031 2019-04-09 10:09:14.000000 django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-ie7-codes.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15304 2019-04-09 10:09:14.000000 django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-ie7.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    32713 2021-08-20 07:03:29.000000 django-listing-0.0.9/django_listing/static/django_listing/css/django_listing.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1857 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/css/animation.css
+drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/static/django_listing/font/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74488 2020-05-06 06:54:52.000000 django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.eot
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    99231 2020-05-06 06:54:52.000000 django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    40228 2020-05-06 06:54:52.000000 django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.woff
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74296 2020-05-06 06:54:52.000000 django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.ttf
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    32996 2020-05-06 06:54:52.000000 django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.woff2
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1841 2021-02-22 10:27:58.000000 django-listing-0.0.9/django_listing/app_settings.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      631 2018-07-26 15:34:44.000000 django-listing-0.0.9/django_listing/exceptions.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      136 2019-08-27 07:31:28.000000 django-listing-0.0.9/django_listing/apps.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10088 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/toolbar.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1725 2018-05-27 16:03:20.000000 django-listing-0.0.9/django_listing/html_attributes.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    12882 2021-08-23 14:09:39.000000 django-listing-0.0.9/django_listing/actions_buttons_column.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8239 2021-08-19 06:44:22.000000 django-listing-0.0.9/django_listing/paginators.py
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)     5410 2021-11-09 08:54:00.000000 django-listing-0.0.9/PKG-INFO
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3639 2020-07-24 13:34:19.000000 django-listing-0.0.9/README.rst
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      215 2020-05-30 19:21:14.000000 django-listing-0.0.9/MANIFEST.in
```

### Comparing `django-listing-0.0.8/django_listing/filters.py` & `django-listing-0.0.9/django_listing/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,19 +130,20 @@
                                     if isinstance(filtr,Filter) ]
         fbuttons = filters.form_buttons
         if isinstance(fbuttons,str):
             filters.form_buttons = list(map(str.strip,fbuttons.split(',')))
         return filters
 
     def datetimepicker_init(self):
-        self.listing.add_onready_snippet("\n"
-            "$('#{filters.id} .edit-datecolumn').datetimepicker({{timepicker:false, format:'{listing.datetimepicker_date_format}'}});\n"
-            "$('#{filters.id} .edit-datetimecolumn').datetimepicker({{format:'{listing.datetimepicker_datetime_format}'}});\n"
-            "$('#{filters.id} .edit-timecolumn').datetimepicker({{datepicker:false, format:'{listing.datetimepicker_time_format}'}});\n"
-            .format(filters=self, listing=self.listing))
+        self.listing.need_media_for('datetimepicker')
+        self.listing.add_onready_snippet(f"""
+            $('#{self.id} .edit-datecolumn').datetimepicker({{timepicker:false, format:'{self.listing.datetimepicker_date_format}'}});
+            $('#{self.id} .edit-datetimecolumn').datetimepicker({{format:'{self.listing.datetimepicker_datetime_format}'}});
+            $('#{self.id} .edit-timecolumn').datetimepicker({{datepicker:false, format:'{self.listing.datetimepicker_time_format}'}});
+            """)
 
     def create_filter(self, name, listing):
         if isinstance(name,str):
             model_attr_name, *_ = name.split('__')
             if issubclass(listing.model,models.Model):
                 field = listing.model._meta.get_field(model_attr_name)
                 if field:
```

### Comparing `django-listing-0.0.8/django_listing/record.py` & `django-listing-0.0.9/django_listing/record.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/views.py` & `django-listing-0.0.9/django_listing/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #
 # Created : 2018-02-09
 #
 # @author: Eric Lapouyade
 #
+import json
+
 from django.db.models import QuerySet
 from django.utils.module_loading import import_string
 from django.utils.safestring import mark_safe
 from django.views.generic import TemplateView
 from django.http import HttpResponse, HttpResponseServerError, \
     HttpResponseRedirect, QueryDict
 from django.template import RequestContext
@@ -32,14 +34,15 @@
 LISTING_REDIRECT_NONE = None
 LISTING_REDIRECT_SAME_PAGE = 1
 LISTING_REDIRECT_NO_EDIT = 2
 
 class ListingViewMixin:
     listing_class = None
     listing_data = None
+    upload_field = 'image'
     context_classes = ()
     listing_context_name = 'listing'
     listing_instance = None
     listing = None
     insert_success_redirect_url = LISTING_REDIRECT_NONE
     insert_success_msg = _('<b>{object}</b> has been successfully added.')
     insert_success_msg_no_save = _(
@@ -73,15 +76,15 @@
                             else:
                                 post[k] = v
                     request.POST = post
                 return self.manage_listing_ajax_request(request, *args, **kwargs)
             response = self.manage_listing_post(request, *args, **kwargs)
             if response:
                 return response
-            return self.get(request, *args, **kwargs)
+            return HttpResponseRedirect('.')
         except ListingException as e:
             return HttpResponseServerError(e)
 
     def get(self, request, *args, **kwargs):
         response = super().get(request, *args, **kwargs)
         # need to force rendering here to know whether a listing created
         # in a template has requested a data export
@@ -91,42 +94,49 @@
             filename = getattr(request,'export_filename','listing')
             response = HttpResponse(data)
             response['Content-Disposition'] = (
                 'attachment; filename="{}"'.format(filename) )
             return response
         return response
 
-    def get_listing_from_post(self, request):
+    def json_response(self, data):
+        response = HttpResponse(json.dumps(data), content_type='application/json')
+        response['Cache-Control'] = 'no-cache'
+        return response
+
+    def get_listing_from_post(self, request, refresh=False):
         listing_id = request.POST.get('listing_id', '')[:-3]  # remove '-id' suffix
         listing_suffix = request.POST.get('listing_suffix', '')
-        listing = self.get_listing_id(listing_id)
+        listing = self.get_listing_id(listing_id, refresh)
         if not listing:
             raise ListingException(
                 '{}-id is a bad listing ID : django-listing library misconf'
                 'iguration. Contact the webmaster !'.format(listing_id))
         Listing.set_suffix(request, listing, listing_suffix)
-        listing.action = request.POST.get('action')
+        listing.action = request.POST.get('force_action') or request.POST.get('action')
         listing.action_col = request.POST.get('action_col')
         return listing
 
     def manage_listing_ajax_request(self, request, *args, **kwargs):
         listing = self.get_listing_from_post(request)
         self.listing = listing
         response = None
         if listing:
             listing_part = request.POST.get('listing_part', 'all')
-            listing.set_attr('ajax_request', True)
-            listing.set_attr('ajax_part', listing_part)
+            listing.ajax_request = True
+            listing.ajax_part = listing_part
             if isinstance(listing.action, str) and listing.action:
                 listing.render_init(RequestContext(request))
                 method = getattr(self,'manage_listing_%s' % listing.action, None)
                 if callable(method):
                     response = method(listing, *args, **kwargs)
         if response:
             return response
+        if listing.have_to_refresh():
+            listing = self.get_listing_from_post(request, refresh=True)
         return HttpResponse(listing.render(RequestContext(request)))
 
     def get_listing_class(self):
         return self.listing_class
 
     def get_listing_data(self):
         return self.listing_data
@@ -142,22 +152,44 @@
 
     def get_listing_instance(self):
         data = self.get_listing_data()
         if isinstance(data, QuerySet) or data:
             listing_class = self.get_listing_class() or Listing
             return listing_class(data,**self.get_listing_params())
 
+    # this set of methods manage a special storage because when using ajax
+    # listing name are taken from div id which has been normalized
+    # by replacing underscores by dashes
+    def get_from_listing_instances(self, name):
+        v = self._listing_instances.get(name.replace('_','-'))
+        if v:
+            return v[1]
+        return None
+
+    def in_listing_instances(self, name):
+        return name.replace('_','-') in self._listing_instances
+
+    def set_to_listing_instances(self, name, instance):
+        self._listing_instances[name.replace('_','-')] = (name, instance)
+
+    def yield_listing_instances(self):
+        for v in self._listing_instances.values():
+            yield v[1]
+
+    def listing_instances_context(self):
+        return dict(self._listing_instances.values())
+
     def get_default_listing_instance(self):
         context_name = self.get_listing_context_name()
-        instance = self._listing_instances.get(context_name)
+        instance = self.get_from_listing_instances(context_name)
         if not instance:
             instance = self.get_listing_instance()
             if instance:
                 instance.id = context_name + '-id'  # Ensure id is set according to method name + '-id'
-                self._listing_instances[context_name] = instance
+                self.set_to_listing_instances(context_name, instance)
         return instance
 
     def get_listing_update_success_redirect_url(self, listing = None):
         url = self.update_success_redirect_url
         if listing:
             if url == LISTING_REDIRECT_SAME_PAGE:
                 url = listing.get_url()
@@ -194,14 +226,20 @@
                         response = method(listing, *args, **kwargs)
                 # elif listing.can_edit:
                 #     response = self.manage_listing_update(listing, *args, **kwargs)
                 # elif listing.can_select:
                 #     response = self.manage_listing_select(listing, *args, **kwargs)
             return response
 
+    def manage_listing_upload(self, listing, *args, **kwargs):
+        listing.model.objects.create(
+            **{self.upload_field:listing.request.FILES['file']}
+        )
+        return self.json_response(dict(message='OK',))
+
     def manage_listing_update(self, listing, *args, **kwargs):
         if listing.editable and listing.editing:
             formset = listing.get_formset()
             if formset.is_valid():
                 return self.manage_listing_update_valid(listing, formset)
             else:
                 # extract error strings from Django ErrorDict
@@ -319,27 +357,27 @@
             msg = ( self.update_success_msg_no_save
                 .format(listing=listing, nb_updates=nb_updates,
                         model_verbose=model_verbose) )
             if msg:
                 messages.add_message(listing.request, messages.INFO,
                     mark_safe(msg))
 
-    def get_listing_id(self, listing_id):
+    def get_listing_id(self, listing_id, refresh=False):
         """ For AJAX purposes : when using multiple listings on the same page
         and having one AJAX request : we need only ONE listing instance :
         the one from the given ID in the request. This avoids to create
         all listing instances when not necessary """
         if isinstance(listing_id,str):
-            instance = self._listing_instances.get(listing_id)
-            if instance is None:
+            instance = self.get_from_listing_instances(listing_id)
+            if instance is None or refresh==True:
                 method = getattr(
-                    self, INSTANCE_METHOD_PREFIX + listing_id, None)
+                    self, INSTANCE_METHOD_PREFIX + listing_id.replace('-','_'), None)
                 if callable(method):
                     instance = method()
-                    self._listing_instances[listing_id] = instance
+                    self.set_to_listing_instances(listing_id, instance)
                 else:
                     instance = self.get_default_listing_instance()
             if instance:
                 instance.id = listing_id + '-id'
             return instance
         return None
 
@@ -347,36 +385,31 @@
         prefix_length = len(INSTANCE_METHOD_PREFIX)
         # find all get_listing_instance_xxx
         for method_name in dir(self.__class__):
             if method_name.startswith(INSTANCE_METHOD_PREFIX):
                 method = getattr(self,method_name)
                 if callable(method):
                     listing_id = method_name[prefix_length:]
-                    if listing_id not in self._listing_instances:
+                    if not self.in_listing_instances(listing_id):
                         instance = method()
                         instance.id = listing_id + '-id' # Ensure id is set according to method name + '-id'
-                        self._listing_instances[listing_id] = instance
+                        self.set_to_listing_instances(listing_id, instance)
         self.get_default_listing_instance()  # will update self._listing_instances
-        for listing in self._listing_instances.values():
+        for listing in self.yield_listing_instances():
             if listing.is_initialized() and not listing.is_render_initialized():
                 listing.render_init(RequestContext(self.request))
 
-        return self._listing_instances
+        return self.listing_instances_context()
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context['request'] = self.request  # no need to add request context processor
         context['posted_listing'] = self.listing
         for cls in self.context_classes:
             context[cls.__name__] = cls
         if self.listing_class:
             context[self.listing_class.__name__] = self.listing_class
         context.update(self.get_listings_instances())
         return context
 
-    def add_listing_header_snippet(self, snippet):
-        if not hasattr(self.request,'django_listing_header_snippets'):
-            self.request.django_listing_header_snippets = []
-        self.request.django_listing_header_snippets.append(snippet)
-
 class ListingView(ListingViewMixin, TemplateView):
     pass
```

### Comparing `django-listing-0.0.8/django_listing/columns.py` & `django-listing-0.0.9/django_listing/columns.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,34 +11,37 @@
 from collections import OrderedDict
 from types import GeneratorType
 
 from django import forms
 from django.conf import settings
 from django.db import models
 from django.forms import widgets
+from django.template.defaultfilters import filesizeformat
 from django.utils import formats
 from django.utils.encoding import force_str
 from django.utils.html import conditional_escape
+from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 from django.utils.translation import ugettext
 
 from .aggregations import AggregationMeta, Aggregation
 from .context import RenderContext
 from .exceptions import *
 from .html_attributes import HTMLAttributes
 from .record import cache_in_record
 from .utils import init_dicts_from_class
+from .app_settings import app_settings
 
 __all__ = ['COLUMNS_PARAMS_KEYS', 'Columns', 'ModelColumns', 'SequenceColumns',
            'Column', 'BooleanColumn', 'CheckboxColumn', 'ChoiceColumn',
            'ManyColumn', 'DateColumn', 'DateTimeColumn', 'TimeColumn',
            'LinkColumn', 'TotalColumn', 'AvgColumn', 'MaxColumn', 'MinColumn',
-           'MultipleChoiceColumn','ButtonColumn','InputColumn',
-           'SelectColumn', 'ForeignKeyColumn', 'LinkObjectColumn',
-           'COLUMNS_FORM_FIELD_KEYS',]
+           'MultipleChoiceColumn','ButtonColumn','InputColumn', 'FileSizeColumn',
+           'SelectColumn', 'ForeignKeyColumn', 'LinkObjectColumn', 'ListingMethodRef',
+           'ButtonLinkColumn', 'COLUMNS_FORM_FIELD_KEYS',]
 
 COLUMNS_PARAMS_KEYS = {
     'name', 'header', 'footer', 'data_key', 'cell_edit_tpl',
     'cell_tpl', 'cell_attrs', 'value_tpl', 'cell_value', 'label',
     'header_tpl', 'header_sortable_tpl',
     'footer_tpl', 'footer_value_tpl', 'sort_key', 'sortable', 'header_attrs',
     'footer_attrs', 'ascending_by_default', 'model_field',
@@ -53,14 +56,24 @@
     'max_length','min_length','strip','empty_value','label','required',
     'label_suffix', 'initial', 'widget', 'help_text', 'error_messages',
     'validators', 'localize', 'disabled','input_formats','min_value',
     'max_value',
 }
 
 
+class ListingMethodRef:
+    """ Helper to reference a Listing method in column.cell_value instead of a lambda"""
+    def __init__(self, method_name):
+        self.method_name = method_name
+
+    def __call__(self, listing, *args, **kwargs):
+        method = getattr(listing, self.method_name)
+        return method(*args, **kwargs)
+
+
 class Columns(list):
     def __init__(self, *cols, params=None):
         if params is None:
             params = {}
         self._params = params
         self.name2col = {}
         if cols:
@@ -385,30 +398,32 @@
             return cls(field.name, model_field=field, **kwargs)
 
     def get_cell_attrs(self, rec, ctx, value):
         cell_attrs = self.cell_attrs
         if callable(cell_attrs):
             cell_attrs = cell_attrs(rec, ctx, value)
         attrs = HTMLAttributes(cell_attrs)
-        attrs.add('class',{'col-'+self.name,
+        attrs.add('class', {'col-'+self.name,
                            'type-'+type(value).__name__,
                            'cls-'+self.__class__.__name__.lower()
                            } | self.theme_cell_class)
         return attrs
 
     def get_default_value(self, rec):
         return self.default_value
 
     # def get_raw_value(self, rec):
     #     return rec.get(self.data_key)
 
     @cache_in_record
-    def get_cell_value(self,rec):
-        if callable(self.cell_value):
-            value = self.cell_value(self,rec)
+    def get_cell_value(self, rec):
+        if isinstance(self.cell_value, ListingMethodRef):
+            value = self.cell_value(self.listing, self, rec)
+        elif callable(self.cell_value):
+            value = self.cell_value(self, rec)
         else:
             value = rec.get(self.data_key)
             if value is None:
                 value = self.get_default_value(rec)
         return value
 
     def get_cell_exported_value(self,rec):
@@ -423,32 +438,28 @@
 
         # get the django form field (a formset form is attached to each record)
         # you get an instance of forms.CharField, forms.DateField etc...
         form_field = rec.get_form()[self.name]
         errors = form_field.errors
         if errors:
             html = ('<div class="form-field errors"><span class='
-                     '"listing-icon-attention">{errors}{form_field}</div>').format(
+                     '"listing-icon-attention"></span>{errors}{form_field}</div>').format(
                      errors=errors, form_field=form_field)
         else:
             html = ('<div class="form-field">{form_field}</div>').format(
                     form_field=form_field)
         return html
 
     def get_cell_context(self, rec, value):
         if isinstance(value,str):
             value = conditional_escape(value)
-        media_url = getattr(settings, 'MEDIA_URL', '/media/')
-        media_upload_url = getattr(settings, 'MEDIA_UPLOAD_URL', media_url+'uploads')
         return RenderContext(self.listing.global_context,
                              rec.get_format_ctx(),
                              value,  # if value is a dict it will be merged (see RenderContext)
                              value=value,  # if value is not a dict it will have the key 'value' in the context
-                             MEDIA_URL=media_url,
-                             MEDIA_UPLOAD_URL=media_upload_url,
                              rec=rec,
                              listing=self.listing,
                              col=self)
 
     def get_edit_value_tpl(self, rec, ctx, value):
         return self.render_form_field(rec)
 
@@ -539,15 +550,15 @@
             listing=self.listing,
             col=self)
 
     def get_header_template(self, ctx):
         if ctx.sort_url:
             return self.header_sortable_tpl or (
                    '<th{attrs}><a class="listing-nav" href="{sort_url}">{value}'
-                   '<span class="sorting{icon}"><span></a></th>')
+                   '<span class="sorting{icon}"></span></a></th>')
         else:
             return self.header_tpl or '<th{attrs}>{value}</th>'
 
     def render_header(self):
         ctx = self.get_header_context()
         ctx.attrs = self.get_header_attrs(ctx)
         tpl = self.get_header_template(ctx)
@@ -861,39 +872,49 @@
 
 
 class DateColumn(Column):
     date_format = settings.DATE_FORMAT
     params_keys = 'date_format'
     from_model_field_classes = (models.DateField,)
     form_field_class = forms.DateField
-    widget_attrs = {'class': 'edit-datecolumn'}
+    widget_attrs = {'class': 'edit-datecolumn', 'autocomplete':'off'}
 
     def get_cell_value(self,rec):
         value = super().get_cell_value(rec)
         if isinstance(value, datetime.date):
             return formats.date_format(value, self.date_format)
         return value
 
 
 class DateTimeColumn(Column):
     datetime_format = settings.DATETIME_FORMAT
     params_keys = 'datetime_format'
     from_model_field_classes = (models.DateTimeField,)
+    widget_attrs = {'class': 'edit-datetimecolumn', 'autocomplete':'off'}
 
     def get_cell_value(self,rec):
         value = super().get_cell_value(rec)
         if isinstance(value, datetime.date):  # date also match datetime
             return formats.date_format(value, self.datetime_format)
         return value
 
 
+class FileSizeColumn(Column):
+    def get_cell_value(self,rec):
+        value = super().get_cell_value(rec)
+        if isinstance(value, (int, float)):
+            return filesizeformat(value)
+        return value
+
+
 class TimeColumn(Column):
     time_format = settings.TIME_FORMAT
     params_keys = 'time_format'
     from_model_field_classes = (models.TimeField,)
+    widget_attrs = {'class': 'edit-timecolumn', 'autocomplete':'off'}
 
     def get_cell_value(self, rec):
         value = super().get_cell_value(rec)
         if isinstance(value, datetime.date):  # date also match datetime
             return formats.time_format(value, self.time_format)
         return value
 
@@ -907,38 +928,56 @@
     cell_edit_tpl = '<td{attrs}>%s</td>'
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def get_link_attrs(self, rec, value):
         link_attrs = self.link_attrs
-        if callable(link_attrs):
+        if isinstance(link_attrs, ListingMethodRef):
+            link_attrs = link_attrs(self.listing, self, rec, value)
+        elif callable(link_attrs):
             link_attrs = link_attrs(rec, value)
         attrs = HTMLAttributes(link_attrs or {})
         return attrs
 
     def get_href_tpl(self, rec, value):
         href_tpl = self.href_tpl
-        if callable(href_tpl):
+        if isinstance(href_tpl, ListingMethodRef):
+            href_tpl = href_tpl(self.listing, self, rec, value)
+        elif callable(href_tpl):
             href_tpl = href_tpl(rec, value)
         return href_tpl
 
     def get_href(self,rec, ctx, value):
         href_tpl = self.get_href_tpl(rec, value)
-        if isinstance(href_tpl,str):
+        if isinstance(href_tpl, str):
             return href_tpl.format(**ctx)
         return None
 
     def get_cell_context(self, rec, value):
         ctx = super().get_cell_context(rec, value)
         ctx.link_attrs = self.get_link_attrs(rec, value)
         if not self.no_link:
-            ctx.link_attrs.add('href',self.get_href(rec, ctx, value))
+            ctx.link_attrs.add('href', self.get_href(rec, ctx, value))
         return ctx
 
+
+class ButtonLinkColumn(LinkColumn):
+    label = 'Button'
+
+    def get_link_attrs(self, rec, value):
+        attrs = super().get_link_attrs(rec, value)
+        attrs.add('class', self.theme_button_class)
+        return attrs
+
+    def get_cell_value(self, rec):
+        value = mark_safe(self.label)
+        return value
+
+
 class URLColumn(LinkColumn):
     href_tpl = '{value}'
     from_model_field_classes = (models.URLField,)
     form_field_widget_class = widgets.URLInput
     params_keys = 'remove_proto'
     remove_proto = True
```

### Comparing `django-listing-0.0.8/django_listing/toolbar.py` & `django-listing-0.0.9/django_listing/toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 import re
 
 __all__ = [
     'TOOLBAR_PARAMS_KEYS', 'Toolbar', 'ToolbarItem',
     'SortSelectToolbarItem', 'VariationsToolbarItem',
     'PerPageSelectToolbarItem', 'ExportSelectToolbarItem',
     'PerPageDropdownToolbarItem', 'ExportDropdownToolbarItem',
-    'SortDropdownToolbarItem',
+    'SortDropdownToolbarItem', 'UpdateToolbarItem',
 ]
 
 TOOLBAR_PARAMS_KEYS = {
     'name', 'label', 'button_label','template_name', 'attrs', 'choices',
+    'theme_button_class',
 }
 
 class Toolbar(list):
     template_name = 'django_listing/toolbar.html'
 
     def __init__(self, *items, params=None, listing=None):
         if params is None:
@@ -100,14 +101,16 @@
 
 
 class ToolbarItem(metaclass=ToolbarItemMeta):
     name = None
     params_keys = ''
     attrs = {}
     listing = None
+    theme_button_class = 'btn btn-secondary'
+
     _ids = count(0)
 
     def __init__(self, *args, **kwargs):
         self.init_args = args
         self.init_kwargs = kwargs
         self.id = next(self._ids)
 
@@ -287,7 +290,12 @@
         ]
 
 
 class ExportDropdownToolbarItem(ExportSelectToolbarItem):
     template_name = 'django_listing/tbi_dropdown.html'
     label = _('Export to...')
     choices = EXPORT_FORMATS
+
+
+class UpdateToolbarItem(ToolbarItem):
+    template_name = 'django_listing/tbi_update.html'
+    label = _('Update')
```

### Comparing `django-listing-0.0.8/django_listing/exceptions.py` & `django-listing-0.0.9/django_listing/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/utils.py` & `django-listing-0.0.9/django_listing/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,9 +62,13 @@
     for k in sorted(qd.keys()):
         v = qd.getlist(k)
         if len(v) == 1:
             v = v[0]
         out += "'{k}' : {v}\n".format(k=k,v=repr(v))
     return out
 
+
+class JsonDirect(str):
+    pass
+
 #TODO : create functions to add sum/min/max/avg columns to a sequence
```

### Comparing `django-listing-0.0.8/django_listing/__init__.py` & `django-listing-0.0.9/django_listing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__='0.0.8'
+__version__='0.0.9'
 __author__ = "Eric Lapouyade"
 __copyright__ = "Copyright 2018, The Django listing Project"
 __credits__ = ["Eric Lapouyade"]
 __license__ = "Dual licensing"
 __maintainer__ = "Eric Lapouyade"
 __status__ = "Alpha"
```

### Comparing `django-listing-0.0.8/django_listing/listing_form.py` & `django-listing-0.0.9/django_listing/listing_form.py`

 * *Files 7% similar despite different names*

```diff
@@ -145,19 +145,19 @@
             self.attrs.add('id',f'{form_css_class}{self.listing.suffix}')
         self.id = self.attrs['id']
         buttons = self.buttons
         if isinstance(buttons,str):
             self.buttons = list(map(str.strip,buttons.split(',')))
 
     def datetimepicker_init(self):
-        self.listing.add_onready_snippet("\n"
-            "$('#{form.id} .edit-datecolumn').datetimepicker({{timepicker:false, format:'{listing.datetimepicker_date_format}'}});\n"
-            "$('#{form.id} .edit-datetimecolumn').datetimepicker({{format:'{listing.datetimepicker_datetime_format}'}});\n"
-            "$('#{form.id} .edit-timecolumn').datetimepicker({{datepicker:false, format:'{listing.datetimepicker_time_format}'}});\n"
-            .format(form=self, listing=self.listing))
+        self.listing.need_media_for('datetimepicker')
+        self.listing.add_footer_dict_list('datetimepickers', dict(
+            listing=self.listing,
+            div_id=self.id
+        ))
 
     def create_form_from_layout(self):
         fields = {}
         if not self.layout:
             raise InvalidListingForm(_('You must specify a list of columns '
                                        'names in the form layout'))
         for row in self.layout:
```

### Comparing `django-listing-0.0.8/django_listing/listing.py` & `django-listing-0.0.9/django_listing/listing.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 from django.template import loader
 from django.db.models import Model
 from django.db.models.query import QuerySet
 from django.conf import settings
 from django import forms
 from django.core.exceptions import ValidationError
 from django.forms.fields import FileField
+from django.middleware.csrf import get_token as get_csrf_token
 from urllib.parse import urlsplit, urlunsplit
+
+from .app_settings import app_settings
 from .exceptions import *
 from .record import RecordManager
 from .html_attributes import HTMLAttributes
 from .context import RenderContext
 from .paginators import Paginator, PAGINATOR_PARAMS_KEYS
 from .columns import ( ModelColumns, SequenceColumns, COLUMNS_PARAMS_KEYS,
                        SelectionColumn, )
@@ -77,15 +80,22 @@
     'editing_hidden_columns', 'row_form_base_class', 'datetimepicker_date_format',
     'datetimepicker_datetime_format', 'datetimepicker_time_format',
     'save_to_database', 'primary_key', 'selectable', 'selecting',
     'selection_multiple', 'selection_position', 'selection_key',
     'row_attrs', 'theme_div_row_container_class', 'selection_mode',
     'selection_overlay_template_name', 'selection_menu_id',
     'onready_snippet','footer_snippet', 'selection_initial', 'form',
-    'link_object_columns', 'anchor_hash', 'theme_spinner_icon'
+    'link_object_columns', 'anchor_hash', 'theme_spinner_icon', 'has_upload',
+    'theme_action_button_class',
+    'theme_action_button_cancel_icon', 'theme_action_button_edit_icon',
+    'theme_action_button_update_icon', 'theme_action_button_upload_icon',
+    'action_button_cancel_label', 'action_button_edit_label',
+    'action_button_update_label', 'action_button_upload_label',
+    'action_footer_template_name', 'action_header_template_name',
+    'has_footer_action_buttons', 'edit_on_demand',
 }
 
 LISTING_VARIATIONS_KEYS = LISTING_PARAMS_KEYS | {'get_url'}
 LISTING_FORMSET_PREFIX = 'listing'
 
 
 class ListingBase:
@@ -276,49 +286,58 @@
             return getattr(self.listing, item)
         return super().__getattribute__(item)
 
 
 class Listing(ListingBase):
     accept_ajax = False
     action = None
+    action_button_cancel_label = pgettext_lazy('action button','Cancel')
+    action_button_edit_label = pgettext_lazy('action button','Edit')
+    action_button_update_label = pgettext_lazy('action button','Update')
+    action_button_upload_label = pgettext_lazy('action button','Upload')
     action_col = None
+    action_footer_template_name = 'django_listing/action_footer.html'
+    action_header_template_name = 'django_listing/action_header.html'
     ajax_part = None
     allow_empty_first_page = True
     anchor_hash = None
     attrs = {'class':'table table-hover table-bordered table-striped table-sm'}
     can_edit = False
     can_select = False
     columns = None
     columns_headers = None
     data = None
     datetimepicker_date_format = 'Y-m-d'
     datetimepicker_datetime_format = 'Y-m-d H:i'
     datetimepicker_time_format = 'H:i'
     div_template_name = 'django_listing/div_row.html'
     row_attrs = {'class':'row-container'}
+    edit_on_demand = False
     editable = False
     editable_columns = set()
     editing = None
     editing_columns = None
     editing_row_pk = None
     editing_hidden_columns = None
-    empty_table_msg = gettext_lazy('<i>Nothing to display</i>')
+    empty_table_msg = gettext_lazy('Nothing to display')
     empty_listing_template_name = 'django_listing/empty_listing.html'
     exclude_columns = None
     export = None
     filters = None
     footer_snippet = None
     footer_template_name = None
     form = None
     has_footer = False
+    has_footer_action_buttons = True
     has_form = False
     has_header = True
     has_hidden_selection = False
     has_paginator = True
     has_toolbar = False
+    has_upload = False
     id = None
     link_object_columns = None
     row_form_base_class = ListingBaseForm
     listing_form_base_class = ListingBaseForm
     listing_template_name = 'django_listing/listing.html'
     model = None
     name = 'listing'
@@ -358,22 +377,28 @@
     unsortable = True
     variation = None
     variations = None
 
     params_keys = set()  # keep it here in the class not in __init__()
 
     theme_listing_class = 'django-listing'
+    theme_action_button_class = 'btn btn-primary'
+    theme_action_button_cancel_icon = ''
+    theme_action_button_edit_icon = ''
+    theme_action_button_update_icon = ''
+    theme_action_button_upload_icon = ''
     theme_container_class = 'django-listing-container'
     theme_sort_asc_icon = 'listing-icon-angle-up'
     theme_sort_desc_icon = 'listing-icon-angle-down'
     theme_sort_none_icon = ''
     theme_spinner_icon = 'animate-spin listing-icon-spin2'
     theme_sortable_class = 'sortable'
     theme_sort_asc_class = 'asc'
     theme_sort_desc_class = 'desc'
+    theme_button_class = 'btn btn-primary'
     theme_button_disabled_class = 'disabled'
     theme_button_active_class = 'active'
     theme_div_row_container_class = ''
 
     def __init__(self, data=None, **kwargs):
         super().__init__(data,**kwargs)
         self.request = None
@@ -388,19 +413,20 @@
         self.col_cell_renderers = {}
         init_dicts_from_class(self,['global_context','attrs','row_attrs'])
         self._initialized = False
         self._render_initialized = False
         self._formset = None
         self._view = None
         self.form_params = {}
+        self._have_to_refresh = False
 
         # listing initialisation must be in 2 steps because when a class is
         # passed to a template, it is automatically instanciated by Django
         # without any parameter.
-        if isinstance(data, QuerySet) or data:
+        if isinstance(data, QuerySet) or data is not None:
             self.init(data, **kwargs)
 
     @classmethod
     def get_params_keys(cls):
         if not Listing.params_keys:
             Listing.params_keys = set(LISTING_PARAMS_KEYS)
             Listing.params_keys.update(
@@ -419,23 +445,48 @@
         self.store_kwargs(**kwargs)
         params_keys = self.get_params_keys()
         for k, v in self.stored_params.items():
             if k in params_keys or ('__' in k and not k.startswith('__')):
                 setattr(self,k,v)
         self.stored_params = {}
 
+    def have_to_refresh(self):
+        return self._have_to_refresh
+
+    def plan_refresh(self):
+        self._have_to_refresh = True
+
     def add_onready_snippet(self, snippet):
         if not hasattr(self.request,'django_listing_onready_snippets'):
             self.request.django_listing_onready_snippets = []
-        self.request.django_listing_onready_snippets.append(snippet)
+        if snippet not in self.request.django_listing_onready_snippets:
+            self.request.django_listing_onready_snippets.append(snippet)
+
+    def add_header_snippet(self, snippet):
+        if not hasattr(self.request,'django_listing_header_snippets'):
+            self.request.django_listing_header_snippets = []
+        if snippet not in self.request.django_listing_header_snippets:
+            self.request.django_listing_header_snippets.append(snippet)
+
+    def add_footer_dict_list(self, key, dct):
+        if not hasattr(self.request,'django_listing_footer_dict_list'):
+            self.request.django_listing_footer_dict_list = {}
+        dict_list = self.request.django_listing_footer_dict_list.setdefault(key, [])
+        dict_list.append(dct)
 
     def add_footer_snippet(self, snippet):
         if not hasattr(self.request,'django_listing_footer_snippets'):
             self.request.django_listing_footer_snippets = []
-        self.request.django_listing_footer_snippets.append(snippet)
+        if snippet not in self.request.django_listing_footer_snippets:
+            self.request.django_listing_footer_snippets.append(snippet)
+
+    def need_media_for(self, feature_name):
+        if not hasattr(self.request, 'need_media_for'):
+            self.request.need_media_for = {}
+        self.request.need_media_for[feature_name] = True
 
     def create_missing_columns(self):
         if self.columns is None:
             if isinstance(self.columns_headers,str):
                 self.columns_headers = self.columns_headers.split(',')
             if self.model:
                 self.columns = ModelColumns(
@@ -479,14 +530,17 @@
     def get_model(self):
         if self.model:
             return self.model
         if self.columns:
             return self.columns.get_model()
         return None
 
+    def is_empty(self):
+        return not bool(self.data)
+
     def is_initialized(self):
         return self._initialized
 
     def is_render_initialized(self):
         return self._render_initialized
 
     def manage_page_context(self, context):
@@ -535,26 +589,34 @@
                 self.toolbar = self.toolbar.bind_to_listing(self)
             self.col_cell_renderers = {
                 col : getattr(self, 'render_{}'.format(col.name), col.render_cell)
                 for col in self.columns }
             self._initialized = True
 
     def datetimepicker_init(self):
-        if self.can_edit:
-            self.add_onready_snippet("\n"
-                "$('#{listing.id} .edit-datecolumn').datetimepicker({{timepicker:false, format:'{listing.datetimepicker_date_format}'}});\n"
-                "$('#{listing.id} .edit-datetimecolumn').datetimepicker({{format:'{listing.datetimepicker_datetime_format}'}});\n"
-                "$('#{listing.id} .edit-timecolumn').datetimepicker({{datepicker:false, format:'{listing.datetimepicker_time_format}'}});\n"
-                .format(listing=self))
+        self.need_media_for('datetimepicker')
+        self.add_footer_dict_list('datetimepickers', dict(
+            listing=self,
+            div_id=self.id
+        ))
+
+    def dropzone_init(self):
+        self.need_media_for('dropzone')
+        dz_suffix = self.suffix[1:] if isinstance(self.suffix, str) else ''
+        dz_camel_name = f'actionForm{dz_suffix}'
+        self.add_footer_dict_list('dropzones', dict(
+            listing=self,
+            dz_camel_name=dz_camel_name,
+            options=app_settings.DROPZONE_PARAMS,
+        ))
 
     def global_context_init(self):
-        self.global_context.update(
-            static_url=settings.STATIC_URL,
-            media_url=settings.MEDIA_URL,
-        )
+        self.global_context.update(app_settings.context)
+        if self.request and ( self.can_edit or self.has_upload ):
+            self.global_context['csrf_token'] = get_csrf_token(self.request)
 
     def render_init(self,context):
         if not self._render_initialized:
             self.manage_page_context(context)
             self.normalize_params()
             for col in self.columns:
                 col.render_init()
@@ -619,16 +681,19 @@
                                                         self.exclude_columns)
             self.can_edit_columns=[ c for c in self.selected_columns if c.can_edit ]
             self.can_edit_columns_names=set( c.name for c in self.can_edit_columns )
             self.editing_really_hidden_columns = \
                 self.editing_hidden_columns - self.can_edit_columns_names
             self.selected_hidden_columns = \
                 self.columns.select(self.editing_really_hidden_columns)
-            self.datetimepicker_init()
-            if self.can_edit or self.can_select or self.form:
+            if self.can_edit:
+                self.datetimepicker_init()
+            if self.has_upload:
+                self.dropzone_init()
+            if self.can_edit or self.can_select or self.form or self.has_upload:
                 self.add_form_input_hiddens(listing_id=self.id,
                                             listing_suffix=self.suffix)
             if self.onready_snippet:
                 self.add_onready_snippet(self.onready_snippet)
             if self.footer_snippet:
                 self.add_footer_snippet(self.footer_snippet)
             if not isinstance(self.selection_initial,list):
@@ -656,15 +721,32 @@
                 for row in self.exported_rows():
                     data.append(row)
                 self.request.export_data = data.export(export_format.lower())
                 self.request.export_filename = '{}.{}'.format(self.name,
                                                           self.export.lower())
         return hasattr(self.request,'export_data')
 
+    def django_listing_info(self):
+        if hasattr(self, 'request'):
+            if self.request.GET.get('__django_listing_info__'):
+                out = '<b><u>django-listing informations :</u></b><br>'
+                import django_listing
+                out += f'django-listing version : {django_listing.__version__}<br>'
+                import django
+                out += f'django version : {django.__version__}<br>'
+                import tablib
+                out += f'tablib version : {tablib.__version__}<br>'
+                import sys
+                out += f'Python version : {sys.version.split()[0]}<br>'
+                return out
+
     def render_template(self):
+        request_for_info = self.django_listing_info()
+        if request_for_info:
+            return request_for_info
         ctx = self.get_listing_context()
         template = loader.get_template(self.listing_template_name)
         out = template.render(ctx)
         return out
 
     def get_listing_context(self):
         has_top_toolbar = ( self.has_toolbar and
@@ -681,14 +763,16 @@
             listing_container_class += ' django-listing-selecting'
             if self.selection_multiple:
                 listing_container_class += ' selection_multiple'
             else:
                 listing_container_class += ' selection_unique'
             listing_container_class += \
                 ' selection_position_{}'.format(self.selection_position)
+        if self.has_upload:
+            listing_container_class += ' has_upload'
         sel_css_class = ( LISTING_SELECTOR_CSS_CLASS
                           if self.selection_has_overlay else '' )
         hover_css_class = ( LISTING_SELECTION_HOVER_CSS_CLASS
                           if self.selection_mode == 'hover' else '' )
         ctx = RenderContext(
             self.global_context,
             self.page_context.flatten(),
```

### Comparing `django-listing-0.0.8/django_listing/templates/django_listing/tbi_variations.html` & `django-listing-0.0.9/django_listing/templates/django_listing/tbi_variations.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/templates/django_listing/tbi_dropdown.html` & `django-listing-0.0.9/django_listing/templates/django_listing/tbi_dropdown.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/templates/django_listing/listing_div.html` & `django-listing-0.0.9/django_listing/templates/django_listing/listing_div.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/templates/django_listing/tbi_select.html` & `django-listing-0.0.9/django_listing/templates/django_listing/tbi_select.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/templates/django_listing/view_object_popup.html` & `django-listing-0.0.9/django_listing/templates/django_listing/view_object_popup.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/templates/django_listing/listing.html` & `django-listing-0.0.9/django_listing/templates/django_listing/listing.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+{% load django_listing %}
 {% autoescape off %}
-    <div id="{{ listing.id }}"
+    <div id="{{ listing.id|underscore_to_dash }}"
          listing-suffix="{{ listing.suffix }}"
          class="{{ listing_container_class }}"
          ajax_url="{{ listing.get_url }}"
          {% if listing.selection_menu_id %}selection-menu-id="{{ listing.selection_menu_id }}"{% endif %}
     >
     <div class="listing-spinner"><span class="{{ listing.theme_spinner_icon }}"></span></div>
 
@@ -17,14 +18,19 @@
         {% if listing.paginator.count or not listing.empty_listing_template_name %}
             {% if has_top_toolbar %}
                 <div class="top-toolbar">
                     {% include listing.toolbar.template_name %}
                 </div>
             {% endif %}
 
+            {% if listing.can_edit or listing.has_upload or listing.edit_on_demand %}
+                {% if listing.action_header_template_name %}
+                    {% include listing.action_header_template_name %}
+                {% endif %}
+            {% endif %}
             {% block listing %}
                 <table{{ listing.attrs }}>
                     {% block listing_header %}
                         {% if listing.has_header %}
                             <thead>
                             <tr>
                                 {% for col in listing.header_columns %}{{ col.html }}
@@ -83,21 +89,43 @@
                 {% if listing.editable and listing.editing %}
                     {% for hidden_field in listing.editing_hidden_form_fields %}
                         {{ hidden_field }}{% endfor %}
                     {{ listing.get_formset.management_form }}
                 {% endif %}
             {% endblock %}
 
+            {% if listing.can_edit or listing.has_upload or listing.edit_on_demand %}
+                </form>
+            {% endif %}
+
             {% if has_bottom_toolbar %}
                 <div class="bottom-toolbar">
                     {% include listing.toolbar.template_name %}
                 </div>
             {% endif %}
 
             {% if listing.has_paginator and not listing.paginator.in_footer %}
                 {% include listing.paginator.template_name %}
             {% endif %}
+
+            {% if listing.can_edit or listing.has_upload or listing.edit_on_demand %}
+                {% if listing.action_footer_template_name %}
+                    {% include listing.action_footer_template_name %}
+                {% endif %}
+            {% endif %}
         {% else %}
+            {% if listing.can_edit or listing.has_upload or listing.edit_on_demand %}
+                {% if listing.action_header_template_name %}
+                    {% include listing.action_header_template_name %}
+                {% endif %}
+            {% endif %}
             {% include listing.empty_listing_template_name %}
+            {% if listing.can_edit or listing.has_upload or listing.edit_on_demand %}
+                {% if listing.action_footer_template_name %}
+                    {% include listing.action_footer_template_name %}
+                {% endif %}
+            {% endif %}
+            </form>
         {% endif %}
+
     </div>
 {% endautoescape %}
```

### Comparing `django-listing-0.0.8/django_listing/templates/django_listing/actions_buttons.html` & `django-listing-0.0.9/django_listing/templates/django_listing/actions_buttons.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+{% load django_listing %}
 {% block actions_buttons %}{% spaceless %}
 <form method="post">
 <input type="hidden" name="csrfmiddlewaretoken" value="{{ csrf_token }}">
+<input type="hidden" name="listing_id" value="{{ listing.id|underscore_to_dash }}">
 <input type="hidden" name="action" value="action_button">
 <input type="hidden" name="action_pk" value="{{ rec.pk }}">
 <input type="hidden" name="action_col" value="{{ action_col }}">
     <ul class="actions-buttons">
         {% for button in buttons %}
             <li class="{{ button.theme_li_class }} {{ button.name_css_class }}{% if button.disabled %} disabled{% endif %}">
                 {% if button.type == "link" %}
```

### Comparing `django-listing-0.0.8/django_listing/templates/django_listing/paginator.html` & `django-listing-0.0.9/django_listing/templates/django_listing/paginator.html`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                                 <li class="listing-nav {{ paginator.theme_button_li_class }} first{% if not current_page.has_previous %} {{ listing.theme_button_disabled_class }}{% endif %}">
                                     <a class="listing-nav {{ paginator.theme_button_a_class }}"
                                        role="button"
                                        href="{{ first_page_url }}">
                                         {% if paginator.theme_first_last_has_icon %}
                                             <span class="{{ paginator.theme_first_icon }}"></span>{% endif %}
                                         {% if paginator.theme_first_last_has_text %}
-                                            {{ paginator.first_text }}{% endif %}
+                                            <span class="{{ paginator.theme_button_text_class }}">{{ paginator.first_text }}</span>{% endif %}
                                     </a>
                                 </li>
                             {% endblock pagination_first %}
                         {% endif %}
                     {% endif %}
                 {% elif part == 'fastprev' %}
                     {# ------------------------------- Fast previous button ---------------------------------- #}
@@ -32,15 +32,15 @@
                                 <li class="listing-nav {{ paginator.theme_button_li_class }} fast_page_prev{% if not current_page.has_previous %} {{ listing.theme_button_disabled_class }}{% endif %}">
                                     <a class="listing-nav {{ paginator.theme_button_a_class }}"
                                        role="button"
                                        href="{{ fast_page_prev_url }}">
                                         {% if paginator.theme_fast_page_has_icon %}
                                             <span class="{{ paginator.theme_fast_prev_icon }}"></span>{% endif %}
                                         {% if paginator.theme_fast_page_has_text %}
-                                            {{ fast_page_prev_text }}{% endif %}
+                                            <span class="{{ paginator.theme_button_text_class }}">{{ fast_page_prev_text }}</span>{% endif %}
                                     </a>
                                 </li>
                             {% endblock fast_page_prev %}
                         {% endif %}
                     {% endif %}
 
                 {% elif part == 'prev' %}
@@ -51,15 +51,15 @@
                                 <li class="listing-nav {{ paginator.theme_button_li_class }} previous{% if not current_page.has_previous %} {{ listing.theme_button_disabled_class }}{% endif %}">
                                     <a class="listing-nav {{ paginator.theme_button_a_class }}"
                                        role="button"
                                        href="{{ prev_page_url }}">
                                         {% if paginator.theme_prev_next_has_icon %}
                                             <span class="{{ paginator.theme_prev_icon }}"></span>{% endif %}
                                         {% if paginator.theme_prev_next_has_text %}
-                                            {{ paginator.prev_text }}{% endif %}
+                                            <span class="{{ paginator.theme_button_text_class }}">{{ paginator.prev_text }}</span>{% endif %}
                                     </a>
                                 </li>
                             {% endblock pagination_previous %}
                         {% endif %}
                     {% endif %}
 
                 {% elif part == 'pageinfo' %}
@@ -130,15 +130,15 @@
                         {% if current_page.has_next or not paginator.hide_disabled_buttons %}
                             {% block pagination_next %}
                                 <li class="listing-nav {{ paginator.theme_button_li_class }} next{% if not current_page.has_next %} {{ listing.theme_button_disabled_class }}{% endif %}">
                                     <a class="listing-nav {{ paginator.theme_button_a_class }}"
                                        role="button"
                                        href="{{ next_page_url }}">
                                         {% if paginator.theme_prev_next_has_text %}
-                                            {{ paginator.next_text }}{% endif %}
+                                            <span class="{{ paginator.theme_button_text_class }}">{{ paginator.next_text }}</span>{% endif %}
                                         {% if paginator.theme_prev_next_has_icon %}
                                             <span class="{{ paginator.theme_next_icon }}"></span>{% endif %}
                                     </a>
                                 </li>
                             {% endblock pagination_next %}
                         {% endif %}
                     {% endif %}
@@ -149,15 +149,15 @@
                         {% if current_page.has_next or not paginator.hide_disabled_buttons %}
                             {% block fast_page_next %}
                                 <li class="listing-nav {{ paginator.theme_button_li_class }} fast_page_next{% if not current_page.has_next %} {{ listing.theme_button_disabled_class }}{% endif %}">
                                     <a class="listing-nav {{ paginator.theme_button_a_class }}"
                                        role="button"
                                        href="{{ fast_page_next_url }}">
                                         {% if paginator.theme_fast_page_has_text %}
-                                            {{ fast_page_next_text }}{% endif %}
+                                            <span class="{{ paginator.theme_button_text_class }}">{{ fast_page_next_text }}</span>{% endif %}
                                         {% if paginator.theme_fast_page_has_icon %}
                                             <span class="{{ paginator.theme_fast_next_icon }}"></span>{% endif %}
                                     </a>
                                 </li>
                             {% endblock fast_page_next %}
                         {% endif %}
                     {% endif %}
@@ -168,15 +168,15 @@
                         {% if current_page.has_next or not paginator.hide_disabled_buttons %}
                             {% block pagination_last %}
                                 <li class="listing-nav {{ paginator.theme_button_li_class }} last{% if not current_page.has_next %} {{ listing.theme_button_disabled_class }}{% endif %}">
                                     <a class="listing-nav {{ paginator.theme_button_a_class }}"
                                        role="button"
                                        href="{{ last_page_url }}">
                                         {% if paginator.theme_first_last_has_text %}
-                                            {{ paginator.last_text }}{% endif %}
+                                            <span class="{{ paginator.theme_button_text_class }}">{{ paginator.last_text }}</span>{% endif %}
                                         {% if paginator.theme_first_last_has_icon %}
                                             <span class="{{ paginator.theme_last_icon }}"></span>{% endif %}
                                     </a>
                                 </li>
                             {% endblock pagination_last %}
                         {% endif %}
                     {% endif %}
```

### Comparing `django-listing-0.0.8/django_listing/templates/django_listing/filters_form.html` & `django-listing-0.0.9/django_listing/templates/django_listing/filters_form.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/templates/django_listing/listing_form.html` & `django-listing-0.0.9/django_listing/templates/django_listing/listing_form.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/html_attributes.py` & `django-listing-0.0.9/django_listing/html_attributes.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/aggregations.py` & `django-listing-0.0.9/django_listing/aggregations.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/actions_buttons_column.py` & `django-listing-0.0.9/django_listing/actions_buttons_column.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.buttons_description = {}
 
     def init(self, *args, **kwargs):
         super().init(*args, **kwargs)
-        if not isinstance(self.listing.data, QuerySet):
-            raise InvalidData('Actions buttons work only with QuerySet as listing data.')
+        # if not isinstance(self.listing.data, QuerySet):
+        #     raise InvalidData('Actions buttons work only with QuerySet as listing data.')
 
     def render_init(self):
         self.extract_action_params()
 
     def set_kwargs(self, **kwargs):
         super().set_kwargs(**kwargs)
         buttons = self.buttons
@@ -72,52 +72,55 @@
                     description[s] = getattr(self,f'buttons_{s}')
             description['name'] = b
             self.buttons_description[b] = description
 
     def extract_action_params(self):
         get_dict = self.listing.request.GET
         post_dict = self.listing.request.POST
-        for k in self.actions_query_string_keys:
-            qs_key = k + self.listing.suffix
+        for qs_key in self.actions_query_string_keys:
             v = None
             if qs_key in post_dict:
                 v = post_dict.get(qs_key)
             elif qs_key in get_dict:
                 v = get_dict.get(qs_key)
-            if v is not None and k in self.actions_query_string_int_keys:
+            if v is not None and qs_key in self.actions_query_string_int_keys:
                 try:
                     v = int(v)
                 except ValueError:
                     pass
-            setattr(self, k, v)
+            setattr(self, qs_key, v)
 
     def get_buttons_template(self, rec):
         if not hasattr(self,'_value_template'):
             self._value_template = loader.get_template(self.buttons_template)
         return self._value_template
 
     def get_buttons_context(self, rec):
         buttons = self.buttons
         if isinstance(buttons,str):
             buttons = map(str.strip,buttons.split(','))
         buttons_context = []
         for b in buttons:
-            try:
-                meth_name = f'get_button_{b}_context'
-                context_method = getattr(self, meth_name)
-            except AttributeError:
-                self.get_button_context(b,rec)
-            context = context_method(b, rec)
+            meth_name = f'get_button_{b}_context'
+            context = {}
+            context_method = getattr(self.listing, meth_name, None)
+            if context_method is not None:
+                context = context_method(self, b, rec)  # give col objet to listing method
+            else:
+                context_method = getattr(self, meth_name, None)
+                if context_method is not None:
+                    context = context_method(b, rec)
             context.update(
                 self.buttons_description[b],
                 name=b,
                 name_css_class=b.replace('_','-'),
             )
             buttons_context.append(context)
         return dict(
+            listing=self.listing,
             buttons=buttons_context,
             rec=rec,
             action_col=self.name,
             csrf_token=get_csrf_token(self.listing.request),
         )
 
     def get_cell_value(self,rec):
@@ -128,18 +131,22 @@
     def get_button_context(self, name, rec):
         return dict(
             name=name,
             type='submit',
         )
 
     def manage_button_action(self, *args, **kwargs):
-        try:
-            meth_name = f'manage_button_{self.action_button}_action'
-            action_method = getattr(self, meth_name)
-        except AttributeError as e:
+        meth_name = f'manage_button_{self.action_button}_action'
+        # Search method in listing object first
+        action_method = getattr(self.listing, meth_name, None)
+        if action_method is not None:
+            return action_method(self, *args, **kwargs)  # give col objet to listing method
+        # Search method in column object otherwise
+        action_method = getattr(self, meth_name, None)
+        if action_method is None:
             raise ListingException(f'Unknown "{self.action_button}" action.')
         return action_method(*args, **kwargs)
 
     #---------------- MOVE UP --------------------------------------------------
     move_up__icon = 'listing-icon-up-open'
     move_up__text = _('Move up')
     move_up__title = _('Change order up')
```

### Comparing `django-listing-0.0.8/django_listing/locale/en/LC_MESSAGES/django.po` & `django-listing-0.0.9/django_listing/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/locale/fr/LC_MESSAGES/django.po` & `django-listing-0.0.9/django_listing/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/js/django_listing.js` & `django-listing-0.0.9/django_listing/static/django_listing/js/django_listing.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -6,23 +6,49 @@
     if (url.search(pattern) >= 0) {
         return url.replace(pattern, '$1' + param_value + '$2');
     }
     url = url.replace(/\?$/, '');
     return url + (url.indexOf('?') > 0 ? '&' : '?') + param_name + '=' + param_value;
 }
 
+function get_csrf_token() {
+    name = 'csrftoken';
+    let cookieValue = null;
+    if (document.cookie && document.cookie !== '') {
+        const cookies = document.cookie.split(';');
+        for (let i = 0; i < cookies.length; i++) {
+            const cookie = cookies[i].trim();
+            // Does this cookie string begin with the name we want?
+            if (cookie.substring(0, name.length + 1) === (name + '=')) {
+                cookieValue = decodeURIComponent(cookie.substring(name.length + 1));
+                break;
+            }
+        }
+    }
+    return cookieValue
+}
+
+function update_csrf_token() {
+    $.ajaxSetup({
+        data: {
+            'csrfmiddlewaretoken': get_csrf_token()
+        }
+    });
+}
+
 function djlst_load_listing_url(nav_obj, url) {
     var listing_div = nav_obj.closest("div.django-listing-ajax");
     listing_div.addClass("spinning");
     var listing_id = $(listing_div).attr("id");
     var listing_suffix = $(listing_div).attr("listing-suffix");
     var listing_target = nav_obj.attr("listing-target");
     if (!listing_target) listing_target = "#" + listing_id;
     var listing_part = nav_obj.attr("listing-part");
     if (!listing_part) listing_part = "all";
+    update_csrf_token();
     $(listing_target).load(
         url, {
             "listing_id": listing_id,
             "listing_suffix": listing_suffix,
             "listing_part": listing_part
         },
         function(responseText, textStatus, req) {
@@ -39,15 +65,14 @@
 
 function djlst_load_listing_href() {
     return djlst_load_listing_url($(this), $(this).attr("href"));
 }
 
 function djlst_load_listing_val() {
     var param_value = $(this).val();
-    console.log("Value = " + param_value);
     var param_name = $(this).attr("name");
     var ajax_url = $(this).closest("div.django-listing-ajax").attr("ajax_url");
     var url = djlst_replaceUrlParam(ajax_url, param_name, param_value);
     return djlst_load_listing_url($(this), url);
 }
 
 function djlst_post_button_action(event) {
@@ -65,14 +90,15 @@
     request_data = {
         listing_id: listing_id,
         listing_suffix: listing_suffix,
         listing_part: listing_part,
         serialized_data: nav_obj.closest('form').serialize()
     };
     request_data[$(this).attr('name')] = $(this).val();
+    update_csrf_token();
     $.ajax({
         type: "POST",
         url: ajax_url,
         data: request_data,
         success: function(response) {
             $(listing_target).html(response);
             $(listing_target).children(":first").unwrap();
@@ -200,14 +226,15 @@
     var listing_suffix = listing_div.attr("listing-suffix");
     request_data = {
         listing_id: listing_id,
         listing_suffix: listing_suffix,
         action_button: 'view_object_popup',
         serialized_data: nav_obj.closest('form').serialize()
     };
+    update_csrf_token();
     $.ajax({
         type: "POST",
         url: ajax_url,
         data: request_data,
         success: function(response) {
             listing_div.removeClass("spinning");
             $("#listing-popup-container").html(response);
@@ -232,8 +259,35 @@
     $(document.body).on("click", "div.django-listing-selecting .selection-overlay.hover", djlst_activate_selection);
     $(document.body).on("click", "[listing-action='select-all']", djlst_select_all);
     $(document.body).on("click", "[listing-action='unselect-all']", djlst_unselect_all);
     $(document.body).on("click", ".listing-selection-menu .listing-menu-close", djlst_deactivate_selection);
     $(document.body).on("click", "li.action-item.view-object-popup a", djlst_view_object_popup);
 
     $('[data-toggle="popover"]').popover();
+
+    var dropzoneCounter = 0;
+
+    $('.dropzone').on('dragenter', function() {
+        dropzoneCounter++;
+        $(this).addClass('drag-over');
+    });
+
+    $('.dropzone').bind('dragleave', function() {
+        dropzoneCounter--;
+        if (dropzoneCounter === 0) {
+            $(this).removeClass('drag-over');
+        }
+    });
+
+    $('.dropzone').bind('drop', function() {
+        dropzoneCounter = 0;
+        $(this).removeClass('drag-over');
+    });
+
+    $('.submit-action-form').on('click', function() {
+        var action = $(this).val();
+        var form = $(this).closest('.django-listing-container').find('.action-form');
+        var hidden = form.find('.action-hidden-value');
+        hidden.val(action);
+        form.submit();
+    });
 });
```

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/css/django_listing-ie7.css` & `django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-ie7.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/css/django_listing-ie7-codes.css` & `django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-ie7-codes.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/css/animation.css` & `django-listing-0.0.9/django_listing/static/django_listing/css/animation.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/css/django_listing-codes.css` & `django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-codes.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/css/django_listing.css` & `django-listing-0.0.9/django_listing/static/django_listing/css/django_listing.css`

 * *Files 1% similar despite different names*

```diff
@@ -511,14 +511,15 @@
 }
 
 
 div.django-listing-container.standard-theme td.cls-totalcolumn {
     font-weight: bold;
 }
 
+div.django-listing-container td.type-str.cls-filesizecolumn,
 div.django-listing-container td.type-int,
 div.django-listing-container td.type-float,
 div.django-listing-container td.agg-minmax,
 div.django-listing-container td.agg-minmaxavg {
     text-align: right;
 }
 
@@ -547,23 +548,28 @@
 
 form.listing-form div.form-field {
     width: 100%;
     margin: 5px;
 }
 
 div.django-listing-container div.form-field.errors,
+div.django-listing-container ul.listing-row-form-errors,
 form.listing-form div.form-field.errors {
     background-color: rgba(255,0,0,.25);
     padding:10px;
     border: 1px solid red;
     border-radius: 6px;
     color: red;
     font-weight: bold;
 }
 
+div.django-listing-container ul.listing-row-form-errors li {
+    list-style: none;
+}
+
 div.django-listing-container div.form-field.errors ul.errorlist,
 form.listing-form div.form-field.errors ul.errorlist {
     list-style: none;
     padding: 0;
     display: inline;
 }
 
@@ -885,8 +891,81 @@
     font-weight: bold;
     font-size: 125%;
     text-decoration: underline;
 }
 
 table.object-popup th {
     vertical-align: top;
+}
+
+.empty-listing-upload-button {
+    text-align: center;
+}
+
+.empty-listing-upload-drop-here {
+    text-align: center;
+    margin: 16px;
+    color: #8d8d8d;
+}
+
+empty-listing-upload-accepted-files {
+    text-align: center;
+    margin: 16px;
+    font-style: italic;
+}
+
+form.dropzone .dz-preview.dz-image-preview {
+    background: none;
+}
+
+form.dropzone {
+    min-height: 150px;
+    border: none;
+    background: none;
+    padding: initial;
+    position: relative;
+}
+
+form.dropzone .dz-preview .dz-image {
+    border-radius: 8px;
+}
+
+form.dropzone .drag-overlay {
+    background: #8888FFA0;
+    border: 3px dashed #4444FF;
+    width: 100%;
+    height: 100%;
+    position: absolute;
+    top: 0;
+    left: 0;
+    display: none;
+    z-index: 10;
+    border-radius: 1rem;
+}
+
+form.dropzone.drag-over .drag-overlay {
+    display: flex;
+}
+
+form.dropzone .drag-overlay .overlay-inner {
+    margin: auto;
+    font-size: 6rem;
+    color: #FFFFFF;
+}
+
+form.dropzone.dz-drag-hover {
+    border: none;
+}
+
+.dz-success-mark svg path {
+    fill: #28a745;
+    fill-opacity: 1;
+    stroke: #444444;
+    stroke-opacity: 1;
+}
+
+.dz-error-mark svg g g {
+    fill: red;
+    fill-opacity: 1;
+    stroke: #444444;
+    stroke-opacity: 1;
 }
```

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/css/django_listing-embedded.css` & `django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-embedded.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/icons/csv.svg` & `django-listing-0.0.9/django_listing/static/django_listing/icons/csv.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/icons/tsv.svg` & `django-listing-0.0.9/django_listing/static/django_listing/icons/tsv.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/icons/xlsx.svg` & `django-listing-0.0.9/django_listing/static/django_listing/icons/xlsx.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/icons/html.svg` & `django-listing-0.0.9/django_listing/static/django_listing/icons/html.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/icons/xls.svg` & `django-listing-0.0.9/django_listing/static/django_listing/icons/xls.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/icons/ods.svg` & `django-listing-0.0.9/django_listing/static/django_listing/icons/ods.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/icons/json.svg` & `django-listing-0.0.9/django_listing/static/django_listing/icons/json.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/icons/dbf.svg` & `django-listing-0.0.9/django_listing/static/django_listing/icons/dbf.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/icons/pdf.svg` & `django-listing-0.0.9/django_listing/static/django_listing/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/font/django_listing.svg` & `django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/font/django_listing.eot` & `django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.eot`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/font/django_listing.woff` & `django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.woff`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/font/django_listing.ttf` & `django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.ttf`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/static/django_listing/font/django_listing.woff2` & `django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.woff2`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing/paginators.py` & `django-listing-0.0.9/django_listing/paginators.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     'theme_first_last_has_text', 'theme_first_icon','theme_last_icon',
     'theme_fast_page_has_icon', 'theme_fast_page_has_text',
     'theme_fast_prev_icon', 'theme_fast_next_icon', 'theme_prev_next_has_icon',
     'theme_prev_next_has_text', 'theme_prev_icon', 'theme_next_icon',
     'has_row_info', 'page_row_tpl', 'parts_order', 'has_goto_page',
     'goto_page_tpl', 'has_editable_page_info', 'theme_button_a_class',
     'theme_button_li_class', 'in_footer', 'hide_single_page',
+    'theme_button_text_class',
 }
 
 class Paginator(DjangoPaginator):
     template_name = 'django_listing/paginator.html'
     has_page_info = True
     has_editable_page_info = False
     page_info_tpl = pgettext_lazy('paginator','Page {page_number} of {nb_pages}')
@@ -42,15 +43,15 @@
     fast_page_prev_tpl = '-{step}'
     fast_page_next_tpl = '+{step}'
     page_scale_size = 0
     page_scale_ellipsis = 0
     hide_disabled_buttons = False
     hide_single_page = False
     parts_order = ( 'first,fastprev,prev,pageinfo,rowinfo,scale,'
-                    'next,fastnext,last;gotopage' )
+                    'next,fastnext,last' )
     has_goto_page = False
     goto_page_tpl = pgettext_lazy('paginator','Go to page {goto_form}')
     in_footer = False
 
     theme_first_last_has_icon = True
     theme_first_last_has_text = True
     theme_first_icon = 'listing-icon-to-start-1'
@@ -61,14 +62,15 @@
     theme_fast_next_icon = 'listing-icon-fast-forward'
     theme_prev_next_has_icon = True
     theme_prev_next_has_text = True
     theme_prev_icon = 'listing-icon-left-dir'
     theme_next_icon = 'listing-icon-right-dir'
     theme_button_a_class = 'page-link'
     theme_button_li_class = 'page-item'
+    theme_button_text_class = 'button-text'
 
     def __init__(self, listing, object_list, per_page, orphans=0,
                  allow_empty_first_page=True):
         super().__init__(object_list, per_page, orphans,
                          allow_empty_first_page)
         self.listing = listing
         for k in PAGINATOR_PARAMS_KEYS:
```

### Comparing `django-listing-0.0.8/django_listing/templatetags/django_listing.py` & `django-listing-0.0.9/django_listing/templatetags/django_listing.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,81 @@
 '''
 Création : 12 janv. 2010
 
 @author: Eric Lapouyade
 '''
 from django import template
-from django.utils.safestring import mark_safe
+from django.conf import settings
+from django.utils.safestring import mark_safe, SafeString
 from ..listing import Listing, ListingVariations
 from ..listing_form import ListingForm
 from itertools import count
+from ..app_settings import app_settings
+from ..utils import JsonDirect
+import json
 
 register = template.Library()
 _uniq_counter = count(0)
 
 
+@register.filter(name='json_options')
+def json_options(dct):
+    out = '{\n'
+    options = []
+    for k,v in sorted(dct.items()):
+        if isinstance(v, SafeString):
+            options.append(f'{k}:{v}')
+        else:
+            options.append(f'{k}:{json.dumps(v, indent=4)}')
+    out += ',\n'.join(options)
+    out += '\n}'
+    return mark_safe(out)
+
+
+@register.filter()
+def underscore_to_dash(s):
+    return s.replace('_','-')
+
+
+class ListingHeaderNode(template.Node):
+    def __init__(self, nodelist):
+        self.nodelist = nodelist
+
+    def render(self, context):
+        remaining_output = self.nodelist.render(context)
+        tpl = template.loader.get_template(app_settings.HEADER_TEMPLATE)
+        request = context.request
+        context = context.flatten()
+        context.update(
+            app_settings.context,
+            need_media_for=getattr(context['request'], 'need_media_for',{})
+        )
+        tpl_output = tpl.render(context, request)
+        return f'{tpl_output}\n{remaining_output}'
+
+
+@register.tag(name="render_listing_header")
+def do_listing_header(parser, token):
+    nodelist = parser.parse()
+    return ListingHeaderNode(nodelist)
+
+
+@register.simple_tag(takes_context=True)
+def render_listing_footer(context):
+    tpl = template.loader.get_template(app_settings.FOOTER_TEMPLATE)
+    request = context.request
+    context = context.flatten()
+    context.update(
+        app_settings.context,
+        need_media_for=getattr(context['request'],'need_media_for',{})
+    )
+    tpl_output = tpl.render(context, request)
+    return tpl_output
+
+
 def initialize_listing(context, listing, data=None, *args, **kwargs):
     if isinstance(listing,str) or listing is None:
         return None
     if not isinstance(listing,(Listing,ListingVariations)):
         data = listing
         listing = Listing()
     # if there is data or a model is specified in columns (if exsiting)
@@ -227,7 +286,43 @@
             else:
                 listing.form.action = action
     if not listing.form:
         listing.form = ListingForm(action, name=name,
                                    layout=layout, *args, **kwargs)
     listing.form.bind_to_listing(listing)
     return mark_safe(listing.form.render(context))
+
+
+@register.simple_tag(takes_context=True)
+def get_dict_list(context, key):
+    request = context.request
+    if hasattr(request, 'django_listing_footer_dict_list'):
+        return request.django_listing_footer_dict_list.get(key, [])
+    return []
+
+
+@register.simple_tag(takes_context=True)
+def header_snippets(context):
+    request = context.request
+    snippets = getattr(request, 'django_listing_header_snippets', None)
+    if snippets:
+        return mark_safe('\n'.join(snippets))
+    return ''
+
+
+@register.simple_tag(takes_context=True)
+def footer_snippets(context):
+    request = context.request
+    snippets = getattr(request, 'django_listing_footer_snippets', None)
+    if snippets:
+        return mark_safe('\n'.join(snippets))
+    return ''
+
+
+@register.simple_tag(takes_context=True)
+def onready_snippets(context):
+    request = context.request
+    snippets = getattr(request, 'django_listing_onready_snippets', None)
+    if snippets:
+        return mark_safe('\n'.join(snippets))
+    return ''
+
```

### Comparing `django-listing-0.0.8/django_listing/context.py` & `django-listing-0.0.9/django_listing/context.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/README.rst` & `django-listing-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/setup.py` & `django-listing-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.8/django_listing.egg-info/SOURCES.txt` & `django-listing-0.0.9/django_listing.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 CHANGES.rst
+LICENSE.rst
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 django_listing/__init__.py
 django_listing/actions_buttons_column.py
 django_listing/aggregations.py
+django_listing/app_settings.py
 django_listing/apps.py
 django_listing/columns.py
 django_listing/context.py
 django_listing/exceptions.py
 django_listing/filters.py
 django_listing/html_attributes.py
 django_listing/listing.py
@@ -21,15 +23,17 @@
 django_listing/views.py
 django_listing.egg-info/PKG-INFO
 django_listing.egg-info/SOURCES.txt
 django_listing.egg-info/dependency_links.txt
 django_listing.egg-info/not-zip-safe
 django_listing.egg-info/requires.txt
 django_listing.egg-info/top_level.txt
+django_listing/locale/en/LC_MESSAGES/django.mo
 django_listing/locale/en/LC_MESSAGES/django.po
+django_listing/locale/fr/LC_MESSAGES/django.mo
 django_listing/locale/fr/LC_MESSAGES/django.po
 django_listing/static/django_listing/css/animation.css
 django_listing/static/django_listing/css/django_listing-codes.css
 django_listing/static/django_listing/css/django_listing-embedded.css
 django_listing/static/django_listing/css/django_listing-ie7-codes.css
 django_listing/static/django_listing/css/django_listing-ie7.css
 django_listing/static/django_listing/css/django_listing.css
@@ -44,25 +48,28 @@
 django_listing/static/django_listing/icons/json.svg
 django_listing/static/django_listing/icons/ods.svg
 django_listing/static/django_listing/icons/pdf.svg
 django_listing/static/django_listing/icons/tsv.svg
 django_listing/static/django_listing/icons/xls.svg
 django_listing/static/django_listing/icons/xlsx.svg
 django_listing/static/django_listing/js/django_listing.js
+django_listing/templates/django_listing/action_footer.html
+django_listing/templates/django_listing/action_header.html
 django_listing/templates/django_listing/actions_buttons.html
 django_listing/templates/django_listing/div_row.html
 django_listing/templates/django_listing/empty_listing.html
 django_listing/templates/django_listing/filters_form.html
 django_listing/templates/django_listing/footer.html
 django_listing/templates/django_listing/header.html
 django_listing/templates/django_listing/listing.html
 django_listing/templates/django_listing/listing_div.html
 django_listing/templates/django_listing/listing_form.html
 django_listing/templates/django_listing/paginator.html
 django_listing/templates/django_listing/selection_overlay.html
 django_listing/templates/django_listing/tbi_dropdown.html
 django_listing/templates/django_listing/tbi_select.html
+django_listing/templates/django_listing/tbi_update.html
 django_listing/templates/django_listing/tbi_variations.html
 django_listing/templates/django_listing/toolbar.html
 django_listing/templates/django_listing/view_object_popup.html
 django_listing/templatetags/__init__.py
 django_listing/templatetags/django_listing.py
```

### Comparing `django-listing-0.0.8/django_listing.egg-info/PKG-INFO` & `django-listing-0.0.9/django_listing.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-listing
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for creating HTML listing / table / data grid
 Home-page: https://github.com/elapouya/django-listing
 Author: Eric Lapouyade
 Author-email: elapouya@gmail.com
 License: GPLv3+
 Description: 
         ==============
@@ -84,14 +84,18 @@
         -------------
         
         Please, `read the doc <http://django-listing.readthedocs.org>`_  (Work in progress)
         
         News
         ----
         
+        0.0.9 (2021-11-09)
+        ------------------
+        - Add possibility to create custom action button linked with listing method
+        
         0.0.7 (2020-07-14)
         ------------------
         - First running version
         
         0.0.1 (2018-02-03)
         ------------------
         - Skeleton commit
```

### Comparing `django-listing-0.0.8/PKG-INFO` & `django-listing-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-listing
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for creating HTML listing / table / data grid
 Home-page: https://github.com/elapouya/django-listing
 Author: Eric Lapouyade
 Author-email: elapouya@gmail.com
 License: GPLv3+
 Description: 
         ==============
@@ -84,14 +84,18 @@
         -------------
         
         Please, `read the doc <http://django-listing.readthedocs.org>`_  (Work in progress)
         
         News
         ----
         
+        0.0.9 (2021-11-09)
+        ------------------
+        - Add possibility to create custom action button linked with listing method
+        
         0.0.7 (2020-07-14)
         ------------------
         - First running version
         
         0.0.1 (2018-02-03)
         ------------------
         - Skeleton commit
```

