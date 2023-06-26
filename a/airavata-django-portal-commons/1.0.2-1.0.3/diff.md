# Comparing `tmp/airavata-django-portal-commons-1.0.2.tar.gz` & `tmp/airavata-django-portal-commons-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airavata-django-portal-commons-1.0.2.tar", last modified: Thu Jun 22 16:56:27 2023, max compression
+gzip compressed data, was "airavata-django-portal-commons-1.0.3.tar", last modified: Mon Jun 26 16:39:46 2023, max compression
```

## Comparing `airavata-django-portal-commons-1.0.2.tar` & `airavata-django-portal-commons-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 16:56:27.537011 airavata-django-portal-commons-1.0.2/
--rw-r--r--   0 machrist (661619347) 1014028542        0 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/MANIFEST.in
--rw-r--r--   0 machrist (661619347) 1014028542     3294 2023-06-22 16:56:27.537073 airavata-django-portal-commons-1.0.2/PKG-INFO
--rw-r--r--   0 machrist (661619347) 1014028542     3111 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/README.md
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 16:56:27.535435 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/
--rw-r--r--   0 machrist (661619347) 1014028542        0 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/__init__.py
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 16:56:27.536779 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/dynamic_apps/
--rw-r--r--   0 machrist (661619347) 1014028542     2094 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/dynamic_apps/__init__.py
--rw-r--r--   0 machrist (661619347) 1014028542     4129 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/dynamic_apps/context_processors.py
--rw-r--r--   0 machrist (661619347) 1014028542      484 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/dynamic_apps/urls.py
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 16:56:27.536113 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/
--rw-r--r--   0 machrist (661619347) 1014028542     3294 2023-06-22 16:56:27.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/PKG-INFO
--rw-r--r--   0 machrist (661619347) 1014028542      541 2023-06-22 16:56:27.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/SOURCES.txt
--rw-r--r--   0 machrist (661619347) 1014028542        1 2023-06-22 16:56:27.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/dependency_links.txt
--rw-r--r--   0 machrist (661619347) 1014028542       26 2023-06-22 16:56:27.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/requires.txt
--rw-r--r--   0 machrist (661619347) 1014028542       31 2023-06-22 16:56:27.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/top_level.txt
--rw-r--r--   0 machrist (661619347) 1014028542      104 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/pyproject.toml
--rw-r--r--   0 machrist (661619347) 1014028542      362 2023-06-22 16:56:27.537352 airavata-django-portal-commons-1.0.2/setup.cfg
--rw-r--r--   0 machrist (661619347) 1014028542       38 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/setup.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-26 16:39:46.540799 airavata-django-portal-commons-1.0.3/
+-rw-r--r--   0 machrist (661619347) 1014028542        0 2023-06-26 16:39:16.000000 airavata-django-portal-commons-1.0.3/MANIFEST.in
+-rw-r--r--   0 machrist (661619347) 1014028542     3294 2023-06-26 16:39:46.540871 airavata-django-portal-commons-1.0.3/PKG-INFO
+-rw-r--r--   0 machrist (661619347) 1014028542     3111 2023-06-26 16:39:16.000000 airavata-django-portal-commons-1.0.3/README.md
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-26 16:39:46.538957 airavata-django-portal-commons-1.0.3/airavata_django_portal_commons/
+-rw-r--r--   0 machrist (661619347) 1014028542        0 2023-06-26 16:39:16.000000 airavata-django-portal-commons-1.0.3/airavata_django_portal_commons/__init__.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-26 16:39:46.540484 airavata-django-portal-commons-1.0.3/airavata_django_portal_commons/dynamic_apps/
+-rw-r--r--   0 machrist (661619347) 1014028542     2058 2023-06-26 16:39:16.000000 airavata-django-portal-commons-1.0.3/airavata_django_portal_commons/dynamic_apps/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542     4129 2023-06-26 16:39:16.000000 airavata-django-portal-commons-1.0.3/airavata_django_portal_commons/dynamic_apps/context_processors.py
+-rw-r--r--   0 machrist (661619347) 1014028542      484 2023-06-26 16:39:16.000000 airavata-django-portal-commons-1.0.3/airavata_django_portal_commons/dynamic_apps/urls.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-26 16:39:46.539862 airavata-django-portal-commons-1.0.3/airavata_django_portal_commons.egg-info/
+-rw-r--r--   0 machrist (661619347) 1014028542     3294 2023-06-26 16:39:46.000000 airavata-django-portal-commons-1.0.3/airavata_django_portal_commons.egg-info/PKG-INFO
+-rw-r--r--   0 machrist (661619347) 1014028542      541 2023-06-26 16:39:46.000000 airavata-django-portal-commons-1.0.3/airavata_django_portal_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 machrist (661619347) 1014028542        1 2023-06-26 16:39:46.000000 airavata-django-portal-commons-1.0.3/airavata_django_portal_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 machrist (661619347) 1014028542       26 2023-06-26 16:39:46.000000 airavata-django-portal-commons-1.0.3/airavata_django_portal_commons.egg-info/requires.txt
+-rw-r--r--   0 machrist (661619347) 1014028542       31 2023-06-26 16:39:46.000000 airavata-django-portal-commons-1.0.3/airavata_django_portal_commons.egg-info/top_level.txt
+-rw-r--r--   0 machrist (661619347) 1014028542      104 2023-06-26 16:39:16.000000 airavata-django-portal-commons-1.0.3/pyproject.toml
+-rw-r--r--   0 machrist (661619347) 1014028542      362 2023-06-26 16:39:46.541156 airavata-django-portal-commons-1.0.3/setup.cfg
+-rw-r--r--   0 machrist (661619347) 1014028542       38 2023-06-26 16:39:16.000000 airavata-django-portal-commons-1.0.3/setup.py
```

### Comparing `airavata-django-portal-commons-1.0.2/PKG-INFO` & `airavata-django-portal-commons-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airavata-django-portal-commons
-Version: 1.0.2
+Version: 1.0.3
 Summary: Utilities for working with dynamically loaded Django apps.
 Description-Content-Type: text/markdown
 
 # Airavata Django Portal Commons
 
 Utilities for working with dynamically loaded Django apps.
```

### Comparing `airavata-django-portal-commons-1.0.2/README.md` & `airavata-django-portal-commons-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/dynamic_apps/__init__.py` & `airavata-django-portal-commons-1.0.3/airavata_django_portal_commons/dynamic_apps/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,23 +9,21 @@
 logger = logging.getLogger(__name__)
 
 
 def load(installed_apps, entry_point_group="airavata.djangoapp"):
     for entry_point in entry_points(group=entry_point_group):
         custom_app_class = entry_point.load()
         custom_app_instance = custom_app_class(
-            entry_point.name, import_module(entry_point.module_name)
+            entry_point.name, import_module(entry_point.module)
         )
         CUSTOM_DJANGO_APPS.append(custom_app_instance)
         # Create path to AppConfig class (otherwise the ready() method doesn't get
         # called)
         logger.info(f"adding dynamic Django app {entry_point.name}")
-        installed_apps.append(
-            "{}.{}".format(entry_point.module_name, entry_point.attrs[0])
-        )
+        installed_apps.append("{}.{}".format(entry_point.module, entry_point.attr))
 
 
 def merge_setting_dict(default, custom_setting):
     # FIXME: only handles dict settings, doesn't handle lists
     if isinstance(custom_setting, dict):
         for k in custom_setting.keys():
             if k not in default:
```

### Comparing `airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/dynamic_apps/context_processors.py` & `airavata-django-portal-commons-1.0.3/airavata_django_portal_commons/dynamic_apps/context_processors.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/PKG-INFO` & `airavata-django-portal-commons-1.0.3/airavata_django_portal_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airavata-django-portal-commons
-Version: 1.0.2
+Version: 1.0.3
 Summary: Utilities for working with dynamically loaded Django apps.
 Description-Content-Type: text/markdown
 
 # Airavata Django Portal Commons
 
 Utilities for working with dynamically loaded Django apps.
```

### Comparing `airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/SOURCES.txt` & `airavata-django-portal-commons-1.0.3/airavata_django_portal_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

