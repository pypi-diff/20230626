# Comparing `tmp/django_bg_task-0.0.2.tar.gz` & `tmp/django_bg_task-0.0.3.tar.gz`

## Comparing `django_bg_task-0.0.2.tar` & `django_bg_task-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,27 @@
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/.isort.cfg
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    20828 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/.pylintrc
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/ignore-spelling-words.txt
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/manage.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/mypy.ini
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/requirements.txt
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/apps.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/common.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/constants.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/handler.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/models.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/serializers.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/services.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/settings.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/urls.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/views.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0001_initial.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0002_alter_task_status.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0003_remove_task_task_id.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0004_alter_task_id.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0005_rename_arguments_task_args_and_more.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0006_remove_task_exception_task_failed_reason_and_more.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0007_alter_task_created_at_alter_task_failed_reason_and_more.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/0008_remove_task_identifier_task_identifiers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/django_task/migrations/__init__.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/LICENSE
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/README.md
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 django_bg_task-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/.isort.cfg
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20827 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/.pylintrc
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/ignore-spelling-words.txt
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/manage.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/mypy.ini
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/apps.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/common.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/constants.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/handler.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/models.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/serializers.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/services.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/settings.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/urls.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/views.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/django_task/migrations/__init__.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/README.md
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 django_bg_task-0.0.3/PKG-INFO
```

### Comparing `django_bg_task-0.0.2/.pre-commit-config.yaml` & `django_bg_task-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.2/.pylintrc` & `django_bg_task-0.0.3/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 # (useful for modules/projects where namespaces are manipulated during runtime
 # and thus existing member attributes cannot be deduced by static analysis). It
 # supports qualified module names, as well as Unix pattern matching.
 ignored-modules=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
-init-hook='from pylint.config import find_pylintrc; import os; import sys; sys.path.append("."); sys.path.append("./task_manager"); sys.path.append("./venv/lib/python3.9/site-packages");'
+init-hook='from pylint.config import find_pylintrc; import os; import sys; sys.path.append("."); sys.path.append("./django_task"); sys.path.append("./venv/lib/python3.9/site-packages");'
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
 # number of processors available to use, and will cap the count on Windows to
 # avoid hangs.
 jobs=1
 
 # Control the amount of potential inferred values when inferring a single
```

### Comparing `django_bg_task-0.0.2/manage.py` & `django_bg_task-0.0.3/manage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!../venv/bin/python
 # -*- coding: utf-8 -*-
 # pylint: disable-all
 import os
 import sys
 
 if __name__ == "__main__":
-    os.environ.setdefault("DJANGO_SETTINGS_MODULE", "task_manager.settings")
+    os.environ.setdefault("DJANGO_SETTINGS_MODULE", "django_task.settings")
     try:
         from django.core.management import execute_from_command_line
     except ImportError as error:
         raise ImportError(
             "Couldn't import Django. Are you sure it's installed and "
             "available on your PYTHONPATH environment variable? Did you "
             "forget to activate a virtual environment?"
```

### Comparing `django_bg_task-0.0.2/.github/workflows/publish.yaml` & `django_bg_task-0.0.3/.github/workflows/publish.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 jobs:
   pypi-publish:
     name: Upload release to PyPI
     runs-on: ubuntu-latest
     environment:
       name: release
-      url: https://pypi.org/p/drf-misc
+      url: https://pypi.org/p/django-bg-task
     permissions:
       id-token: write # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
       - name: "Checkout Code"
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
```

### Comparing `django_bg_task-0.0.2/django_task/handler.py` & `django_bg_task-0.0.3/django_task/handler.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.2/django_task/models.py` & `django_bg_task-0.0.3/django_task/models.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.2/django_task/services.py` & `django_bg_task-0.0.3/django_task/services.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.2/django_task/settings.py` & `django_bg_task-0.0.3/django_task/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class AppSettings:
     def __init__(self):
         self.app_settings = getattr(settings, "DRF_MISC_SETTINGS", {})
 
     @property
     def SERVICE_NAME(self):
         """Control how many times a task will be attempted."""
-        return getattr(self.app_settings, "SERVICE_NAME", "task_manager")
+        return getattr(self.app_settings, "SERVICE_NAME", "django_task")
 
     @property
     def USE_SERVICE_CACHE(self):
         return getattr(self.app_settings, "USE_SERVICE_CACHE", False)
 
 
 app_settings = AppSettings()
```

### Comparing `django_bg_task-0.0.2/django_task/views.py` & `django_bg_task-0.0.3/django_task/views.py`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.2/.gitignore` & `django_bg_task-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.2/LICENSE` & `django_bg_task-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.2/README.md` & `django_bg_task-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django_bg_task-0.0.2/pyproject.toml` & `django_bg_task-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "django-bg-task"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Abhishek Sharma", email="abhishm20@gmail.com" },
 ]
 description = "A small Django DRF extension for managing background task with celery"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_bg_task-0.0.2/PKG-INFO` & `django_bg_task-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bg-task
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small Django DRF extension for managing background task with celery
 Project-URL: Homepage, https://github.com/abhishm20/django-task
 Project-URL: Bug Tracker, https://github.com/abhishm20/django-task/issues
 Author-email: Abhishek Sharma <abhishm20@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

