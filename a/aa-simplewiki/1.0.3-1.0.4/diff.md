# Comparing `tmp/aa-simplewiki-1.0.3.tar.gz` & `tmp/aa-simplewiki-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-simplewiki-1.0.3.tar", last modified: Thu Jun 22 13:24:11 2023, max compression
+gzip compressed data, was "aa-simplewiki-1.0.4.tar", last modified: Mon Jun 26 14:49:20 2023, max compression
```

## Comparing `aa-simplewiki-1.0.3.tar` & `aa-simplewiki-1.0.4.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.884516 aa-simplewiki-1.0.3/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    35164 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/LICENSE
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      123 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/MANIFEST.in
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5719 2023-06-22 13:24:11.884516 aa-simplewiki-1.0.3/PKG-INFO
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4701 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/README.md
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.868511 aa-simplewiki-1.0.3/aa_simplewiki.egg-info/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5719 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.3/aa_simplewiki.egg-info/PKG-INFO
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2607 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.3/aa_simplewiki.egg-info/SOURCES.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.3/aa_simplewiki.egg-info/dependency_links.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.3/aa_simplewiki.egg-info/not-zip-safe
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       24 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.3/aa_simplewiki.egg-info/requires.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       20 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.3/aa_simplewiki.egg-info/top_level.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      104 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/pyproject.toml
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1462 2023-06-22 13:24:11.884516 aa-simplewiki-1.0.3/setup.cfg
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1206 2023-06-22 13:22:42.000000 aa-simplewiki-1.0.3/setup.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.868511 aa-simplewiki-1.0.3/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       47 2023-06-22 13:23:52.000000 aa-simplewiki-1.0.3/simplewiki/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      231 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/admin.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    11916 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/admin_helper_menus.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     8956 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/admin_helper_sections.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      169 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/app_settings.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      284 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/apps.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/auth_hooks.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.876514 aa-simplewiki-1.0.3/simplewiki/migrations/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1489 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0001_initial.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      395 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0002_pageitem_page_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      401 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0003_menuitem_icon.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1532 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1522 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      374 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0006_rename_pageitem_sectionitem.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      392 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1657 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      658 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      381 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0010_rename_path_menuitem_name.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      372 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0011_rename_name_menuitem_path.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      576 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0012_menuitem_group.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      579 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0013_alter_menuitem_group.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3030 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      685 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      831 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      399 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0018_rename_group_menuitem_groups.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      492 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0019_alter_general_options.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      538 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/0020_menuitem_parent.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/migrations/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4236 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/models.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.864510 aa-simplewiki-1.0.3/simplewiki/static/
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.876514 aa-simplewiki-1.0.3/simplewiki/static/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/static/simplewiki/.gitkeep
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      199 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/static/simplewiki/custom.css
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      226 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/tasks.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.864510 aa-simplewiki-1.0.3/simplewiki/templates/
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.880515 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6324 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/base.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/dynamic_page.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.880515 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6630 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/editor_menus.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9500 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/editor_sections.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.880515 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/partials/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2320 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/partials/_create_menu.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2468 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      593 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/error.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      460 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/index.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1578 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/search.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.880515 aa-simplewiki-1.0.3/simplewiki/templatetags/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2327 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templatetags/custom_filters.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/templatetags/markdown_filters.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.880515 aa-simplewiki-1.0.3/simplewiki/tests/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       27 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/tests/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      448 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/tests/test_example.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      488 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/simplewiki/urls.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    12930 2023-06-22 11:57:18.000000 aa-simplewiki-1.0.3/simplewiki/views.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 13:24:11.884516 aa-simplewiki-1.0.3/testauth/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       52 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/testauth/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      654 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/testauth/celery.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9481 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/testauth/settings.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      167 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/testauth/urls.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      425 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.3/testauth/wsgi.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.703167 aa-simplewiki-1.0.4/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    35164 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/LICENSE
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      123 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/MANIFEST.in
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5930 2023-06-26 14:49:20.703167 aa-simplewiki-1.0.4/PKG-INFO
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4921 2023-06-26 14:44:07.000000 aa-simplewiki-1.0.4/README.md
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.695167 aa-simplewiki-1.0.4/aa_simplewiki.egg-info/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5930 2023-06-26 14:49:20.000000 aa-simplewiki-1.0.4/aa_simplewiki.egg-info/PKG-INFO
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2708 2023-06-26 14:49:20.000000 aa-simplewiki-1.0.4/aa_simplewiki.egg-info/SOURCES.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-06-26 14:49:20.000000 aa-simplewiki-1.0.4/aa_simplewiki.egg-info/dependency_links.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-06-22 13:24:11.000000 aa-simplewiki-1.0.4/aa_simplewiki.egg-info/not-zip-safe
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       28 2023-06-26 14:49:20.000000 aa-simplewiki-1.0.4/aa_simplewiki.egg-info/requires.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       20 2023-06-26 14:49:20.000000 aa-simplewiki-1.0.4/aa_simplewiki.egg-info/top_level.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      104 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/pyproject.toml
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1434 2023-06-26 14:49:20.703167 aa-simplewiki-1.0.4/setup.cfg
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1253 2023-06-26 14:24:39.000000 aa-simplewiki-1.0.4/setup.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.699167 aa-simplewiki-1.0.4/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       47 2023-06-26 14:22:59.000000 aa-simplewiki-1.0.4/simplewiki/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      231 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/admin.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    11916 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/admin_helper_menus.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     8956 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/admin_helper_sections.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      169 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/app_settings.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      284 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/apps.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/auth_hooks.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.699167 aa-simplewiki-1.0.4/simplewiki/migrations/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1489 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0001_initial.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      395 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0002_pageitem_page_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      401 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0003_menuitem_icon.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1532 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1522 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      374 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0006_rename_pageitem_sectionitem.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      392 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1657 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      658 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      381 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0010_rename_path_menuitem_name.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      372 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0011_rename_name_menuitem_path.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      576 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0012_menuitem_group.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      579 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0013_alter_menuitem_group.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3030 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      685 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      831 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      399 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0018_rename_group_menuitem_groups.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      492 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0019_alter_general_options.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      538 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/0020_menuitem_parent.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/migrations/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4236 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/models.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.695167 aa-simplewiki-1.0.4/simplewiki/static/
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.699167 aa-simplewiki-1.0.4/simplewiki/static/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/static/simplewiki/.gitkeep
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    44136 2023-06-22 23:46:34.000000 aa-simplewiki-1.0.4/simplewiki/static/simplewiki/Sortable.min.js
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      199 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/static/simplewiki/custom.css
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      226 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/tasks.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.695167 aa-simplewiki-1.0.4/simplewiki/templates/
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.699167 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6725 2023-06-26 13:24:54.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/base.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-06-26 12:25:27.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/dynamic_page.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.699167 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6630 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/editor_menus.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9500 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/editor_sections.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3001 2023-06-23 00:32:43.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/editor_sort.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.699167 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/partials/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2320 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/partials/_create_menu.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2468 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      593 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/error.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      460 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/index.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1578 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/search.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.703167 aa-simplewiki-1.0.4/simplewiki/templatetags/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2327 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/templatetags/custom_filters.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2145 2023-06-26 14:07:13.000000 aa-simplewiki-1.0.4/simplewiki/templatetags/markdown_filters.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.703167 aa-simplewiki-1.0.4/simplewiki/tests/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       27 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/tests/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      448 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/simplewiki/tests/test_example.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      561 2023-06-26 13:47:46.000000 aa-simplewiki-1.0.4/simplewiki/urls.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    13176 2023-06-26 13:47:40.000000 aa-simplewiki-1.0.4/simplewiki/views.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-06-26 14:49:20.703167 aa-simplewiki-1.0.4/testauth/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       52 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/testauth/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      654 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/testauth/celery.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9481 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/testauth/settings.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      167 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/testauth/urls.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      425 2023-06-22 11:32:12.000000 aa-simplewiki-1.0.4/testauth/wsgi.py
```

### Comparing `aa-simplewiki-1.0.3/LICENSE` & `aa-simplewiki-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/PKG-INFO` & `aa-simplewiki-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: aa-simplewiki
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alliance Auth Wiki Plugin
 Home-page: https://github.com/meowosaurus/aa-simplewiki
 Author: Meowosaurus
 Author-email: info@bjsonnen.de
-Maintainer: Peter Pfeufer
-Maintainer-email: development@ppfeufer.de
+Maintainer: Meowosaurus
+Maintainer-email: info@bjsonnen.de
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/aa-simplewiki-plugin/issues
 Project-URL: Changelog, https://github.com/ppfeufer/aa-simplewiki-plugin/blob/master/CHANGELOG.md
 Keywords: allianceauth,simplewiki
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -39,28 +39,33 @@
 * [Usage](#usage)
 * [Permissions](#permissions)
 * [Support](#support)
 
 # Current Features
 * Create custom wiki menus with dropdowns plus different sections on each menu
 * Add an icon next to menus or sections
-* Edit pages on the admin panel with [markdown](https://commonmark.org/help/)
+* Edit pages on the admin panel with [markdown](https://www.markdownguide.org/cheat-sheet/)
+  * Support for images
+  * Support for videos (YouTube and Vimeo)
 * Search function: Search across all wiki menus and sections
 * Permission system:
   * Editor permissions can be added to single users or groups via the admin panel
   * Alliance Auth groups are synced to simplewiki: Certain pages can only be seen by a specific group
   * Multiple groups support: As long as the user is in any of the required groups, they can access the menu
 * Editor interface
   * Users with editor permission can create, edit and delete custom menus and sections (editor_access)
   * Users with editor permission see edit and delete buttons above all sections (editor_access)
 
 ## ToDo:
 * Quality-of-life updates
 * Improve code documentation
 * Clean-up code
+* Markdown
+  * Tables
+  * Buttons
 
 ## Planned
 * Drag and drop system to make indexing menus and sections easier
 * Add translations for 
   * German
   * Spanish
   * Chinese
@@ -75,17 +80,17 @@
 ## Screenshots
 ![Showcase](https://i.postimg.cc/BQc3hPYb/vmplayer-Kvz8-DNZa-M0.gif)
 
 ### Search
 ![Search](https://i.imgur.com/wW69LFN.png)
 
 ### Admin Panel
-![Menu Admin](https://i.imgur.com/VGssV4d.png)
+![Menu Admin](https://github.com/meowosaurus/aa-simplewiki/blob/master/images/menu_admin_panel.png)
 
-![Menu Edit](https://i.imgur.com/15DSNfZ.png)
+![Menu Edit](https://github.com/meowosaurus/aa-simplewiki/blob/master/images/menu_admin_panel_edit.png)
 
 ![Section Edit](https://i.imgur.com/3LrysW7.png)
 
 ## Installation
 
 ### Alliance Auth Production
 
@@ -150,8 +155,8 @@
 ## Permissions
 Perm | Admin Site | Auth Site 
  --- | --- | --- 
 basic_access | None | Can view all wiki pages
 editor_access | None | Can create, edit and delete wiki pages and menus
 
 ## Support
-* On Discord: Meowlicious#7045
+* On Discord: meowlicious
```

### Comparing `aa-simplewiki-1.0.3/README.md` & `aa-simplewiki-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,33 @@
 * [Usage](#usage)
 * [Permissions](#permissions)
 * [Support](#support)
 
 # Current Features
 * Create custom wiki menus with dropdowns plus different sections on each menu
 * Add an icon next to menus or sections
-* Edit pages on the admin panel with [markdown](https://commonmark.org/help/)
+* Edit pages on the admin panel with [markdown](https://www.markdownguide.org/cheat-sheet/)
+  * Support for images
+  * Support for videos (YouTube and Vimeo)
 * Search function: Search across all wiki menus and sections
 * Permission system:
   * Editor permissions can be added to single users or groups via the admin panel
   * Alliance Auth groups are synced to simplewiki: Certain pages can only be seen by a specific group
   * Multiple groups support: As long as the user is in any of the required groups, they can access the menu
 * Editor interface
   * Users with editor permission can create, edit and delete custom menus and sections (editor_access)
   * Users with editor permission see edit and delete buttons above all sections (editor_access)
 
 ## ToDo:
 * Quality-of-life updates
 * Improve code documentation
 * Clean-up code
+* Markdown
+  * Tables
+  * Buttons
 
 ## Planned
 * Drag and drop system to make indexing menus and sections easier
 * Add translations for 
   * German
   * Spanish
   * Chinese
@@ -50,17 +55,17 @@
 ## Screenshots
 ![Showcase](https://i.postimg.cc/BQc3hPYb/vmplayer-Kvz8-DNZa-M0.gif)
 
 ### Search
 ![Search](https://i.imgur.com/wW69LFN.png)
 
 ### Admin Panel
-![Menu Admin](https://i.imgur.com/VGssV4d.png)
+![Menu Admin](https://github.com/meowosaurus/aa-simplewiki/blob/master/images/menu_admin_panel.png)
 
-![Menu Edit](https://i.imgur.com/15DSNfZ.png)
+![Menu Edit](https://github.com/meowosaurus/aa-simplewiki/blob/master/images/menu_admin_panel_edit.png)
 
 ![Section Edit](https://i.imgur.com/3LrysW7.png)
 
 ## Installation
 
 ### Alliance Auth Production
 
@@ -125,8 +130,8 @@
 ## Permissions
 Perm | Admin Site | Auth Site 
  --- | --- | --- 
 basic_access | None | Can view all wiki pages
 editor_access | None | Can create, edit and delete wiki pages and menus
 
 ## Support
-* On Discord: Meowlicious#7045
+* On Discord: meowlicious
```

### Comparing `aa-simplewiki-1.0.3/aa_simplewiki.egg-info/PKG-INFO` & `aa-simplewiki-1.0.4/aa_simplewiki.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: aa-simplewiki
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alliance Auth Wiki Plugin
 Home-page: https://github.com/meowosaurus/aa-simplewiki
 Author: Meowosaurus
 Author-email: info@bjsonnen.de
-Maintainer: Peter Pfeufer
-Maintainer-email: development@ppfeufer.de
+Maintainer: Meowosaurus
+Maintainer-email: info@bjsonnen.de
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/aa-simplewiki-plugin/issues
 Project-URL: Changelog, https://github.com/ppfeufer/aa-simplewiki-plugin/blob/master/CHANGELOG.md
 Keywords: allianceauth,simplewiki
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -39,28 +39,33 @@
 * [Usage](#usage)
 * [Permissions](#permissions)
 * [Support](#support)
 
 # Current Features
 * Create custom wiki menus with dropdowns plus different sections on each menu
 * Add an icon next to menus or sections
-* Edit pages on the admin panel with [markdown](https://commonmark.org/help/)
+* Edit pages on the admin panel with [markdown](https://www.markdownguide.org/cheat-sheet/)
+  * Support for images
+  * Support for videos (YouTube and Vimeo)
 * Search function: Search across all wiki menus and sections
 * Permission system:
   * Editor permissions can be added to single users or groups via the admin panel
   * Alliance Auth groups are synced to simplewiki: Certain pages can only be seen by a specific group
   * Multiple groups support: As long as the user is in any of the required groups, they can access the menu
 * Editor interface
   * Users with editor permission can create, edit and delete custom menus and sections (editor_access)
   * Users with editor permission see edit and delete buttons above all sections (editor_access)
 
 ## ToDo:
 * Quality-of-life updates
 * Improve code documentation
 * Clean-up code
+* Markdown
+  * Tables
+  * Buttons
 
 ## Planned
 * Drag and drop system to make indexing menus and sections easier
 * Add translations for 
   * German
   * Spanish
   * Chinese
@@ -75,17 +80,17 @@
 ## Screenshots
 ![Showcase](https://i.postimg.cc/BQc3hPYb/vmplayer-Kvz8-DNZa-M0.gif)
 
 ### Search
 ![Search](https://i.imgur.com/wW69LFN.png)
 
 ### Admin Panel
-![Menu Admin](https://i.imgur.com/VGssV4d.png)
+![Menu Admin](https://github.com/meowosaurus/aa-simplewiki/blob/master/images/menu_admin_panel.png)
 
-![Menu Edit](https://i.imgur.com/15DSNfZ.png)
+![Menu Edit](https://github.com/meowosaurus/aa-simplewiki/blob/master/images/menu_admin_panel_edit.png)
 
 ![Section Edit](https://i.imgur.com/3LrysW7.png)
 
 ## Installation
 
 ### Alliance Auth Production
 
@@ -150,8 +155,8 @@
 ## Permissions
 Perm | Admin Site | Auth Site 
  --- | --- | --- 
 basic_access | None | Can view all wiki pages
 editor_access | None | Can create, edit and delete wiki pages and menus
 
 ## Support
-* On Discord: Meowlicious#7045
+* On Discord: meowlicious
```

### Comparing `aa-simplewiki-1.0.3/aa_simplewiki.egg-info/SOURCES.txt` & `aa-simplewiki-1.0.4/aa_simplewiki.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,22 +39,24 @@
 simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
 simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
 simplewiki/migrations/0018_rename_group_menuitem_groups.py
 simplewiki/migrations/0019_alter_general_options.py
 simplewiki/migrations/0020_menuitem_parent.py
 simplewiki/migrations/__init__.py
 simplewiki/static/simplewiki/.gitkeep
+simplewiki/static/simplewiki/Sortable.min.js
 simplewiki/static/simplewiki/custom.css
 simplewiki/templates/simplewiki/base.html
 simplewiki/templates/simplewiki/dynamic_page.html
 simplewiki/templates/simplewiki/error.html
 simplewiki/templates/simplewiki/index.html
 simplewiki/templates/simplewiki/search.html
 simplewiki/templates/simplewiki/editor/editor_menus.html
 simplewiki/templates/simplewiki/editor/editor_sections.html
+simplewiki/templates/simplewiki/editor/editor_sort.html
 simplewiki/templates/simplewiki/editor/partials/_create_menu.html
 simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
 simplewiki/templatetags/custom_filters.py
 simplewiki/templatetags/markdown_filters.py
 simplewiki/tests/__init__.py
 simplewiki/tests/test_example.py
 testauth/__init__.py
```

### Comparing `aa-simplewiki-1.0.3/setup.cfg` & `aa-simplewiki-1.0.4/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
-name = aa_simplewiki_plugin
+name = aa_simplewiki
 version = attr: simplewiki.__version__
-description = simplewiki Plugin for Alliance Auth (GitHub Version)
+description = SimpleWiki Plugin for Alliance Auth (GitHub Version)
 long_description = file: README.md
 long_description_content_type = text/markdown
-author = Peter Pfeufer
-author_email = development@ppfeufer.de
-maintainer = Peter Pfeufer
-maintainer_email = development@ppfeufer.de
+author = Meowosaurus
+author_email = info@bjsonnen.de
+maintainer = Meowosaurus
+maintainer_email = info@bjsonnen.de
 license = GPL-3.0
 license_file = LICENSE
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 4.0
 	Intended Audience :: Developers
@@ -31,16 +31,16 @@
 project_urls = 
 	Issue / Bug Reports = https://github.com/ppfeufer/aa-simplewiki-plugin/issues
 	Changelog = https://github.com/ppfeufer/aa-simplewiki-plugin/blob/master/CHANGELOG.md
 
 [options]
 packages = find_namespace:
 install_requires = 
-	allianceauth>=3.0.0
-	commonmark>=0.9.1
+	allianceauth>=3.4.0
+	mistune>=3.0.1
 python_requires = ~=3.8
 include_package_data = True
 zip_safe = False
 
 [options.packages.find]
 include = simplewiki*
```

### Comparing `aa-simplewiki-1.0.3/setup.py` & `aa-simplewiki-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 install_requires = [
-    'commonmark',
+    'mistune>=3.0.1',
     'allianceauth',
 ]
 
 setup(
     name='aa-simplewiki',
     version=__version__,
     packages=find_packages(),
     include_package_data=True,
+    exclude_package_data={'': ['images']},
     license='GNU General Public License v3 (GPLv3)',
     description='Alliance Auth Wiki Plugin',
     install_requires=install_requires,
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/meowosaurus/aa-simplewiki',
     author='Meowosaurus',
```

### Comparing `aa-simplewiki-1.0.3/simplewiki/admin_helper_menus.py` & `aa-simplewiki-1.0.4/simplewiki/admin_helper_menus.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/admin_helper_sections.py` & `aa-simplewiki-1.0.4/simplewiki/admin_helper_sections.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/auth_hooks.py` & `aa-simplewiki-1.0.4/simplewiki/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/migrations/0001_initial.py` & `aa-simplewiki-1.0.4/simplewiki/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.4/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py` & `aa-simplewiki-1.0.4/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.4/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py` & `aa-simplewiki-1.0.4/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/migrations/0012_menuitem_group.py` & `aa-simplewiki-1.0.4/simplewiki/migrations/0012_menuitem_group.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/migrations/0013_alter_menuitem_group.py` & `aa-simplewiki-1.0.4/simplewiki/migrations/0013_alter_menuitem_group.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.4/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py` & `aa-simplewiki-1.0.4/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py` & `aa-simplewiki-1.0.4/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/migrations/0020_menuitem_parent.py` & `aa-simplewiki-1.0.4/simplewiki/migrations/0020_menuitem_parent.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/models.py` & `aa-simplewiki-1.0.4/simplewiki/models.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/base.html` & `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,22 @@
                                 </li>
                                 <li>
                                     <a href="{% url 'simplewiki:editor_sections' %}">
                                         <i class="fas fa-pen"></i>
                                         Sections
                                     </a>
                                 </li>
+                                {% if False %}
+                                <li>
+                                    <a href="{% url 'simplewiki:editor_sort' %}">
+                                        <i class="fas fa-pen"></i>
+                                        Sort
+                                    </a>
+                                </li>
+                                {% endif %}
                             </ul>
                         </li>
                     {% endif %}
                   </ul>
             </div>
         </div>
     </nav>
```

#### html2text {}

```diff
@@ -23,11 +23,14 @@
     *  {{_menu_item.title_}}
     * {% endif %} {% endif %} {% endif %} {% endfor %}
     *  Search
     * {% if is_editor is True %}
     *  Editor
           o  Menus
           o  Sections
+          o {% if False %}
+          o  Sort
+          o {% endif %}
     * {% endif %}
  {% block details %}{% endblock %}
 {% endblock %} {% block extra_css %}
  {% endblock %}
```

### Comparing `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/dynamic_page.html` & `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/dynamic_page.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/editor_menus.html` & `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/editor_menus.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/editor_sections.html` & `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/editor_sections.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/partials/_create_menu.html` & `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/partials/_create_menu.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html` & `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/error.html` & `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/error.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/templates/simplewiki/search.html` & `aa-simplewiki-1.0.4/simplewiki/templates/simplewiki/search.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/templatetags/custom_filters.py` & `aa-simplewiki-1.0.4/simplewiki/templatetags/custom_filters.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/simplewiki/views.py` & `aa-simplewiki-1.0.4/simplewiki/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,7 +317,17 @@
             load_section_delete_form(request, context, delete)
         else:
             # Just list all sections if no button was pressed
             context.update({'user_action': 'none'})
 
     return render(request, "simplewiki/editor/editor_sections.html", context)
 
+"""
+# ToDo
+@login_required
+@permission_required("simplewiki.editor_access")
+def editor_sort(request: WSGIRequest) -> HttpResponse:
+    context = gen_context(request)
+
+    return render(request, "simplewiki/editor/editor_sort.html", context)
+"""
+
```

### Comparing `aa-simplewiki-1.0.3/testauth/celery.py` & `aa-simplewiki-1.0.4/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-1.0.3/testauth/settings.py` & `aa-simplewiki-1.0.4/testauth/settings.py`

 * *Files identical despite different names*

