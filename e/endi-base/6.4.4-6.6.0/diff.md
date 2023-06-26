# Comparing `tmp/endi_base-6.4.4.tar.gz` & `tmp/endi_base-6.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endi_base-6.4.4.tar", last modified: Fri Nov  4 12:00:41 2022, max compression
+gzip compressed data, was "endi_base-6.6.0.tar", last modified: Mon Jun 26 11:46:54 2023, max compression
```

## Comparing `endi_base-6.4.4.tar` & `endi_base-6.6.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2022-11-04 12:00:41.538680 endi_base-6.4.4/
--rw-r--r--   0 gas       (1000) gas       (1000)        6 2022-11-04 12:00:06.000000 endi_base-6.4.4/CURRENT_VERSION
--rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:08.000000 endi_base-6.4.4/LICENSE.txt
--rw-r--r--   0 gas       (1000) gas       (1000)      184 2020-06-24 14:37:08.000000 endi_base-6.4.4/MANIFEST.in
--rw-r--r--   0 gas       (1000) gas       (1000)     1059 2022-11-04 12:00:41.538680 endi_base-6.4.4/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)      483 2020-06-24 14:37:08.000000 endi_base-6.4.4/README.rst
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2022-11-04 12:00:41.534680 endi_base-6.4.4/endi_base/
--rw-r--r--   0 gas       (1000) gas       (1000)        0 2020-06-24 14:37:08.000000 endi_base-6.4.4/endi_base/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)      191 2020-11-09 12:49:57.000000 endi_base-6.4.4/endi_base/consts.py
--rw-r--r--   0 gas       (1000) gas       (1000)      213 2020-11-09 12:49:57.000000 endi_base-6.4.4/endi_base/exception.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3155 2022-09-08 13:24:47.000000 endi_base-6.4.4/endi_base/mail.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2022-11-04 12:00:41.536680 endi_base-6.4.4/endi_base/models/
--rw-r--r--   0 gas       (1000) gas       (1000)       49 2020-06-24 14:37:08.000000 endi_base-6.4.4/endi_base/models/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2100 2021-03-31 12:52:42.000000 endi_base-6.4.4/endi_base/models/base.py
--rw-r--r--   0 gas       (1000) gas       (1000)      976 2022-11-04 11:59:03.000000 endi_base-6.4.4/endi_base/models/initialize.py
--rw-r--r--   0 gas       (1000) gas       (1000)     5250 2021-03-12 18:07:04.000000 endi_base-6.4.4/endi_base/models/mixins.py
--rw-r--r--   0 gas       (1000) gas       (1000)     4621 2021-06-14 10:07:09.000000 endi_base-6.4.4/endi_base/models/types.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1396 2021-06-24 16:53:32.000000 endi_base-6.4.4/endi_base/models/utils.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2022-11-04 12:00:41.538680 endi_base-6.4.4/endi_base/utils/
--rw-r--r--   0 gas       (1000) gas       (1000)        0 2020-06-24 14:37:08.000000 endi_base-6.4.4/endi_base/utils/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2537 2020-11-09 12:49:57.000000 endi_base-6.4.4/endi_base/utils/ascii.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2701 2022-04-28 11:57:44.000000 endi_base-6.4.4/endi_base/utils/date.py
--rw-r--r--   0 gas       (1000) gas       (1000)      102 2020-11-09 12:49:57.000000 endi_base-6.4.4/endi_base/utils/export.py
--rw-r--r--   0 gas       (1000) gas       (1000)     5334 2020-11-09 12:49:57.000000 endi_base-6.4.4/endi_base/utils/math.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2419 2020-11-09 12:49:57.000000 endi_base-6.4.4/endi_base/utils/renderers.py
--rw-r--r--   0 gas       (1000) gas       (1000)      321 2020-11-09 12:49:57.000000 endi_base-6.4.4/endi_base/utils/strings.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2022-11-04 12:00:41.535680 endi_base-6.4.4/endi_base.egg-info/
--rw-r--r--   0 gas       (1000) gas       (1000)     1059 2022-11-04 12:00:41.000000 endi_base-6.4.4/endi_base.egg-info/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)      749 2022-11-04 12:00:41.000000 endi_base-6.4.4/endi_base.egg-info/SOURCES.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2022-11-04 12:00:41.000000 endi_base-6.4.4/endi_base.egg-info/dependency_links.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       43 2022-11-04 12:00:41.000000 endi_base-6.4.4/endi_base.egg-info/entry_points.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2020-06-24 14:37:08.000000 endi_base-6.4.4/endi_base.egg-info/not-zip-safe
--rw-r--r--   0 gas       (1000) gas       (1000)      124 2022-11-04 12:00:41.000000 endi_base-6.4.4/endi_base.egg-info/requires.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       10 2022-11-04 12:00:41.000000 endi_base-6.4.4/endi_base.egg-info/top_level.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       51 2020-06-24 14:37:08.000000 endi_base-6.4.4/pytest.ini
--rw-r--r--   0 gas       (1000) gas       (1000)       80 2022-03-15 12:24:55.000000 endi_base-6.4.4/requirements.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       38 2022-11-04 12:00:41.538680 endi_base-6.4.4/setup.cfg
--rw-r--r--   0 gas       (1000) gas       (1000)     1407 2020-11-09 12:49:57.000000 endi_base-6.4.4/setup.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-26 11:46:54.221003 endi_base-6.6.0/
+-rw-r--r--   0 gas       (1000) gas       (1000)        6 2023-06-26 11:46:08.000000 endi_base-6.6.0/CURRENT_VERSION
+-rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:08.000000 endi_base-6.6.0/LICENSE.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)      184 2020-06-24 14:37:08.000000 endi_base-6.6.0/MANIFEST.in
+-rw-r--r--   0 gas       (1000) gas       (1000)     1039 2023-06-26 11:46:54.221003 endi_base-6.6.0/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)      483 2023-03-14 16:52:57.000000 endi_base-6.6.0/README.rst
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-26 11:46:54.216003 endi_base-6.6.0/endi_base/
+-rw-r--r--   0 gas       (1000) gas       (1000)        0 2020-06-24 14:37:08.000000 endi_base-6.6.0/endi_base/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      191 2020-11-09 12:49:57.000000 endi_base-6.6.0/endi_base/consts.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      213 2020-11-09 12:49:57.000000 endi_base-6.6.0/endi_base/exception.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3155 2022-09-08 13:24:47.000000 endi_base-6.6.0/endi_base/mail.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-26 11:46:54.219003 endi_base-6.6.0/endi_base/models/
+-rw-r--r--   0 gas       (1000) gas       (1000)       49 2020-06-24 14:37:08.000000 endi_base-6.6.0/endi_base/models/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2100 2022-11-21 12:42:09.000000 endi_base-6.6.0/endi_base/models/base.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1070 2023-01-12 09:26:43.000000 endi_base-6.6.0/endi_base/models/initialize.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     5338 2023-06-26 11:37:41.000000 endi_base-6.6.0/endi_base/models/mixins.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     4621 2021-06-14 10:07:09.000000 endi_base-6.6.0/endi_base/models/types.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1396 2021-06-24 16:53:32.000000 endi_base-6.6.0/endi_base/models/utils.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-26 11:46:54.220003 endi_base-6.6.0/endi_base/utils/
+-rw-r--r--   0 gas       (1000) gas       (1000)        0 2020-06-24 14:37:08.000000 endi_base-6.6.0/endi_base/utils/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2537 2020-11-09 12:49:57.000000 endi_base-6.6.0/endi_base/utils/ascii.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2701 2022-04-28 11:57:44.000000 endi_base-6.6.0/endi_base/utils/date.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      102 2020-11-09 12:49:57.000000 endi_base-6.6.0/endi_base/utils/export.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     5334 2020-11-09 12:49:57.000000 endi_base-6.6.0/endi_base/utils/math.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2419 2020-11-09 12:49:57.000000 endi_base-6.6.0/endi_base/utils/renderers.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      321 2020-11-09 12:49:57.000000 endi_base-6.6.0/endi_base/utils/strings.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-26 11:46:54.217003 endi_base-6.6.0/endi_base.egg-info/
+-rw-r--r--   0 gas       (1000) gas       (1000)     1039 2023-06-26 11:46:53.000000 endi_base-6.6.0/endi_base.egg-info/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)      749 2023-06-26 11:46:54.000000 endi_base-6.6.0/endi_base.egg-info/SOURCES.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2023-06-26 11:46:53.000000 endi_base-6.6.0/endi_base.egg-info/dependency_links.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       42 2023-06-26 11:46:53.000000 endi_base-6.6.0/endi_base.egg-info/entry_points.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2020-06-24 14:37:08.000000 endi_base-6.6.0/endi_base.egg-info/not-zip-safe
+-rw-r--r--   0 gas       (1000) gas       (1000)      124 2023-06-26 11:46:53.000000 endi_base-6.6.0/endi_base.egg-info/requires.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       10 2023-06-26 11:46:53.000000 endi_base-6.6.0/endi_base.egg-info/top_level.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       51 2020-06-24 14:37:08.000000 endi_base-6.6.0/pytest.ini
+-rw-r--r--   0 gas       (1000) gas       (1000)       80 2022-03-15 12:24:55.000000 endi_base-6.6.0/requirements.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       38 2023-06-26 11:46:54.222003 endi_base-6.6.0/setup.cfg
+-rw-r--r--   0 gas       (1000) gas       (1000)     1407 2020-11-09 12:49:57.000000 endi_base-6.6.0/setup.py
```

### Comparing `endi_base-6.4.4/LICENSE.txt` & `endi_base-6.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `endi_base-6.4.4/PKG-INFO` & `endi_base-6.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: endi_base
-Version: 6.4.4
+Version: 6.6.0
 Summary: endi_base
 Home-page: https://framagit.org/endi/endi_base
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid endi
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Provides-Extra: testing
 License-File: LICENSE.txt
@@ -33,9 +32,7 @@
 * Custom SQLAlchemy column types
 * String formatting utilities
 * Date formatting utilities
 * Constants
 * ...
 
 It should not be installed directly but should be installed as a dependency
-
-
```

### Comparing `endi_base-6.4.4/endi_base/mail.py` & `endi_base-6.6.0/endi_base/mail.py`

 * *Files identical despite different names*

### Comparing `endi_base-6.4.4/endi_base/models/base.py` & `endi_base-6.6.0/endi_base/models/base.py`

 * *Files identical despite different names*

### Comparing `endi_base-6.4.4/endi_base/models/mixins.py` & `endi_base-6.6.0/endi_base/models/mixins.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,32 +19,34 @@
 
 class TimeStampedMixin(object):
     @declared_attr
     def created_at(cls):
         return Column(
             DateTime(),
             info={
-                'colanderalchemy': {
-                    'exclude': True, 'title': "Créé(e) le",
+                "colanderalchemy": {
+                    "exclude": True,
+                    "title": "Créé(e) le",
                 }
             },
             default=datetime.now,
         )
 
     @declared_attr
     def updated_at(cls):
         return Column(
             DateTime(),
             info={
-                'colanderalchemy': {
-                    'exclude': True, 'title': "Mis(e) à jour le",
+                "colanderalchemy": {
+                    "exclude": True,
+                    "title": "Mis(e) à jour le",
                 }
             },
             default=datetime.now,
-            onupdate=datetime.now
+            onupdate=datetime.now,
         )
 
 
 class OfficialNumberMixin:
     """
     Models that implements that mixin are then able to be numbered using
     numbering sequence mechanisms with guarantees on non-duplicate.
@@ -67,29 +69,31 @@
     - redefine official_number and company_id as long as name and type are kept
       as-is
 
     - redefine validation_date_column if the validation is not stored into
       self.date
     """
 
-    validation_date_column = 'date'
+    validation_date_column = "date"
 
     @declared_attr
     def official_number(cls):
         return Column(
             String(255),
             default=None,
+            info={"export": {"label": "N° de pièce"}},
         )
 
     @declared_attr
     def company_id(cls):
         return Column(
             Integer,
-            ForeignKey('company.id'),
+            ForeignKey("company.id"),
             nullable=False,
+            info={"export": {"exclude": True}},
         )
 
     @property
     def validation_date(self) -> datetime.date:
         return getattr(self, self.validation_date_column)
 
     @classmethod
@@ -109,37 +113,35 @@
       class or directly on instance.
 
     If both are defined, ``__acl__``, the more specific, is prefered.
 
     Use actual callables, not properties, in subclasses to prevent pyramid from
     silently ignoring any AttributeError your callable should trigger.
     """
+
     @declared_attr
     def _acl(cls):
         """
         Customizable _acl column
         """
         return Column(
             MutableList.as_mutable(ACLType),
-            info={
-                'colanderalchemy': {'exclude': True},
-                'export': {'exclude': True}
-            },
+            info={"colanderalchemy": {"exclude": True}, "export": {"exclude": True}},
         )
 
     def _get_acl(self):
         # Any AttributeError raised at this function level would be masked.
         # See https://github.com/Pylons/pyramid/pull/2613/files
-        if getattr(self, '_acl', None) is None:
+        if getattr(self, "_acl", None) is None:
             if getattr(self, "__default_acl__", None) is not None:
                 return self.__default_acl__
             elif getattr(self, "parent", None) is not None:
                 return self.parent.__acl__
             else:
-                raise AttributeError('__acl__')
+                raise AttributeError("__acl__")
         return self._acl
 
     def _set_acl(self, value):
         self._acl = value
 
     def _del_acl(self):
         self._acl = None
@@ -150,14 +152,15 @@
 class DuplicableMixin(object):
     """
     Factorize duplication logic on sqlalchemy models
 
     __duplicable_fields__ attr should contain the list of attributes to be
     copied from a model to its duplicate.
     """
+
     __duplicable_fields__ = None
 
     def duplicate(self, factory=None, **kwargs):
         """
         Duplicate all fields listed in __duplicable_fields__ plus optional
         ad-hoc values.
 
@@ -166,16 +169,15 @@
           new instance. They will take precedence over copied values.
         :returns: new instance combining fields copied from self, and ad-hoc
           args. The instance is not saved.
         """
 
         if self.__duplicable_fields__ is None:
             raise NotImplementedError(
-               "DuplicableMixin implementors should define "
-               + "__duplicable_fields__"
+                "DuplicableMixin implementors should define " + "__duplicable_fields__"
             )
 
         if factory is None:
             factory = self.__class__
 
         duplicate_obj = factory()
         for i in self.__duplicable_fields__:
```

### Comparing `endi_base-6.4.4/endi_base/models/types.py` & `endi_base-6.6.0/endi_base/models/types.py`

 * *Files identical despite different names*

### Comparing `endi_base-6.4.4/endi_base/models/utils.py` & `endi_base-6.6.0/endi_base/models/utils.py`

 * *Files identical despite different names*

### Comparing `endi_base-6.4.4/endi_base/utils/ascii.py` & `endi_base-6.6.0/endi_base/utils/ascii.py`

 * *Files identical despite different names*

### Comparing `endi_base-6.4.4/endi_base/utils/date.py` & `endi_base-6.6.0/endi_base/utils/date.py`

 * *Files identical despite different names*

### Comparing `endi_base-6.4.4/endi_base/utils/math.py` & `endi_base-6.6.0/endi_base/utils/math.py`

 * *Files identical despite different names*

### Comparing `endi_base-6.4.4/endi_base/utils/renderers.py` & `endi_base-6.6.0/endi_base/utils/renderers.py`

 * *Files identical despite different names*

### Comparing `endi_base-6.4.4/endi_base.egg-info/PKG-INFO` & `endi_base-6.6.0/endi_base.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: endi-base
-Version: 6.4.4
+Version: 6.6.0
 Summary: endi_base
 Home-page: https://framagit.org/endi/endi_base
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid endi
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Provides-Extra: testing
 License-File: LICENSE.txt
@@ -33,9 +32,7 @@
 * Custom SQLAlchemy column types
 * String formatting utilities
 * Date formatting utilities
 * Constants
 * ...
 
 It should not be installed directly but should be installed as a dependency
-
-
```

### Comparing `endi_base-6.4.4/endi_base.egg-info/SOURCES.txt` & `endi_base-6.6.0/endi_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `endi_base-6.4.4/setup.py` & `endi_base-6.6.0/setup.py`

 * *Files identical despite different names*

