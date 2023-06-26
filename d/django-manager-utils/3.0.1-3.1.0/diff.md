# Comparing `tmp/django-manager-utils-3.0.1.tar.gz` & `tmp/django-manager-utils-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-manager-utils-3.0.1.tar", last modified: Tue Aug 23 03:01:42 2022, max compression
+gzip compressed data, was "django-manager-utils-3.1.0.tar", last modified: Mon Jun 26 21:27:39 2023, max compression
```

## Comparing `django-manager-utils-3.0.1.tar` & `django-manager-utils-3.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2022-08-23 03:01:42.852473 django-manager-utils-3.0.1/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2022-08-19 22:35:12.000000 django-manager-utils-3.0.1/LICENSE
--rw-rw-r--   0 wes       (1000) wes       (1000)       68 2022-08-19 22:50:28.000000 django-manager-utils-3.0.1/MANIFEST.in
--rw-rw-r--   0 wes       (1000) wes       (1000)     2445 2022-08-23 03:01:42.856474 django-manager-utils-3.0.1/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)      943 2022-08-19 22:35:12.000000 django-manager-utils-3.0.1/README.rst
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2022-08-23 03:01:42.852473 django-manager-utils-3.0.1/django_manager_utils.egg-info/
--rw-rw-r--   0 wes       (1000) wes       (1000)     2445 2022-08-23 03:01:42.000000 django-manager-utils-3.0.1/django_manager_utils.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)      592 2022-08-23 03:01:42.000000 django-manager-utils-3.0.1/django_manager_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2022-08-23 03:01:42.000000 django-manager-utils-3.0.1/django_manager_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       40 2022-08-23 03:01:42.000000 django-manager-utils-3.0.1/django_manager_utils.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       14 2022-08-23 03:01:42.000000 django-manager-utils-3.0.1/django_manager_utils.egg-info/top_level.txt
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2022-08-23 03:01:42.852473 django-manager-utils-3.0.1/manager_utils/
--rw-rw-r--   0 wes       (1000) wes       (1000)      326 2022-08-19 22:35:12.000000 django-manager-utils-3.0.1/manager_utils/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      142 2022-08-19 22:35:12.000000 django-manager-utils-3.0.1/manager_utils/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    31061 2022-08-23 03:01:21.000000 django-manager-utils-3.0.1/manager_utils/manager_utils.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2022-08-23 03:01:42.852473 django-manager-utils-3.0.1/manager_utils/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-08-19 22:35:12.000000 django-manager-utils-3.0.1/manager_utils/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    97585 2022-08-19 22:35:12.000000 django-manager-utils-3.0.1/manager_utils/tests/manager_utils_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2343 2022-08-19 22:35:12.000000 django-manager-utils-3.0.1/manager_utils/tests/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    11906 2022-08-19 22:35:12.000000 django-manager-utils-3.0.1/manager_utils/upsert2.py
--rw-rw-r--   0 wes       (1000) wes       (1000)       22 2022-08-23 03:01:21.000000 django-manager-utils-3.0.1/manager_utils/version.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2022-08-23 03:01:42.852473 django-manager-utils-3.0.1/requirements/
--rw-rw-r--   0 wes       (1000) wes       (1000)       31 2022-08-19 22:35:12.000000 django-manager-utils-3.0.1/requirements/docs.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)      126 2022-08-23 03:01:21.000000 django-manager-utils-3.0.1/requirements/requirements-testing.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       40 2022-08-23 03:01:21.000000 django-manager-utils-3.0.1/requirements/requirements.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)      293 2022-08-23 03:01:42.856474 django-manager-utils-3.0.1/setup.cfg
--rw-rw-r--   0 wes       (1000) wes       (1000)     2242 2022-08-23 03:01:21.000000 django-manager-utils-3.0.1/setup.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-26 21:27:39.353124 django-manager-utils-3.1.0/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2022-08-19 22:35:12.000000 django-manager-utils-3.1.0/LICENSE
+-rw-rw-r--   0 wes       (1000) wes       (1000)       68 2022-08-19 22:50:28.000000 django-manager-utils-3.1.0/MANIFEST.in
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2027 2023-06-26 21:27:39.353124 django-manager-utils-3.1.0/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)      943 2022-08-19 22:35:12.000000 django-manager-utils-3.1.0/README.rst
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-26 21:27:39.353124 django-manager-utils-3.1.0/django_manager_utils.egg-info/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2027 2023-06-26 21:27:39.000000 django-manager-utils-3.1.0/django_manager_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)      592 2023-06-26 21:27:39.000000 django-manager-utils-3.1.0/django_manager_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-26 21:27:39.000000 django-manager-utils-3.1.0/django_manager_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       40 2023-06-26 21:27:39.000000 django-manager-utils-3.1.0/django_manager_utils.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       14 2023-06-26 21:27:39.000000 django-manager-utils-3.1.0/django_manager_utils.egg-info/top_level.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-26 21:27:39.353124 django-manager-utils-3.1.0/manager_utils/
+-rw-rw-r--   0 wes       (1000) wes       (1000)      264 2023-06-26 21:27:07.000000 django-manager-utils-3.1.0/manager_utils/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      142 2022-08-19 22:35:12.000000 django-manager-utils-3.1.0/manager_utils/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    31061 2022-08-23 03:01:21.000000 django-manager-utils-3.1.0/manager_utils/manager_utils.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-26 21:27:39.353124 django-manager-utils-3.1.0/manager_utils/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-08-19 22:35:12.000000 django-manager-utils-3.1.0/manager_utils/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    97385 2023-06-26 21:27:07.000000 django-manager-utils-3.1.0/manager_utils/tests/manager_utils_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2343 2022-08-19 22:35:12.000000 django-manager-utils-3.1.0/manager_utils/tests/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    11906 2022-08-19 22:35:12.000000 django-manager-utils-3.1.0/manager_utils/upsert2.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-26 21:27:07.000000 django-manager-utils-3.1.0/manager_utils/version.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-26 21:27:39.353124 django-manager-utils-3.1.0/requirements/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       31 2022-08-19 22:35:12.000000 django-manager-utils-3.1.0/requirements/docs.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      116 2023-06-26 21:27:07.000000 django-manager-utils-3.1.0/requirements/requirements-testing.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       40 2023-06-26 21:27:07.000000 django-manager-utils-3.1.0/requirements/requirements.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      293 2023-06-26 21:27:39.353124 django-manager-utils-3.1.0/setup.cfg
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2117 2023-06-26 21:27:07.000000 django-manager-utils-3.1.0/setup.py
```

### Comparing `django-manager-utils-3.0.1/LICENSE` & `django-manager-utils-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-manager-utils-3.0.1/PKG-INFO` & `django-manager-utils-3.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,57 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: django-manager-utils
-Version: 3.0.1
+Version: 3.1.0
 Summary: Model manager utilities for Django
 Home-page: http://github.com/ambitioninc/django-manager-utils/
 Author: Wes Kendall
 Author-email: opensource@ambition.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ambitioninc/django-manager-utils/issues
 Project-URL: Changes, https://django-manager-utils.readthedocs.io/en/latest/release_notes.html
 Project-URL: Documentation, https://django-manager-utils.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/ambitioninc/django-manager-utils
-Description: .. image:: https://travis-ci.org/ambitioninc/django-manager-utils.png
-           :target: https://travis-ci.org/ambitioninc/django-manager-utils
-        
-        .. image:: https://img.shields.io/pypi/v/django-manager-utils.svg
-            :target: https://pypi.python.org/pypi/django-manager-utils/
-            :alt: Latest PyPI version
-        
-        .. image:: https://img.shields.io/pypi/dm/django-manager-utils.svg
-            :target: https://pypi.python.org/pypi/django-manager-utils/
-            :alt: Number of PyPI downloads
-        
-        django-manager-utils
-        ====================
-        Additional utilities for Django model managers.
-        
-        Installation
-        ------------
-        To install the latest release, type::
-        
-            pip install django-manager-utils
-        
-        To install the latest code directly from source, type::
-        
-            pip install git+git://github.com/ambitioninc/django-manager-utils.git
-        
-        Documentation
-        -------------
-        
-        Full documentation is available at http://django-manager-utils.readthedocs.org
-        
-        License
-        -------
-        MIT License (see LICENSE)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/ambitioninc/django-manager-utils.png
+   :target: https://travis-ci.org/ambitioninc/django-manager-utils
+
+.. image:: https://img.shields.io/pypi/v/django-manager-utils.svg
+    :target: https://pypi.python.org/pypi/django-manager-utils/
+    :alt: Latest PyPI version
+
+.. image:: https://img.shields.io/pypi/dm/django-manager-utils.svg
+    :target: https://pypi.python.org/pypi/django-manager-utils/
+    :alt: Number of PyPI downloads
+
+django-manager-utils
+====================
+Additional utilities for Django model managers.
+
+Installation
+------------
+To install the latest release, type::
+
+    pip install django-manager-utils
+
+To install the latest code directly from source, type::
+
+    pip install git+git://github.com/ambitioninc/django-manager-utils.git
+
+Documentation
+-------------
+
+Full documentation is available at http://django-manager-utils.readthedocs.org
+
+License
+-------
+MIT License (see LICENSE)
```

### Comparing `django-manager-utils-3.0.1/README.rst` & `django-manager-utils-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-manager-utils-3.0.1/django_manager_utils.egg-info/PKG-INFO` & `django-manager-utils-3.1.0/django_manager_utils.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,57 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: django-manager-utils
-Version: 3.0.1
+Version: 3.1.0
 Summary: Model manager utilities for Django
 Home-page: http://github.com/ambitioninc/django-manager-utils/
 Author: Wes Kendall
 Author-email: opensource@ambition.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ambitioninc/django-manager-utils/issues
 Project-URL: Changes, https://django-manager-utils.readthedocs.io/en/latest/release_notes.html
 Project-URL: Documentation, https://django-manager-utils.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/ambitioninc/django-manager-utils
-Description: .. image:: https://travis-ci.org/ambitioninc/django-manager-utils.png
-           :target: https://travis-ci.org/ambitioninc/django-manager-utils
-        
-        .. image:: https://img.shields.io/pypi/v/django-manager-utils.svg
-            :target: https://pypi.python.org/pypi/django-manager-utils/
-            :alt: Latest PyPI version
-        
-        .. image:: https://img.shields.io/pypi/dm/django-manager-utils.svg
-            :target: https://pypi.python.org/pypi/django-manager-utils/
-            :alt: Number of PyPI downloads
-        
-        django-manager-utils
-        ====================
-        Additional utilities for Django model managers.
-        
-        Installation
-        ------------
-        To install the latest release, type::
-        
-            pip install django-manager-utils
-        
-        To install the latest code directly from source, type::
-        
-            pip install git+git://github.com/ambitioninc/django-manager-utils.git
-        
-        Documentation
-        -------------
-        
-        Full documentation is available at http://django-manager-utils.readthedocs.org
-        
-        License
-        -------
-        MIT License (see LICENSE)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/ambitioninc/django-manager-utils.png
+   :target: https://travis-ci.org/ambitioninc/django-manager-utils
+
+.. image:: https://img.shields.io/pypi/v/django-manager-utils.svg
+    :target: https://pypi.python.org/pypi/django-manager-utils/
+    :alt: Latest PyPI version
+
+.. image:: https://img.shields.io/pypi/dm/django-manager-utils.svg
+    :target: https://pypi.python.org/pypi/django-manager-utils/
+    :alt: Number of PyPI downloads
+
+django-manager-utils
+====================
+Additional utilities for Django model managers.
+
+Installation
+------------
+To install the latest release, type::
+
+    pip install django-manager-utils
+
+To install the latest code directly from source, type::
+
+    pip install git+git://github.com/ambitioninc/django-manager-utils.git
+
+Documentation
+-------------
+
+Full documentation is available at http://django-manager-utils.readthedocs.org
+
+License
+-------
+MIT License (see LICENSE)
```

### Comparing `django-manager-utils-3.0.1/django_manager_utils.egg-info/SOURCES.txt` & `django-manager-utils-3.1.0/django_manager_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-manager-utils-3.0.1/manager_utils/manager_utils.py` & `django-manager-utils-3.1.0/manager_utils/manager_utils.py`

 * *Files identical despite different names*

### Comparing `django-manager-utils-3.0.1/manager_utils/tests/manager_utils_tests.py` & `django-manager-utils-3.1.0/manager_utils/tests/manager_utils_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime as dt
 
 from django.test import TestCase
 from django_dynamic_fixture import G
 import freezegun
 from manager_utils import post_bulk_operation
 from manager_utils.manager_utils import _get_prepped_model_field
-from mock import patch
+from unittest.mock import patch
 from parameterized import parameterized
 from pytz import timezone
 
 from manager_utils.tests import models
 
 
 class TestGetPreppedModelField(TestCase):
@@ -33,36 +33,36 @@
         extant_obj3 = G(models.TestPkChar, my_key='3', char_field='1')
 
         models.TestPkChar.objects.sync([
             models.TestPkChar(my_key='3', char_field='2'), models.TestPkChar(my_key='4', char_field='2'),
             models.TestPkChar(my_key='5', char_field='2')
         ], ['my_key'], ['char_field'], native=native)
 
-        self.assertEquals(models.TestPkChar.objects.count(), 3)
+        self.assertEqual(models.TestPkChar.objects.count(), 3)
         self.assertTrue(models.TestPkChar.objects.filter(my_key='3').exists())
         self.assertTrue(models.TestPkChar.objects.filter(my_key='4').exists())
         self.assertTrue(models.TestPkChar.objects.filter(my_key='5').exists())
 
         with self.assertRaises(models.TestPkChar.DoesNotExist):
             models.TestPkChar.objects.get(pk=extant_obj1.pk)
         with self.assertRaises(models.TestPkChar.DoesNotExist):
             models.TestPkChar.objects.get(pk=extant_obj2.pk)
         test_model = models.TestPkChar.objects.get(pk=extant_obj3.pk)
-        self.assertEquals(test_model.char_field, '2')
+        self.assertEqual(test_model.char_field, '2')
 
     @parameterized.expand([(True,), (False,)])
     def test_no_existing_objs(self, native):
         """
         Tests when there are no existing objects before the sync.
         """
         models.TestModel.objects.sync([
             models.TestModel(int_field=1), models.TestModel(int_field=3),
             models.TestModel(int_field=4)
         ], ['int_field'], ['float_field'], native=native)
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         self.assertTrue(models.TestModel.objects.filter(int_field=1).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=3).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=4).exists())
 
     @parameterized.expand([(True,), (False,)])
     def test_existing_objs_all_deleted(self, native):
         """
@@ -72,15 +72,15 @@
         extant_obj2 = G(models.TestModel, int_field=2)
         extant_obj3 = G(models.TestModel, int_field=3)
 
         models.TestModel.objects.sync([
             models.TestModel(int_field=4), models.TestModel(int_field=5), models.TestModel(int_field=6)
         ], ['int_field'], ['float_field'], native=native)
 
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         self.assertTrue(models.TestModel.objects.filter(int_field=4).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=5).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=6).exists())
 
         with self.assertRaises(models.TestModel.DoesNotExist):
             models.TestModel.objects.get(id=extant_obj1.id)
         with self.assertRaises(models.TestModel.DoesNotExist):
@@ -95,15 +95,15 @@
         """
         extant_obj1 = G(models.TestModel, int_field=1)
         extant_obj2 = G(models.TestModel, int_field=2)
         extant_obj3 = G(models.TestModel, int_field=3)
 
         models.TestModel.objects.sync([], ['int_field'], ['float_field'], native=native)
 
-        self.assertEquals(models.TestModel.objects.count(), 0)
+        self.assertEqual(models.TestModel.objects.count(), 0)
         with self.assertRaises(models.TestModel.DoesNotExist):
             models.TestModel.objects.get(id=extant_obj1.id)
         with self.assertRaises(models.TestModel.DoesNotExist):
             models.TestModel.objects.get(id=extant_obj2.id)
         with self.assertRaises(models.TestModel.DoesNotExist):
             models.TestModel.objects.get(id=extant_obj3.id)
 
@@ -117,25 +117,25 @@
         extant_obj3 = G(models.TestModel, int_field=3, float_field=1)
 
         models.TestModel.objects.sync([
             models.TestModel(int_field=3, float_field=2), models.TestModel(int_field=4, float_field=2),
             models.TestModel(int_field=5, float_field=2)
         ], ['int_field'], ['float_field'], native=native)
 
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         self.assertTrue(models.TestModel.objects.filter(int_field=3).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=4).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=5).exists())
 
         with self.assertRaises(models.TestModel.DoesNotExist):
             models.TestModel.objects.get(id=extant_obj1.id)
         with self.assertRaises(models.TestModel.DoesNotExist):
             models.TestModel.objects.get(id=extant_obj2.id)
         test_model = models.TestModel.objects.get(id=extant_obj3.id)
-        self.assertEquals(test_model.int_field, 3)
+        self.assertEqual(test_model.int_field, 3)
 
     @parameterized.expand([(True,), (False,)])
     def test_existing_objs_some_deleted_w_queryset(self, native):
         """
         Tests when some existing objects will be deleted on a queryset
         """
         extant_obj0 = G(models.TestModel, int_field=0, float_field=1)
@@ -145,30 +145,30 @@
         extant_obj4 = G(models.TestModel, int_field=4, float_field=0)
 
         models.TestModel.objects.filter(int_field__lt=4).sync([
             models.TestModel(int_field=1, float_field=2), models.TestModel(int_field=2, float_field=2),
             models.TestModel(int_field=3, float_field=2)
         ], ['int_field'], ['float_field'], native=native)
 
-        self.assertEquals(models.TestModel.objects.count(), 4)
+        self.assertEqual(models.TestModel.objects.count(), 4)
         self.assertTrue(models.TestModel.objects.filter(int_field=1).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=2).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=3).exists())
 
         with self.assertRaises(models.TestModel.DoesNotExist):
             models.TestModel.objects.get(id=extant_obj0.id)
 
         test_model = models.TestModel.objects.get(id=extant_obj1.id)
-        self.assertEquals(test_model.float_field, 2)
+        self.assertEqual(test_model.float_field, 2)
         test_model = models.TestModel.objects.get(id=extant_obj2.id)
-        self.assertEquals(test_model.float_field, 2)
+        self.assertEqual(test_model.float_field, 2)
         test_model = models.TestModel.objects.get(id=extant_obj3.id)
-        self.assertEquals(test_model.float_field, 2)
+        self.assertEqual(test_model.float_field, 2)
         test_model = models.TestModel.objects.get(id=extant_obj4.id)
-        self.assertEquals(test_model.float_field, 0)
+        self.assertEqual(test_model.float_field, 0)
 
 
 class Sync2Test(TestCase):
     """
     Tests the sync2 function.
     """
     def test_w_char_pk(self):
@@ -180,35 +180,35 @@
         extant_obj3 = G(models.TestPkChar, my_key='3', char_field='1')
 
         models.TestPkChar.objects.sync2([
             models.TestPkChar(my_key='3', char_field='2'), models.TestPkChar(my_key='4', char_field='2'),
             models.TestPkChar(my_key='5', char_field='2')
         ], ['my_key'], ['char_field'])
 
-        self.assertEquals(models.TestPkChar.objects.count(), 3)
+        self.assertEqual(models.TestPkChar.objects.count(), 3)
         self.assertTrue(models.TestPkChar.objects.filter(my_key='3').exists())
         self.assertTrue(models.TestPkChar.objects.filter(my_key='4').exists())
         self.assertTrue(models.TestPkChar.objects.filter(my_key='5').exists())
 
         with self.assertRaises(models.TestPkChar.DoesNotExist):
             models.TestPkChar.objects.get(pk=extant_obj1.pk)
         with self.assertRaises(models.TestPkChar.DoesNotExist):
             models.TestPkChar.objects.get(pk=extant_obj2.pk)
         test_model = models.TestPkChar.objects.get(pk=extant_obj3.pk)
-        self.assertEquals(test_model.char_field, '2')
+        self.assertEqual(test_model.char_field, '2')
 
     def test_no_existing_objs(self):
         """
         Tests when there are no existing objects before the sync.
         """
         models.TestModel.objects.sync([
             models.TestModel(int_field=1), models.TestModel(int_field=3),
             models.TestModel(int_field=4)
         ], ['int_field'], ['float_field'])
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         self.assertTrue(models.TestModel.objects.filter(int_field=1).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=3).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=4).exists())
 
     def test_existing_objs_all_deleted(self):
         """
         Tests when there are existing objects that will all be deleted.
@@ -217,15 +217,15 @@
         extant_obj2 = G(models.TestModel, int_field=2)
         extant_obj3 = G(models.TestModel, int_field=3)
 
         models.TestModel.objects.sync2([
             models.TestModel(int_field=4), models.TestModel(int_field=5), models.TestModel(int_field=6)
         ], ['int_field'], ['float_field'])
 
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         self.assertTrue(models.TestModel.objects.filter(int_field=4).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=5).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=6).exists())
 
         with self.assertRaises(models.TestModel.DoesNotExist):
             models.TestModel.objects.get(id=extant_obj1.id)
         with self.assertRaises(models.TestModel.DoesNotExist):
@@ -239,15 +239,15 @@
         """
         extant_obj1 = G(models.TestModel, int_field=1)
         extant_obj2 = G(models.TestModel, int_field=2)
         extant_obj3 = G(models.TestModel, int_field=3)
 
         models.TestModel.objects.sync2([], ['int_field'], ['float_field'])
 
-        self.assertEquals(models.TestModel.objects.count(), 0)
+        self.assertEqual(models.TestModel.objects.count(), 0)
         with self.assertRaises(models.TestModel.DoesNotExist):
             models.TestModel.objects.get(id=extant_obj1.id)
         with self.assertRaises(models.TestModel.DoesNotExist):
             models.TestModel.objects.get(id=extant_obj2.id)
         with self.assertRaises(models.TestModel.DoesNotExist):
             models.TestModel.objects.get(id=extant_obj3.id)
 
@@ -260,25 +260,25 @@
         extant_obj3 = G(models.TestModel, int_field=3, float_field=1)
 
         models.TestModel.objects.sync2([
             models.TestModel(int_field=3, float_field=2), models.TestModel(int_field=4, float_field=2),
             models.TestModel(int_field=5, float_field=2)
         ], ['int_field'], ['float_field'])
 
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         self.assertTrue(models.TestModel.objects.filter(int_field=3).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=4).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=5).exists())
 
         with self.assertRaises(models.TestModel.DoesNotExist):
             models.TestModel.objects.get(id=extant_obj1.id)
         with self.assertRaises(models.TestModel.DoesNotExist):
             models.TestModel.objects.get(id=extant_obj2.id)
         test_model = models.TestModel.objects.get(id=extant_obj3.id)
-        self.assertEquals(test_model.int_field, 3)
+        self.assertEqual(test_model.int_field, 3)
 
     def test_existing_objs_some_deleted_w_queryset(self):
         """
         Tests when some existing objects will be deleted on a queryset
         """
         extant_obj0 = G(models.TestModel, int_field=0, float_field=1)
         extant_obj1 = G(models.TestModel, int_field=1, float_field=1)
@@ -287,94 +287,94 @@
         extant_obj4 = G(models.TestModel, int_field=4, float_field=0)
 
         models.TestModel.objects.filter(int_field__lt=4).sync2([
             models.TestModel(int_field=1, float_field=2), models.TestModel(int_field=2, float_field=2),
             models.TestModel(int_field=3, float_field=2)
         ], ['int_field'], ['float_field'])
 
-        self.assertEquals(models.TestModel.objects.count(), 4)
+        self.assertEqual(models.TestModel.objects.count(), 4)
         self.assertTrue(models.TestModel.objects.filter(int_field=1).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=2).exists())
         self.assertTrue(models.TestModel.objects.filter(int_field=3).exists())
 
         with self.assertRaises(models.TestModel.DoesNotExist):
             models.TestModel.objects.get(id=extant_obj0.id)
 
         test_model = models.TestModel.objects.get(id=extant_obj1.id)
-        self.assertEquals(test_model.float_field, 2)
+        self.assertEqual(test_model.float_field, 2)
         test_model = models.TestModel.objects.get(id=extant_obj2.id)
-        self.assertEquals(test_model.float_field, 2)
+        self.assertEqual(test_model.float_field, 2)
         test_model = models.TestModel.objects.get(id=extant_obj3.id)
-        self.assertEquals(test_model.float_field, 2)
+        self.assertEqual(test_model.float_field, 2)
         test_model = models.TestModel.objects.get(id=extant_obj4.id)
-        self.assertEquals(test_model.float_field, 0)
+        self.assertEqual(test_model.float_field, 0)
 
     def test_existing_objs_some_deleted_wo_update(self):
         """
         Tests when some existing objects will be deleted on a queryset. Run syncing
         with no update fields and verify they are untouched in the sync
         """
         objs = [G(models.TestModel, int_field=i, float_field=i) for i in range(5)]
 
         results = models.TestModel.objects.filter(int_field__lt=4).sync2([
             models.TestModel(int_field=1, float_field=2), models.TestModel(int_field=2, float_field=2),
             models.TestModel(int_field=3, float_field=2)
         ], ['int_field'], [], returning=True)
 
-        self.assertEquals(len(list(results)), 4)
-        self.assertEquals(len(list(results.deleted)), 1)
-        self.assertEquals(len(list(results.untouched)), 3)
-        self.assertEquals(list(results.deleted)[0].id, objs[0].id)
+        self.assertEqual(len(list(results)), 4)
+        self.assertEqual(len(list(results.deleted)), 1)
+        self.assertEqual(len(list(results.untouched)), 3)
+        self.assertEqual(list(results.deleted)[0].id, objs[0].id)
 
     def test_existing_objs_some_deleted_some_updated(self):
         """
         Tests when some existing objects will be deleted on a queryset. Run syncing
         with some update fields.
         """
         objs = [G(models.TestModel, int_field=i, float_field=i) for i in range(5)]
 
         results = models.TestModel.objects.filter(int_field__lt=4).sync2([
             models.TestModel(int_field=1, float_field=2), models.TestModel(int_field=2, float_field=2),
             models.TestModel(int_field=3, float_field=2)
         ], ['int_field'], ['float_field'], returning=True, ignore_duplicate_updates=True)
 
-        self.assertEquals(len(list(results)), 4)
-        self.assertEquals(len(list(results.deleted)), 1)
-        self.assertEquals(len(list(results.updated)), 2)
-        self.assertEquals(len(list(results.untouched)), 1)
-        self.assertEquals(list(results.deleted)[0].id, objs[0].id)
+        self.assertEqual(len(list(results)), 4)
+        self.assertEqual(len(list(results.deleted)), 1)
+        self.assertEqual(len(list(results.updated)), 2)
+        self.assertEqual(len(list(results.untouched)), 1)
+        self.assertEqual(list(results.deleted)[0].id, objs[0].id)
 
 
 class BulkUpsertTest(TestCase):
     """
     Tests the bulk_upsert function.
     """
     def test_return_upserts_none(self):
         """
         Tests the return_upserts flag on bulk upserts when there is no data.
         """
         return_values = models.TestModel.objects.bulk_upsert([], ['float_field'], ['float_field'], return_upserts=True)
-        self.assertEquals(return_values, [])
+        self.assertEqual(return_values, [])
 
     def test_return_upserts_distinct_none(self):
         """
         Tests the return_upserts_distinct flag on bulk upserts when there is no data.
         """
         return_values = models.TestModel.objects.bulk_upsert(
             [], ['float_field'], ['float_field'], return_upserts_distinct=True)
-        self.assertEquals(return_values, ([], []))
+        self.assertEqual(return_values, ([], []))
 
     def test_return_upserts_none_native(self):
         """
         Tests the return_upserts flag on bulk upserts when there is no data.
         """
         return_values = models.TestModel.objects.bulk_upsert(
             [], ['float_field'], ['float_field'], return_upserts=True, native=True
         )
-        self.assertEquals(return_values, [])
+        self.assertEqual(return_values, [])
 
     def test_return_upserts_distinct_none_native(self):
         """
         verifies that return_upserts_distinct flag with native is not supported
         """
         with self.assertRaises(NotImplementedError):
             models.TestModel.objects.bulk_upsert(
@@ -393,33 +393,33 @@
             ],
             ['int_field', 'char_field'],
             ['float_field'],
             return_upserts=True
         )
 
         # Assert that we properly returned the models
-        self.assertEquals(len(return_values), 3)
+        self.assertEqual(len(return_values), 3)
         for test_model, expected_int in zip(sorted(return_values, key=lambda k: k.int_field), [1, 3, 4]):
-            self.assertEquals(test_model.int_field, expected_int)
+            self.assertEqual(test_model.int_field, expected_int)
             self.assertIsNotNone(test_model.id)
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
 
         # Run additional upserts
         return_values = models.TestModel.objects.bulk_upsert(
             [
                 models.TestModel(int_field=1, char_field='1', float_field=10),
                 models.TestModel(int_field=3, char_field='3'),
                 models.TestModel(int_field=4, char_field='4'),
                 models.TestModel(int_field=5, char_field='5', float_field=50),
             ],
             ['int_field', 'char_field'],
             ['float_field'],
             return_upserts=True
         )
-        self.assertEquals(len(return_values), 4)
+        self.assertEqual(len(return_values), 4)
         self.assertEqual(
             [
                 [1, '1', 10],
                 [3, '3', None],
                 [4, '4', None],
                 [5, '5', 50],
             ],
@@ -441,39 +441,39 @@
             ],
             ['int_field', 'char_field'],
             ['float_field'],
             return_upserts=True,
             native=True
         )
 
-        self.assertEquals(len(return_values), 3)
+        self.assertEqual(len(return_values), 3)
         for test_model, expected_int in zip(sorted(return_values, key=lambda k: k.int_field), [1, 3, 4]):
-            self.assertEquals(test_model.int_field, expected_int)
+            self.assertEqual(test_model.int_field, expected_int)
             self.assertIsNotNone(test_model.id)
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
 
     def test_return_created_updated_values(self):
         """
         Tests returning values when the items are either updated or created.
         """
         # Create an item that will be updated
         G(models.TestModel, int_field=2, float_field=1.0)
         return_values = models.TestModel.objects.bulk_upsert(
             [
                 models.TestModel(int_field=1, float_field=3.0), models.TestModel(int_field=2.0, float_field=3.0),
                 models.TestModel(int_field=3, float_field=3.0), models.TestModel(int_field=4, float_field=3.0)
             ],
             ['int_field'], ['float_field'], return_upserts=True)
 
-        self.assertEquals(len(return_values), 4)
+        self.assertEqual(len(return_values), 4)
         for test_model, expected_int in zip(sorted(return_values, key=lambda k: k.int_field), [1, 2, 3, 4]):
-            self.assertEquals(test_model.int_field, expected_int)
-            self.assertAlmostEquals(test_model.float_field, 3.0)
+            self.assertEqual(test_model.int_field, expected_int)
+            self.assertAlmostEqual(test_model.float_field, 3.0)
             self.assertIsNotNone(test_model.id)
-        self.assertEquals(models.TestModel.objects.count(), 4)
+        self.assertEqual(models.TestModel.objects.count(), 4)
 
     def test_return_created_updated_values_native(self):
         """
         Tests returning values when the items are either updated or created.
         """
         # Create an item that will be updated
         G(models.TestModel, int_field=2, float_field=1.0)
@@ -487,20 +487,20 @@
             model_objects,
             ['int_field'],
             ['float_field'],
             return_upserts=True,
             native=True
         )
 
-        self.assertEquals(len(return_values), 4)
+        self.assertEqual(len(return_values), 4)
         for test_model, expected_int in zip(sorted(return_values, key=lambda k: k.int_field), [1, 2, 3, 4]):
-            self.assertEquals(test_model.int_field, expected_int)
-            self.assertAlmostEquals(test_model.float_field, 3.0)
+            self.assertEqual(test_model.int_field, expected_int)
+            self.assertAlmostEqual(test_model.float_field, 3.0)
             self.assertIsNotNone(test_model.id)
-        self.assertEquals(models.TestModel.objects.count(), 4)
+        self.assertEqual(models.TestModel.objects.count(), 4)
 
     def test_return_created_updated_values_distinct(self):
         """
         Tests returning distinct sets of values when the items are either updated or created.
         """
         # Create an item that will be updated
         G(models.TestModel, int_field=2, float_field=1.0)
@@ -508,22 +508,22 @@
             models.TestModel(int_field=1, float_field=3.0),
             models.TestModel(int_field=2.0, float_field=3.0),
             models.TestModel(int_field=3, float_field=3.0),
             models.TestModel(int_field=4, float_field=3.0)
         ]
         updated, created = models.TestModel.objects.bulk_upsert(
             model_objects, ['int_field'], ['float_field'], return_upserts_distinct=True)
-        self.assertEquals(
+        self.assertEqual(
             [(2, 3.0)],
             [
                 (obj.int_field, obj.float_field)
                 for obj in sorted(updated, key=lambda k: k.int_field)
             ]
         )
-        self.assertEquals(
+        self.assertEqual(
             [(1, 3.0), (3, 3.0), (4, 3.0)],
             [
                 (obj.int_field, obj.float_field)
                 for obj in sorted(created, key=lambda k: k.int_field)
             ]
         )
 
@@ -544,17 +544,17 @@
         G(models.TestModel, int_field=1)
         G(models.TestModel, int_field=2)
         # Perform a bulk_upsert with one new model
         models.TestModel.objects.bulk_upsert([
             models.TestModel(int_field=1), models.TestModel(int_field=2), models.TestModel(int_field=3)
         ], ['int_field'])
         # Three objects should now exist
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for test_model, expected_int_value in zip(models.TestModel.objects.order_by('int_field'), [1, 2, 3]):
-            self.assertEquals(test_model.int_field, expected_int_value)
+            self.assertEqual(test_model.int_field, expected_int_value)
 
     def test_wo_update_fields_native(self):
         """
         Tests bulk_upsert with no update fields. This function in turn should just do a bulk create for any
         models that do not already exist.
         """
         # Create models that already exist
@@ -565,35 +565,35 @@
             [
                 models.TestModel(int_field=1), models.TestModel(int_field=2), models.TestModel(int_field=3)
             ],
             ['int_field'],
             native=True
         )
         # Three objects should now exist
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for test_model, expected_int_value in zip(models.TestModel.objects.order_by('int_field'), [1, 2, 3]):
-            self.assertEquals(test_model.int_field, expected_int_value)
+            self.assertEqual(test_model.int_field, expected_int_value)
 
     def test_w_blank_arguments(self):
         """
         Tests using required arguments and using blank arguments for everything else.
         """
         models.TestModel.objects.bulk_upsert([], ['field'], ['field'])
-        self.assertEquals(models.TestModel.objects.count(), 0)
+        self.assertEqual(models.TestModel.objects.count(), 0)
 
         # Test native
         models.TestModel.objects.bulk_upsert([], ['field'], ['field'], native=True)
-        self.assertEquals(models.TestModel.objects.count(), 0)
+        self.assertEqual(models.TestModel.objects.count(), 0)
 
     def test_w_blank_arguments_native(self):
         """
         Tests using required arguments and using blank arguments for everything else.
         """
         models.TestModel.objects.bulk_upsert([], ['field'], ['field'], native=True)
-        self.assertEquals(models.TestModel.objects.count(), 0)
+        self.assertEqual(models.TestModel.objects.count(), 0)
 
     def test_no_updates(self):
         """
         Tests the case when no updates were previously stored (i.e objects are only created)
         """
         models.TestModel.objects.bulk_upsert([
             models.TestModel(int_field=0, char_field='0', float_field=0),
@@ -634,15 +634,15 @@
         models.TestModel.objects.bulk_upsert([
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=1, char_field='1', float_field=1),
             models.TestModel(int_field=2, char_field='2', float_field=2),
         ], ['int_field'], ['char_field', 'float_field'])
 
         # Verify that the fields were updated
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, str(i))
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_all_updates_unique_int_field_native(self):
         """
@@ -657,15 +657,15 @@
         models.TestModel.objects.bulk_upsert([
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=1, char_field='1', float_field=1),
             models.TestModel(int_field=2, char_field='2', float_field=2),
         ], ['int_field'], ['char_field', 'float_field'], native=True)
 
         # Verify that the fields were updated
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, str(i))
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_all_updates_unique_int_field_update_float_field(self):
         """
@@ -680,15 +680,15 @@
         models.TestModel.objects.bulk_upsert([
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=1, char_field='1', float_field=1),
             models.TestModel(int_field=2, char_field='2', float_field=2),
         ], ['int_field'], update_fields=['float_field'])
 
         # Verify that the float field was updated
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, '-1')
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_all_updates_unique_int_field_update_float_field_native(self):
         """
@@ -703,15 +703,15 @@
         models.TestModel.objects.bulk_upsert([
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=1, char_field='1', float_field=1),
             models.TestModel(int_field=2, char_field='2', float_field=2),
         ], ['int_field'], update_fields=['float_field'], native=True)
 
         # Verify that the float field was updated
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, '-1')
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_some_updates_unique_int_field_update_float_field(self):
         """
@@ -727,15 +727,15 @@
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=1, char_field='1', float_field=1),
             models.TestModel(int_field=2, char_field='2', float_field=2),
         ], ['int_field'], ['float_field'])
 
         # Verify that the float field was updated for the first two models and the char field was not updated for
         # the first two. The char field, however, should be '2' for the third model since it was created
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, '-1' if i < 2 else '2')
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_some_updates_unique_int_field_update_float_field_native(self):
         """
@@ -751,15 +751,15 @@
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=1, char_field='1', float_field=1),
             models.TestModel(int_field=2, char_field='2', float_field=2),
         ], ['int_field'], ['float_field'], native=True)
 
         # Verify that the float field was updated for the first two models and the char field was not updated for
         # the first two. The char field, however, should be '2' for the third model since it was created
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, '-1' if i < 2 else '2')
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_some_updates_unique_timezone_field_update_float_field(self):
         """
@@ -776,24 +776,24 @@
             models.TestModel(time_zone=timezone('US/Central'), char_field='1', float_field=1),
             models.TestModel(time_zone=timezone('UTC'), char_field='2', float_field=2),
         ], ['time_zone'], ['float_field'])
 
         # Verify that the float field was updated for the first two models and the char field was not updated for
         # the first two. The char field, however, should be '2' for the third model since it was created
         m1 = models.TestModel.objects.get(time_zone=timezone('US/Eastern'))
-        self.assertEquals(m1.char_field, '-1')
-        self.assertAlmostEquals(m1.float_field, 0)
+        self.assertEqual(m1.char_field, '-1')
+        self.assertAlmostEqual(m1.float_field, 0)
 
         m2 = models.TestModel.objects.get(time_zone=timezone('US/Central'))
-        self.assertEquals(m2.char_field, '-1')
-        self.assertAlmostEquals(m2.float_field, 1)
+        self.assertEqual(m2.char_field, '-1')
+        self.assertAlmostEqual(m2.float_field, 1)
 
         m3 = models.TestModel.objects.get(time_zone=timezone('UTC'))
-        self.assertEquals(m3.char_field, '2')
-        self.assertAlmostEquals(m3.float_field, 2)
+        self.assertEqual(m3.char_field, '2')
+        self.assertAlmostEqual(m3.float_field, 2)
 
     def test_some_updates_unique_int_char_field_update_float_field(self):
         """
         Tests the case when some updates were previously stored and the int and char fields are used as a uniqueness
         constraint. Only updates the float field.
         """
         # Create previously stored test models with a unique int and char field
@@ -805,15 +805,15 @@
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=1, char_field='1', float_field=1),
             models.TestModel(int_field=2, char_field='2', float_field=2),
         ], ['int_field', 'char_field'], ['float_field'])
 
         # Verify that the float field was updated for the first two models and the char field was not updated for
         # the first two. The char field, however, should be '2' for the third model since it was created
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, str(i))
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_some_updates_unique_int_char_field_update_float_field_native(self):
         """
@@ -829,15 +829,15 @@
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=1, char_field='1', float_field=1),
             models.TestModel(int_field=2, char_field='2', float_field=2),
         ], ['int_field', 'char_field'], ['float_field'], native=True)
 
         # Verify that the float field was updated for the first two models and the char field was not updated for
         # the first two. The char field, however, should be '2' for the third model since it was created
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, str(i))
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_no_updates_unique_int_char_field(self):
         """
@@ -852,21 +852,21 @@
         models.TestModel.objects.bulk_upsert([
             models.TestModel(int_field=3, char_field='0', float_field=0),
             models.TestModel(int_field=4, char_field='1', float_field=1),
             models.TestModel(int_field=5, char_field='2', float_field=2),
         ], ['int_field', 'char_field'], ['float_field'])
 
         # Verify that no updates occured
-        self.assertEquals(models.TestModel.objects.count(), 6)
-        self.assertEquals(models.TestModel.objects.filter(char_field='-1').count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 6)
+        self.assertEqual(models.TestModel.objects.filter(char_field='-1').count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.filter(char_field='-1').order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, '-1')
             self.assertAlmostEqual(model_obj.float_field, -1)
-        self.assertEquals(models.TestModel.objects.exclude(char_field='-1').count(), 3)
+        self.assertEqual(models.TestModel.objects.exclude(char_field='-1').count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.exclude(char_field='-1').order_by('int_field')):
             self.assertEqual(model_obj.int_field, i + 3)
             self.assertEqual(model_obj.char_field, str(i))
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_no_updates_unique_int_char_field_native(self):
         """
@@ -881,21 +881,21 @@
         models.TestModel.objects.bulk_upsert([
             models.TestModel(int_field=3, char_field='0', float_field=0),
             models.TestModel(int_field=4, char_field='1', float_field=1),
             models.TestModel(int_field=5, char_field='2', float_field=2),
         ], ['int_field', 'char_field'], ['float_field'], native=True)
 
         # Verify that no updates occured
-        self.assertEquals(models.TestModel.objects.count(), 6)
-        self.assertEquals(models.TestModel.objects.filter(char_field='-1').count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 6)
+        self.assertEqual(models.TestModel.objects.filter(char_field='-1').count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.filter(char_field='-1').order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, '-1')
             self.assertAlmostEqual(model_obj.float_field, -1)
-        self.assertEquals(models.TestModel.objects.exclude(char_field='-1').count(), 3)
+        self.assertEqual(models.TestModel.objects.exclude(char_field='-1').count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.exclude(char_field='-1').order_by('int_field')):
             self.assertEqual(model_obj.int_field, i + 3)
             self.assertEqual(model_obj.char_field, str(i))
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_some_updates_unique_int_char_field_queryset(self):
         """
@@ -909,16 +909,16 @@
         models.TestModel.objects.filter(int_field=0).bulk_upsert([
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=4, char_field='1', float_field=1),
             models.TestModel(int_field=5, char_field='2', float_field=2),
         ], ['int_field'], ['float_field'])
 
         # Verify that two new objecs were created
-        self.assertEquals(models.TestModel.objects.count(), 5)
-        self.assertEquals(models.TestModel.objects.filter(char_field='-1').count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 5)
+        self.assertEqual(models.TestModel.objects.filter(char_field='-1').count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.filter(char_field='-1').order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, '-1')
 
     def test_some_updates_unique_int_char_field_queryset_native(self):
         """
         Tests the case when some updates were previously stored and a queryset is used on the bulk upsert.
@@ -931,71 +931,71 @@
         models.TestModel.objects.filter(int_field=0).bulk_upsert([
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=4, char_field='1', float_field=1),
             models.TestModel(int_field=5, char_field='2', float_field=2),
         ], ['int_field'], ['float_field'], native=True)
 
         # Verify that two new objecs were created
-        self.assertEquals(models.TestModel.objects.count(), 5)
-        self.assertEquals(models.TestModel.objects.filter(char_field='-1').count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 5)
+        self.assertEqual(models.TestModel.objects.filter(char_field='-1').count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.filter(char_field='-1').order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, '-1')
 
 
 class BulkUpsert2Test(TestCase):
     """
     Tests the bulk_upsert2 function.
     """
     def test_return_upserts_none(self):
         """
         Tests the return_upserts flag on bulk upserts when there is no data.
         """
         return_values = models.TestModel.objects.bulk_upsert2([], ['float_field'], ['float_field'], returning=True)
-        self.assertEquals(return_values, [])
+        self.assertEqual(return_values, [])
 
     def test_return_multi_unique_fields_not_supported(self):
         """
         The new manager utils supports returning bulk upserts when there are multiple unique fields.
         """
         return_values = models.TestModel.objects.bulk_upsert2([], ['float_field', 'int_field'], ['float_field'],
                                                               returning=True)
-        self.assertEquals(return_values, [])
+        self.assertEqual(return_values, [])
 
     def test_return_created_values(self):
         """
         Tests that values that are created are returned properly when returning is True.
         """
         results = models.TestModel.objects.bulk_upsert2(
             [models.TestModel(int_field=1), models.TestModel(int_field=3), models.TestModel(int_field=4)],
             ['int_field'], ['float_field'], returning=True
         )
 
-        self.assertEquals(len(list(results.created)), 3)
+        self.assertEqual(len(list(results.created)), 3)
         for test_model, expected_int in zip(sorted(results.created, key=lambda k: k.int_field), [1, 3, 4]):
-            self.assertEquals(test_model.int_field, expected_int)
+            self.assertEqual(test_model.int_field, expected_int)
             self.assertIsNotNone(test_model.id)
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
 
     def test_return_list_of_values(self):
         """
         Tests that values that are created are returned properly when returning is True.
         Set returning to a list of fields
         """
         results = models.TestModel.objects.bulk_upsert2(
             [models.TestModel(int_field=1, float_field=2),
              models.TestModel(int_field=3, float_field=4),
              models.TestModel(int_field=4, float_field=5)],
             ['int_field'], ['float_field'], returning=['float_field']
         )
 
-        self.assertEquals(len(list(results.created)), 3)
+        self.assertEqual(len(list(results.created)), 3)
         with self.assertRaises(AttributeError):
             list(results.created)[0].int_field
-        self.assertEquals(set([2, 4, 5]), set([m.float_field for m in results.created]))
+        self.assertEqual(set([2, 4, 5]), set([m.float_field for m in results.created]))
 
     def test_return_created_updated_values(self):
         """
         Tests returning values when the items are either updated or created.
         """
         # Create an item that will be updated
         G(models.TestModel, int_field=2, float_field=1.0)
@@ -1004,25 +1004,25 @@
                 models.TestModel(int_field=1, float_field=3.0), models.TestModel(int_field=2.0, float_field=3.0),
                 models.TestModel(int_field=3, float_field=3.0), models.TestModel(int_field=4, float_field=3.0)
             ],
             ['int_field'], ['float_field'], returning=True)
 
         created = list(results.created)
         updated = list(results.updated)
-        self.assertEquals(len(created), 3)
-        self.assertEquals(len(updated), 1)
+        self.assertEqual(len(created), 3)
+        self.assertEqual(len(updated), 1)
         for test_model, expected_int in zip(sorted(created, key=lambda k: k.int_field), [1, 3, 4]):
-            self.assertEquals(test_model.int_field, expected_int)
-            self.assertAlmostEquals(test_model.float_field, 3.0)
+            self.assertEqual(test_model.int_field, expected_int)
+            self.assertAlmostEqual(test_model.float_field, 3.0)
             self.assertIsNotNone(test_model.id)
 
-        self.assertEquals(updated[0].int_field, 2)
-        self.assertAlmostEquals(updated[0].float_field, 3.0)
+        self.assertEqual(updated[0].int_field, 2)
+        self.assertAlmostEqual(updated[0].float_field, 3.0)
         self.assertIsNotNone(updated[0].id)
-        self.assertEquals(models.TestModel.objects.count(), 4)
+        self.assertEqual(models.TestModel.objects.count(), 4)
 
     def test_created_updated_auto_datetime_values(self):
         """
         Tests when the items are either updated or created when auto_now
         and auto_now_add datetime values are used
         """
         # Create an item that will be updated
@@ -1035,24 +1035,24 @@
                     models.TestAutoDateTimeModel(int_field=1),
                     models.TestAutoDateTimeModel(int_field=2),
                     models.TestAutoDateTimeModel(int_field=3),
                     models.TestAutoDateTimeModel(int_field=4)
                 ],
                 ['int_field'], returning=True)
 
-        self.assertEquals(len(list(results.created)), 3)
-        self.assertEquals(len(list(results.updated)), 1)
+        self.assertEqual(len(list(results.created)), 3)
+        self.assertEqual(len(list(results.updated)), 1)
 
         expected_auto_now = [dt.datetime(2018, 9, 2), dt.datetime(2018, 9, 2),
                              dt.datetime(2018, 9, 2), dt.datetime(2018, 9, 2)]
         expected_auto_now_add = [dt.datetime(2018, 9, 1), dt.datetime(2018, 9, 2),
                                  dt.datetime(2018, 9, 2), dt.datetime(2018, 9, 2)]
         for i, test_model in enumerate(sorted(results, key=lambda k: k.int_field)):
-            self.assertEquals(test_model.auto_now_field, expected_auto_now[i])
-            self.assertEquals(test_model.auto_now_add_field, expected_auto_now_add[i])
+            self.assertEqual(test_model.auto_now_field, expected_auto_now[i])
+            self.assertEqual(test_model.auto_now_add_field, expected_auto_now_add[i])
 
     def test_wo_update_fields(self):
         """
         Tests bulk_upsert with no update fields. This function in turn should just do a bulk create for any
         models that do not already exist.
         """
         # Create models that already exist
@@ -1061,25 +1061,25 @@
         # Perform a bulk_upsert with one new model
         models.TestModel.objects.bulk_upsert2([
             models.TestModel(int_field=1, float_field=3),
             models.TestModel(int_field=2, float_field=3),
             models.TestModel(int_field=3, float_field=3)
         ], ['int_field'], update_fields=[])
         # Three objects should now exist, but no float fields should be updated
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for test_model, expected_int_value in zip(models.TestModel.objects.order_by('int_field'), [1, 2, 3]):
-            self.assertEquals(test_model.int_field, expected_int_value)
-            self.assertEquals(test_model.float_field, expected_int_value)
+            self.assertEqual(test_model.int_field, expected_int_value)
+            self.assertEqual(test_model.float_field, expected_int_value)
 
     def test_w_blank_arguments(self):
         """
         Tests using required arguments and using blank arguments for everything else.
         """
         models.TestModel.objects.bulk_upsert2([], ['field'], ['field'])
-        self.assertEquals(models.TestModel.objects.count(), 0)
+        self.assertEqual(models.TestModel.objects.count(), 0)
 
     def test_no_updates(self):
         """
         Tests the case when no updates were previously stored (i.e objects are only created)
         """
         models.TestModel.objects.bulk_upsert([
             models.TestModel(int_field=0, char_field='0', float_field=0),
@@ -1106,19 +1106,19 @@
         # Update using the int field as a uniqueness constraint
         results = models.TestModel.objects.bulk_upsert2([
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=1, char_field='1', float_field=1),
             models.TestModel(int_field=2, char_field='2', float_field=2),
         ], ['int_field'], returning=True)
 
-        self.assertEquals(list(results.created), [])
-        self.assertEquals(set([u.id for u in results.updated]), set([t.id for t in test_models]))
-        self.assertEquals(set([u.int_field for u in results.updated]), set([0, 1, 2]))
-        self.assertEquals(set([u.float_field for u in results.updated]), set([0, 1, 2]))
-        self.assertEquals(set([u.char_field for u in results.updated]), set(['0', '1', '2']))
+        self.assertEqual(list(results.created), [])
+        self.assertEqual(set([u.id for u in results.updated]), set([t.id for t in test_models]))
+        self.assertEqual(set([u.int_field for u in results.updated]), set([0, 1, 2]))
+        self.assertEqual(set([u.float_field for u in results.updated]), set([0, 1, 2]))
+        self.assertEqual(set([u.char_field for u in results.updated]), set(['0', '1', '2']))
 
     def test_no_update_fields_returning(self):
         """
         Tests the case when all updates were previously stored and the int field is used as a uniqueness
         constraint. This test does not update any fields
         """
         # Create previously stored test models with a unique int field and -1 for all other fields
@@ -1128,15 +1128,15 @@
         # Update using the int field as a uniqueness constraint
         results = models.TestModel.objects.bulk_upsert2([
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=1, char_field='1', float_field=1),
             models.TestModel(int_field=2, char_field='2', float_field=2),
         ], ['int_field'], [], returning=True)
 
-        self.assertEquals(list(results), [])
+        self.assertEqual(list(results), [])
 
     def test_update_duplicate_fields_returning_none_updated(self):
         """
         Tests the case when all updates were previously stored and the upsert tries to update the rows
         with duplicate values.
         """
         # Create previously stored test models with a unique int field and -1 for all other fields
@@ -1146,15 +1146,15 @@
         # Update using the int field as a uniqueness constraint
         results = models.TestModel.objects.bulk_upsert2([
             models.TestModel(int_field=0, char_field='-1', float_field=-1),
             models.TestModel(int_field=1, char_field='-1', float_field=-1),
             models.TestModel(int_field=2, char_field='-1', float_field=-1),
         ], ['int_field'], ['char_field', 'float_field'], returning=True, ignore_duplicate_updates=True)
 
-        self.assertEquals(list(results), [])
+        self.assertEqual(list(results), [])
 
     def test_update_duplicate_fields_returning_some_updated(self):
         """
         Tests the case when all updates were previously stored and the upsert tries to update the rows
         with duplicate values. Test when some aren't duplicates
         """
         # Create previously stored test models with a unique int field and -1 for all other fields
@@ -1164,17 +1164,17 @@
         # Update using the int field as a uniqueness constraint
         results = models.TestModel.objects.bulk_upsert2([
             models.TestModel(int_field=0, char_field='-1', float_field=-1),
             models.TestModel(int_field=1, char_field='-1', float_field=-1),
             models.TestModel(int_field=2, char_field='0', float_field=-1),
         ], ['int_field'], ['char_field', 'float_field'], returning=['char_field'], ignore_duplicate_updates=True)
 
-        self.assertEquals(list(results.created), [])
-        self.assertEquals(len(list(results.updated)), 1)
-        self.assertEquals(list(results.updated)[0].char_field, '0')
+        self.assertEqual(list(results.created), [])
+        self.assertEqual(len(list(results.updated)), 1)
+        self.assertEqual(list(results.updated)[0].char_field, '0')
 
     def test_update_duplicate_fields_returning_some_updated_return_untouched(self):
         """
         Tests the case when all updates were previously stored and the upsert tries to update the rows
         with duplicate values. Test when some aren't duplicates
         """
         # Create previously stored test models with a unique int field and -1 for all other fields
@@ -1188,19 +1188,19 @@
                 models.TestModel(int_field=1, char_field='-1', float_field=-1),
                 models.TestModel(int_field=2, char_field='0', float_field=-1),
                 models.TestModel(int_field=3, char_field='3', float_field=3),
             ],
             ['int_field'], ['char_field', 'float_field'],
             returning=['char_field'], ignore_duplicate_updates=True, return_untouched=True)
 
-        self.assertEquals(len(list(results.updated)), 1)
-        self.assertEquals(len(list(results.untouched)), 2)
-        self.assertEquals(len(list(results.created)), 1)
-        self.assertEquals(list(results.updated)[0].char_field, '0')
-        self.assertEquals(list(results.created)[0].char_field, '3')
+        self.assertEqual(len(list(results.updated)), 1)
+        self.assertEqual(len(list(results.untouched)), 2)
+        self.assertEqual(len(list(results.created)), 1)
+        self.assertEqual(list(results.updated)[0].char_field, '0')
+        self.assertEqual(list(results.created)[0].char_field, '3')
 
     def test_update_duplicate_fields_returning_some_updated_return_untouched_ignore_dups(self):
         """
         Tests the case when all updates were previously stored and the upsert tries to update the rows
         with duplicate values. Test when some aren't duplicates and return untouched results.
         There will be no untouched results in this test since we turn off ignoring duplicate
         updates
@@ -1216,18 +1216,18 @@
                 models.TestModel(int_field=1, char_field='-1', float_field=-1),
                 models.TestModel(int_field=2, char_field='0', float_field=-1),
                 models.TestModel(int_field=3, char_field='3', float_field=3),
             ],
             ['int_field'], ['char_field', 'float_field'],
             returning=['char_field'], ignore_duplicate_updates=False, return_untouched=True)
 
-        self.assertEquals(len(list(results.untouched)), 0)
-        self.assertEquals(len(list(results.updated)), 3)
-        self.assertEquals(len(list(results.created)), 1)
-        self.assertEquals(list(results.created)[0].char_field, '3')
+        self.assertEqual(len(list(results.untouched)), 0)
+        self.assertEqual(len(list(results.updated)), 3)
+        self.assertEqual(len(list(results.created)), 1)
+        self.assertEqual(list(results.created)[0].char_field, '3')
 
     def test_all_updates_unique_int_field(self):
         """
         Tests the case when all updates were previously stored and the int field is used as a uniqueness
         constraint.
         """
         # Create previously stored test models with a unique int field and -1 for all other fields
@@ -1238,15 +1238,15 @@
         models.TestModel.objects.bulk_upsert2([
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=1, char_field='1', float_field=1),
             models.TestModel(int_field=2, char_field='2', float_field=2),
         ], ['int_field'], ['char_field', 'float_field'])
 
         # Verify that the fields were updated
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, str(i))
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_all_updates_unique_int_field_update_float_field(self):
         """
@@ -1261,15 +1261,15 @@
         models.TestModel.objects.bulk_upsert2([
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=1, char_field='1', float_field=1),
             models.TestModel(int_field=2, char_field='2', float_field=2),
         ], ['int_field'], update_fields=['float_field'])
 
         # Verify that the float field was updated
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, '-1')
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_some_updates_unique_int_field_update_float_field(self):
         """
@@ -1285,15 +1285,15 @@
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=1, char_field='1', float_field=1),
             models.TestModel(int_field=2, char_field='2', float_field=2),
         ], ['int_field'], ['float_field'])
 
         # Verify that the float field was updated for the first two models and the char field was not updated for
         # the first two. The char field, however, should be '2' for the third model since it was created
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, '-1' if i < 2 else '2')
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_some_updates_unique_timezone_field_update_float_field(self):
         """
@@ -1310,24 +1310,24 @@
             models.TestModel(time_zone=timezone('US/Central'), char_field='1', float_field=1),
             models.TestModel(time_zone=timezone('UTC'), char_field='2', float_field=2),
         ], ['time_zone'], ['float_field'])
 
         # Verify that the float field was updated for the first two models and the char field was not updated for
         # the first two. The char field, however, should be '2' for the third model since it was created
         m1 = models.TestUniqueTzModel.objects.get(time_zone=timezone('US/Eastern'))
-        self.assertEquals(m1.char_field, '-1')
-        self.assertAlmostEquals(m1.float_field, 0)
+        self.assertEqual(m1.char_field, '-1')
+        self.assertAlmostEqual(m1.float_field, 0)
 
         m2 = models.TestUniqueTzModel.objects.get(time_zone=timezone('US/Central'))
-        self.assertEquals(m2.char_field, '-1')
-        self.assertAlmostEquals(m2.float_field, 1)
+        self.assertEqual(m2.char_field, '-1')
+        self.assertAlmostEqual(m2.float_field, 1)
 
         m3 = models.TestUniqueTzModel.objects.get(time_zone=timezone('UTC'))
-        self.assertEquals(m3.char_field, '2')
-        self.assertAlmostEquals(m3.float_field, 2)
+        self.assertEqual(m3.char_field, '2')
+        self.assertAlmostEqual(m3.float_field, 2)
 
     def test_some_updates_unique_int_char_field_update_float_field(self):
         """
         Tests the case when some updates were previously stored and the int and char fields are used as a uniqueness
         constraint. Only updates the float field.
         """
         # Create previously stored test models with a unique int and char field
@@ -1339,15 +1339,15 @@
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=1, char_field='1', float_field=1),
             models.TestModel(int_field=2, char_field='2', float_field=2),
         ], ['int_field', 'char_field'], ['float_field'])
 
         # Verify that the float field was updated for the first two models and the char field was not updated for
         # the first two. The char field, however, should be '2' for the third model since it was created
-        self.assertEquals(models.TestModel.objects.count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, str(i))
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_no_updates_unique_int_char_field(self):
         """
@@ -1362,21 +1362,21 @@
         models.TestModel.objects.bulk_upsert2([
             models.TestModel(int_field=3, char_field='0', float_field=0),
             models.TestModel(int_field=4, char_field='1', float_field=1),
             models.TestModel(int_field=5, char_field='2', float_field=2),
         ], ['int_field', 'char_field'], ['float_field'])
 
         # Verify that no updates occured
-        self.assertEquals(models.TestModel.objects.count(), 6)
-        self.assertEquals(models.TestModel.objects.filter(char_field='-1').count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 6)
+        self.assertEqual(models.TestModel.objects.filter(char_field='-1').count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.filter(char_field='-1').order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, '-1')
             self.assertAlmostEqual(model_obj.float_field, -1)
-        self.assertEquals(models.TestModel.objects.exclude(char_field='-1').count(), 3)
+        self.assertEqual(models.TestModel.objects.exclude(char_field='-1').count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.exclude(char_field='-1').order_by('int_field')):
             self.assertEqual(model_obj.int_field, i + 3)
             self.assertEqual(model_obj.char_field, str(i))
             self.assertAlmostEqual(model_obj.float_field, i)
 
     def test_some_updates_unique_int_char_field_queryset(self):
         """
@@ -1390,16 +1390,16 @@
         models.TestModel.objects.filter(int_field=0).bulk_upsert2([
             models.TestModel(int_field=0, char_field='0', float_field=0),
             models.TestModel(int_field=4, char_field='1', float_field=1),
             models.TestModel(int_field=5, char_field='2', float_field=2),
         ], ['int_field'], ['float_field'])
 
         # Verify that two new objecs were created
-        self.assertEquals(models.TestModel.objects.count(), 5)
-        self.assertEquals(models.TestModel.objects.filter(char_field='-1').count(), 3)
+        self.assertEqual(models.TestModel.objects.count(), 5)
+        self.assertEqual(models.TestModel.objects.filter(char_field='-1').count(), 3)
         for i, model_obj in enumerate(models.TestModel.objects.filter(char_field='-1').order_by('int_field')):
             self.assertEqual(model_obj.int_field, i)
             self.assertEqual(model_obj.char_field, '-1')
 
 
 class PostBulkOperationSignalTest(TestCase):
     """
@@ -1427,149 +1427,149 @@
         post_bulk_operation.disconnect(self.signal_handler)
 
     def test_custom_field_bulk_update(self):
         model_obj = models.TestModel.objects.create(int_field=2)
         model_obj.time_zone = timezone('US/Eastern')
         models.TestModel.objects.bulk_update([model_obj], ['time_zone'])
         model_obj = models.TestModel.objects.get(id=model_obj.id)
-        self.assertEquals(model_obj.time_zone, timezone('US/Eastern'))
+        self.assertEqual(model_obj.time_zone, timezone('US/Eastern'))
 
     def test_post_bulk_operation_queryset_update(self):
         """
         Tests that the update operation on a queryset emits the post_bulk_operation signal.
         """
         models.TestModel.objects.all().update(int_field=1)
 
-        self.assertEquals(self.signal_handler.model, models.TestModel)
-        self.assertEquals(self.signal_handler.num_times_called, 1)
+        self.assertEqual(self.signal_handler.model, models.TestModel)
+        self.assertEqual(self.signal_handler.num_times_called, 1)
 
     def test_post_bulk_operation_manager_update(self):
         """
         Tests that the update operation on a manager emits the post_bulk_operation signal.
         """
         models.TestModel.objects.update(int_field=1)
 
-        self.assertEquals(self.signal_handler.model, models.TestModel)
-        self.assertEquals(self.signal_handler.num_times_called, 1)
+        self.assertEqual(self.signal_handler.model, models.TestModel)
+        self.assertEqual(self.signal_handler.num_times_called, 1)
 
     def test_post_bulk_operation_bulk_update(self):
         """
         Tests that the bulk_update operation emits the post_bulk_operation signal.
         """
         model_obj = models.TestModel.objects.create(int_field=2)
         models.TestModel.objects.bulk_update([model_obj], ['int_field'])
 
-        self.assertEquals(self.signal_handler.model, models.TestModel)
-        self.assertEquals(self.signal_handler.num_times_called, 1)
+        self.assertEqual(self.signal_handler.model, models.TestModel)
+        self.assertEqual(self.signal_handler.num_times_called, 1)
 
     def test_post_bulk_operation_bulk_upsert2(self):
         """
         Tests that the bulk_upsert2 operation emits the post_bulk_operation signal.
         """
         model_obj = models.TestModel.objects.create(int_field=2)
         models.TestModel.objects.bulk_upsert2([model_obj], ['int_field'])
 
-        self.assertEquals(self.signal_handler.model, models.TestModel)
-        self.assertEquals(self.signal_handler.num_times_called, 1)
+        self.assertEqual(self.signal_handler.model, models.TestModel)
+        self.assertEqual(self.signal_handler.num_times_called, 1)
 
     def test_post_bulk_operation_bulk_create(self):
         """
         Tests that the bulk_create operation emits the post_bulk_operation signal.
         """
         models.TestModel.objects.bulk_create([models.TestModel(int_field=2)])
 
-        self.assertEquals(self.signal_handler.model, models.TestModel)
-        self.assertEquals(self.signal_handler.num_times_called, 1)
+        self.assertEqual(self.signal_handler.model, models.TestModel)
+        self.assertEqual(self.signal_handler.num_times_called, 1)
 
     def test_post_bulk_operation_bulk_create_queryset(self):
         """
         Tests that the bulk_create operation emits the post_bulk_operation signal.
         """
         models.TestModel.objects.all().bulk_create([models.TestModel(int_field=2)])
 
-        self.assertEquals(self.signal_handler.model, models.TestModel)
-        self.assertEquals(self.signal_handler.num_times_called, 1)
+        self.assertEqual(self.signal_handler.model, models.TestModel)
+        self.assertEqual(self.signal_handler.num_times_called, 1)
 
     def test_save_doesnt_emit_signal(self):
         """
         Tests that a non-bulk operation doesn't emit the signal.
         """
         model_obj = models.TestModel.objects.create(int_field=2)
         model_obj.save()
 
-        self.assertEquals(self.signal_handler.num_times_called, 0)
+        self.assertEqual(self.signal_handler.num_times_called, 0)
 
 
 class IdDictTest(TestCase):
     """
     Tests the id_dict function.
     """
     def test_no_objects_manager(self):
         """
         Tests the output when no objects are present in the manager.
         """
-        self.assertEquals(models.TestModel.objects.id_dict(), {})
+        self.assertEqual(models.TestModel.objects.id_dict(), {})
 
     def test_objects_manager(self):
         """
         Tests retrieving a dict of objects keyed on their ID from the manager.
         """
         model_obj1 = G(models.TestModel, int_field=1)
         model_obj2 = G(models.TestModel, int_field=2)
-        self.assertEquals(models.TestModel.objects.id_dict(), {model_obj1.id: model_obj1, model_obj2.id: model_obj2})
+        self.assertEqual(models.TestModel.objects.id_dict(), {model_obj1.id: model_obj1, model_obj2.id: model_obj2})
 
     def test_no_objects_queryset(self):
         """
         Tests the case when no objects are returned via a queryset.
         """
         G(models.TestModel, int_field=1)
         G(models.TestModel, int_field=2)
-        self.assertEquals(models.TestModel.objects.filter(int_field__gte=3).id_dict(), {})
+        self.assertEqual(models.TestModel.objects.filter(int_field__gte=3).id_dict(), {})
 
     def test_objects_queryset(self):
         """
         Tests the case when objects are returned via a queryset.
         """
         G(models.TestModel, int_field=1)
         model_obj = G(models.TestModel, int_field=2)
-        self.assertEquals(models.TestModel.objects.filter(int_field__gte=2).id_dict(), {model_obj.id: model_obj})
+        self.assertEqual(models.TestModel.objects.filter(int_field__gte=2).id_dict(), {model_obj.id: model_obj})
 
 
 class GetOrNoneTest(TestCase):
     """
     Tests the get_or_none function in the manager utils
     """
     def test_existing_using_objects(self):
         """
         Tests get_or_none on an existing object from Model.objects.
         """
         # Create an existing model
         model_obj = G(models.TestModel)
         # Verify that get_or_none on objects returns the test model
-        self.assertEquals(model_obj, models.TestModel.objects.get_or_none(id=model_obj.id))
+        self.assertEqual(model_obj, models.TestModel.objects.get_or_none(id=model_obj.id))
 
     def test_multiple_error_using_objects(self):
         """
         Tests get_or_none on multiple existing objects from Model.objects.
         """
         # Create an existing model
         model_obj = G(models.TestModel, char_field='hi')
         model_obj = G(models.TestModel, char_field='hi')
         # Verify that get_or_none on objects returns the test model
         with self.assertRaises(models.TestModel.MultipleObjectsReturned):
-            self.assertEquals(model_obj, models.TestModel.objects.get_or_none(char_field='hi'))
+            self.assertEqual(model_obj, models.TestModel.objects.get_or_none(char_field='hi'))
 
     def test_existing_using_queryset(self):
         """
         Tests get_or_none on an existing object from a queryst.
         """
         # Create an existing model
         model_obj = G(models.TestModel)
         # Verify that get_or_none on objects returns the test model
-        self.assertEquals(model_obj, models.TestModel.objects.filter(id=model_obj.id).get_or_none(id=model_obj.id))
+        self.assertEqual(model_obj, models.TestModel.objects.filter(id=model_obj.id).get_or_none(id=model_obj.id))
 
     def test_none_using_objects(self):
         """
         Tests when no object exists when using Model.objects.
         """
         # Verify that get_or_none on objects returns the test model
         self.assertIsNone(models.TestModel.objects.get_or_none(id=1))
@@ -1619,31 +1619,31 @@
             models.TestModel.objects.filter(id__gte=0).single()
 
     def test_single_using_objects(self):
         """
         Tests accessing a single object using Model.objects.
         """
         model_obj = G(models.TestModel)
-        self.assertEquals(model_obj, models.TestModel.objects.single())
+        self.assertEqual(model_obj, models.TestModel.objects.single())
 
     def test_single_using_queryset(self):
         """
         Tests accessing a single object using a queryset.
         """
         model_obj = G(models.TestModel)
-        self.assertEquals(model_obj, models.TestModel.objects.filter(id__gte=0).single())
+        self.assertEqual(model_obj, models.TestModel.objects.filter(id__gte=0).single())
 
     def test_mutliple_to_single_using_queryset(self):
         """
         Tests accessing a single object using a queryset. The queryset is what filters it
         down to a single object.
         """
         model_obj = G(models.TestModel)
         G(models.TestModel)
-        self.assertEquals(model_obj, models.TestModel.objects.filter(id=model_obj.id).single())
+        self.assertEqual(model_obj, models.TestModel.objects.filter(id=model_obj.id).single())
 
 
 class BulkUpdateTest(TestCase):
     """
     Tests the bulk_update function.
     """
     def test_update_foreign_key_by_id(self):
@@ -1664,36 +1664,36 @@
         """
         Tests a bulk update on a model that has a primary key to a foreign key. It uses the id of the pk in the
         update
         """
         t = G(models.TestPkForeignKey, char_field='hi')
         models.TestPkForeignKey.objects.bulk_update(
             [models.TestPkForeignKey(my_key_id=t.my_key_id, char_field='hello')], ['char_field'])
-        self.assertEquals(models.TestPkForeignKey.objects.count(), 1)
+        self.assertEqual(models.TestPkForeignKey.objects.count(), 1)
         self.assertTrue(models.TestPkForeignKey.objects.filter(char_field='hello', my_key=t.my_key).exists())
 
     def test_foreign_key_pk(self):
         """
         Tests a bulk update on a model that has a primary key to a foreign key. It uses the foreign key itself
         in the update
         """
         t = G(models.TestPkForeignKey, char_field='hi')
         models.TestPkForeignKey.objects.bulk_update(
             [models.TestPkForeignKey(my_key=t.my_key, char_field='hello')], ['char_field'])
-        self.assertEquals(models.TestPkForeignKey.objects.count(), 1)
+        self.assertEqual(models.TestPkForeignKey.objects.count(), 1)
         self.assertTrue(models.TestPkForeignKey.objects.filter(char_field='hello', my_key=t.my_key).exists())
 
     def test_char_pk(self):
         """
         Tests a bulk update on a model that has a primary key to a char field.
         """
         G(models.TestPkChar, char_field='hi', my_key='1')
         models.TestPkChar.objects.bulk_update(
             [models.TestPkChar(my_key='1', char_field='hello')], ['char_field'])
-        self.assertEquals(models.TestPkChar.objects.count(), 1)
+        self.assertEqual(models.TestPkChar.objects.count(), 1)
         self.assertTrue(models.TestPkChar.objects.filter(char_field='hello', my_key='1').exists())
 
     def test_none(self):
         """
         Tests when no values are provided to bulk update.
         """
         models.TestModel.objects.bulk_update([], [])
@@ -1757,16 +1757,16 @@
         test_obj_1.int_field = 3
         test_obj_2.int_field = 4
         # Do a bulk update with no update fields
         models.TestModel.objects.bulk_update([test_obj_1, test_obj_2], [])
         # The test objects int fields should be untouched
         test_obj_1 = models.TestModel.objects.get(id=test_obj_1.id)
         test_obj_2 = models.TestModel.objects.get(id=test_obj_2.id)
-        self.assertEquals(test_obj_1.int_field, 1)
-        self.assertEquals(test_obj_2.int_field, 2)
+        self.assertEqual(test_obj_1.int_field, 1)
+        self.assertEqual(test_obj_2.int_field, 2)
 
     def test_objs_one_field_to_update(self):
         """
         Tests when objects are given to bulk update with one field to update.
         """
         test_obj_1 = G(models.TestModel, int_field=1)
         test_obj_2 = G(models.TestModel, int_field=2)
@@ -1774,16 +1774,16 @@
         test_obj_1.int_field = 3
         test_obj_2.int_field = 4
         # Do a bulk update with the int fields
         models.TestModel.objects.bulk_update([test_obj_1, test_obj_2], ['int_field'])
         # The test objects int fields should be untouched
         test_obj_1 = models.TestModel.objects.get(id=test_obj_1.id)
         test_obj_2 = models.TestModel.objects.get(id=test_obj_2.id)
-        self.assertEquals(test_obj_1.int_field, 3)
-        self.assertEquals(test_obj_2.int_field, 4)
+        self.assertEqual(test_obj_1.int_field, 3)
+        self.assertEqual(test_obj_2.int_field, 4)
 
     def test_objs_one_field_to_update_ignore_other_field(self):
         """
         Tests when objects are given to bulk update with one field to update. This test changes another field
         not included in the update and verifies it is not updated.
         """
         test_obj_1 = G(models.TestModel, int_field=1, float_field=1.0)
@@ -1794,19 +1794,19 @@
         test_obj_1.float_field = 3.0
         test_obj_2.float_field = 4.0
         # Do a bulk update with the int fields
         models.TestModel.objects.bulk_update([test_obj_1, test_obj_2], ['int_field'])
         # The test objects int fields should be untouched
         test_obj_1 = models.TestModel.objects.get(id=test_obj_1.id)
         test_obj_2 = models.TestModel.objects.get(id=test_obj_2.id)
-        self.assertEquals(test_obj_1.int_field, 3)
-        self.assertEquals(test_obj_2.int_field, 4)
+        self.assertEqual(test_obj_1.int_field, 3)
+        self.assertEqual(test_obj_2.int_field, 4)
         # The float fields should not be updated
-        self.assertEquals(test_obj_1.float_field, 1.0)
-        self.assertEquals(test_obj_2.float_field, 2.0)
+        self.assertEqual(test_obj_1.float_field, 1.0)
+        self.assertEqual(test_obj_2.float_field, 2.0)
 
     def test_objs_two_fields_to_update(self):
         """
         Tests when objects are given to bulk update with two fields to update.
         """
         test_obj_1 = G(models.TestModel, int_field=1, float_field=1.0)
         test_obj_2 = G(models.TestModel, int_field=2, float_field=2.0)
@@ -1816,19 +1816,19 @@
         test_obj_1.float_field = 3.0
         test_obj_2.float_field = 4.0
         # Do a bulk update with the int fields
         models.TestModel.objects.bulk_update([test_obj_1, test_obj_2], ['int_field', 'float_field'])
         # The test objects int fields should be untouched
         test_obj_1 = models.TestModel.objects.get(id=test_obj_1.id)
         test_obj_2 = models.TestModel.objects.get(id=test_obj_2.id)
-        self.assertEquals(test_obj_1.int_field, 3)
-        self.assertEquals(test_obj_2.int_field, 4)
+        self.assertEqual(test_obj_1.int_field, 3)
+        self.assertEqual(test_obj_2.int_field, 4)
         # The float fields should be updated
-        self.assertEquals(test_obj_1.float_field, 3.0)
-        self.assertEquals(test_obj_2.float_field, 4.0)
+        self.assertEqual(test_obj_1.float_field, 3.0)
+        self.assertEqual(test_obj_2.float_field, 4.0)
 
     def test_updating_objects_with_custom_db_field_types(self):
         """
         Tests when objects are updated that have custom field types
         """
         test_obj_1 = G(
             models.TestModel,
@@ -1859,169 +1859,169 @@
         )
 
         # Refetch the objects
         test_obj_1 = models.TestModel.objects.get(id=test_obj_1.id)
         test_obj_2 = models.TestModel.objects.get(id=test_obj_2.id)
 
         # Assert that the json field was updated
-        self.assertEquals(test_obj_1.json_field, {'test': 'updated'})
-        self.assertEquals(test_obj_2.json_field, {'test2': 'updated'})
+        self.assertEqual(test_obj_1.json_field, {'test': 'updated'})
+        self.assertEqual(test_obj_2.json_field, {'test2': 'updated'})
 
         # Assert that the array field was updated
-        self.assertEquals(test_obj_1.array_field, ['one', 'two', 'updated'])
-        self.assertEquals(test_obj_2.array_field, ['three', 'four', 'updated'])
+        self.assertEqual(test_obj_1.array_field, ['one', 'two', 'updated'])
+        self.assertEqual(test_obj_2.array_field, ['three', 'four', 'updated'])
 
 
 class UpsertTest(TestCase):
     """
     Tests the upsert method in the manager utils.
     """
     @patch.object(models.TestModel, 'save', spec_set=True)
     def test_no_double_save_on_create(self, mock_save):
         """
         Tests that save isn't called on upsert after the object has been created.
         """
         model_obj, created = models.TestModel.objects.upsert(int_field=1, updates={'float_field': 1.0})
-        self.assertEquals(mock_save.call_count, 1)
+        self.assertEqual(mock_save.call_count, 1)
 
     def test_save_on_update(self):
         """
         Tests that save is called when the model is updated
         """
         model_obj, created = models.TestModel.objects.upsert(int_field=1, updates={'float_field': 1.0})
 
         with patch.object(models.TestModel, 'save', spec_set=True) as mock_save:
             models.TestModel.objects.upsert(int_field=1, updates={'float_field': 1.1})
-            self.assertEquals(mock_save.call_count, 1)
+            self.assertEqual(mock_save.call_count, 1)
 
     def test_no_save_on_no_update(self):
         """
         Tests that save is not called on upsert if the model is not actually updated.
         """
         model_obj, created = models.TestModel.objects.upsert(int_field=1, updates={'float_field': 1.0})
 
         with patch.object(models.TestModel, 'save', spec_set=True) as mock_save:
             models.TestModel.objects.upsert(int_field=1, updates={'float_field': 1.0})
-            self.assertEquals(mock_save.call_count, 0)
+            self.assertEqual(mock_save.call_count, 0)
 
     def test_upsert_creation_no_defaults(self):
         """
         Tests an upsert that results in a created object. Don't use defaults
         """
         model_obj, created = models.TestModel.objects.upsert(int_field=1)
         self.assertTrue(created)
-        self.assertEquals(model_obj.int_field, 1)
+        self.assertEqual(model_obj.int_field, 1)
         self.assertIsNone(model_obj.float_field)
         self.assertIsNone(model_obj.char_field)
 
     def test_upsert_creation_defaults(self):
         """
         Tests an upsert that results in a created object. Defaults are used.
         """
         model_obj, created = models.TestModel.objects.upsert(int_field=1, defaults={'float_field': 1.0})
         self.assertTrue(created)
-        self.assertEquals(model_obj.int_field, 1)
-        self.assertEquals(model_obj.float_field, 1.0)
+        self.assertEqual(model_obj.int_field, 1)
+        self.assertEqual(model_obj.float_field, 1.0)
         self.assertIsNone(model_obj.char_field)
 
     def test_upsert_creation_updates(self):
         """
         Tests an upsert that results in a created object. Updates are used.
         """
         model_obj, created = models.TestModel.objects.upsert(int_field=1, updates={'float_field': 1.0})
         self.assertTrue(created)
-        self.assertEquals(model_obj.int_field, 1)
-        self.assertEquals(model_obj.float_field, 1.0)
+        self.assertEqual(model_obj.int_field, 1)
+        self.assertEqual(model_obj.float_field, 1.0)
         self.assertIsNone(model_obj.char_field)
 
     def test_upsert_creation_defaults_updates(self):
         """
         Tests an upsert that results in a created object. Defaults are used and so are updates.
         """
         model_obj, created = models.TestModel.objects.upsert(
             int_field=1, defaults={'float_field': 1.0}, updates={'char_field': 'Hello'})
         self.assertTrue(created)
-        self.assertEquals(model_obj.int_field, 1)
-        self.assertEquals(model_obj.float_field, 1.0)
-        self.assertEquals(model_obj.char_field, 'Hello')
+        self.assertEqual(model_obj.int_field, 1)
+        self.assertEqual(model_obj.float_field, 1.0)
+        self.assertEqual(model_obj.char_field, 'Hello')
 
     def test_upsert_creation_no_defaults_override(self):
         """
         Tests an upsert that results in a created object. Defaults are not used and
         the updates values override the defaults on creation.
         """
         test_model = G(models.TestModel)
         model_obj, created = models.TestForeignKeyModel.objects.upsert(int_field=1, updates={
             'test_model': test_model,
         })
         self.assertTrue(created)
-        self.assertEquals(model_obj.int_field, 1)
-        self.assertEquals(model_obj.test_model, test_model)
+        self.assertEqual(model_obj.int_field, 1)
+        self.assertEqual(model_obj.test_model, test_model)
 
     def test_upsert_creation_defaults_updates_override(self):
         """
         Tests an upsert that results in a created object. Defaults are used and so are updates. Updates
         override the defaults.
         """
         model_obj, created = models.TestModel.objects.upsert(
             int_field=1, defaults={'float_field': 1.0}, updates={'char_field': 'Hello', 'float_field': 2.0})
         self.assertTrue(created)
-        self.assertEquals(model_obj.int_field, 1)
-        self.assertEquals(model_obj.float_field, 2.0)
-        self.assertEquals(model_obj.char_field, 'Hello')
+        self.assertEqual(model_obj.int_field, 1)
+        self.assertEqual(model_obj.float_field, 2.0)
+        self.assertEqual(model_obj.char_field, 'Hello')
 
     def test_upsert_no_creation_no_defaults(self):
         """
         Tests an upsert that already exists. Don't use defaults
         """
         G(models.TestModel, int_field=1, float_field=None, char_field=None)
         model_obj, created = models.TestModel.objects.upsert(int_field=1)
         self.assertFalse(created)
-        self.assertEquals(model_obj.int_field, 1)
+        self.assertEqual(model_obj.int_field, 1)
         self.assertIsNone(model_obj.float_field)
         self.assertIsNone(model_obj.char_field)
 
     def test_upsert_no_creation_defaults(self):
         """
         Tests an upsert that already exists. Defaults are used but don't matter since the object already existed.
         """
         G(models.TestModel, int_field=1, float_field=None, char_field=None)
         model_obj, created = models.TestModel.objects.upsert(int_field=1, defaults={'float_field': 1.0})
         self.assertFalse(created)
-        self.assertEquals(model_obj.int_field, 1)
+        self.assertEqual(model_obj.int_field, 1)
         self.assertIsNone(model_obj.float_field)
         self.assertIsNone(model_obj.char_field)
 
     def test_upsert_no_creation_updates(self):
         """
         Tests an upsert that already exists. Updates are used.
         """
         G(models.TestModel, int_field=1, float_field=2.0, char_field=None)
         model_obj, created = models.TestModel.objects.upsert(int_field=1, updates={'float_field': 1.0})
         self.assertFalse(created)
-        self.assertEquals(model_obj.int_field, 1)
-        self.assertEquals(model_obj.float_field, 1.0)
+        self.assertEqual(model_obj.int_field, 1)
+        self.assertEqual(model_obj.float_field, 1.0)
         self.assertIsNone(model_obj.char_field)
 
     def test_upsert_no_creation_defaults_updates(self):
         """
         Tests an upsert that already exists. Defaults are used and so are updates.
         """
         G(models.TestModel, int_field=1, float_field=2.0, char_field='Hi')
         model_obj, created = models.TestModel.objects.upsert(
             int_field=1, defaults={'float_field': 1.0}, updates={'char_field': 'Hello'})
         self.assertFalse(created)
-        self.assertEquals(model_obj.int_field, 1)
-        self.assertEquals(model_obj.float_field, 2.0)
-        self.assertEquals(model_obj.char_field, 'Hello')
+        self.assertEqual(model_obj.int_field, 1)
+        self.assertEqual(model_obj.float_field, 2.0)
+        self.assertEqual(model_obj.char_field, 'Hello')
 
     def test_upsert_no_creation_defaults_updates_override(self):
         """
         Tests an upsert that already exists. Defaults are used and so are updates. Updates override the defaults.
         """
         G(models.TestModel, int_field=1, float_field=3.0, char_field='Hi')
         model_obj, created = models.TestModel.objects.upsert(
             int_field=1, defaults={'float_field': 1.0}, updates={'char_field': 'Hello', 'float_field': 2.0})
         self.assertFalse(created)
-        self.assertEquals(model_obj.int_field, 1)
-        self.assertEquals(model_obj.float_field, 2.0)
-        self.assertEquals(model_obj.char_field, 'Hello')
+        self.assertEqual(model_obj.int_field, 1)
+        self.assertEqual(model_obj.float_field, 2.0)
+        self.assertEqual(model_obj.char_field, 'Hello')
```

### Comparing `django-manager-utils-3.0.1/manager_utils/tests/models.py` & `django-manager-utils-3.1.0/manager_utils/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-manager-utils-3.0.1/manager_utils/upsert2.py` & `django-manager-utils-3.1.0/manager_utils/upsert2.py`

 * *Files identical despite different names*

### Comparing `django-manager-utils-3.0.1/setup.py` & `django-manager-utils-3.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,26 +38,23 @@
         "Changes": "https://django-manager-utils.readthedocs.io/en/latest/release_notes.html",
         "Documentation": "https://django-manager-utils.readthedocs.io/en/latest/",
         "Source Code": "https://github.com/ambitioninc/django-manager-utils",
     },
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
-        'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
     install_requires=install_requires,
     tests_require=tests_require,
     test_suite='run_tests.run',
     include_package_data=True,
 )
```

