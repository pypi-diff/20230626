# Comparing `tmp/cozo_client-0.1.4.tar.gz` & `tmp/cozo_client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cozo_client-0.1.4.tar", last modified: Sun Jun 25 11:49:49 2023, max compression
+gzip compressed data, was "cozo_client-0.1.5.tar", last modified: Mon Jun 26 10:13:33 2023, max compression
```

## Comparing `cozo_client-0.1.4.tar` & `cozo_client-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-25 11:49:49.871245 cozo_client-0.1.4/
--rw-r--r--   0 zh217      (501) staff       (20)     3106 2023-06-19 09:16:44.000000 cozo_client-0.1.4/.gitignore
--rw-r--r--   0 zh217      (501) staff       (20)      304 2023-06-25 11:49:49.871045 cozo_client-0.1.4/PKG-INFO
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-25 11:49:49.870120 cozo_client-0.1.4/cozo_client/
--rw-r--r--   0 zh217      (501) staff       (20)      464 2023-05-30 06:34:19.000000 cozo_client-0.1.4/cozo_client/__init__.py
--rw-r--r--   0 zh217      (501) staff       (20)     7424 2023-05-30 06:27:28.000000 cozo_client-0.1.4/cozo_client/_builder.py
--rw-r--r--   0 zh217      (501) staff       (20)    29722 2023-06-25 10:45:58.000000 cozo_client-0.1.4/cozo_client/_client.py
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-25 11:49:49.870804 cozo_client-0.1.4/cozo_client.egg-info/
--rw-r--r--   0 zh217      (501) staff       (20)      304 2023-06-25 11:49:49.000000 cozo_client-0.1.4/cozo_client.egg-info/PKG-INFO
--rw-r--r--   0 zh217      (501) staff       (20)      296 2023-06-25 11:49:49.000000 cozo_client-0.1.4/cozo_client.egg-info/SOURCES.txt
--rw-r--r--   0 zh217      (501) staff       (20)        1 2023-06-25 11:49:49.000000 cozo_client-0.1.4/cozo_client.egg-info/dependency_links.txt
--rw-r--r--   0 zh217      (501) staff       (20)       38 2023-06-25 11:49:49.000000 cozo_client-0.1.4/cozo_client.egg-info/requires.txt
--rw-r--r--   0 zh217      (501) staff       (20)       12 2023-06-25 11:49:49.000000 cozo_client-0.1.4/cozo_client.egg-info/top_level.txt
--rw-r--r--   0 zh217      (501) staff       (20)      532 2023-06-25 10:48:08.000000 cozo_client-0.1.4/pyproject.toml
--rw-r--r--   0 zh217      (501) staff       (20)       37 2023-06-13 21:28:10.000000 cozo_client-0.1.4/requirements.txt
--rw-r--r--   0 zh217      (501) staff       (20)       38 2023-06-25 11:49:49.871301 cozo_client-0.1.4/setup.cfg
--rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-20 12:04:30.000000 cozo_client-0.1.4/setup.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-26 10:13:33.466845 cozo_client-0.1.5/
+-rw-r--r--   0 zh217      (501) staff       (20)     3106 2023-06-19 09:16:44.000000 cozo_client-0.1.5/.gitignore
+-rw-r--r--   0 zh217      (501) staff       (20)      304 2023-06-26 10:13:33.466680 cozo_client-0.1.5/PKG-INFO
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-26 10:13:33.465468 cozo_client-0.1.5/cozo_client/
+-rw-r--r--   0 zh217      (501) staff       (20)      464 2023-05-30 06:34:19.000000 cozo_client-0.1.5/cozo_client/__init__.py
+-rw-r--r--   0 zh217      (501) staff       (20)     7424 2023-05-30 06:27:28.000000 cozo_client-0.1.5/cozo_client/_builder.py
+-rw-r--r--   0 zh217      (501) staff       (20)    29809 2023-06-26 08:17:33.000000 cozo_client-0.1.5/cozo_client/_client.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-26 10:13:33.466482 cozo_client-0.1.5/cozo_client.egg-info/
+-rw-r--r--   0 zh217      (501) staff       (20)      304 2023-06-26 10:13:33.000000 cozo_client-0.1.5/cozo_client.egg-info/PKG-INFO
+-rw-r--r--   0 zh217      (501) staff       (20)      296 2023-06-26 10:13:33.000000 cozo_client-0.1.5/cozo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 zh217      (501) staff       (20)        1 2023-06-26 10:13:33.000000 cozo_client-0.1.5/cozo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       38 2023-06-26 10:13:33.000000 cozo_client-0.1.5/cozo_client.egg-info/requires.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       12 2023-06-26 10:13:33.000000 cozo_client-0.1.5/cozo_client.egg-info/top_level.txt
+-rw-r--r--   0 zh217      (501) staff       (20)      532 2023-06-26 08:18:15.000000 cozo_client-0.1.5/pyproject.toml
+-rw-r--r--   0 zh217      (501) staff       (20)       37 2023-06-13 21:28:10.000000 cozo_client-0.1.5/requirements.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       38 2023-06-26 10:13:33.466904 cozo_client-0.1.5/setup.cfg
+-rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-20 12:04:30.000000 cozo_client-0.1.5/setup.py
```

### Comparing `cozo_client-0.1.4/.gitignore` & `cozo_client-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `cozo_client-0.1.4/cozo_client/_builder.py` & `cozo_client-0.1.5/cozo_client/_builder.py`

 * *Files identical despite different names*

### Comparing `cozo_client-0.1.4/cozo_client/_client.py` & `cozo_client-0.1.5/cozo_client/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,39 +356,43 @@
 
 class CozoClient:
     def __init__(self,
                  path: str | None = None,
                  engine: StorageEngine = StorageEngine.mem,
                  remote_host: str = 'http://127.0.0.1:9070/',
                  remote_token: str | None = None,
-                 remote_auth: str | None = None):
+                 remote_auth: str | None = None,
+                 timeout=600):
 
         if engine == StorageEngine.mem and path is not None:
             engine = StorageEngine.sqlite
 
         self.engine = engine
 
         if engine == StorageEngine.remote:
             if remote_host.endswith('/'):
                 remote_host = remote_host[:len(remote_host) - 1]
             self.host = remote_host
             self.embedded = None
             self._remote_sse = {}
             self._remote_cb_id = 0
-            self._session = httpx.Client(timeout=600)
-            self._asession = httpx.AsyncClient(timeout=600)
+            self._session = httpx.Client(timeout=timeout)
+            self._asession = httpx.AsyncClient(timeout=timeout)
             if remote_token:
                 self._session.headers.update({'Authorization': f'Bearer {remote_token}'})
                 self._asession.headers.update({'Authorization': f'Bearer {remote_token}'})
             elif remote_auth:
                 self._session.headers.update({'x-cozo-auth': remote_auth})
                 self._asession.headers.update({'x-cozo-auth': remote_auth})
         else:
             self.embedded = cozo_embedded.CozoDbPy(engine, path or '', '{}')
 
+    def __hash__(self):
+        return id(self)
+
     def ensure_index(self, name: str, idx_name: str, cols: list[str]):
         try:
             existing_cols = self.run(f'::columns {name}:{idx_name}')
             for i, row in enumerate(existing_cols):
                 assert row['column'] == cols[i], f'Column {i} is {row["column"]} not {cols[i]}'
 
         except QueryException as e:
```

### Comparing `cozo_client-0.1.4/pyproject.toml` & `cozo_client-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 ]
 dependencies = [
     "cozo-embedded",
     "httpx",
     "pydantic",
     "openpyxl"
 ]
-version = "0.1.4"
+version = "0.1.5"
```

