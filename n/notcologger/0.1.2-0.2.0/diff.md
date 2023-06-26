# Comparing `tmp/notcologger-0.1.2.tar.gz` & `tmp/notcologger-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/notcologger-0.1.2.tar", last modified: Tue Jul  7 09:44:34 2020, max compression
+gzip compressed data, was "notcologger-0.2.0.tar", max compression
```

## Comparing `notcologger-0.1.2.tar` & `notcologger-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,6 @@
-drwxr-xr-x   0 jmtapio    (501) staff       (20)        0 2020-07-07 09:44:34.000000 notcologger-0.1.2/
--rw-r--r--   0 jmtapio    (501) staff       (20)       18 2020-04-23 11:05:28.000000 notcologger-0.1.2/MANIFEST.in
--rw-r--r--   0 jmtapio    (501) staff       (20)      712 2020-07-07 09:44:34.000000 notcologger-0.1.2/PKG-INFO
--rw-r--r--   0 jmtapio    (501) staff       (20)     1099 2020-04-23 11:05:28.000000 notcologger-0.1.2/README.md
-drwxr-xr-x   0 jmtapio    (501) staff       (20)        0 2020-07-07 09:44:34.000000 notcologger-0.1.2/notcologger/
--rw-r--r--   0 jmtapio    (501) staff       (20)     6396 2020-07-07 09:44:05.000000 notcologger-0.1.2/notcologger/__init__.py
-drwxr-xr-x   0 jmtapio    (501) staff       (20)        0 2020-07-07 09:44:34.000000 notcologger-0.1.2/notcologger.egg-info/
--rw-r--r--   0 jmtapio    (501) staff       (20)      712 2020-07-07 09:44:33.000000 notcologger-0.1.2/notcologger.egg-info/PKG-INFO
--rw-r--r--   0 jmtapio    (501) staff       (20)      224 2020-07-07 09:44:33.000000 notcologger-0.1.2/notcologger.egg-info/SOURCES.txt
--rw-r--r--   0 jmtapio    (501) staff       (20)        1 2020-07-07 09:44:33.000000 notcologger-0.1.2/notcologger.egg-info/dependency_links.txt
--rw-r--r--   0 jmtapio    (501) staff       (20)       12 2020-07-07 09:44:33.000000 notcologger-0.1.2/notcologger.egg-info/top_level.txt
--rw-r--r--   0 jmtapio    (501) staff       (20)        1 2020-04-23 11:09:35.000000 notcologger-0.1.2/notcologger.egg-info/zip-safe
--rw-r--r--   0 jmtapio    (501) staff       (20)       38 2020-07-07 09:44:34.000000 notcologger-0.1.2/setup.cfg
--rwxr-xr-x   0 jmtapio    (501) staff       (20)      931 2020-07-07 09:44:05.000000 notcologger-0.1.2/setup.py
+-rw-r--r--   0        0        0     1079 2023-06-26 20:02:44.730633 notcologger-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2622 2023-06-26 19:39:59.035130 notcologger-0.2.0/README.md
+-rw-r--r--   0        0        0     7739 2023-06-26 19:41:12.115961 notcologger-0.2.0/notcologger/__init__.py
+-rw-r--r--   0        0        0      443 2023-06-26 19:40:20.747377 notcologger-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3371 1970-01-01 00:00:00.000000 notcologger-0.2.0/setup.py
+-rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 notcologger-0.2.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `notcologger-0.1.2/notcologger/__init__.py` & `notcologger-0.2.0/notcologger/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import os
 import datetime
 import json
 import uuid
 
-__all__ = ['LogSpan', 'debug', 'info', 'warn', 'error']
+__all__ = ['LogSpan', 'ExceptionSpan', 'debug', 'info', 'warn', 'error']
 
 
 _loglevel_map = {
     'debug': ('debug', 'info', 'warning', 'error'),
     'info': ('info', 'warning', 'error'),
     'warning': ('warning', 'error'),
     'error': ('error',)
@@ -22,28 +22,32 @@
     loggings made with self logger, or one can be generated
     automatically.
     """
     
     def __init__(self, requestId=None):
         self.requestId = requestId or str(uuid.uuid4())
         self.annotation = dict()
+        self._stdout = sys.stdout
+
+    def _make_timestamp(self):
+        return datetime.datetime.now().isoformat()
 
     def _output(self, loglevel='info', **kwargs):
         # Check if self loglevel should get logged, default to debug if unknown level
         if loglevel not in _loglevel_map.get(os.environ.get('NOTCO_LOGLEVEL', 'debug'), 'debug'):
             return
 
         if 'user' in kwargs and kwargs['user'] is None:
             kwargs['user'] = 'SYSTEM'
 
         meta = dict()
         meta.update(self.annotation)
         meta.update(kwargs.get('meta', None) or dict())
-        
-        logentry = dict(timestamp=datetime.datetime.now().isoformat(), level=loglevel, rid=self.requestId)
+
+        logentry = dict(timestamp=self._make_timestamp(), level=loglevel, rid=self.requestId)
         logentry.update(kwargs)
 
         if not logentry['meta']: del logentry['meta']
 
         for key in logentry:
             if isinstance(logentry[key], bytes):
                 logentry[key] = logentry[key].decode('utf-8', errors='ignore')
@@ -52,18 +56,18 @@
             meta = logentry['meta']
             for key in meta:
                 if isinstance(meta[key], bytes):
                     meta[key] = meta[key].decode('utf-8', errors='ignore')
                 elif isinstance(meta[key], BaseException):
                     meta[key] = repr(meta[key])
 
-        sys.stdout.write('{}\n'.format(json.dumps(logentry, skipkeys=True)))
+        self._stdout.write('{}\n'.format(json.dumps(logentry, skipkeys=True)))
 
         if loglevel != 'debug':
-            sys.stdout.flush()
+            self._stdout.flush()
 
     def annotate(self, **kwargs):
         """Add key-value-pairs to add to new logged entrie's metadata
 
         Self method can be used to add recurring metadata items such
         as session id's.
         """
@@ -138,14 +142,53 @@
             type=logtype,
             message=message,
             group=group,
             user=user,
             meta=meta)
 
 
+class ExceptionSpan(LogSpan):
+    """Logger that is activated when an exception is raised in a with-block
+
+    Usage example:
+
+    with ExceptionSpan('mylog.problem', 'Doing something fails') as log:
+        do_something_that_fails()
+
+    """
+
+    def __init__(self, logtype, message, group, requestId=None, level='error', user=None, meta=None):
+        super().__init__(requestId)
+        self.default_level = level
+        self.default_logtype = logtype
+        self.default_message = message
+        self.default_group = group
+        self.default_user = user
+        self.annotation = meta or dict()
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if exc_type:
+            self._output(
+                loglevel = self.default_level,
+                type     = self.default_logtype,
+                message  = self.default_message,
+                group    = self.default_group,
+                user     = self.default_user,
+                meta     = dict(
+                    exc_type = exc_type.__qualname__,
+                    exc_val = str(getattr(exc_val, 'args', ''))
+                    ))
+
+        # We will not catch the exception
+        return None
+
+
 def debug(logtype, message, group=None, user=None, meta=None):
     """Log a debug entry
 
     logtype: a string identifying this logging location, for example "lambda.handler.start"
     message: human readable message
     group: log group, for example technical, session or request
     user: some kind of user identifier
```

