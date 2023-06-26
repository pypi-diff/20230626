# Comparing `tmp/trycourier-4.4.0.tar.gz` & `tmp/trycourier-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycourier-4.4.0.tar", last modified: Wed Aug  3 21:55:53 2022, max compression
+gzip compressed data, was "trycourier-4.5.0.tar", last modified: Mon Jun 26 21:20:05 2023, max compression
```

## Comparing `trycourier-4.4.0.tar` & `trycourier-4.5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 21:55:53.109073 trycourier-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-08-03 21:55:42.000000 trycourier-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15375 2022-08-03 21:55:53.109073 trycourier-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14875 2022-08-03 21:55:42.000000 trycourier-4.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-03 21:55:53.109073 trycourier-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-08-03 21:55:42.000000 trycourier-4.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 21:55:53.109073 trycourier-4.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 21:55:42.000000 trycourier-4.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5554 2022-08-03 21:55:42.000000 trycourier-4.4.0/tests/test_audiences.py
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2022-08-03 21:55:42.000000 trycourier-4.4.0/tests/test_audit_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-08-03 21:55:42.000000 trycourier-4.4.0/tests/test_automations.py
--rw-r--r--   0 runner    (1001) docker     (121)     6449 2022-08-03 21:55:42.000000 trycourier-4.4.0/tests/test_bulk.py
--rw-r--r--   0 runner    (1001) docker     (121)    23714 2022-08-03 21:55:42.000000 trycourier-4.4.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-08-03 21:55:42.000000 trycourier-4.4.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    12202 2022-08-03 21:55:42.000000 trycourier-4.4.0/tests/test_lists.py
--rw-r--r--   0 runner    (1001) docker     (121)     3532 2022-08-03 21:55:42.000000 trycourier-4.4.0/tests/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     6104 2022-08-03 21:55:42.000000 trycourier-4.4.0/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     6223 2022-08-03 21:55:42.000000 trycourier-4.4.0/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-08-03 21:55:42.000000 trycourier-4.4.0/tests/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 21:55:53.109073 trycourier-4.4.0/trycourier/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-08-03 21:55:42.000000 trycourier-4.4.0/trycourier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2941 2022-08-03 21:55:42.000000 trycourier-4.4.0/trycourier/audiences.py
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-08-03 21:55:42.000000 trycourier-4.4.0/trycourier/audit_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     3873 2022-08-03 21:55:42.000000 trycourier-4.4.0/trycourier/automations.py
--rw-r--r--   0 runner    (1001) docker     (121)     5456 2022-08-03 21:55:42.000000 trycourier-4.4.0/trycourier/bulk.py
--rw-r--r--   0 runner    (1001) docker     (121)    17516 2022-08-03 21:55:42.000000 trycourier-4.4.0/trycourier/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-08-03 21:55:42.000000 trycourier-4.4.0/trycourier/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9441 2022-08-03 21:55:42.000000 trycourier-4.4.0/trycourier/lists.py
--rw-r--r--   0 runner    (1001) docker     (121)     3564 2022-08-03 21:55:42.000000 trycourier-4.4.0/trycourier/messages.py
--rw-r--r--   0 runner    (1001) docker     (121)    10966 2022-08-03 21:55:42.000000 trycourier-4.4.0/trycourier/notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     4839 2022-08-03 21:55:42.000000 trycourier-4.4.0/trycourier/profiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-08-03 21:55:42.000000 trycourier-4.4.0/trycourier/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 21:55:53.109073 trycourier-4.4.0/trycourier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15375 2022-08-03 21:55:53.000000 trycourier-4.4.0/trycourier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-08-03 21:55:53.000000 trycourier-4.4.0/trycourier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 21:55:53.000000 trycourier-4.4.0/trycourier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-03 21:55:53.000000 trycourier-4.4.0/trycourier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-03 21:55:53.000000 trycourier-4.4.0/trycourier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:20:05.131554 trycourier-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-26 21:19:49.000000 trycourier-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-06-26 21:20:05.131554 trycourier-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-06-26 21:19:49.000000 trycourier-4.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:20:05.131554 trycourier-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-26 21:19:49.000000 trycourier-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:20:05.127554 trycourier-4.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_audiences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_audit_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_automations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23714 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-26 21:19:49.000000 trycourier-4.5.0/tests/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:20:05.131554 trycourier-4.5.0/trycourier/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/audiences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/audit_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/automations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17516 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-26 21:19:49.000000 trycourier-4.5.0/trycourier/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:20:05.131554 trycourier-4.5.0/trycourier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-06-26 21:20:05.000000 trycourier-4.5.0/trycourier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-26 21:20:05.000000 trycourier-4.5.0/trycourier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:20:05.000000 trycourier-4.5.0/trycourier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 21:20:05.000000 trycourier-4.5.0/trycourier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 21:20:05.000000 trycourier-4.5.0/trycourier.egg-info/top_level.txt
```

### Comparing `trycourier-4.4.0/LICENSE` & `trycourier-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/PKG-INFO` & `trycourier-4.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: trycourier
-Version: 4.4.0
+Version: 4.5.0
 Summary: A Python Package for communicating with the Courier REST API.
 Home-page: https://github.com/trycourier/courier-python
 Author: Courier
 Author-email: support@courier.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -681,9 +679,7 @@
 ## Contributing
 
 Bug reports and pull requests are welcome on GitHub at https://github.com/trycourier/courier-python. See [CONTRIBUTING.md](CONTRIBUTING.md) for more info.
 
 ## License
 
 The package is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
-
-
```

### Comparing `trycourier-4.4.0/README.md` & `trycourier-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/setup.py` & `trycourier-4.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="trycourier",
-    version="4.4.0",
+    version="4.5.0",
     author="Courier",
     author_email="support@courier.com",
     description="A Python Package for communicating with the Courier REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/trycourier/courier-python",
     packages=setuptools.find_packages(),
```

### Comparing `trycourier-4.4.0/tests/test_audiences.py` & `trycourier-4.5.0/tests/test_audiences.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/tests/test_audit_events.py` & `trycourier-4.5.0/tests/test_audit_events.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/tests/test_automations.py` & `trycourier-4.5.0/tests/test_automations.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/tests/test_bulk.py` & `trycourier-4.5.0/tests/test_bulk.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/tests/test_client.py` & `trycourier-4.5.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/tests/test_lists.py` & `trycourier-4.5.0/tests/test_lists.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/tests/test_messages.py` & `trycourier-4.5.0/tests/test_messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import responses
 import pytest
 
 from trycourier.client import Courier
 from trycourier.exceptions import CourierAPIException
 
+
 @responses.activate
 def test_success_messages_list():
     responses.add(
         responses.GET,
         'https://api.courier.com/messages',
         status=200,
         content_type='application/json',
@@ -95,30 +96,31 @@
         content_type='application/json',
         body='{"results": []}'
     )
 
     c = Courier(auth_token='123456789ABCDF')
     r = c.messages.get_history(message_id="my.message.id")
 
-    assert r == {'results':[]}
+    assert r == {'results': []}
+
 
 @responses.activate
 def test_success_messages_get_history_with_params():
     responses.add(
         responses.GET,
         'https://api.courier.com/messages/my.message.id/history?type=my.type',
         status=200,
         content_type='application/json',
         body='{"results": []}'
     )
 
     c = Courier(auth_token='123456789ABCDF')
     r = c.messages.get_history(message_id="my.message.id", type="my.type")
 
-    assert r == {'results':[]}
+    assert r == {'results': []}
 
 
 @responses.activate
 def test_fail_messages_get_history():
     responses.add(
         responses.GET,
         'https://api.courier.com/messages/my.message.id/history',
@@ -129,10 +131,21 @@
 
     c = Courier(auth_token='123456789ABCDF')
 
     with pytest.raises(CourierAPIException):
         c.messages.get_history("my.message.id")
 
 
+@responses.activate
+def test_messages_cancel():
+    responses.add(
+        responses.POST,
+        'https://api.courier.com/messages/id/cancel',
+        status=200,
+        content_type='application/json',
+        body='{}'
+    )
 
+    c = Courier(auth_token='123456789ABCDF')
+    r = c.messages.cancel(message_id="id")
 
-
+    assert r == {}
```

### Comparing `trycourier-4.4.0/tests/test_notifications.py` & `trycourier-4.5.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/tests/test_profiles.py` & `trycourier-4.5.0/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/tests/test_session.py` & `trycourier-4.5.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/trycourier/audiences.py` & `trycourier-4.5.0/trycourier/audiences.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/trycourier/audit_events.py` & `trycourier-4.5.0/trycourier/audit_events.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/trycourier/automations.py` & `trycourier-4.5.0/trycourier/automations.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/trycourier/bulk.py` & `trycourier-4.5.0/trycourier/bulk.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/trycourier/client.py` & `trycourier-4.5.0/trycourier/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/trycourier/lists.py` & `trycourier-4.5.0/trycourier/lists.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/trycourier/messages.py` & `trycourier-4.5.0/trycourier/messages.py`

 * *Files 13% similar despite different names*

```diff
@@ -108,7 +108,33 @@
 
         resp = self.session.get(url, params=params)
 
         if resp.status_code >= 400:
             raise CourierAPIException(resp)
 
         return resp.json()
+
+    def cancel(self, message_id):
+        """
+        Cancel the message delivery.
+
+        Args:
+            message_id (str): A unique identifier associated with the message
+            you wish to retrieve (returned after each 'send()' call.
+            See
+            https://www.courier.com/docs/reference/send/message/#requestid-details
+            for details.)
+
+        Raises:
+            CourierAPIException: Any error returned by the Courier API
+
+        Returns:
+            dict: Contains message item
+        """
+        url = "%s/%s/cancel" % (self.uri, message_id)
+
+        resp = self.session.post(url)
+
+        if resp.status_code >= 400:
+            raise CourierAPIException(resp)
+
+        return resp.json()
```

### Comparing `trycourier-4.4.0/trycourier/notifications.py` & `trycourier-4.5.0/trycourier/notifications.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/trycourier/profiles.py` & `trycourier-4.5.0/trycourier/profiles.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/trycourier/session.py` & `trycourier-4.5.0/trycourier/session.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.4.0/trycourier.egg-info/PKG-INFO` & `trycourier-4.5.0/trycourier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: trycourier
-Version: 4.4.0
+Version: 4.5.0
 Summary: A Python Package for communicating with the Courier REST API.
 Home-page: https://github.com/trycourier/courier-python
 Author: Courier
 Author-email: support@courier.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -681,9 +679,7 @@
 ## Contributing
 
 Bug reports and pull requests are welcome on GitHub at https://github.com/trycourier/courier-python. See [CONTRIBUTING.md](CONTRIBUTING.md) for more info.
 
 ## License
 
 The package is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
-
-
```

### Comparing `trycourier-4.4.0/trycourier.egg-info/SOURCES.txt` & `trycourier-4.5.0/trycourier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

