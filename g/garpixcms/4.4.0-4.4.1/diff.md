# Comparing `tmp/garpixcms-4.4.0.tar.gz` & `tmp/garpixcms-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpixcms-4.4.0.tar", last modified: Sat Jun 24 09:57:15 2023, max compression
+gzip compressed data, was "garpixcms-4.4.1.tar", last modified: Mon Jun 26 12:02:51 2023, max compression
```

## Comparing `garpixcms-4.4.0.tar` & `garpixcms-4.4.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.369606 garpixcms-4.4.0/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-06-24 09:57:15.000000 garpixcms-4.4.0/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1766 2023-06-24 09:57:15.369450 garpixcms-4.4.0/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.326425 garpixcms-4.4.0/garpixcms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    13753 2023-06-23 07:49:04.000000 garpixcms-4.4.0/garpixcms/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1084 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1207 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/README.rst
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.335874 garpixcms-4.4.0/garpixcms/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      161 2023-04-18 20:28:30.000000 garpixcms-4.4.0/garpixcms/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-04-18 20:28:30.000000 garpixcms-4.4.0/garpixcms/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6796 2023-04-18 20:28:30.000000 garpixcms-4.4.0/garpixcms/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1743 2023-04-18 20:28:31.000000 garpixcms-4.4.0/garpixcms/__pycache__/urls.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.336371 garpixcms-4.4.0/garpixcms/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/admin/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.336989 garpixcms-4.4.0/garpixcms/admin/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      205 2023-04-18 20:28:31.000000 garpixcms-4.4.0/garpixcms/admin/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      487 2023-04-18 20:28:31.000000 garpixcms-4.4.0/garpixcms/admin/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      173 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/admin/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       93 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/apps.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.337346 garpixcms-4.4.0/garpixcms/contexts/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/contexts/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      691 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/contexts/global_context.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.337795 garpixcms-4.4.0/garpixcms/management/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/management/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.337899 garpixcms-4.4.0/garpixcms/management/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:01:00.000000 garpixcms-4.4.0/garpixcms/management/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.339135 garpixcms-4.4.0/garpixcms/management/commands/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/management/commands/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      872 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/management/commands/update_user_module.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.339789 garpixcms-4.4.0/garpixcms/middleware/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/middleware/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.341436 garpixcms-4.4.0/garpixcms/middleware/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:00:43.000000 garpixcms-4.4.0/garpixcms/middleware/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2037 2023-05-10 14:00:43.000000 garpixcms-4.4.0/garpixcms/middleware/__pycache__/locale.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2196 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/middleware/locale.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.342084 garpixcms-4.4.0/garpixcms/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/models/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.343197 garpixcms-4.4.0/garpixcms/models/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      201 2023-04-18 20:28:31.000000 garpixcms-4.4.0/garpixcms/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      818 2023-04-18 20:28:31.000000 garpixcms-4.4.0/garpixcms/models/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      413 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/models/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1697 2023-06-23 07:46:05.000000 garpixcms-4.4.0/garpixcms/setup.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.323098 garpixcms-4.4.0/garpixcms/static/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.323289 garpixcms-4.4.0/garpixcms/static/admin/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.354033 garpixcms-4.4.0/garpixcms/static/admin/css/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/css/autocomplete.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    22662 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/css/base.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6469 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/css/changelists.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      355 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/css/dashboard.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      423 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/css/fonts.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8370 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/css/forms.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1185 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/css/login.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/css/nav_sidebar.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    18344 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/css/responsive.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1741 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/css/responsive_rtl.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3487 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/css/rtl.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/css/tabbed_translation_fields.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10010 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/css/widgets.css
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.355928 garpixcms-4.4.0/garpixcms/static/admin/img/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      908 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/img/icon-addlink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      825 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/img/icon-changelink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      218 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/img/icon-custom-checked.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      705 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/img/icon-deletelink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      930 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/img/search.svg
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.358570 garpixcms-4.4.0/garpixcms/static/admin/js/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      291 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/static/admin/js/admin.js
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.323474 garpixcms-4.4.0/garpixcms/templates/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.361870 garpixcms-4.4.0/garpixcms/templates/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4421 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/templates/admin/app_list.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4395 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/templates/admin/base.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      809 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/templates/admin/base_site.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.362025 garpixcms-4.4.0/garpixcms/templates/garpixcms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      450 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/templates/garpixcms/base.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.362444 garpixcms-4.4.0/garpixcms/templates/garpixcms/include/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      730 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/templates/garpixcms/include/footer.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      642 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/templates/garpixcms/include/header.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      428 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/templates/garpixcms/include/login.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.362711 garpixcms-4.4.0/garpixcms/templates/garpixcms/menus/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/templates/garpixcms/menus/footer_menu.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/templates/garpixcms/menus/header_menu.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.364198 garpixcms-4.4.0/garpixcms/templates/garpixcms/pages/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      139 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/templates/garpixcms/pages/default.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/templates/garpixcms/pages/home.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      346 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/templates/garpixcms/pages/login.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.369012 garpixcms-4.4.0/garpixcms/translation/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       49 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/translation/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.369258 garpixcms-4.4.0/garpixcms/translation/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      224 2023-04-18 20:28:31.000000 garpixcms-4.4.0/garpixcms/translation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 20:28:31.000000 garpixcms-4.4.0/garpixcms/translation/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      189 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/translation/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1842 2023-04-18 19:40:20.000000 garpixcms-4.4.0/garpixcms/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-24 09:57:15.329868 garpixcms-4.4.0/garpixcms.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1766 2023-06-24 09:57:15.000000 garpixcms-4.4.0/garpixcms.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2848 2023-06-24 09:57:15.000000 garpixcms-4.4.0/garpixcms.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-24 09:57:15.000000 garpixcms-4.4.0/garpixcms.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-24 09:57:15.000000 garpixcms-4.4.0/garpixcms.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-06-24 09:57:15.000000 garpixcms-4.4.0/garpixcms.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       10 2023-06-24 09:57:15.000000 garpixcms-4.4.0/garpixcms.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-06-24 09:57:15.369651 garpixcms-4.4.0/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1697 2023-06-24 09:57:15.000000 garpixcms-4.4.0/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.679024 garpixcms-4.4.1/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-06-26 12:02:51.000000 garpixcms-4.4.1/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1766 2023-06-26 12:02:51.678759 garpixcms-4.4.1/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.669427 garpixcms-4.4.1/garpixcms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    13819 2023-06-26 12:01:36.000000 garpixcms-4.4.1/garpixcms/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1084 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1207 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/README.rst
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.670539 garpixcms-4.4.1/garpixcms/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      161 2023-04-18 20:28:30.000000 garpixcms-4.4.1/garpixcms/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-04-18 20:28:30.000000 garpixcms-4.4.1/garpixcms/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6796 2023-04-18 20:28:30.000000 garpixcms-4.4.1/garpixcms/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1743 2023-04-18 20:28:31.000000 garpixcms-4.4.1/garpixcms/__pycache__/urls.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.670762 garpixcms-4.4.1/garpixcms/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/admin/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.670991 garpixcms-4.4.1/garpixcms/admin/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      205 2023-04-18 20:28:31.000000 garpixcms-4.4.1/garpixcms/admin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      487 2023-04-18 20:28:31.000000 garpixcms-4.4.1/garpixcms/admin/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      173 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/admin/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       93 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/apps.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.671184 garpixcms-4.4.1/garpixcms/contexts/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/contexts/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      691 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/contexts/global_context.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.671290 garpixcms-4.4.1/garpixcms/management/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/management/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.671384 garpixcms-4.4.1/garpixcms/management/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:01:00.000000 garpixcms-4.4.1/garpixcms/management/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.671597 garpixcms-4.4.1/garpixcms/management/commands/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/management/commands/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      872 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/management/commands/update_user_module.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.671790 garpixcms-4.4.1/garpixcms/middleware/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/middleware/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.672019 garpixcms-4.4.1/garpixcms/middleware/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:00:43.000000 garpixcms-4.4.1/garpixcms/middleware/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2037 2023-05-10 14:00:43.000000 garpixcms-4.4.1/garpixcms/middleware/__pycache__/locale.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2196 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/middleware/locale.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.672232 garpixcms-4.4.1/garpixcms/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.672464 garpixcms-4.4.1/garpixcms/models/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      201 2023-04-18 20:28:31.000000 garpixcms-4.4.1/garpixcms/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      818 2023-04-18 20:28:31.000000 garpixcms-4.4.1/garpixcms/models/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      413 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/models/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1697 2023-06-26 12:01:36.000000 garpixcms-4.4.1/garpixcms/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.667356 garpixcms-4.4.1/garpixcms/static/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.667537 garpixcms-4.4.1/garpixcms/static/admin/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.674202 garpixcms-4.4.1/garpixcms/static/admin/css/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/css/autocomplete.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    22662 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/css/base.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6469 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/css/changelists.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      355 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/css/dashboard.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      423 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/css/fonts.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8370 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/css/forms.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1185 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/css/login.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/css/nav_sidebar.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    18344 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/css/responsive.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1741 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/css/responsive_rtl.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3487 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/css/rtl.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/css/tabbed_translation_fields.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10010 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/css/widgets.css
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.674789 garpixcms-4.4.1/garpixcms/static/admin/img/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      908 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/img/icon-addlink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      825 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/img/icon-changelink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      218 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/img/icon-custom-checked.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      705 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/img/icon-deletelink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      930 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/img/search.svg
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.674900 garpixcms-4.4.1/garpixcms/static/admin/js/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      291 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/static/admin/js/admin.js
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.667723 garpixcms-4.4.1/garpixcms/templates/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.675242 garpixcms-4.4.1/garpixcms/templates/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4421 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/templates/admin/app_list.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4395 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/templates/admin/base.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      809 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/templates/admin/base_site.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.675350 garpixcms-4.4.1/garpixcms/templates/garpixcms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      450 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/templates/garpixcms/base.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.675683 garpixcms-4.4.1/garpixcms/templates/garpixcms/include/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      730 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/templates/garpixcms/include/footer.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      642 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/templates/garpixcms/include/header.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      428 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/templates/garpixcms/include/login.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.675907 garpixcms-4.4.1/garpixcms/templates/garpixcms/menus/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/templates/garpixcms/menus/footer_menu.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/templates/garpixcms/menus/header_menu.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.676250 garpixcms-4.4.1/garpixcms/templates/garpixcms/pages/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      139 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/templates/garpixcms/pages/default.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/templates/garpixcms/pages/home.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      346 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/templates/garpixcms/pages/login.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.676483 garpixcms-4.4.1/garpixcms/translation/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       49 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/translation/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.678480 garpixcms-4.4.1/garpixcms/translation/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      224 2023-04-18 20:28:31.000000 garpixcms-4.4.1/garpixcms/translation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 20:28:31.000000 garpixcms-4.4.1/garpixcms/translation/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      189 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/translation/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1842 2023-04-18 19:40:20.000000 garpixcms-4.4.1/garpixcms/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-26 12:02:51.670092 garpixcms-4.4.1/garpixcms.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1766 2023-06-26 12:02:51.000000 garpixcms-4.4.1/garpixcms.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2848 2023-06-26 12:02:51.000000 garpixcms-4.4.1/garpixcms.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-26 12:02:51.000000 garpixcms-4.4.1/garpixcms.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-26 12:02:51.000000 garpixcms-4.4.1/garpixcms.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-06-26 12:02:51.000000 garpixcms-4.4.1/garpixcms.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       10 2023-06-26 12:02:51.000000 garpixcms-4.4.1/garpixcms.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-06-26 12:02:51.679081 garpixcms-4.4.1/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1697 2023-06-26 12:02:51.000000 garpixcms-4.4.1/setup.py
```

### Comparing `garpixcms-4.4.0/PKG-INFO` & `garpixcms-4.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpixcms
-Version: 4.4.0
+Version: 4.4.1
 Home-page: https://github.com/garpixcms/garpixcms
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpixcms-4.4.0/garpixcms/CHANGELOG.md` & `garpixcms-4.4.1/garpixcms/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-### 4.4.0 (09.06.2023)
+### 4.4.1 (26.06.2023)
+
+- Upgrade `garpix_user` to version 3.8.1
+
+### 4.4.0 (23.06.2023)
 
 - Upgrade `garpix_user` to version 3.8.0
 - `django.contrib.auth.backends.ModelBackend` deprecated
 
 ### 4.3.1 (09.06.2023)
 
 - Upgrade `garpix_user` to version 3.6.1
```

### Comparing `garpixcms-4.4.0/garpixcms/CONTRIBUTING.md` & `garpixcms-4.4.1/garpixcms/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/README.rst` & `garpixcms-4.4.1/garpixcms/README.rst`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/__pycache__/settings.cpython-38.pyc` & `garpixcms-4.4.1/garpixcms/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/__pycache__/urls.cpython-38.pyc` & `garpixcms-4.4.1/garpixcms/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/contexts/global_context.py` & `garpixcms-4.4.1/garpixcms/contexts/global_context.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/management/commands/update_user_module.py` & `garpixcms-4.4.1/garpixcms/management/commands/update_user_module.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/middleware/__pycache__/locale.cpython-38.pyc` & `garpixcms-4.4.1/garpixcms/middleware/__pycache__/locale.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/middleware/locale.py` & `garpixcms-4.4.1/garpixcms/middleware/locale.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/models/__pycache__/page.cpython-38.pyc` & `garpixcms-4.4.1/garpixcms/models/__pycache__/page.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/settings.py` & `garpixcms-4.4.1/garpixcms/settings.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/setup.py` & `garpixcms-4.4.1/garpixcms/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpixcms')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpixcms',
-    version='4.4.0',
+    version='4.4.1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpixcms',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -33,15 +33,15 @@
         'Django >= 3.1, < 4',
         'garpix_utils == 1.8.0',
         'garpix_page == 2.48.0',
         'garpix_menu == 1.16.0',
         'eqator == 2.7.0',
         'garpix_auth == 2.3.0',
         'garpix_notify == 5.16.0',
-        'garpix_user == 3.8.0',
+        'garpix_user == 3.8.1',
         'garpix_package == 2.0.1',
         'psycopg2-binary >= 2.8.6',
         'uwsgi >= 2.0.19.1',
         'environs >= 9.3.2',
         'django-ckeditor == 6.3.0',
         'djangorestframework >= 3.12.4',
         'django-cors-headers >= 3.7.0, <= 3.13.0',
```

### Comparing `garpixcms-4.4.0/garpixcms/static/admin/css/autocomplete.css` & `garpixcms-4.4.1/garpixcms/static/admin/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/static/admin/css/base.css` & `garpixcms-4.4.1/garpixcms/static/admin/css/base.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/static/admin/css/changelists.css` & `garpixcms-4.4.1/garpixcms/static/admin/css/changelists.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/static/admin/css/forms.css` & `garpixcms-4.4.1/garpixcms/static/admin/css/forms.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/static/admin/css/login.css` & `garpixcms-4.4.1/garpixcms/static/admin/css/login.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/static/admin/css/nav_sidebar.css` & `garpixcms-4.4.1/garpixcms/static/admin/css/nav_sidebar.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/static/admin/css/responsive.css` & `garpixcms-4.4.1/garpixcms/static/admin/css/responsive.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/static/admin/css/responsive_rtl.css` & `garpixcms-4.4.1/garpixcms/static/admin/css/responsive_rtl.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/static/admin/css/rtl.css` & `garpixcms-4.4.1/garpixcms/static/admin/css/rtl.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/static/admin/css/widgets.css` & `garpixcms-4.4.1/garpixcms/static/admin/css/widgets.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/static/admin/img/icon-addlink.svg` & `garpixcms-4.4.1/garpixcms/static/admin/img/icon-addlink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/static/admin/img/icon-changelink.svg` & `garpixcms-4.4.1/garpixcms/static/admin/img/icon-changelink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/static/admin/img/icon-deletelink.svg` & `garpixcms-4.4.1/garpixcms/static/admin/img/icon-deletelink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/static/admin/img/search.svg` & `garpixcms-4.4.1/garpixcms/static/admin/img/search.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/templates/admin/app_list.html` & `garpixcms-4.4.1/garpixcms/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/templates/admin/base.html` & `garpixcms-4.4.1/garpixcms/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/templates/admin/base_site.html` & `garpixcms-4.4.1/garpixcms/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/templates/garpixcms/include/footer.html` & `garpixcms-4.4.1/garpixcms/templates/garpixcms/include/footer.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/templates/garpixcms/include/header.html` & `garpixcms-4.4.1/garpixcms/templates/garpixcms/include/header.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms/urls.py` & `garpixcms-4.4.1/garpixcms/urls.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/garpixcms.egg-info/PKG-INFO` & `garpixcms-4.4.1/garpixcms.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpixcms
-Version: 4.4.0
+Version: 4.4.1
 Home-page: https://github.com/garpixcms/garpixcms
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpixcms-4.4.0/garpixcms.egg-info/SOURCES.txt` & `garpixcms-4.4.1/garpixcms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpixcms-4.4.0/setup.py` & `garpixcms-4.4.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpixcms')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpixcms',
-    version='4.4.0',
+    version='4.4.1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpixcms',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -33,15 +33,15 @@
         'Django >= 3.1, < 4',
         'garpix_utils == 1.8.0',
         'garpix_page == 2.48.0',
         'garpix_menu == 1.16.0',
         'eqator == 2.7.0',
         'garpix_auth == 2.3.0',
         'garpix_notify == 5.16.0',
-        'garpix_user == 3.8.0',
+        'garpix_user == 3.8.1',
         'garpix_package == 2.0.1',
         'psycopg2-binary >= 2.8.6',
         'uwsgi >= 2.0.19.1',
         'environs >= 9.3.2',
         'django-ckeditor == 6.3.0',
         'djangorestframework >= 3.12.4',
         'django-cors-headers >= 3.7.0, <= 3.13.0',
```

