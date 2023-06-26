# Comparing `tmp/bx_django_utils-8.tar.gz` & `tmp/bx_django_utils-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bx_django_utils-8.tar", max compression
+gzip compressed data, was "bx_django_utils-9.tar", max compression
```

## Comparing `bx_django_utils-8.tar` & `bx_django_utils-9.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0     1068 2021-11-18 08:53:35.584586 bx_django_utils-8/LICENSE
--rw-r--r--   0        0        0    11201 2021-11-18 08:53:35.584586 bx_django_utils-8/README.md
--rw-r--r--   0        0        0       18 2021-11-18 08:54:04.552705 bx_django_utils-8/bx_django_utils/__init__.py
--rw-r--r--   0        0        0      100 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/approve_workflow/__init__.py
--rw-r--r--   0        0        0     4025 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/approve_workflow/admin.py
--rw-r--r--   0        0        0       30 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/approve_workflow/constants.py
--rw-r--r--   0        0        0     1621 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/approve_workflow/forms.py
--rw-r--r--   0        0        0     1573 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/approve_workflow/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1798 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/approve_workflow/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1126 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/approve_workflow/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1625 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/approve_workflow/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8294 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/approve_workflow/models.py
--rw-r--r--   0        0        0      288 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/approve_workflow/templates/approve_workflow/change_form.html
--rw-r--r--   0        0        0     1186 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/approve_workflow/templates/approve_workflow/submit_line.html
--rw-r--r--   0        0        0        0 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/data_types/__init__.py
--rw-r--r--   0        0        0      754 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/data_types/gtin/README.md
--rw-r--r--   0        0        0       74 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/data_types/gtin/__init__.py
--rw-r--r--   0        0        0       85 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/data_types/gtin/constants.py
--rw-r--r--   0        0        0      974 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/data_types/gtin/form_fields.py
--rw-r--r--   0        0        0     1170 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/data_types/gtin/model_fields.py
--rw-r--r--   0        0        0     1584 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/data_types/gtin/validators.py
--rw-r--r--   0        0        0        0 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/dbperf/__init__.py
--rw-r--r--   0        0        0     3826 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/dbperf/cursor.py
--rw-r--r--   0        0        0     6229 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/dbperf/query_recorder.py
--rw-r--r--   0        0        0     1712 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/filename.py
--rw-r--r--   0        0        0        0 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/humanize/__init__.py
--rw-r--r--   0        0        0      641 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/humanize/pformat.py
--rw-r--r--   0        0        0     2003 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/humanize/time.py
--rw-r--r--   0        0        0     1772 2021-11-18 08:53:35.584586 bx_django_utils-8/bx_django_utils/json_utils.py
--rw-r--r--   0        0        0     1013 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1256 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      597 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1063 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/models/__init__.py
--rw-r--r--   0        0        0     1052 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/models/color_field.py
--rw-r--r--   0        0        0     7807 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/models/manipulate.py
--rw-r--r--   0        0        0     2256 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/models/timetracking.py
--rw-r--r--   0        0        0     3294 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/stacktrace.py
--rw-r--r--   0        0        0        0 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/templatetags/__init__.py
--rw-r--r--   0        0        0     1330 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/templatetags/humanize_time.py
--rw-r--r--   0        0        0       50 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/test_utils/__init__.py
--rw-r--r--   0        0        0     6602 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/test_utils/assert_queries.py
--rw-r--r--   0        0        0     1365 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/test_utils/datetime.py
--rw-r--r--   0        0        0     4676 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/test_utils/html_assertion.py
--rw-r--r--   0        0        0     2667 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/test_utils/model_clean_assert.py
--rw-r--r--   0        0        0     3987 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/test_utils/users.py
--rw-r--r--   0        0        0        0 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/view_utils/__init__.py
--rw-r--r--   0        0        0     1336 2021-11-18 08:53:35.588586 bx_django_utils-8/bx_django_utils/view_utils/dynamic_menu_urls.py
--rw-r--r--   0        0        0     3440 2021-11-18 08:56:30.221300 bx_django_utils-8/pyproject.toml
--rw-r--r--   0        0        0    12811 2021-11-18 08:56:33.719135 bx_django_utils-8/setup.py
--rw-r--r--   0        0        0    12160 2021-11-18 08:56:33.719797 bx_django_utils-8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2021-05-21 07:08:17.723145 bx_django_utils-9/LICENSE
+-rw-r--r--   0        0        0    11787 2021-11-18 11:58:36.111553 bx_django_utils-9/README.md
+-rw-r--r--   0        0        0       18 2021-11-18 11:59:13.175235 bx_django_utils-9/bx_django_utils/__init__.py
+-rw-r--r--   0        0        0      100 2021-05-31 10:25:20.490038 bx_django_utils-9/bx_django_utils/approve_workflow/__init__.py
+-rw-r--r--   0        0        0     4025 2021-05-31 10:26:32.125522 bx_django_utils-9/bx_django_utils/approve_workflow/admin.py
+-rw-r--r--   0        0        0       30 2021-05-21 07:08:17.723145 bx_django_utils-9/bx_django_utils/approve_workflow/constants.py
+-rw-r--r--   0        0        0     1621 2021-05-21 07:11:18.073966 bx_django_utils-9/bx_django_utils/approve_workflow/forms.py
+-rw-r--r--   0        0        0     1573 2021-05-21 07:08:17.723145 bx_django_utils-9/bx_django_utils/approve_workflow/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1798 2021-05-21 07:11:18.225965 bx_django_utils-9/bx_django_utils/approve_workflow/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1126 2021-05-21 07:08:17.723145 bx_django_utils-9/bx_django_utils/approve_workflow/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1625 2021-05-21 07:11:18.057966 bx_django_utils-9/bx_django_utils/approve_workflow/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8294 2021-05-21 07:11:18.197965 bx_django_utils-9/bx_django_utils/approve_workflow/models.py
+-rw-r--r--   0        0        0      288 2021-05-21 07:08:17.723145 bx_django_utils-9/bx_django_utils/approve_workflow/templates/approve_workflow/change_form.html
+-rw-r--r--   0        0        0     1186 2021-05-21 07:08:17.723145 bx_django_utils-9/bx_django_utils/approve_workflow/templates/approve_workflow/submit_line.html
+-rw-r--r--   0        0        0        0 2021-05-21 07:08:17.723145 bx_django_utils-9/bx_django_utils/data_types/__init__.py
+-rw-r--r--   0        0        0      754 2021-05-21 07:11:18.085966 bx_django_utils-9/bx_django_utils/data_types/gtin/README.md
+-rw-r--r--   0        0        0       74 2021-05-31 10:38:04.980338 bx_django_utils-9/bx_django_utils/data_types/gtin/__init__.py
+-rw-r--r--   0        0        0       85 2021-05-21 07:08:17.723145 bx_django_utils-9/bx_django_utils/data_types/gtin/constants.py
+-rw-r--r--   0        0        0      974 2021-06-01 06:50:05.631759 bx_django_utils-9/bx_django_utils/data_types/gtin/form_fields.py
+-rw-r--r--   0        0        0     1170 2021-05-31 10:28:02.584803 bx_django_utils-9/bx_django_utils/data_types/gtin/model_fields.py
+-rw-r--r--   0        0        0     1584 2021-05-21 07:11:18.041966 bx_django_utils-9/bx_django_utils/data_types/gtin/validators.py
+-rw-r--r--   0        0        0        0 2021-05-21 07:08:17.723145 bx_django_utils-9/bx_django_utils/dbperf/__init__.py
+-rw-r--r--   0        0        0     3826 2021-05-21 07:11:18.333964 bx_django_utils-9/bx_django_utils/dbperf/cursor.py
+-rw-r--r--   0        0        0     6229 2021-05-21 07:11:18.149965 bx_django_utils-9/bx_django_utils/dbperf/query_recorder.py
+-rw-r--r--   0        0        0     1712 2021-05-31 10:37:54.584412 bx_django_utils-9/bx_django_utils/filename.py
+-rw-r--r--   0        0        0        0 2021-05-21 07:08:17.727145 bx_django_utils-9/bx_django_utils/humanize/__init__.py
+-rw-r--r--   0        0        0      641 2021-05-31 10:39:16.559830 bx_django_utils-9/bx_django_utils/humanize/pformat.py
+-rw-r--r--   0        0        0     2003 2021-09-27 10:08:38.492658 bx_django_utils-9/bx_django_utils/humanize/time.py
+-rw-r--r--   0        0        0     1772 2021-11-03 09:18:38.601714 bx_django_utils-9/bx_django_utils/json_utils.py
+-rw-r--r--   0        0        0     1013 2021-05-21 07:08:17.727145 bx_django_utils-9/bx_django_utils/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1256 2021-05-21 07:11:18.185965 bx_django_utils-9/bx_django_utils/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      597 2021-05-21 07:08:17.727145 bx_django_utils-9/bx_django_utils/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1063 2021-05-21 07:11:18.361964 bx_django_utils-9/bx_django_utils/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2021-05-21 07:08:17.727145 bx_django_utils-9/bx_django_utils/models/__init__.py
+-rw-r--r--   0        0        0     1052 2021-11-18 11:05:36.108954 bx_django_utils-9/bx_django_utils/models/color_field.py
+-rw-r--r--   0        0        0     7807 2021-11-18 11:05:36.108954 bx_django_utils-9/bx_django_utils/models/manipulate.py
+-rw-r--r--   0        0        0      679 2021-11-18 11:05:36.128954 bx_django_utils-9/bx_django_utils/models/queryset_utils.py
+-rw-r--r--   0        0        0     2256 2021-05-21 07:11:18.137966 bx_django_utils-9/bx_django_utils/models/timetracking.py
+-rw-r--r--   0        0        0     3294 2021-05-21 07:11:18.317964 bx_django_utils-9/bx_django_utils/stacktrace.py
+-rw-r--r--   0        0        0        0 2021-05-21 07:08:17.727145 bx_django_utils-9/bx_django_utils/templatetags/__init__.py
+-rw-r--r--   0        0        0     1330 2021-11-03 08:59:25.950570 bx_django_utils-9/bx_django_utils/templatetags/humanize_time.py
+-rw-r--r--   0        0        0       50 2021-05-31 10:35:29.693452 bx_django_utils-9/bx_django_utils/test_utils/__init__.py
+-rw-r--r--   0        0        0     6602 2021-05-31 10:35:29.685452 bx_django_utils-9/bx_django_utils/test_utils/assert_queries.py
+-rw-r--r--   0        0        0     1365 2021-05-31 10:41:10.355028 bx_django_utils-9/bx_django_utils/test_utils/datetime.py
+-rw-r--r--   0        0        0     4676 2021-06-10 07:40:36.699496 bx_django_utils-9/bx_django_utils/test_utils/html_assertion.py
+-rw-r--r--   0        0        0     2667 2021-05-21 07:08:17.727145 bx_django_utils-9/bx_django_utils/test_utils/model_clean_assert.py
+-rw-r--r--   0        0        0     3987 2021-05-31 10:37:54.576412 bx_django_utils-9/bx_django_utils/test_utils/users.py
+-rw-r--r--   0        0        0        0 2021-05-21 07:08:17.727145 bx_django_utils-9/bx_django_utils/view_utils/__init__.py
+-rw-r--r--   0        0        0     1336 2021-05-21 07:11:18.077966 bx_django_utils-9/bx_django_utils/view_utils/dynamic_menu_urls.py
+-rw-r--r--   0        0        0     3440 2021-11-18 11:59:47.198943 bx_django_utils-9/pyproject.toml
+-rw-r--r--   0        0        0    13407 2021-11-18 11:59:52.138788 bx_django_utils-9/setup.py
+-rw-r--r--   0        0        0    12695 2021-11-18 11:59:52.139405 bx_django_utils-9/PKG-INFO
```

### Comparing `bx_django_utils-8/LICENSE` & `bx_django_utils-9/LICENSE`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/README.md` & `bx_django_utils-9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,18 @@
 
 * [`CreateOrUpdateResult()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L39-L63) - Result object returned by create_or_update2() with all information about create/save a model.
 * [`InvalidStoreBehavior()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L19-L23) - Exception used in create_or_update() if "store_behavior" contains not existing field names.
 * [`create()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L26-L36) - Create a new model instance with optional validate before create.
 * [`create_or_update()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L197-L217) - Create a new model instance or update a existing one. Deprecated! Use: create_or_update2()
 * [`create_or_update2()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L66-L194) - Create a new model instance or update a existing one and returns CreateOrUpdateResult instance
 
+#### bx_django_utils.models.queryset_utils
+
+* [`remove_filter()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/queryset_utils.py#L6-L23) - Remove a applied .filter() from a QuerySet
+
 #### bx_django_utils.models.timetracking
 
 * [`TimetrackingBaseModel()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/timetracking.py#L8-L62) - Abstract base model that will automaticly set create/update Datetimes.
 
 ### bx_django_utils.stacktrace
 
 * [`StackTrace()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/stacktrace.py#L21-L22) - Built-in mutable sequence.
@@ -186,10 +190,16 @@
 ...and start the test server again ;)
 
 
 ## License
 
 [MIT](LICENSE). Patches welcome!
 
+## About us
+
+We’ve been rethinking the listening experience for kids and have created an ecosystem where haptic and listening experience are combined via smart technology - the Toniebox.
+
+We are constantly looking for engineers to join our team in different areas. If you’d be interested in contributing to our platform, have a look at: https://tonies.com/jobs/
+    
 ## Links
 
 * https://pypi.org/project/bx-django-utils/
```

### Comparing `bx_django_utils-8/bx_django_utils/approve_workflow/admin.py` & `bx_django_utils-9/bx_django_utils/approve_workflow/admin.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/approve_workflow/forms.py` & `bx_django_utils-9/bx_django_utils/approve_workflow/forms.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/approve_workflow/locale/de/LC_MESSAGES/django.mo` & `bx_django_utils-9/bx_django_utils/approve_workflow/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/approve_workflow/locale/de/LC_MESSAGES/django.po` & `bx_django_utils-9/bx_django_utils/approve_workflow/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/approve_workflow/locale/en/LC_MESSAGES/django.mo` & `bx_django_utils-9/bx_django_utils/approve_workflow/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/approve_workflow/locale/en/LC_MESSAGES/django.po` & `bx_django_utils-9/bx_django_utils/approve_workflow/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/approve_workflow/models.py` & `bx_django_utils-9/bx_django_utils/approve_workflow/models.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/approve_workflow/templates/approve_workflow/submit_line.html` & `bx_django_utils-9/bx_django_utils/approve_workflow/templates/approve_workflow/submit_line.html`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/data_types/gtin/README.md` & `bx_django_utils-9/bx_django_utils/data_types/gtin/README.md`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/data_types/gtin/form_fields.py` & `bx_django_utils-9/bx_django_utils/data_types/gtin/form_fields.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/data_types/gtin/model_fields.py` & `bx_django_utils-9/bx_django_utils/data_types/gtin/model_fields.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/data_types/gtin/validators.py` & `bx_django_utils-9/bx_django_utils/data_types/gtin/validators.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/dbperf/cursor.py` & `bx_django_utils-9/bx_django_utils/dbperf/cursor.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/dbperf/query_recorder.py` & `bx_django_utils-9/bx_django_utils/dbperf/query_recorder.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/filename.py` & `bx_django_utils-9/bx_django_utils/filename.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/humanize/pformat.py` & `bx_django_utils-9/bx_django_utils/humanize/pformat.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/humanize/time.py` & `bx_django_utils-9/bx_django_utils/humanize/time.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/json_utils.py` & `bx_django_utils-9/bx_django_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/locale/de/LC_MESSAGES/django.mo` & `bx_django_utils-9/bx_django_utils/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/locale/de/LC_MESSAGES/django.po` & `bx_django_utils-9/bx_django_utils/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/locale/en/LC_MESSAGES/django.mo` & `bx_django_utils-9/bx_django_utils/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/locale/en/LC_MESSAGES/django.po` & `bx_django_utils-9/bx_django_utils/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/models/color_field.py` & `bx_django_utils-9/bx_django_utils/models/color_field.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/models/manipulate.py` & `bx_django_utils-9/bx_django_utils/models/manipulate.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/models/timetracking.py` & `bx_django_utils-9/bx_django_utils/models/timetracking.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/stacktrace.py` & `bx_django_utils-9/bx_django_utils/stacktrace.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/templatetags/humanize_time.py` & `bx_django_utils-9/bx_django_utils/templatetags/humanize_time.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/test_utils/assert_queries.py` & `bx_django_utils-9/bx_django_utils/test_utils/assert_queries.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/test_utils/datetime.py` & `bx_django_utils-9/bx_django_utils/test_utils/datetime.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/test_utils/html_assertion.py` & `bx_django_utils-9/bx_django_utils/test_utils/html_assertion.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/test_utils/model_clean_assert.py` & `bx_django_utils-9/bx_django_utils/test_utils/model_clean_assert.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/test_utils/users.py` & `bx_django_utils-9/bx_django_utils/test_utils/users.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/bx_django_utils/view_utils/dynamic_menu_urls.py` & `bx_django_utils-9/bx_django_utils/view_utils/dynamic_menu_urls.py`

 * *Files identical despite different names*

### Comparing `bx_django_utils-8/pyproject.toml` & `bx_django_utils-9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'bx_django_utils'
-version = "8"
+version = "9"
 description = 'Various Django utility functions'
 homepage = "https://github.com/boxine/bx_django_utils/"
 authors = [
     'Jens Diemer <jens.diemer@boxine.de>',
     'Philipp Hagemeister <phihag@phihag.de>',
     'Florian Braun <mail@chiron-online.de>'
 ]
```

### Comparing `bx_django_utils-8/setup.py` & `bx_django_utils-9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
 entry_points = \
 {'console_scripts': ['publish = '
                      'bx_django_utils_tests.test_project.publish:publish']}
 
 setup_kwargs = {
     'name': 'bx-django-utils',
-    'version': '8',
+    'version': '9',
     'description': 'Various Django utility functions',
-    'long_description': '# Boxine - bx_django_utils\n\nVarious Django utility functions\n\n\n## Quickstart\n\n```bash\npip install bx_django_utils\n```\n\n\n## Existing stuff\n\nHere only a simple list about existing utilities.\nPlease take a look into the sources and tests for deeper informations.\n\n[comment]: <> (✂✂✂ auto generated start ✂✂✂)\n\n### bx_django_utils.approve_workflow\n\nBase model/admin/form classes to implement a model with draft/approve versions workflow\n\n\n#### bx_django_utils.approve_workflow.admin\n\n* [`BaseApproveModelAdmin()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/approve_workflow/admin.py#L15-L107) - Base admin class for a draft/approve Model\n\n#### bx_django_utils.approve_workflow.forms\n\n* [`PublishAdminForm()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/approve_workflow/forms.py#L7-L46) - Activate models REQUIRED_FIELDS_PUBLIC on approve\n\n#### bx_django_utils.approve_workflow.models\n\n* [`BaseApproveModel()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/approve_workflow/models.py#L14-L202) - Base model class for approve models *and* this relation models.\n* [`BaseApproveWorkflowModel()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/approve_workflow/models.py#L205-L255) - Base model for approve workflow models.\n\n#### bx_django_utils.data_types.gtin\n\nModelField, FormField and validators for GTIN/UPC/EAN numbers\n\n\n##### bx_django_utils.data_types.gtin.form_fields\n\n* [`GtinFormField()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/data_types/gtin/form_fields.py#L8-L28) - Form field with GTIN validator.\n\n##### bx_django_utils.data_types.gtin.model_fields\n\n* [`GtinModelField()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/data_types/gtin/model_fields.py#L10-L33) - GTIN model field\n\n##### bx_django_utils.data_types.gtin.validators\n\n* [`GtinValidator()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/data_types/gtin/validators.py#L33-L52) - Validate GTIN number\n* [`validate_gtin()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/data_types/gtin/validators.py#L12-L30) - It\'s the same as stdnum.ean.validate() but also accept ISBN-10\n\n#### bx_django_utils.dbperf.cursor\n\n* [`RecordingCursorWrapper()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/dbperf/cursor.py#L17-L115) - An implementation of django.db.backends.utils.CursorWrapper.\n\n#### bx_django_utils.dbperf.query_recorder\n\n* [`SQLQueryRecorder()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/dbperf/query_recorder.py#L95-L167) - A context manager that allows recording SQL queries executed during its lifetime.\n\n### bx_django_utils.filename\n\n* [`clean_filename()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/filename.py#L34-L64) - Convert filename to ASCII only via slugify.\n* [`filename2human_name()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/filename.py#L7-L31) - Convert filename to a capitalized name.\n\n#### bx_django_utils.humanize.pformat\n\n* [`pformat()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/humanize/pformat.py#L6-L20) - Better `pretty-print-format` using `DjangoJSONEncoder` with fallback to `pprint.pformat()`\n\n#### bx_django_utils.humanize.time\n\n* [`human_timedelta()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/humanize/time.py#L18-L63) - Converts a time duration into a friendly text representation. (`X ms`, `sec`, `minutes` etc.)\n\n### bx_django_utils.json_utils\n\n* [`make_json_serializable()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/json_utils.py#L20-L37) - Convert value to a JSON serializable value, with convert callback for special objects.\n* [`to_json()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/json_utils.py#L40-L56) - Convert value to JSON via make_json_serializable() and DjangoJSONEncoder()\n\n#### bx_django_utils.models.color_field\n\n* [`ColorModelField()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/color_field.py#L14-L29) - Hex color model field, e.g.: "#0055ff" (It\'s not a html color picker widget)\n* [`HexColorValidator()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/color_field.py#L6-L11) - Hex color validator (seven-character hexadecimal notation, e.g.: "#0055ff")\n\n#### bx_django_utils.models.manipulate\n\nUtilities to manipulate objects in database via models:\n\n* [`CreateOrUpdateResult()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L39-L63) - Result object returned by create_or_update2() with all information about create/save a model.\n* [`InvalidStoreBehavior()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L19-L23) - Exception used in create_or_update() if "store_behavior" contains not existing field names.\n* [`create()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L26-L36) - Create a new model instance with optional validate before create.\n* [`create_or_update()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L197-L217) - Create a new model instance or update a existing one. Deprecated! Use: create_or_update2()\n* [`create_or_update2()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L66-L194) - Create a new model instance or update a existing one and returns CreateOrUpdateResult instance\n\n#### bx_django_utils.models.timetracking\n\n* [`TimetrackingBaseModel()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/timetracking.py#L8-L62) - Abstract base model that will automaticly set create/update Datetimes.\n\n### bx_django_utils.stacktrace\n\n* [`StackTrace()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/stacktrace.py#L21-L22) - Built-in mutable sequence.\n* [`StacktraceAfter()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/stacktrace.py#L83-L111) - Generate a stack trace after a package was visited.\n* [`get_stacktrace()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/stacktrace.py#L63-L80) - Returns a StackTrace object, which is a list of FrameInfo objects.\n\n#### bx_django_utils.templatetags.humanize_time\n\n* [`human_duration()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/templatetags/humanize_time.py#L15-L45) - Verbose time since template tag, e.g.: `<span title="Jan. 1, 2000, noon">2.0 seconds</span>`\n\n### bx_django_utils.test_utils\n\nUtilities / helper for writing tests.\n\n\n#### bx_django_utils.test_utils.assert_queries\n\n* [`AssertQueries()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/assert_queries.py#L30-L200) - Assert executed database queries: Check table names, duplicate/similar Queries.\n\n#### bx_django_utils.test_utils.datetime\n\n* [`MockDatetimeGenerator()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/datetime.py#L4-L50) - Mock django `timezone.now()` with generic time stamps in tests.\n\n#### bx_django_utils.test_utils.html_assertion\n\n* [`HtmlAssertionMixin()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/html_assertion.py#L29-L127) - Unittest mixin class with useful assertments around Django test client tests\n* [`assert_html_response_snapshot()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/html_assertion.py#L9-L26) - Assert a HttpResponse via snapshot file. (Strip all empty lines from html)\n\n#### bx_django_utils.test_utils.model_clean_assert\n\n* [`AssertModelCleanCalled()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/model_clean_assert.py#L35-L86) - Context manager for assert that full_clean() was called for every model instance.\n* [`CleanMock()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/model_clean_assert.py#L6-L32) - Track if full_clean() was called.\n\n#### bx_django_utils.test_utils.users\n\n* [`assert_permissions()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/users.py#L29-L44) - Check user permissions.\n* [`filter_permission_names()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/users.py#L8-L26) - Generate a Permission model query filtered by names, e.g.: [\'<app_label>.<codename>\', ...]\n* [`make_max_test_user()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/users.py#L106-L140) - Create a test user with all permissions *except* the {exclude_permissions} ones.\n* [`make_minimal_test_user()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/users.py#L79-L103) - Create a test user and set given permissions.\n* [`make_test_user()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/users.py#L47-L76) - Create a test user and set given permissions.\n\n#### bx_django_utils.view_utils.dynamic_menu_urls\n\n* [`DynamicViewMenu()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/view_utils/dynamic_menu_urls.py#L4-L45) - Simple storage for store information about views/urls to build a menu.\n\n[comment]: <> (✂✂✂ auto generated end ✂✂✂)\n\n## developing\n\nTo start developing e.g.:\n\n```bash\n~$ git clone https://github.com/boxine/bx_django_utils.git\n~$ cd bx_django_utils\n~/bx_django_utils$ make\nhelp                 List all commands\ninstall-poetry       install or update poetry\ninstall              install via poetry\nupdate               Update the dependencies as according to the pyproject.toml file\nlint                 Run code formatters and linter\nfix-code-style       Fix code formatting\ntox-listenvs         List all tox test environments\ntox                  Run pytest via tox with all environments\ntox-py36             Run pytest via tox with *python v3.6*\ntox-py37             Run pytest via tox with *python v3.7*\ntox-py38             Run pytest via tox with *python v3.8*\ntox-py39             Run pytest via tox with *python v3.9*\npytest               Run pytest\npytest-ci            Run pytest with CI settings\npublish              Release new version to PyPi\nmakemessages         Make and compile locales message files\nstart-dev-server     Start Django dev. server with the test project\nclean                Remove created files from the test project (e.g.: SQlite, static files)\n```\n\nYou can start the test project with the Django developing server, e.g.:\n```bash\n~/bx_django_utils$ make start-dev-server\n```\nThis is a own manage command, that will create migrations files from our test app, migrate, collectstatic and create a super user if no user exists ;)\n\nIf you like to start from stretch, just delete related test project files with:\n```bash\n~/bx_django_utils$ make clean\n```\n...and start the test server again ;)\n\n\n## License\n\n[MIT](LICENSE). Patches welcome!\n\n## Links\n\n* https://pypi.org/project/bx-django-utils/\n',
+    'long_description': '# Boxine - bx_django_utils\n\nVarious Django utility functions\n\n\n## Quickstart\n\n```bash\npip install bx_django_utils\n```\n\n\n## Existing stuff\n\nHere only a simple list about existing utilities.\nPlease take a look into the sources and tests for deeper informations.\n\n[comment]: <> (✂✂✂ auto generated start ✂✂✂)\n\n### bx_django_utils.approve_workflow\n\nBase model/admin/form classes to implement a model with draft/approve versions workflow\n\n\n#### bx_django_utils.approve_workflow.admin\n\n* [`BaseApproveModelAdmin()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/approve_workflow/admin.py#L15-L107) - Base admin class for a draft/approve Model\n\n#### bx_django_utils.approve_workflow.forms\n\n* [`PublishAdminForm()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/approve_workflow/forms.py#L7-L46) - Activate models REQUIRED_FIELDS_PUBLIC on approve\n\n#### bx_django_utils.approve_workflow.models\n\n* [`BaseApproveModel()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/approve_workflow/models.py#L14-L202) - Base model class for approve models *and* this relation models.\n* [`BaseApproveWorkflowModel()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/approve_workflow/models.py#L205-L255) - Base model for approve workflow models.\n\n#### bx_django_utils.data_types.gtin\n\nModelField, FormField and validators for GTIN/UPC/EAN numbers\n\n\n##### bx_django_utils.data_types.gtin.form_fields\n\n* [`GtinFormField()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/data_types/gtin/form_fields.py#L8-L28) - Form field with GTIN validator.\n\n##### bx_django_utils.data_types.gtin.model_fields\n\n* [`GtinModelField()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/data_types/gtin/model_fields.py#L10-L33) - GTIN model field\n\n##### bx_django_utils.data_types.gtin.validators\n\n* [`GtinValidator()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/data_types/gtin/validators.py#L33-L52) - Validate GTIN number\n* [`validate_gtin()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/data_types/gtin/validators.py#L12-L30) - It\'s the same as stdnum.ean.validate() but also accept ISBN-10\n\n#### bx_django_utils.dbperf.cursor\n\n* [`RecordingCursorWrapper()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/dbperf/cursor.py#L17-L115) - An implementation of django.db.backends.utils.CursorWrapper.\n\n#### bx_django_utils.dbperf.query_recorder\n\n* [`SQLQueryRecorder()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/dbperf/query_recorder.py#L95-L167) - A context manager that allows recording SQL queries executed during its lifetime.\n\n### bx_django_utils.filename\n\n* [`clean_filename()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/filename.py#L34-L64) - Convert filename to ASCII only via slugify.\n* [`filename2human_name()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/filename.py#L7-L31) - Convert filename to a capitalized name.\n\n#### bx_django_utils.humanize.pformat\n\n* [`pformat()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/humanize/pformat.py#L6-L20) - Better `pretty-print-format` using `DjangoJSONEncoder` with fallback to `pprint.pformat()`\n\n#### bx_django_utils.humanize.time\n\n* [`human_timedelta()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/humanize/time.py#L18-L63) - Converts a time duration into a friendly text representation. (`X ms`, `sec`, `minutes` etc.)\n\n### bx_django_utils.json_utils\n\n* [`make_json_serializable()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/json_utils.py#L20-L37) - Convert value to a JSON serializable value, with convert callback for special objects.\n* [`to_json()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/json_utils.py#L40-L56) - Convert value to JSON via make_json_serializable() and DjangoJSONEncoder()\n\n#### bx_django_utils.models.color_field\n\n* [`ColorModelField()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/color_field.py#L14-L29) - Hex color model field, e.g.: "#0055ff" (It\'s not a html color picker widget)\n* [`HexColorValidator()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/color_field.py#L6-L11) - Hex color validator (seven-character hexadecimal notation, e.g.: "#0055ff")\n\n#### bx_django_utils.models.manipulate\n\nUtilities to manipulate objects in database via models:\n\n* [`CreateOrUpdateResult()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L39-L63) - Result object returned by create_or_update2() with all information about create/save a model.\n* [`InvalidStoreBehavior()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L19-L23) - Exception used in create_or_update() if "store_behavior" contains not existing field names.\n* [`create()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L26-L36) - Create a new model instance with optional validate before create.\n* [`create_or_update()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L197-L217) - Create a new model instance or update a existing one. Deprecated! Use: create_or_update2()\n* [`create_or_update2()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L66-L194) - Create a new model instance or update a existing one and returns CreateOrUpdateResult instance\n\n#### bx_django_utils.models.queryset_utils\n\n* [`remove_filter()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/queryset_utils.py#L6-L23) - Remove a applied .filter() from a QuerySet\n\n#### bx_django_utils.models.timetracking\n\n* [`TimetrackingBaseModel()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/timetracking.py#L8-L62) - Abstract base model that will automaticly set create/update Datetimes.\n\n### bx_django_utils.stacktrace\n\n* [`StackTrace()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/stacktrace.py#L21-L22) - Built-in mutable sequence.\n* [`StacktraceAfter()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/stacktrace.py#L83-L111) - Generate a stack trace after a package was visited.\n* [`get_stacktrace()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/stacktrace.py#L63-L80) - Returns a StackTrace object, which is a list of FrameInfo objects.\n\n#### bx_django_utils.templatetags.humanize_time\n\n* [`human_duration()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/templatetags/humanize_time.py#L15-L45) - Verbose time since template tag, e.g.: `<span title="Jan. 1, 2000, noon">2.0 seconds</span>`\n\n### bx_django_utils.test_utils\n\nUtilities / helper for writing tests.\n\n\n#### bx_django_utils.test_utils.assert_queries\n\n* [`AssertQueries()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/assert_queries.py#L30-L200) - Assert executed database queries: Check table names, duplicate/similar Queries.\n\n#### bx_django_utils.test_utils.datetime\n\n* [`MockDatetimeGenerator()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/datetime.py#L4-L50) - Mock django `timezone.now()` with generic time stamps in tests.\n\n#### bx_django_utils.test_utils.html_assertion\n\n* [`HtmlAssertionMixin()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/html_assertion.py#L29-L127) - Unittest mixin class with useful assertments around Django test client tests\n* [`assert_html_response_snapshot()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/html_assertion.py#L9-L26) - Assert a HttpResponse via snapshot file. (Strip all empty lines from html)\n\n#### bx_django_utils.test_utils.model_clean_assert\n\n* [`AssertModelCleanCalled()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/model_clean_assert.py#L35-L86) - Context manager for assert that full_clean() was called for every model instance.\n* [`CleanMock()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/model_clean_assert.py#L6-L32) - Track if full_clean() was called.\n\n#### bx_django_utils.test_utils.users\n\n* [`assert_permissions()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/users.py#L29-L44) - Check user permissions.\n* [`filter_permission_names()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/users.py#L8-L26) - Generate a Permission model query filtered by names, e.g.: [\'<app_label>.<codename>\', ...]\n* [`make_max_test_user()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/users.py#L106-L140) - Create a test user with all permissions *except* the {exclude_permissions} ones.\n* [`make_minimal_test_user()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/users.py#L79-L103) - Create a test user and set given permissions.\n* [`make_test_user()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/test_utils/users.py#L47-L76) - Create a test user and set given permissions.\n\n#### bx_django_utils.view_utils.dynamic_menu_urls\n\n* [`DynamicViewMenu()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/view_utils/dynamic_menu_urls.py#L4-L45) - Simple storage for store information about views/urls to build a menu.\n\n[comment]: <> (✂✂✂ auto generated end ✂✂✂)\n\n## developing\n\nTo start developing e.g.:\n\n```bash\n~$ git clone https://github.com/boxine/bx_django_utils.git\n~$ cd bx_django_utils\n~/bx_django_utils$ make\nhelp                 List all commands\ninstall-poetry       install or update poetry\ninstall              install via poetry\nupdate               Update the dependencies as according to the pyproject.toml file\nlint                 Run code formatters and linter\nfix-code-style       Fix code formatting\ntox-listenvs         List all tox test environments\ntox                  Run pytest via tox with all environments\ntox-py36             Run pytest via tox with *python v3.6*\ntox-py37             Run pytest via tox with *python v3.7*\ntox-py38             Run pytest via tox with *python v3.8*\ntox-py39             Run pytest via tox with *python v3.9*\npytest               Run pytest\npytest-ci            Run pytest with CI settings\npublish              Release new version to PyPi\nmakemessages         Make and compile locales message files\nstart-dev-server     Start Django dev. server with the test project\nclean                Remove created files from the test project (e.g.: SQlite, static files)\n```\n\nYou can start the test project with the Django developing server, e.g.:\n```bash\n~/bx_django_utils$ make start-dev-server\n```\nThis is a own manage command, that will create migrations files from our test app, migrate, collectstatic and create a super user if no user exists ;)\n\nIf you like to start from stretch, just delete related test project files with:\n```bash\n~/bx_django_utils$ make clean\n```\n...and start the test server again ;)\n\n\n## License\n\n[MIT](LICENSE). Patches welcome!\n\n## About us\n\nWe’ve been rethinking the listening experience for kids and have created an ecosystem where haptic and listening experience are combined via smart technology - the Toniebox.\n\nWe are constantly looking for engineers to join our team in different areas. If you’d be interested in contributing to our platform, have a look at: https://tonies.com/jobs/\n    \n## Links\n\n* https://pypi.org/project/bx-django-utils/\n',
     'author': 'Jens Diemer',
     'author_email': 'jens.diemer@boxine.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/boxine/bx_django_utils/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `bx_django_utils-8/PKG-INFO` & `bx_django_utils-9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: bx-django-utils
-Version: 8
+Version: 9
 Summary: Various Django utility functions
 Home-page: https://github.com/boxine/bx_django_utils/
 License: MIT
 Keywords: django,utilities
 Author: Jens Diemer
 Author-email: jens.diemer@boxine.de
 Requires-Python: >=3.6,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: bx_py_utils (>=41)
 Requires-Dist: django
@@ -116,14 +115,18 @@
 
 * [`CreateOrUpdateResult()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L39-L63) - Result object returned by create_or_update2() with all information about create/save a model.
 * [`InvalidStoreBehavior()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L19-L23) - Exception used in create_or_update() if "store_behavior" contains not existing field names.
 * [`create()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L26-L36) - Create a new model instance with optional validate before create.
 * [`create_or_update()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L197-L217) - Create a new model instance or update a existing one. Deprecated! Use: create_or_update2()
 * [`create_or_update2()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/manipulate.py#L66-L194) - Create a new model instance or update a existing one and returns CreateOrUpdateResult instance
 
+#### bx_django_utils.models.queryset_utils
+
+* [`remove_filter()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/queryset_utils.py#L6-L23) - Remove a applied .filter() from a QuerySet
+
 #### bx_django_utils.models.timetracking
 
 * [`TimetrackingBaseModel()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/models/timetracking.py#L8-L62) - Abstract base model that will automaticly set create/update Datetimes.
 
 ### bx_django_utils.stacktrace
 
 * [`StackTrace()`](https://github.com/boxine/bx_django_utils/blob/master/bx_django_utils/stacktrace.py#L21-L22) - Built-in mutable sequence.
@@ -212,11 +215,17 @@
 ...and start the test server again ;)
 
 
 ## License
 
 [MIT](LICENSE). Patches welcome!
 
+## About us
+
+We’ve been rethinking the listening experience for kids and have created an ecosystem where haptic and listening experience are combined via smart technology - the Toniebox.
+
+We are constantly looking for engineers to join our team in different areas. If you’d be interested in contributing to our platform, have a look at: https://tonies.com/jobs/
+    
 ## Links
 
 * https://pypi.org/project/bx-django-utils/
```

