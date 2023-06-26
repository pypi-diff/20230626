# Comparing `tmp/django-pgschemas-0.8.0.tar.gz` & `tmp/django-pgschemas-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pgschemas-0.8.0.tar", max compression
+gzip compressed data, was "django-pgschemas-0.9.0.tar", max compression
```

## Comparing `django-pgschemas-0.8.0.tar` & `django-pgschemas-0.9.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1070 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/LICENSE
--rw-r--r--   0        0        0     4737 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/README.rst
--rw-r--r--   0        0        0      172 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/__init__.py
--rw-r--r--   0        0        0     4593 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/apps.py
--rw-r--r--   0        0        0     5096 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/checks.py
--rw-r--r--   0        0        0    34354 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/clone_schema.sql
--rw-r--r--   0        0        0        0 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/contrib/__init__.py
--rw-r--r--   0        0        0      563 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/contrib/cache.py
--rw-r--r--   0        0        0       49 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/contrib/channels2/__init__.py
--rw-r--r--   0        0        0     1884 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/contrib/channels2/auth.py
--rw-r--r--   0        0        0     3271 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/contrib/channels2/router.py
--rw-r--r--   0        0        0       49 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/contrib/channels3/__init__.py
--rw-r--r--   0        0        0     1884 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/contrib/channels3/auth.py
--rw-r--r--   0        0        0     3436 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/contrib/channels3/router.py
--rw-r--r--   0        0        0       53 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/contrib/files/__init__.py
--rw-r--r--   0        0        0     2063 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/contrib/files/storage.py
--rw-r--r--   0        0        0      394 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/log.py
--rw-r--r--   0        0        0        0 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/management/__init__.py
--rw-r--r--   0        0        0    10722 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/management/commands/__init__.py
--rw-r--r--   0        0        0     4058 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/management/commands/_executors.py
--rw-r--r--   0        0        0     5101 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/management/commands/cloneschema.py
--rw-r--r--   0        0        0     1670 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/management/commands/createrefschema.py
--rw-r--r--   0        0        0       80 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/management/commands/migrate.py
--rw-r--r--   0        0        0     1039 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/management/commands/migrateschema.py
--rw-r--r--   0        0        0     3384 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/management/commands/runschema.py
--rw-r--r--   0        0        0      401 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/management/commands/whowill.py
--rw-r--r--   0        0        0     3262 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/middleware.py
--rw-r--r--   0        0        0     5205 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/models.py
--rw-r--r--   0        0        0        0 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/postgresql_backend/__init__.py
--rw-r--r--   0        0        0     4424 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/postgresql_backend/_constraints.py
--rw-r--r--   0        0        0     3318 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/postgresql_backend/base.py
--rw-r--r--   0        0        0     5826 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/postgresql_backend/introspection.py
--rw-r--r--   0        0        0      308 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/postgresql_backend/settings.py
--rw-r--r--   0        0        0     1211 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/routers.py
--rw-r--r--   0        0        0     1082 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/schema.py
--rw-r--r--   0        0        0     1108 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/signals.py
--rw-r--r--   0        0        0        0 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/test/__init__.py
--rw-r--r--   0        0        0     5902 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/test/cases.py
--rw-r--r--   0        0        0     2530 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/test/client.py
--rw-r--r--   0        0        0     3020 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/urlresolvers.py
--rw-r--r--   0        0        0     6684 2021-11-24 20:15:34.130806 django-pgschemas-0.8.0/django_pgschemas/utils.py
--rw-r--r--   0        0        0     1348 2021-11-24 20:15:34.134806 django-pgschemas-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5866 2021-11-24 20:16:49.229676 django-pgschemas-0.8.0/setup.py
--rw-r--r--   0        0        0     5822 2021-11-24 20:16:49.230227 django-pgschemas-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4803 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/README.rst
+-rw-r--r--   0        0        0      172 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/__init__.py
+-rw-r--r--   0        0        0     4593 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/apps.py
+-rw-r--r--   0        0        0     5096 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/checks.py
+-rw-r--r--   0        0        0    34354 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/clone_schema.sql
+-rw-r--r--   0        0        0        0 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/contrib/__init__.py
+-rw-r--r--   0        0        0      563 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/contrib/cache.py
+-rw-r--r--   0        0        0       49 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/contrib/channels2/__init__.py
+-rw-r--r--   0        0        0     1884 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/contrib/channels2/auth.py
+-rw-r--r--   0        0        0     3269 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/contrib/channels2/router.py
+-rw-r--r--   0        0        0       49 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/contrib/channels3/__init__.py
+-rw-r--r--   0        0        0     1884 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/contrib/channels3/auth.py
+-rw-r--r--   0        0        0     3434 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/contrib/channels3/router.py
+-rw-r--r--   0        0        0       53 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/contrib/files/__init__.py
+-rw-r--r--   0        0        0     2063 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/contrib/files/storage.py
+-rw-r--r--   0        0        0      394 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/log.py
+-rw-r--r--   0        0        0        0 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/management/__init__.py
+-rw-r--r--   0        0        0    10722 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/management/commands/__init__.py
+-rw-r--r--   0        0        0     4058 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/management/commands/_executors.py
+-rw-r--r--   0        0        0     5101 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/management/commands/cloneschema.py
+-rw-r--r--   0        0        0     1670 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/management/commands/createrefschema.py
+-rw-r--r--   0        0        0       80 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/management/commands/migrate.py
+-rw-r--r--   0        0        0     1039 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/management/commands/migrateschema.py
+-rw-r--r--   0        0        0     3384 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/management/commands/runschema.py
+-rw-r--r--   0        0        0      401 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/management/commands/whowill.py
+-rw-r--r--   0        0        0     3262 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/middleware.py
+-rw-r--r--   0        0        0     5205 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/models.py
+-rw-r--r--   0        0        0        0 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/postgresql_backend/__init__.py
+-rw-r--r--   0        0        0     4424 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/postgresql_backend/_constraints.py
+-rw-r--r--   0        0        0     3318 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/postgresql_backend/base.py
+-rw-r--r--   0        0        0     5978 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/postgresql_backend/introspection.py
+-rw-r--r--   0        0        0      389 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/postgresql_backend/settings.py
+-rw-r--r--   0        0        0     1211 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/routers.py
+-rw-r--r--   0        0        0     1082 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/schema.py
+-rw-r--r--   0        0        0     1008 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/signals.py
+-rw-r--r--   0        0        0        0 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/test/__init__.py
+-rw-r--r--   0        0        0     5902 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/test/cases.py
+-rw-r--r--   0        0        0     2530 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/test/client.py
+-rw-r--r--   0        0        0     3020 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/urlresolvers.py
+-rw-r--r--   0        0        0     6684 2022-02-10 15:40:19.687308 django-pgschemas-0.9.0/django_pgschemas/utils.py
+-rw-r--r--   0        0        0     1340 2022-02-10 15:40:19.691308 django-pgschemas-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5927 2022-02-10 15:41:15.806802 django-pgschemas-0.9.0/setup.py
+-rw-r--r--   0        0        0     5828 2022-02-10 15:41:15.807233 django-pgschemas-0.9.0/PKG-INFO
```

### Comparing `django-pgschemas-0.8.0/LICENSE` & `django-pgschemas-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/README.rst` & `django-pgschemas-0.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,19 @@
 -------------
 
 https://django-pgschemas.readthedocs.io/
 
 Breaking changes
 ----------------
 
+v0.9.0
+++++++
+
+- Dropped support for Python < 3.8, Django < 3.1.
+
 v0.7.0
 ++++++
 
 - Changed public API for getting/setting active schema. Public API is now
   ``get_current_schema``, ``activate(schema)``, ``activate_public()``. Any
   schema descriptor can still be used as context manager.
 - Changed location of tenant model and domain model in settings.
```

### Comparing `django-pgschemas-0.8.0/django_pgschemas/apps.py` & `django-pgschemas-0.9.0/django_pgschemas/apps.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/checks.py` & `django-pgschemas-0.9.0/django_pgschemas/checks.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/clone_schema.sql` & `django-pgschemas-0.9.0/django_pgschemas/clone_schema.sql`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/contrib/cache.py` & `django-pgschemas-0.9.0/django_pgschemas/contrib/cache.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/contrib/channels2/auth.py` & `django-pgschemas-0.9.0/django_pgschemas/contrib/channels2/auth.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/contrib/channels2/router.py` & `django-pgschemas-0.9.0/django_pgschemas/contrib/channels3/router.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,48 @@
+from channels.db import database_sync_to_async
 from channels.routing import ProtocolTypeRouter, URLRouter
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.module_loading import import_string
 
 from ...schema import SchemaDescriptor
 from ...utils import get_domain_model, remove_www
 from .auth import TenantAuthMiddlewareStack
 
 
 class TenantAwareProtocolTypeRouter(ProtocolTypeRouter):
     def __init__(self, application_mapping, tenant_prefix):
         self.tenant_prefix = tenant_prefix
         super().__init__(application_mapping)
 
-    def __call__(self, scope):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             scope["path"] = scope["path"][len(self.tenant_prefix) + 1 :]
-        return super().__call__(scope)
+        return await super().__call__(scope, receive, send)
 
 
 class TenantProtocolRouter:
     """
     ProtocolRouter that handles multi-tenancy.
     """
 
     def __init__(self):
         self.root_ws_urlconf = settings.TENANTS["default"].get("WS_URLCONF")
         if self.root_ws_urlconf is None:
             raise ImproperlyConfigured(
                 "TENANTS['default'] must contain a 'WS_URLCONF' key in order to use TenantProtocolRouter."
             )
 
+    @database_sync_to_async
     def get_tenant_scope(self, scope):
         """
         Get tenant and websockets urlconf based on scope host.
         """
-        hostname = force_text(dict(scope["headers"]).get(b"host", b""))
+        hostname = force_str(dict(scope["headers"]).get(b"host", b""))
         hostname = remove_www(hostname.split(":")[0])
 
         tenant = None
         ws_urlconf = self.root_ws_urlconf
 
         # Checking for static tenants
         for schema, data in settings.TENANTS.items():
@@ -72,11 +74,11 @@
         """
         Subclasses can override this to include more protocols.
         """
         return TenantAwareProtocolTypeRouter(
             {"websocket": TenantAuthMiddlewareStack(URLRouter(ws_urlconf))}, tenant_prefix
         )
 
-    def __call__(self, scope):
-        tenant, tenant_prefix, ws_urlconf = self.get_tenant_scope(scope)
+    async def __call__(self, scope, receive, send):
+        tenant, tenant_prefix, ws_urlconf = await self.get_tenant_scope(scope)
         scope.update({"tenant": tenant})
-        return self.get_protocol_type_router(tenant_prefix, ws_urlconf)(scope)
+        return await self.get_protocol_type_router(tenant_prefix, ws_urlconf)(scope, receive, send)
```

### Comparing `django-pgschemas-0.8.0/django_pgschemas/contrib/channels3/auth.py` & `django-pgschemas-0.9.0/django_pgschemas/contrib/channels3/auth.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/contrib/channels3/router.py` & `django-pgschemas-0.9.0/django_pgschemas/contrib/channels2/router.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,46 @@
-from channels.db import database_sync_to_async
 from channels.routing import ProtocolTypeRouter, URLRouter
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.module_loading import import_string
 
 from ...schema import SchemaDescriptor
 from ...utils import get_domain_model, remove_www
 from .auth import TenantAuthMiddlewareStack
 
 
 class TenantAwareProtocolTypeRouter(ProtocolTypeRouter):
     def __init__(self, application_mapping, tenant_prefix):
         self.tenant_prefix = tenant_prefix
         super().__init__(application_mapping)
 
-    async def __call__(self, scope, receive, send):
+    def __call__(self, scope):
         if scope["type"] != "http":
             scope["path"] = scope["path"][len(self.tenant_prefix) + 1 :]
-        return await super().__call__(scope, receive, send)
+        return super().__call__(scope)
 
 
 class TenantProtocolRouter:
     """
     ProtocolRouter that handles multi-tenancy.
     """
 
     def __init__(self):
         self.root_ws_urlconf = settings.TENANTS["default"].get("WS_URLCONF")
         if self.root_ws_urlconf is None:
             raise ImproperlyConfigured(
                 "TENANTS['default'] must contain a 'WS_URLCONF' key in order to use TenantProtocolRouter."
             )
 
-    @database_sync_to_async
     def get_tenant_scope(self, scope):
         """
         Get tenant and websockets urlconf based on scope host.
         """
-        hostname = force_text(dict(scope["headers"]).get(b"host", b""))
+        hostname = force_str(dict(scope["headers"]).get(b"host", b""))
         hostname = remove_www(hostname.split(":")[0])
 
         tenant = None
         ws_urlconf = self.root_ws_urlconf
 
         # Checking for static tenants
         for schema, data in settings.TENANTS.items():
@@ -74,11 +72,11 @@
         """
         Subclasses can override this to include more protocols.
         """
         return TenantAwareProtocolTypeRouter(
             {"websocket": TenantAuthMiddlewareStack(URLRouter(ws_urlconf))}, tenant_prefix
         )
 
-    async def __call__(self, scope, receive, send):
-        tenant, tenant_prefix, ws_urlconf = await self.get_tenant_scope(scope)
+    def __call__(self, scope):
+        tenant, tenant_prefix, ws_urlconf = self.get_tenant_scope(scope)
         scope.update({"tenant": tenant})
-        return await self.get_protocol_type_router(tenant_prefix, ws_urlconf)(scope, receive, send)
+        return self.get_protocol_type_router(tenant_prefix, ws_urlconf)(scope)
```

### Comparing `django-pgschemas-0.8.0/django_pgschemas/contrib/files/storage.py` & `django-pgschemas-0.9.0/django_pgschemas/contrib/files/storage.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/management/commands/__init__.py` & `django-pgschemas-0.9.0/django_pgschemas/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/management/commands/_executors.py` & `django-pgschemas-0.9.0/django_pgschemas/management/commands/_executors.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/management/commands/cloneschema.py` & `django-pgschemas-0.9.0/django_pgschemas/management/commands/cloneschema.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/management/commands/createrefschema.py` & `django-pgschemas-0.9.0/django_pgschemas/management/commands/createrefschema.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/management/commands/migrateschema.py` & `django-pgschemas-0.9.0/django_pgschemas/management/commands/migrateschema.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/management/commands/runschema.py` & `django-pgschemas-0.9.0/django_pgschemas/management/commands/runschema.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/middleware.py` & `django-pgschemas-0.9.0/django_pgschemas/middleware.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/models.py` & `django-pgschemas-0.9.0/django_pgschemas/models.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/postgresql_backend/_constraints.py` & `django-pgschemas-0.9.0/django_pgschemas/postgresql_backend/_constraints.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/postgresql_backend/base.py` & `django-pgschemas-0.9.0/django_pgschemas/postgresql_backend/base.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/postgresql_backend/introspection.py` & `django-pgschemas-0.9.0/django_pgschemas/postgresql_backend/introspection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from django.db.backends.base.introspection import FieldInfo, TableInfo
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 from . import _constraints
-from .settings import original_backend
+from .settings import base_backend, original_backend
 
+try:
+    DatabaseIntrospection = original_backend.DatabaseIntrospection
+except AttributeError:
+    DatabaseIntrospection = base_backend.DatabaseIntrospection
 
-class DatabaseSchemaIntrospection(original_backend.DatabaseIntrospection):  # pragma: no cover
+
+class DatabaseSchemaIntrospection(DatabaseIntrospection):  # pragma: no cover
     """
     database schema introspection class
     """
 
     _get_indexes_query = """
         SELECT attr.attname, idx.indkey, idx.indisunique, idx.indisprimary
         FROM pg_catalog.pg_class c,
@@ -54,17 +59,17 @@
             [self.connection._schema.schema_name, table_name],
         )
         field_map = {line[0]: line[1:] for line in cursor.fetchall()}
         cursor.execute("SELECT * FROM %s LIMIT 1" % self.connection.ops.quote_name(table_name))
         return [
             FieldInfo(
                 *(
-                    (force_text(line[0]),)
+                    (force_str(line[0]),)
                     + line[1:6]
-                    + (field_map[force_text(line[0])][0] == "YES", field_map[force_text(line[0])][1])
+                    + (field_map[force_str(line[0])][0] == "YES", field_map[force_str(line[0])][1])
                 )
             )
             for line in cursor.description
         ]
 
     def get_indexes(self, cursor, table_name):
         # This query retrieves each index on the given table, including the
```

### Comparing `django-pgschemas-0.8.0/django_pgschemas/routers.py` & `django-pgschemas-0.9.0/django_pgschemas/routers.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/schema.py` & `django-pgschemas-0.9.0/django_pgschemas/schema.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/test/cases.py` & `django-pgschemas-0.9.0/django_pgschemas/test/cases.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/test/client.py` & `django-pgschemas-0.9.0/django_pgschemas/test/client.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/urlresolvers.py` & `django-pgschemas-0.9.0/django_pgschemas/urlresolvers.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/django_pgschemas/utils.py` & `django-pgschemas-0.9.0/django_pgschemas/utils.py`

 * *Files identical despite different names*

### Comparing `django-pgschemas-0.8.0/pyproject.toml` & `django-pgschemas-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "django-pgschemas"
-version = "0.8.0"
+version = "0.9.0"
 description = "Multi-tenancy on Django using PostgreSQL schemas."
 license = "MIT"
 authors = ["Lorenzo Peña <lorinkoz@gmail.com>"]
 readme = "README.rst"
 repository = "https://github.com/lorinkoz/django-pgschemas"
 documentation = "https://django-pgschemas.readthedocs.io/"
 keywords = ["django", "tenants", "schemas", "multi-tenancy", "postgresql"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Django",
-    "Framework :: Django :: 2.2",
     "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.0",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
-django = ">=2.2,!=3.0,<3.3"
-psycopg2 = "~2.8.0"
+python = "^3.8"
+django = ">=3.1,<4.1"
+psycopg2 = "^2.9.3"
 
 [tool.poetry.dev-dependencies]
-black = "^21.9b0"
+black = "^22.1.0"
 channels = "^2.1"
-coverage = {extras = ["toml"], version = "^5.1"}
+coverage = {extras = ["toml"], version = "^6.3"}
 doc8 = "^0.8.0"
 flake8 = "^3.8.4"
 flake8-bugbear = "^20.11.1"
 flake8-comprehensions = "^3.3.1"
 flake8-no-types = "^1.1.1"
 flake8-tidy-imports = "^4.2.1"
 isort = "^5.6.4"
```

### Comparing `django-pgschemas-0.8.0/setup.py` & `django-pgschemas-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,27 @@
  'django_pgschemas.postgresql_backend',
  'django_pgschemas.test']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['django>=2.2,!=3.0,<3.3', 'psycopg2>=2.8.0,<2.9.0']
+['django>=3.1,<4.1', 'psycopg2>=2.9.3,<3.0.0']
 
 setup_kwargs = {
     'name': 'django-pgschemas',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Multi-tenancy on Django using PostgreSQL schemas.',
-    'long_description': 'django-pgschemas\n================\n\n.. image:: https://img.shields.io/badge/packaging-poetry-purple.svg\n    :alt: Packaging: poetry\n    :target: https://github.com/sdispater/poetry\n\n.. image:: https://img.shields.io/badge/code%20style-black-black.svg\n    :alt: Code style: black\n    :target: https://github.com/ambv/black\n\n.. image:: https://github.com/lorinkoz/django-pgschemas/workflows/code/badge.svg\n    :alt: Build status\n    :target: https://github.com/lorinkoz/django-pgschemas/actions\n\n.. image:: https://readthedocs.org/projects/django-pgschemas/badge/?version=latest\n    :alt: Documentation status\n    :target: https://django-pgschemas.readthedocs.io/\n\n.. image:: https://coveralls.io/repos/github/lorinkoz/django-pgschemas/badge.svg?branch=master\n    :alt: Code coverage\n    :target: https://coveralls.io/github/lorinkoz/django-pgschemas?branch=master\n\n.. image:: https://badge.fury.io/py/django-pgschemas.svg\n    :alt: PyPi version\n    :target: http://badge.fury.io/py/django-pgschemas\n\n.. image:: https://pepy.tech/badge/django-pgschemas/month\n    :alt: Downloads\n    :target: https://pepy.tech/project/django-pgschemas/\n\n|\n\nThis app uses PostgreSQL schemas to support data multi-tenancy in a single\nDjango project. It is a fork of `django-tenants`_ with some conceptual changes:\n\n- There are static tenants and dynamic tenants. Static tenants can have their\n  own apps and urlconf.\n- Tenants can be simultaneously routed via subdomain and via subfolder on shared\n  subdomain.\n- Public is no longer the schema for storing the main site data. Public should\n  be used only for true shared data across all tenants. Table "overriding" via\n  search path is no longer encouraged.\n- Management commands can be run on multiple schemas via wildcards - the\n  multiproc behavior of migrations was extended to just any tenant command.\n\n.. _django-tenants: https://github.com/tomturner/django-tenants\n\nWhich package to use?\n---------------------\n\nThere are currently multiple packages to handle multi-tenancy via PostgreSQL schemas.\nThis table should help you make an informed decision on which one to choose.\n\n.. list-table::\n   :widths: 50 50\n   :header-rows: 1\n\n   * - Package\n     - Features\n   * - `django-tenant-schemas`_\n     - Original project.\n       Active and maintained by `@goodtune`_.\n   * - `django-tenants`_\n     - Active and maintained by `@tomturner`_.\n       Built on top of `django-tenant-schemas`_.\n       Uses a ``Domain`` model for allowing multiple domains per tenant.\n       Allows for parallel migrations with custom migration executor.\n       Other multiple improvements.\n   * - `django-pgschemas`_\n     - Active and maintained by `@lorinkoz`_.\n       Built on top of `django-tenants`_.\n       Different philosphy for tenants.\n       Other improvements listed above.\n\n.. _django-tenants-schemas: https://github.com/bernardopires/django-tenant-schemas\n.. _@goodtune: https://github.com/goodtune\n.. _django-tenants: https://github.com/tomturner/django-tenants\n.. _@tomturner: https://github.com/tomturner\n.. _django-pgschemas: https://github.com/lorinkoz/django-pgschemas\n.. _@lorinkoz: https://github.com/lorinkoz\n\nDocumentation\n-------------\n\nhttps://django-pgschemas.readthedocs.io/\n\nBreaking changes\n----------------\n\nv0.7.0\n++++++\n\n- Changed public API for getting/setting active schema. Public API is now\n  ``get_current_schema``, ``activate(schema)``, ``activate_public()``. Any\n  schema descriptor can still be used as context manager.\n- Changed location of tenant model and domain model in settings.\n  ``TENANT_MODEL`` and ``DOMAIN_MODEL`` keys are now under ``TENANTS["default"]``\n  instead of ``TENANTS["public"]``. This is required for future\n  static-tenant-only configurations.\n- Module ``cache`` renamed to ``contrib.cache``.\n- Module ``contrib.channels`` renamed to ``contrib.channels2``.\n- Added module ``contrib.channels3``.\n- Management command option ``--executor {sequential, parallel}`` renamed to\n  ``--parallel``.\n- All signals renamed. Added ``schema_activate`` signal.\n\nContributing\n------------\n\n- Join the discussion at https://github.com/lorinkoz/django-pgschemas/discussions.\n- PRs are welcome! If you have questions or comments, please use the link\n  above.\n- To run the test suite run ``make`` or ``make coverage``. The tests for this\n  project live inside a small django project called ``dpgs_sandbox``. Database\n  password and database host can be set through the environment variables\n  ``DATABASE_PASSWORD`` and ``DATABASE_HOST``.\n\nCredits\n-------\n\n* Tom Turner for `django-tenants`_\n* Bernardo Pires for `django-tenant-schemas`_\n\n.. _django-tenants: https://github.com/tomturner/django-tenants\n.. _django-tenant-schemas: https://github.com/bernardopires/django-tenant-schemas\n',
+    'long_description': 'django-pgschemas\n================\n\n.. image:: https://img.shields.io/badge/packaging-poetry-purple.svg\n    :alt: Packaging: poetry\n    :target: https://github.com/sdispater/poetry\n\n.. image:: https://img.shields.io/badge/code%20style-black-black.svg\n    :alt: Code style: black\n    :target: https://github.com/ambv/black\n\n.. image:: https://github.com/lorinkoz/django-pgschemas/workflows/code/badge.svg\n    :alt: Build status\n    :target: https://github.com/lorinkoz/django-pgschemas/actions\n\n.. image:: https://readthedocs.org/projects/django-pgschemas/badge/?version=latest\n    :alt: Documentation status\n    :target: https://django-pgschemas.readthedocs.io/\n\n.. image:: https://coveralls.io/repos/github/lorinkoz/django-pgschemas/badge.svg?branch=master\n    :alt: Code coverage\n    :target: https://coveralls.io/github/lorinkoz/django-pgschemas?branch=master\n\n.. image:: https://badge.fury.io/py/django-pgschemas.svg\n    :alt: PyPi version\n    :target: http://badge.fury.io/py/django-pgschemas\n\n.. image:: https://pepy.tech/badge/django-pgschemas/month\n    :alt: Downloads\n    :target: https://pepy.tech/project/django-pgschemas/\n\n|\n\nThis app uses PostgreSQL schemas to support data multi-tenancy in a single\nDjango project. It is a fork of `django-tenants`_ with some conceptual changes:\n\n- There are static tenants and dynamic tenants. Static tenants can have their\n  own apps and urlconf.\n- Tenants can be simultaneously routed via subdomain and via subfolder on shared\n  subdomain.\n- Public is no longer the schema for storing the main site data. Public should\n  be used only for true shared data across all tenants. Table "overriding" via\n  search path is no longer encouraged.\n- Management commands can be run on multiple schemas via wildcards - the\n  multiproc behavior of migrations was extended to just any tenant command.\n\n.. _django-tenants: https://github.com/tomturner/django-tenants\n\nWhich package to use?\n---------------------\n\nThere are currently multiple packages to handle multi-tenancy via PostgreSQL schemas.\nThis table should help you make an informed decision on which one to choose.\n\n.. list-table::\n   :widths: 50 50\n   :header-rows: 1\n\n   * - Package\n     - Features\n   * - `django-tenant-schemas`_\n     - Original project.\n       Active and maintained by `@goodtune`_.\n   * - `django-tenants`_\n     - Active and maintained by `@tomturner`_.\n       Built on top of `django-tenant-schemas`_.\n       Uses a ``Domain`` model for allowing multiple domains per tenant.\n       Allows for parallel migrations with custom migration executor.\n       Other multiple improvements.\n   * - `django-pgschemas`_\n     - Active and maintained by `@lorinkoz`_.\n       Built on top of `django-tenants`_.\n       Different philosphy for tenants.\n       Other improvements listed above.\n\n.. _django-tenants-schemas: https://github.com/bernardopires/django-tenant-schemas\n.. _@goodtune: https://github.com/goodtune\n.. _django-tenants: https://github.com/tomturner/django-tenants\n.. _@tomturner: https://github.com/tomturner\n.. _django-pgschemas: https://github.com/lorinkoz/django-pgschemas\n.. _@lorinkoz: https://github.com/lorinkoz\n\nDocumentation\n-------------\n\nhttps://django-pgschemas.readthedocs.io/\n\nBreaking changes\n----------------\n\nv0.9.0\n++++++\n\n- Dropped support for Python < 3.8, Django < 3.1.\n\nv0.7.0\n++++++\n\n- Changed public API for getting/setting active schema. Public API is now\n  ``get_current_schema``, ``activate(schema)``, ``activate_public()``. Any\n  schema descriptor can still be used as context manager.\n- Changed location of tenant model and domain model in settings.\n  ``TENANT_MODEL`` and ``DOMAIN_MODEL`` keys are now under ``TENANTS["default"]``\n  instead of ``TENANTS["public"]``. This is required for future\n  static-tenant-only configurations.\n- Module ``cache`` renamed to ``contrib.cache``.\n- Module ``contrib.channels`` renamed to ``contrib.channels2``.\n- Added module ``contrib.channels3``.\n- Management command option ``--executor {sequential, parallel}`` renamed to\n  ``--parallel``.\n- All signals renamed. Added ``schema_activate`` signal.\n\nContributing\n------------\n\n- Join the discussion at https://github.com/lorinkoz/django-pgschemas/discussions.\n- PRs are welcome! If you have questions or comments, please use the link\n  above.\n- To run the test suite run ``make`` or ``make coverage``. The tests for this\n  project live inside a small django project called ``dpgs_sandbox``. Database\n  password and database host can be set through the environment variables\n  ``DATABASE_PASSWORD`` and ``DATABASE_HOST``.\n\nCredits\n-------\n\n* Tom Turner for `django-tenants`_\n* Bernardo Pires for `django-tenant-schemas`_\n\n.. _django-tenants: https://github.com/tomturner/django-tenants\n.. _django-tenant-schemas: https://github.com/bernardopires/django-tenant-schemas\n',
     'author': 'Lorenzo Peña',
     'author_email': 'lorinkoz@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/lorinkoz/django-pgschemas',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6.2,<4.0.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `django-pgschemas-0.8.0/PKG-INFO` & `django-pgschemas-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: django-pgschemas
-Version: 0.8.0
+Version: 0.9.0
 Summary: Multi-tenancy on Django using PostgreSQL schemas.
 Home-page: https://github.com/lorinkoz/django-pgschemas
 License: MIT
 Keywords: django,tenants,schemas,multi-tenancy,postgresql
 Author: Lorenzo Peña
 Author-email: lorinkoz@gmail.com
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: django (>=2.2,!=3.0,<3.3)
-Requires-Dist: psycopg2 (>=2.8.0,<2.9.0)
+Requires-Dist: django (>=3.1,<4.1)
+Requires-Dist: psycopg2 (>=2.9.3,<3.0.0)
 Project-URL: Documentation, https://django-pgschemas.readthedocs.io/
 Project-URL: Repository, https://github.com/lorinkoz/django-pgschemas
 Description-Content-Type: text/x-rst
 
 django-pgschemas
 ================
 
@@ -111,14 +110,19 @@
 -------------
 
 https://django-pgschemas.readthedocs.io/
 
 Breaking changes
 ----------------
 
+v0.9.0
+++++++
+
+- Dropped support for Python < 3.8, Django < 3.1.
+
 v0.7.0
 ++++++
 
 - Changed public API for getting/setting active schema. Public API is now
   ``get_current_schema``, ``activate(schema)``, ``activate_public()``. Any
   schema descriptor can still be used as context manager.
 - Changed location of tenant model and domain model in settings.
```

