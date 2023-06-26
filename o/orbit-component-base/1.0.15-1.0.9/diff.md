# Comparing `tmp/orbit_component_base-1.0.15.tar.gz` & `tmp/orbit_component_base-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_base-1.0.15.tar", max compression
+gzip compressed data, was "orbit_component_base-1.0.9.tar", max compression
```

## Comparing `orbit_component_base-1.0.15.tar` & `orbit_component_base-1.0.9.tar`

### file list

```diff
@@ -1,33 +1,28 @@
--rw-r--r--   0        0        0     1099 2023-05-30 15:19:20.188832 orbit_component_base-1.0.15/LICENSE.md
--rw-r--r--   0        0        0      307 2023-05-30 15:19:20.188832 orbit_component_base-1.0.15/README.md
--rw-r--r--   0        0        0      248 2023-05-30 15:19:20.188832 orbit_component_base-1.0.15/orbit_component_base/__init__.py
--rw-r--r--   0        0        0      206 2023-05-30 15:19:46.404293 orbit_component_base-1.0.15/orbit_component_base/cli/cli_base.py
--rw-r--r--   0        0        0     2316 2023-06-23 14:35:50.930022 orbit_component_base-1.0.15/orbit_component_base/cli/permissions.py
--rw-r--r--   0        0        0     1691 2023-06-10 13:38:38.437638 orbit_component_base-1.0.15/orbit_component_base/cli/sessions.py
--rw-r--r--   0        0        0     2003 2023-06-10 13:39:02.825128 orbit_component_base-1.0.15/orbit_component_base/cli/users.py
--rw-r--r--   0        0        0     2952 2023-06-23 14:33:00.689608 orbit_component_base-1.0.15/orbit_component_base/plugin.py
--rw-r--r--   0        0        0     1613 2023-06-23 14:35:03.647017 orbit_component_base-1.0.15/orbit_component_base/schema/OrbitPermissions.py
--rw-r--r--   0        0        0     1342 2023-06-22 12:00:55.061359 orbit_component_base-1.0.15/orbit_component_base/schema/OrbitSessions.py
--rw-r--r--   0        0        0      626 2023-06-22 11:38:57.280314 orbit_component_base-1.0.15/orbit_component_base/schema/OrbitUsers.py
--rwxr-xr-x   0        0        0     3603 2023-06-08 10:02:49.715966 orbit_component_base-1.0.15/orbit_component_base/src/orbit_app.py
--rw-r--r--   0        0        0     6555 2023-06-22 11:38:34.572765 orbit_component_base-1.0.15/orbit_component_base/src/orbit_auth.py
--rw-r--r--   0        0        0     7048 2023-06-26 16:58:29.265828 orbit_component_base-1.0.15/orbit_component_base/src/orbit_config.py
--rw-r--r--   0        0        0     1232 2023-05-30 15:19:20.188832 orbit_component_base-1.0.15/orbit_component_base/src/orbit_database.py
--rw-r--r--   0        0        0     5072 2023-06-23 14:40:23.328298 orbit_component_base-1.0.15/orbit_component_base/src/orbit_decorators.py
--rw-r--r--   0        0        0      290 2023-05-30 15:19:20.188832 orbit_component_base-1.0.15/orbit_component_base/src/orbit_logger.py
--rw-r--r--   0        0        0      834 2023-05-30 16:30:11.592032 orbit_component_base-1.0.15/orbit_component_base/src/orbit_make_ssl.py
--rw-r--r--   0        0        0     8612 2023-06-07 11:18:34.376181 orbit_component_base-1.0.15/orbit_component_base/src/orbit_nql.py
--rw-r--r--   0        0        0     3534 2023-05-30 15:19:20.188832 orbit_component_base-1.0.15/orbit_component_base/src/orbit_nql_buffer.py
--rw-r--r--   0        0        0      895 2023-06-23 14:40:36.048032 orbit_component_base-1.0.15/orbit_component_base/src/orbit_nql_emitter.py
--rw-r--r--   0        0        0     4442 2023-05-30 15:19:20.188832 orbit_component_base-1.0.15/orbit_component_base/src/orbit_nql_session.py
--rw-r--r--   0        0        0     6554 2023-06-07 23:22:03.266791 orbit_component_base-1.0.15/orbit_component_base/src/orbit_orm.py
--rw-r--r--   0        0        0     2669 2023-06-23 12:05:05.287826 orbit_component_base-1.0.15/orbit_component_base/src/orbit_plugin.py
--rw-r--r--   0        0        0     2148 2023-06-02 16:17:04.740333 orbit_component_base-1.0.15/orbit_component_base/src/orbit_plugins.py
--rw-r--r--   0        0        0     2323 2023-06-05 13:10:08.334760 orbit_component_base-1.0.15/orbit_component_base/src/orbit_router.py
--rw-r--r--   0        0        0      629 2023-05-30 15:19:20.192832 orbit_component_base-1.0.15/orbit_component_base/src/orbit_shared.py
--rw-r--r--   0        0        0     6489 2023-06-23 12:53:38.130760 orbit_component_base-1.0.15/orbit_component_base/src/orbit_shells.py
--rw-r--r--   0        0        0       21 2023-05-30 15:19:20.192832 orbit_component_base-1.0.15/orbit_component_base/src/orbit_version.py
--rw-r--r--   0        0        0       76 2023-05-30 15:19:20.192832 orbit_component_base-1.0.15/orbit_component_base/tests/test_main.py
--rw-r--r--   0        0        0       23 2023-06-26 16:59:27.640620 orbit_component_base-1.0.15/orbit_component_base/version.py
--rw-r--r--   0        0        0     1408 2023-06-26 16:59:27.640620 orbit_component_base-1.0.15/pyproject.toml
--rw-r--r--   0        0        0     1624 1970-01-01 00:00:00.000000 orbit_component_base-1.0.15/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/LICENSE.md
+-rw-r--r--   0        0        0      307 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/README.md
+-rw-r--r--   0        0        0      248 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-07 22:18:42.405891 orbit_component_base-1.0.9/orbit_component_base/plugin.py
+-rw-r--r--   0        0        0     1290 2023-06-08 11:30:57.895776 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitSessions.py
+-rw-r--r--   0        0        0      343 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitUsers.py
+-rw-r--r--   0        0        0     1787 2023-06-08 11:31:11.007490 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitVersions.py
+-rwxr-xr-x   0        0        0     3603 2023-06-08 10:02:49.715966 orbit_component_base-1.0.9/orbit_component_base/src/orbit_app.py
+-rw-r--r--   0        0        0     6551 2023-06-08 12:34:02.238300 orbit_component_base-1.0.9/orbit_component_base/src/orbit_auth.py
+-rw-r--r--   0        0        0     6878 2023-06-05 13:02:31.115557 orbit_component_base-1.0.9/orbit_component_base/src/orbit_config.py
+-rw-r--r--   0        0        0     1232 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_database.py
+-rw-r--r--   0        0        0     3749 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_decorators.py
+-rw-r--r--   0        0        0      290 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_logger.py
+-rw-r--r--   0        0        0      834 2023-05-30 16:30:11.592032 orbit_component_base-1.0.9/orbit_component_base/src/orbit_make_ssl.py
+-rw-r--r--   0        0        0     8612 2023-06-07 11:18:34.376181 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql.py
+-rw-r--r--   0        0        0     3534 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_buffer.py
+-rw-r--r--   0        0        0      895 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_emitter.py
+-rw-r--r--   0        0        0     4442 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_session.py
+-rw-r--r--   0        0        0     6554 2023-06-07 23:22:03.266791 orbit_component_base-1.0.9/orbit_component_base/src/orbit_orm.py
+-rw-r--r--   0        0        0     2983 2023-06-08 12:54:23.664990 orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugin.py
+-rw-r--r--   0        0        0     2148 2023-06-02 16:17:04.740333 orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugins.py
+-rw-r--r--   0        0        0     2323 2023-06-05 13:10:08.334760 orbit_component_base-1.0.9/orbit_component_base/src/orbit_router.py
+-rw-r--r--   0        0        0      629 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_shared.py
+-rw-r--r--   0        0        0       21 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_version.py
+-rw-r--r--   0        0        0       76 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/tests/test_main.py
+-rw-r--r--   0        0        0       22 2023-06-08 17:25:09.459041 orbit_component_base-1.0.9/orbit_component_base/version.py
+-rw-r--r--   0        0        0     1394 2023-06-08 17:25:09.459041 orbit_component_base-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 orbit_component_base-1.0.9/PKG-INFO
```

### Comparing `orbit_component_base-1.0.15/LICENSE.md` & `orbit_component_base-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.15/orbit_component_base/schema/OrbitSessions.py` & `orbit_component_base-1.0.9/orbit_component_base/schema/OrbitSessions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from orbit_component_base.src.orbit_orm import BaseTable, BaseCollection
 from orbit_database import SerialiserType, Doc
 from datetime import datetime
-from loguru import logger as log
 
 
 class SessionsTable (BaseTable):
+
     norm_table_name = 'sessions'
     norm_auditing = True
     norm_codec = SerialiserType.UJSON
     norm_ensure = [
         {'index_name': 'by_when'   , 'duplicates': True , 'func': '{when:14.6f}'},
-        {'index_name': 'by_sid'    , 'duplicates': False, 'func': '{sid}'},
+        {'index_name': 'by_sid'    , 'duplicates': False, 'func': '{sid}', 'force': True},
         {'index_name': 'by_ns'     , 'duplicates': True,  'func': '{ns}'},
     ]
 
     def from_sid (self, sid, transaction=None):
         self.set(self.norm_tb.seek_one('by_sid', Doc({'sid': sid}), txn=transaction))
         return self
 
     @property
     def when (self):
         return datetime.utcfromtimestamp(self._when).strftime('%Y-%m-%d %H:%M:%S')
 
 
 class SessionsCollection (BaseCollection):
+
     table_class = SessionsTable
     table_strip = ['address', 'sid', 'user_id']
-    table_methods = ['get_ids']
-    
+
     def flush (self, nsp):
         limit = Doc({'ns': nsp})
         for result in self.filter(index_name='by_ns', lower=limit, upper=limit):
             result.doc.delete()
         return self
 
     def disconnect (self):
```

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_app.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_app.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_auth.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def activate_user(self, user):
         user.update({'active': True, 'code': None}).save()
         return {'ok': True, 'validate': False}
 
     def activate_session (self, user_id, auth, session):
         SessionsTable().from_doc(Doc({
-            # 'user_id'   : user_id,
+            'user_id'   : user_id,
             'when'      : datetime.now().timestamp(),
             'vendor'    : auth.get('vendor', 'unknown'),
             'platform'  : auth.get('platform', 'unknown'),
             'language'  : auth.get('language', 'unknown'),
             'address'   : session['address'],
             'host_id'   : session['host_id'],
             'sid'       : self._sid,
@@ -93,15 +93,15 @@
             user_id = cipher.decrypt(b64decode(secret)).decode()
             user = UsersTable().from_key(host_id)
             if user.isValid:
                 if user._user_id == user_id:
                     if user._active or world.conf.authentication == 'autoenroll':
                         session['activated'] = True
                         session['perm'] = user._perm
-                        # log.debug(f'Save: {self._sid} / {self._ns} => {session}')
+                        log.debug(f'Save: {self._sid} / {self._ns} => {session}')
                         try:
                             await save_session(self._sid, session)
                             self.activate_session(user._user_id, auth, session)
                         except Exception as e:
                             log.error(e)
                             
                         return {'ok': True, 'validate': False}
```

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_config.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,23 +116,15 @@
         self._path.mkdir(parents=True, exist_ok=True)
         self._conf = ConfigParser()
         self._conf.read(self._file.as_posix())
         for section in ['BASE', 'NETWORK', 'TOOLS', 'DATA', 'SSL', 'DEV']:
             if section not in self._conf.sections():
                 self._conf.add_section(section)
                 self._changed = True
-                
-        if system() == 'Darwin':
-            code_path = f'/Applications/{self._appl}.app/Contents/Resources/'
-        else:
-            if world.args.dev:
-                code_path = f'~/{self._appl}/server'
-            else:
-                code_path = f'/opt/{self._appl}'
-
+        code_path = f'/Applications/{self._appl}.app/Contents/Resources/' if system() == 'Darwin' else f'/opt/{self._appl}'
         self._option('BASE', 'path', f'~/.local/{self._appl}', 'base location for this application')
         self._option('BASE', 'code', code_path, "where the application's code is located")
         self._option('BASE', 'authentication', self.BASE_authentication, 'the default type of authentication (autoenroll/secure)')
         self._option('SSL', 'name', 'localhost', 'the host name (CN) for our SSL certificate')
         self._option('SSL', 'ssl', 'ssl', 'the folder to store SSL files in')
         self._option('SSL', 'secure', 'true', 'whether to use SSL or not')
         self._option('NETWORK', 'host', '127.0.0.1', 'the host to expose the server on, use "0.0.0.0" for a local network')
```

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_database.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_database.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_decorators.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -91,38 +91,7 @@
                         await sleep(0.1)
                         continue
                     return await run_and_log(func, args, kwargs)
             except Exception as e:
                 log.exception(e)
         return wrapper
     return navGuard
-
-
-def Sentry(fn=None):
-    def navGuard(func):
-        @functools.wraps(func)
-        async def wrapper(*args, **kwargs):
-            try:
-                retrying = False
-                while True:
-                    try:
-                        session = await args[0].get_session(args[1])
-                    except KeyError:
-                        log.warning('<< disconnected dead session >>')
-                        return {'ok': False, 'error': 'Server was restarted'}
-                    except Exception as e:
-                        log.exception(e)
-                        raise
-                    if not session.get('activated', False):
-                        if not retrying:
-                            log.debug(f'<< waiting for authentication >> {args[1]}')
-                            retrying = True
-                        await sleep(0.1)
-                        continue
-                    if fn and not fn(args, session, func.__name__, args[3]):
-                        log.error(error := f'you do not have permission to access this endpoint: {args[1]}')
-                        return { 'ok': False, 'error': error }
-                    return await run_and_log(func, args, kwargs)
-            except Exception as e:
-                log.exception(e)
-        return wrapper
-    return navGuard
```

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_make_ssl.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_make_ssl.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_nql.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_nql_buffer.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_buffer.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_nql_emitter.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_emitter.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_nql_session.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_session.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_orm.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_orm.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_plugin.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from socketio import AsyncNamespace
 from orbit_component_base.src.orbit_nql import NQL
 from orbit_component_base.src.orbit_auth import OrbitAuth
 from orbit_component_base.src.orbit_decorators import navGuard
 from orbit_component_base.schema.OrbitSessions import SessionsCollection
 from orbit_component_base.schema.OrbitSessions import SessionsTable
+from orbit_component_base.schema.OrbitVersions import VersionsCollection
 from loguru import logger as log
 
 
 class PluginBase (AsyncNamespace):
 
     NAMESPACE = ''
     COLLECTIONS = []
 
     @property
     def ns (self):
         return f'/{self.NAMESPACE}'
 
     def __init__(self, *args, **kwargs):
-        # log.debug(f'Initialise namespace: {self.ns}')
+        log.debug(f'Initialise namespace: {self.ns}')
         kwargs['namespace'] = self.ns
         self._odb = kwargs.pop('odb')
         self._nql = None
         self._collections = []
         super().__init__(*args, **kwargs)
 
     def open (self, nql=True):
-        log.debug(f'Open namespace: {self.ns} / {nql}')
         if nql:
             self._nql = NQL(self.emit, self.ns).open()
         for cls in self.COLLECTIONS:
             cls().open(self._odb, self._nql)
         if nql:
             SessionsCollection().flush(self.ns)
         return self
@@ -42,17 +42,22 @@
         await self.save_session(sid, {
             'sid': sid,
             'address': environ['aiohttp.request'].transport.get_extra_info('peername')[0]
         })
         self._nql.connect(sid)
 
     async def on_disconnect(self, sid):
+        log.error(f"DISCONNECT={sid}")
         self._nql.disconnect(sid)
         SessionsTable().from_sid(sid).delete()
 
+    async def on_get_version (self, sid, product, version):
+        log.debug(f"NS={self.ns} product={product} version={version}")
+        return await VersionsCollection(sid=sid, session=await self.get_session(sid), ns=self.ns).get_version(product, version)
+
     async def on_auth_hello(self, sid, auth):
         return await OrbitAuth(sid, self.ns).hello(auth, self.get_session, self.save_session)
 
     async def on_auth_validate(self, sid, auth):
         log.info(f'Validate: {sid} / {self.NAMESPACE}')
         return await OrbitAuth(sid, self.ns).validate(auth, self.get_session, self.save_session)
```

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_plugins.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugins.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_router.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_router.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.15/orbit_component_base/src/orbit_shared.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_shared.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-1.0.15/pyproject.toml` & `orbit_component_base-1.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-base"
-version = "1.0.15"
+version = "1.0.9"
 description = "Orbit Framework - base component"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "orbit_component_base"}]
 include = ['README.md', 'LICENSE.md']
 keywords = ['orbit-framework', 'orbit-component', 'orbit-database']
@@ -24,21 +24,20 @@
 [project.urls]
 "Homepage" = "https://gitlab.com/madpenguin/orbit-component-base"
 "Bug Tracker" = "https://gitlab.com/madpenguin/orbit-component-base/-/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 python-socketio = "^5.8.0"
-orbit-database = "^1.0"
+orbit-database = "^0.99.91"
 loguru = "^0.7.0"
 ujson = "^5.7.0"
 pycryptodome = "^3.18.0"
 tqdm = "^4.65.0"
 aiohttp = "^3.8.4"
-rich = "^13.4.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `orbit_component_base-1.0.15/PKG-INFO` & `orbit_component_base-1.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-component-base
-Version: 1.0.15
+Version: 1.0.9
 Summary: Orbit Framework - base component
 Home-page: https://gitlab.com/madpenguin/orbit-component-base
 License: MIT
 Keywords: orbit-framework,orbit-component,orbit-database
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
@@ -15,18 +15,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: orbit-database (>=1.0,<2.0)
+Requires-Dist: orbit-database (>=0.99.91,<0.100.0)
 Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
 Requires-Dist: python-socketio (>=5.8.0,<6.0.0)
-Requires-Dist: rich (>=13.4.1,<14.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Project-URL: Documentation, https://gitlab.com/madpenguin/orbit-component-base
 Project-URL: Repository, https://gitlab.com/madpenguin/orbit-component-base
 Description-Content-Type: text/markdown
 
 # Orbit Component :: Base : Server
```

