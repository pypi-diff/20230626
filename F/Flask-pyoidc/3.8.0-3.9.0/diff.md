# Comparing `tmp/Flask_pyoidc-3.8.0-py3-none-any.whl.zip` & `tmp/Flask_pyoidc-3.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 18523 bytes, number of entries: 13
+Zip file size: 18593 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       45 b- defN 20-Jan-23 08:07 flask_pyoidc/__init__.py
 -rw-r--r--  2.0 unx     4867 b- defN 20-Dec-04 14:39 flask_pyoidc/auth_response_handler.py
--rw-r--r--  2.0 unx    13516 b- defN 21-Oct-19 08:29 flask_pyoidc/flask_pyoidc.py
+-rw-r--r--  2.0 unx    13836 b- defN 21-Dec-14 08:02 flask_pyoidc/flask_pyoidc.py
 -rw-r--r--  2.0 unx      431 b- defN 21-Oct-19 08:29 flask_pyoidc/parse_fragment.html
 -rw-r--r--  2.0 unx     7441 b- defN 21-Oct-19 08:29 flask_pyoidc/provider_configuration.py
 -rw-r--r--  2.0 unx     9632 b- defN 21-Jun-14 18:41 flask_pyoidc/pyoidc_facade.py
 -rw-r--r--  2.0 unx     2235 b- defN 20-Nov-10 20:41 flask_pyoidc/redirect_uri_config.py
 -rw-r--r--  2.0 unx     3960 b- defN 20-Jul-06 18:03 flask_pyoidc/user_session.py
--rw-r--r--  2.0 unx    11357 b- defN 21-Oct-19 08:39 Flask_pyoidc-3.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1461 b- defN 21-Oct-19 08:39 Flask_pyoidc-3.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Oct-19 08:39 Flask_pyoidc-3.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 21-Oct-19 08:39 Flask_pyoidc-3.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1117 b- defN 21-Oct-19 08:39 Flask_pyoidc-3.8.0.dist-info/RECORD
-13 files, 56167 bytes uncompressed, 16643 bytes compressed:  70.4%
+-rw-r--r--  2.0 unx    11357 b- defN 21-Dec-14 08:04 Flask_pyoidc-3.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1461 b- defN 21-Dec-14 08:04 Flask_pyoidc-3.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Dec-14 08:04 Flask_pyoidc-3.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 21-Dec-14 08:04 Flask_pyoidc-3.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1117 b- defN 21-Dec-14 08:04 Flask_pyoidc-3.9.0.dist-info/RECORD
+13 files, 56487 bytes uncompressed, 16713 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: flask_pyoidc/redirect_uri_config.py
 Comment: 
 
 Filename: flask_pyoidc/user_session.py
 Comment: 
 
-Filename: Flask_pyoidc-3.8.0.dist-info/LICENSE
+Filename: Flask_pyoidc-3.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: Flask_pyoidc-3.8.0.dist-info/METADATA
+Filename: Flask_pyoidc-3.9.0.dist-info/METADATA
 Comment: 
 
-Filename: Flask_pyoidc-3.8.0.dist-info/WHEEL
+Filename: Flask_pyoidc-3.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: Flask_pyoidc-3.8.0.dist-info/top_level.txt
+Filename: Flask_pyoidc-3.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: Flask_pyoidc-3.8.0.dist-info/RECORD
+Filename: Flask_pyoidc-3.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flask_pyoidc/flask_pyoidc.py

```diff
@@ -22,14 +22,15 @@
 import flask
 import importlib_resources
 from flask import current_app
 from flask.helpers import url_for
 from oic import rndstr
 from oic.oic import AuthorizationRequest
 from oic.oic.message import EndSessionRequest
+from werkzeug.routing import BuildError
 from werkzeug.utils import redirect
 
 from .auth_response_handler import AuthResponseProcessError, AuthResponseHandler, AuthResponseErrorResponseError
 from .pyoidc_facade import PyoidcFacade
 from .redirect_uri_config import RedirectUriConfig
 from .user_session import UninitialisedSession, UserSession
 
@@ -78,30 +79,38 @@
 
     def _get_post_logout_redirect_uri(self, client):
         if client.post_logout_redirect_uris:
             return client.post_logout_redirect_uris[0]
         return self._get_url_for_logout_view()
 
     def _get_url_for_logout_view(self):
-        return url_for(self._logout_view.__name__, _external=True) if self._logout_view else None
+        if not self._logout_view:
+            return None
+
+        try:
+            return url_for(self._logout_view.__name__, _external=True)
+        except BuildError:
+            logger.error('could not build url for logout view, it might be mounted under a custom endpoint')
+            raise
 
     def _register_client(self, client):
         def default_post_logout_redirect_uris():
             url_for_logout_view = self._get_url_for_logout_view()
             if url_for_logout_view:
                 return [url_for_logout_view]
             return []
 
         client_registration_args = {}
-        post_logout_redirect_uris = client._provider_configuration._client_registration_info.get(
-            'post_logout_redirect_uris',
-            default_post_logout_redirect_uris())
+        post_logout_redirect_uris = client._provider_configuration._client_registration_info.get('post_logout_redirect_uris')
         if post_logout_redirect_uris:
-            logger.debug('registering with post_logout_redirect_uris=%s', post_logout_redirect_uris)
             client_registration_args['post_logout_redirect_uris'] = post_logout_redirect_uris
+        else:
+            client_registration_args['post_logout_redirect_uris'] = default_post_logout_redirect_uris()
+
+        logger.debug('registering with post_logout_redirect_uris=%s', client_registration_args['post_logout_redirect_uris'])
         client.register(client_registration_args)
 
     def _authenticate(self, client, interactive=True):
         if not client.is_registered():
             self._register_client(client)
 
         flask.session['destination'] = flask.request.url
```

## Comparing `Flask_pyoidc-3.8.0.dist-info/LICENSE` & `Flask_pyoidc-3.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Flask_pyoidc-3.8.0.dist-info/METADATA` & `Flask_pyoidc-3.9.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-pyoidc
-Version: 3.8.0
+Version: 3.9.0
 Summary: Flask extension for OpenID Connect authentication.
 Home-page: https://github.com/zamzterz/flask-pyoidc
 Author: Samuel Gulliksson
 Author-email: samuel.gulliksson@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `Flask_pyoidc-3.8.0.dist-info/RECORD` & `Flask_pyoidc-3.9.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 flask_pyoidc/__init__.py,sha256=IlfEFoaGc82nTV54NpjX0RoCdAidtojc02G7F-14tj0,45
 flask_pyoidc/auth_response_handler.py,sha256=JFRIzghjprhFFZJpfvhLVjWV4aAtaqBOSTgsJ12HvL4,4867
-flask_pyoidc/flask_pyoidc.py,sha256=ZZqPR3Lh7r8hmMIzQerdFgyp4tz_on8DFn4YO8vlYLU,13516
+flask_pyoidc/flask_pyoidc.py,sha256=RrjLJhyVnFeDy4bVtcJT0wft48c5IrMmLAiuZ_k9poA,13836
 flask_pyoidc/parse_fragment.html,sha256=oCaRWQv0cUKaXvbCziBz1eywbWQAdKPRHq7p5kBVc2M,431
 flask_pyoidc/provider_configuration.py,sha256=dcnJXumjv1qos1SpZu4SYWA9ntEbT9ktj4X61eC_geY,7441
 flask_pyoidc/pyoidc_facade.py,sha256=TGagUCKAGKfjK-P2HLFJcP1EdqvFOrnXw9Q4p9tk1WI,9632
 flask_pyoidc/redirect_uri_config.py,sha256=h8D9eQtbZzv4dCuKNt1YFT1mbSLHRy2h_ABiq8qUB74,2235
 flask_pyoidc/user_session.py,sha256=21FK282Rnbfxl9ctRzOucXzjcMGW4Mk434LKv-ETMcY,3960
-Flask_pyoidc-3.8.0.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
-Flask_pyoidc-3.8.0.dist-info/METADATA,sha256=LHL1AodkjbNX8ONNRi1IkBVoJjfVfhcnvLqPFOB7Ets,1461
-Flask_pyoidc-3.8.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-Flask_pyoidc-3.8.0.dist-info/top_level.txt,sha256=gcaUKy4F97xZ8HublXZi3bjZdYyj4-5p2FJy-jvjE4o,13
-Flask_pyoidc-3.8.0.dist-info/RECORD,,
+Flask_pyoidc-3.9.0.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
+Flask_pyoidc-3.9.0.dist-info/METADATA,sha256=TLDxjHKdkPjsVgrPjje_dbJRe1DmGvRdrX8Ld26imLU,1461
+Flask_pyoidc-3.9.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+Flask_pyoidc-3.9.0.dist-info/top_level.txt,sha256=gcaUKy4F97xZ8HublXZi3bjZdYyj4-5p2FJy-jvjE4o,13
+Flask_pyoidc-3.9.0.dist-info/RECORD,,
```

