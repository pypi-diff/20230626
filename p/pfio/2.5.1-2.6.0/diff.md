# Comparing `tmp/pfio-2.5.1.tar.gz` & `tmp/pfio-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfio-2.5.1.tar", last modified: Tue Feb  7 10:38:53 2023, max compression
+gzip compressed data, was "pfio-2.6.0.tar", last modified: Mon Jun 26 09:52:18 2023, max compression
```

## Comparing `pfio-2.5.1.tar` & `pfio-2.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-02-07 10:38:53.875869 pfio-2.5.1/
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1064 2022-07-29 03:35:32.000000 pfio-2.5.1/LICENSE
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     2281 2023-02-07 10:38:53.875869 pfio-2.5.1/PKG-INFO
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1421 2022-07-29 03:35:32.000000 pfio-2.5.1/README.md
-drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-02-07 10:38:53.872536 pfio-2.5.1/pfio/
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)       94 2022-07-29 03:35:32.000000 pfio-2.5.1/pfio/__init__.py
-drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-02-07 10:38:53.875869 pfio-2.5.1/pfio/cache/
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     2031 2022-11-16 00:53:29.000000 pfio-2.5.1/pfio/cache/__init__.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    12895 2023-01-31 03:32:03.000000 pfio-2.5.1/pfio/cache/file_cache.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     5161 2023-02-07 10:07:31.000000 pfio-2.5.1/pfio/cache/http_cache.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     3537 2022-07-29 03:35:32.000000 pfio-2.5.1/pfio/cache/mmap_file_cache.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    14863 2023-02-07 08:22:42.000000 pfio-2.5.1/pfio/cache/multiprocess_file_cache.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1141 2022-07-29 03:35:32.000000 pfio-2.5.1/pfio/cache/naive.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    18660 2023-02-07 10:07:31.000000 pfio-2.5.1/pfio/cache/sparse_file.py
-drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-02-07 10:38:53.875869 pfio-2.5.1/pfio/testing/
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     4124 2022-11-16 00:53:29.000000 pfio-2.5.1/pfio/testing/__init__.py
-drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-02-07 10:38:53.875869 pfio-2.5.1/pfio/v2/
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      755 2022-10-06 00:27:41.000000 pfio-2.5.1/pfio/v2/__init__.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    15149 2023-02-07 10:09:07.000000 pfio-2.5.1/pfio/v2/fs.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    12249 2023-02-07 10:07:31.000000 pfio-2.5.1/pfio/v2/hdfs.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     5164 2023-02-07 10:07:31.000000 pfio-2.5.1/pfio/v2/local.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     5344 2022-07-29 03:35:32.000000 pfio-2.5.1/pfio/v2/pathlib.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    19085 2023-02-07 10:09:07.000000 pfio-2.5.1/pfio/v2/s3.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     9467 2023-02-07 10:07:31.000000 pfio-2.5.1/pfio/v2/zip.py
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)       22 2023-02-07 10:37:59.000000 pfio-2.5.1/pfio/version.py
-drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-02-07 10:38:53.875869 pfio-2.5.1/pfio.egg-info/
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     2281 2023-02-07 10:38:53.000000 pfio-2.5.1/pfio.egg-info/PKG-INFO
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      562 2023-02-07 10:38:53.000000 pfio-2.5.1/pfio.egg-info/SOURCES.txt
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)        1 2023-02-07 10:38:53.000000 pfio-2.5.1/pfio.egg-info/dependency_links.txt
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)        1 2022-09-26 06:27:07.000000 pfio-2.5.1/pfio.egg-info/not-zip-safe
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      192 2023-02-07 10:38:53.000000 pfio-2.5.1/pfio.egg-info/requires.txt
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)        5 2023-02-07 10:38:53.000000 pfio-2.5.1/pfio.egg-info/top_level.txt
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      343 2023-02-07 10:38:53.875869 pfio-2.5.1/setup.cfg
--rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     2144 2023-02-07 10:07:31.000000 pfio-2.5.1/setup.py
+drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-06-26 09:52:18.891142 pfio-2.6.0/
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1064 2022-08-01 01:58:37.000000 pfio-2.6.0/LICENSE
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     2148 2023-06-26 09:52:18.891142 pfio-2.6.0/PKG-INFO
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1340 2023-06-26 09:42:38.000000 pfio-2.6.0/README.md
+drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-06-26 09:52:18.887809 pfio-2.6.0/pfio/
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)       94 2022-08-01 01:58:37.000000 pfio-2.6.0/pfio/__init__.py
+drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-06-26 09:52:18.887809 pfio-2.6.0/pfio/cache/
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     2031 2023-03-20 05:53:44.000000 pfio-2.6.0/pfio/cache/__init__.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    12899 2023-06-26 09:42:38.000000 pfio-2.6.0/pfio/cache/file_cache.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     5161 2023-03-20 05:53:44.000000 pfio-2.6.0/pfio/cache/http_cache.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     3537 2022-08-01 01:58:37.000000 pfio-2.6.0/pfio/cache/mmap_file_cache.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    14863 2022-08-01 01:58:37.000000 pfio-2.6.0/pfio/cache/multiprocess_file_cache.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     1141 2022-08-01 01:58:37.000000 pfio-2.6.0/pfio/cache/naive.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    18668 2023-06-26 09:42:38.000000 pfio-2.6.0/pfio/cache/sparse_file.py
+drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-06-26 09:52:18.887809 pfio-2.6.0/pfio/testing/
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     4164 2023-06-26 09:42:38.000000 pfio-2.6.0/pfio/testing/__init__.py
+drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-06-26 09:52:18.891142 pfio-2.6.0/pfio/v2/
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      755 2022-08-01 01:58:37.000000 pfio-2.6.0/pfio/v2/__init__.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    14518 2023-06-26 09:42:38.000000 pfio-2.6.0/pfio/v2/fs.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    12419 2023-06-26 09:42:38.000000 pfio-2.6.0/pfio/v2/hdfs.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     5318 2023-06-26 09:42:38.000000 pfio-2.6.0/pfio/v2/local.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     5344 2022-08-01 01:58:37.000000 pfio-2.6.0/pfio/v2/pathlib.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)    19105 2023-06-26 09:42:38.000000 pfio-2.6.0/pfio/v2/s3.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     9656 2023-06-26 09:42:38.000000 pfio-2.6.0/pfio/v2/zip.py
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)       22 2023-06-26 09:43:31.000000 pfio-2.6.0/pfio/version.py
+drwxr-xr-x   0 kuenishi  (1000) kuenishi  (1000)        0 2023-06-26 09:52:18.887809 pfio-2.6.0/pfio.egg-info/
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     2148 2023-06-26 09:52:18.000000 pfio-2.6.0/pfio.egg-info/PKG-INFO
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      562 2023-06-26 09:52:18.000000 pfio-2.6.0/pfio.egg-info/SOURCES.txt
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)        1 2023-06-26 09:52:18.000000 pfio-2.6.0/pfio.egg-info/dependency_links.txt
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)        1 2023-03-20 05:54:42.000000 pfio-2.6.0/pfio.egg-info/not-zip-safe
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      205 2023-06-26 09:52:18.000000 pfio-2.6.0/pfio.egg-info/requires.txt
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)        5 2023-06-26 09:52:18.000000 pfio-2.6.0/pfio.egg-info/top_level.txt
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)      343 2023-06-26 09:52:18.891142 pfio-2.6.0/setup.cfg
+-rw-r--r--   0 kuenishi  (1000) kuenishi  (1000)     2092 2023-06-26 09:42:38.000000 pfio-2.6.0/setup.py
```

### Comparing `pfio-2.5.1/LICENSE` & `pfio-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pfio-2.5.1/PKG-INFO` & `pfio-2.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: pfio
-Version: 2.5.1
+Version: 2.6.0
 Summary: PFN IO library
 Home-page: http://github.com/pfnet/pfio
 Author: Tianqi Xu, Kota Uenishi
 Author-email: tianqi@preferred.jp, kota@preferred.jp
 Keywords: filesystem hdfs chainer development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Filesystems
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: bench
+Provides-Extra: hdfs
 License-File: LICENSE
 
 ## PFIO
 
 PFIO is an IO abstraction library developed by PFN, optimized for deep
 learning training with batteries included. It supports
 
@@ -33,15 +32,15 @@
 - IO performance tracing and metrics stats, and
 - Fileset container utilities to save metadata.
 
 
 ## Dependency
 
 - HDFS client and libhdfs for HDFS access
-- CPython >= 3.6
+- CPython >= 3.8
 
 ## Installation and Document build
 
 Installation
 
 ```shell
 $ git clone https://github.com/pfnet/pfio.git
@@ -52,34 +51,27 @@
 Documentation
 ```sh
 $ cd pfio/docs
 $ make html
 $ open build/html/index.html
 ```
 
-Test
-```sh
-$ cd pfio
-$ pip install .[test]
-$ pytest tests/
-```
-
 ## How to use
 
 Please refer to the [official document](https://pfio.readthedocs.io) for more information about the usage.
 
 ## Release
 
 Check [the official document](https://packaging.python.org/tutorials/packaging-projects/) for latest release procedure.
 
 Run tests locally:
 
 ```sh
-$ pip install --user -e .[test]
-$ pytest
+$ pip install tox
+$ tox
 ```
 
 Bump version numbers in `pfio/version.py` .
 
 Push and open a pull request to invoke CI. Once CI passed and the pull request merged,
 tag a release:
```

### Comparing `pfio-2.5.1/README.md` & `pfio-2.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 - IO performance tracing and metrics stats, and
 - Fileset container utilities to save metadata.
 
 
 ## Dependency
 
 - HDFS client and libhdfs for HDFS access
-- CPython >= 3.6
+- CPython >= 3.8
 
 ## Installation and Document build
 
 Installation
 
 ```shell
 $ git clone https://github.com/pfnet/pfio.git
@@ -27,34 +27,27 @@
 Documentation
 ```sh
 $ cd pfio/docs
 $ make html
 $ open build/html/index.html
 ```
 
-Test
-```sh
-$ cd pfio
-$ pip install .[test]
-$ pytest tests/
-```
-
 ## How to use
 
 Please refer to the [official document](https://pfio.readthedocs.io) for more information about the usage.
 
 ## Release
 
 Check [the official document](https://packaging.python.org/tutorials/packaging-projects/) for latest release procedure.
 
 Run tests locally:
 
 ```sh
-$ pip install --user -e .[test]
-$ pytest
+$ pip install tox
+$ tox
 ```
 
 Bump version numbers in `pfio/version.py` .
 
 Push and open a pull request to invoke CI. Once CI passed and the pull request merged,
 tag a release:
```

### Comparing `pfio-2.5.1/pfio/cache/__init__.py` & `pfio-2.6.0/pfio/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `pfio-2.5.1/pfio/cache/file_cache.py` & `pfio-2.6.0/pfio/cache/file_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from struct import calcsize, pack, unpack
 
 from pfio import cache
 
 # Deprecated, but leaving for backward compatibility just in case any
 # system directly using this value
 _DEFAULT_CACHE_PATH = os.path.join(
-    os.getenv('HOME'), ".pfio", "cache")
+    os.getenv('HOME', ""), ".pfio", "cache")
 
 _FORCE_LOCAL = True
 
 
 def _default_cache_path():
     basedir = os.getenv('XDG_CACHE_HOME')
```

### Comparing `pfio-2.5.1/pfio/cache/http_cache.py` & `pfio-2.6.0/pfio/cache/http_cache.py`

 * *Files identical despite different names*

### Comparing `pfio-2.5.1/pfio/cache/mmap_file_cache.py` & `pfio-2.6.0/pfio/cache/mmap_file_cache.py`

 * *Files identical despite different names*

### Comparing `pfio-2.5.1/pfio/cache/multiprocess_file_cache.py` & `pfio-2.6.0/pfio/cache/multiprocess_file_cache.py`

 * *Files identical despite different names*

### Comparing `pfio-2.5.1/pfio/cache/naive.py` & `pfio-2.6.0/pfio/cache/naive.py`

 * *Files identical despite different names*

### Comparing `pfio-2.5.1/pfio/cache/sparse_file.py` & `pfio-2.6.0/pfio/cache/sparse_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import shutil
 import struct
 import tempfile
 from contextlib import contextmanager
 from dataclasses import dataclass
 from types import TracebackType
-from typing import Optional
+from typing import Optional, Tuple
 
 from .file_cache import DummyLock, RWLock
 
 
 @dataclass(frozen=True)
 class _Range:
     start: int
@@ -121,15 +121,15 @@
         raise NotImplementedError()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type: Optional[BaseException],
                  exc_value: Optional[BaseException],
-                 traceback: Optional[TracebackType]) -> bool:
+                 traceback: Optional[TracebackType]):
         self.close()
 
     def flush(self):
         pass
 
     @property
     def closed(self):
@@ -280,15 +280,15 @@
             # [ r1 [ ] r0 ]
             yield self._get_range(_Range(r0.start, r1.right - r0.start,
                                          r1.cached))
             # print('[ r1 [ ] r0 ]', r, len(data))
 
             r0 = _Range(r1.right, r0.right - r1.right)
 
-    def _get_range(self, r) -> (bytearray, _Range):
+    def _get_range(self, r: _Range) -> Tuple[bytes, _Range]:
         # print('get range:', r)
         if r.cached:
             return os.pread(self.cachefp.fileno(), r.length, r.start), r
 
         assert not self._frozen
         self.fileobj.seek(r.start, io.SEEK_SET)
         data = self.fileobj.read(r.length)
```

### Comparing `pfio-2.5.1/pfio/testing/__init__.py` & `pfio-2.6.0/pfio/testing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import http.server
 import os
 import random
 import string
 import subprocess
 from contextlib import contextmanager
 from threading import Thread
+from typing import Dict
 from unittest import mock
 from zipfile import ZipFile
 
 
 class ZipForTest:
     def __init__(self, destfile, data=None):
         if data is None:
@@ -88,15 +89,15 @@
                 subprocess.run = orig_method
 
         return wrapper
     return decorator
 
 
 class OnMemoryHTTPServerForTest(http.server.BaseHTTPRequestHandler):
-    files = {}
+    files: Dict[str, str] = {}
 
     def do_GET(self):
         content = OnMemoryHTTPServerForTest.files.get(self.path)
 
         if content is None:
             self.send_response_only(http.HTTPStatus.NOT_FOUND)
             self.end_headers()
```

### Comparing `pfio-2.5.1/pfio/v2/__init__.py` & `pfio-2.6.0/pfio/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `pfio-2.5.1/pfio/v2/fs.py` & `pfio-2.6.0/pfio/v2/fs.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,22 +102,24 @@
     @abstractmethod
     def open(self, file_path: str, mode: str = 'rb',
              buffering: int = -1, encoding: Optional[str] = None,
              errors: Optional[str] = None,
              newline: Optional[str] = None,
              closefd: bool = True,
              opener: Optional[Callable[
-                 [str, int], Any]] = None) -> Type["IOBase"]:
+                 [str, int], Any]] = None) -> IOBase:
         raise NotImplementedError()
 
-    def open_zip(self, file_path: str, mode='r', **kwargs) -> Type["Zip"]:  # NOQA
-        from .zip import Zip
-        return Zip(self, file_path, mode, **kwargs)
+    def open_zip(self, file_path: str, mode='r', **kwargs):
+        # Avoid circular import
+        from .zip import _open_zip
+        return _open_zip(self, file_path, mode, **kwargs)
 
-    def subfs(self, rel_path: str) -> Type["FS"]:
+    # Self-typing needs Python 3.11, PEP-673
+    def subfs(self, rel_path: str) -> 'FS':
         '''Virtually changes the working directory
 
         By default it performs shallow copy. If any resource that as
         different lifecycles than the copy source (e.g. HDFS
         connection and zipfile.ZipFile object), they also will be
         copied by overriding this method.
 
@@ -195,15 +197,15 @@
         raise NotImplementedError()
 
     def __enter__(self) -> 'FS':
         return self
 
     def __exit__(self, exc_type: Optional[Type[BaseException]],
                  exc_value: Optional[BaseException],
-                 traceback: Optional[TracebackType]) -> bool:
+                 traceback: Optional[TracebackType]):
         self.close()
 
     @abstractmethod
     def isdir(self, file_path: str) -> bool:
         """Returns ``True`` if the path is an existing directory
 
         Args:
@@ -286,15 +288,15 @@
                    When the path is a file, this option is ignored.
 
         """
         raise NotImplementedError()
 
 
 @contextlib.contextmanager
-def open_url(url: str, mode: str = 'r', **kwargs) -> 'IOBase':
+def open_url(url: str, mode: str = 'r', **kwargs) -> Iterator[IOBase]:
     '''Opens a file regardless of the backend FS type
 
     ``url`` must be compliant with URL standard in
     https://url.spec.whatwg.org/ .  As this function implements
     context manager, the FileObject can be written as::
 
        with open_url("s3://bucket.example.com/path/your-file.txt", 'r') as f:
@@ -456,34 +458,12 @@
         raise RuntimeError("bug: scheme '{}' is not supported".format(scheme))
 
     return fs
 
 
 @deprecated(deprecated_in='2.2.0', removed_in='2.3.0',
             current_version=__version__)
-def lazify(init_func, lazy_init=True, recreate_on_fork=True) -> "FS":
+def lazify(init_func, lazy_init=True, recreate_on_fork=True):
     '''Make FS init lazy and recreate on fork
 
     '''
-    return _LazyFS(init_func, lazy_init, recreate_on_fork)
-
-
-class _LazyFS:
-    def __init__(self, func, lazy_init, recreate_on_fork):
-        if not lazy_init:
-            self.mixin = func()
-        else:
-            self.mixin = None
-        self.func = func
-
-    def __getattr__(self, attr):
-        if self.mixin is None or self.mixin.is_forked:
-            self.mixin = self.func()
-        return getattr(self.mixin, attr)
-
-    def __enter__(self) -> 'FS':
-        return self
-
-    def __exit__(self, exc_type: Optional[Type[BaseException]],
-                 exc_value: Optional[BaseException],
-                 traceback: Optional[TracebackType]) -> bool:
-        self.close()
+    pass
```

### Comparing `pfio-2.5.1/pfio/v2/hdfs.py` & `pfio-2.6.0/pfio/v2/hdfs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 import io
 import logging
 import multiprocessing
 import os
 import re
 import subprocess
 import warnings
+from typing import Optional
 from xml.etree import ElementTree
 
-import pyarrow
-from pyarrow.fs import FileSelector, FileType, HadoopFileSystem
+try:
+    import pyarrow
+    from pyarrow.fs import FileSelector, FileType, HadoopFileSystem
+    has_hdfs = True
+except ImportError:
+    has_hdfs = False
 
 from .fs import FS, FileStat, ForkedError
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.StreamHandler())
 
 
@@ -302,21 +307,21 @@
 
     def subfs(self, rel_path):
         return Hdfs(os.path.join(self.cwd, rel_path))
 
     def close(self):
         pass
 
-    def list(self, path: str = "", recursive=False, detail=False):
+    def list(self, path: Optional[str] = "", recursive=False, detail=False):
         self._checkfork()
 
         if not self.isdir(path):
             raise NotADirectoryError(path)
 
-        path = os.path.join(self.cwd, path)
+        path = os.path.join(self.cwd, "" if path is None else path)
         norm_path = self._fs.normalize_path(path).rstrip('/')
 
         infos = self._fs.get_file_info(FileSelector(path, recursive=recursive))
         for file_info in infos:
             if detail:
                 yield HdfsFileStat(file_info)
             else:
@@ -327,17 +332,17 @@
         path = os.path.join(self.cwd, path)
         info = self._fs.get_file_info(path)
         if info.type == FileType.NotFound:
             raise FileNotFoundError()
         else:
             return HdfsFileStat(info)
 
-    def isdir(self, path: str):
+    def isdir(self, path: Optional[str]):
         self._checkfork()
-        path = os.path.join(self.cwd, path)
+        path = os.path.join(self.cwd, "" if path is None else path)
         info = self._fs.get_file_info(path)
         return info.type == FileType.Directory
 
     def mkdir(self, path: str, *args, dir_fd=None):
         self._checkfork()
         path = os.path.join(self.cwd, path)
         return self._fs.create_dir(path)
```

### Comparing `pfio-2.5.1/pfio/v2/local.py` & `pfio-2.6.0/pfio/v2/local.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import io
 import os
 import shutil
+from typing import Optional
 
 from .fs import FS, FileStat
 
 
 class LocalFileStat(FileStat):
     """Detailed information of a POSIX file
 
@@ -62,29 +63,34 @@
     @property
     def cwd(self):
         if self._cwd:
             return self._cwd
 
         return os.getcwd()
 
+    @cwd.setter
+    def cwd(self, value: str):
+        self._cwd = value
+
     def _reset(self):
         pass
 
     def open(self, file_path, mode='r',
              buffering=-1, encoding=None, errors=None,
              newline=None, closefd=True, opener=None):
 
         path = os.path.join(self.cwd, file_path)
         return io.open(path, mode,
                        buffering, encoding, errors,
                        newline, closefd, opener)
 
-    def list(self, path_or_prefix: str = '', recursive=False,
+    def list(self, path: Optional[str] = '', recursive=False,
              detail=False):
-        path_or_prefix = os.path.join(self.cwd, path_or_prefix)
+        path_or_prefix = os.path.join(self.cwd,
+                                      "" if path is None else path)
 
         if recursive:
             path_or_prefix = path_or_prefix.rstrip("/")
             # plus 1 to include the trailing slash
             prefix_end_index = len(path_or_prefix) + 1
             yield from self._recursive_list(prefix_end_index,
                                             path_or_prefix, detail)
```

### Comparing `pfio-2.5.1/pfio/v2/pathlib.py` & `pfio-2.6.0/pfio/v2/pathlib.py`

 * *Files identical despite different names*

### Comparing `pfio-2.5.1/pfio/v2/s3.py` & `pfio-2.6.0/pfio/v2/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         self._closed = True
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type: Optional[Type[BaseException]],
                  exc_value: Optional[BaseException],
-                 traceback: Optional[TracebackType]) -> bool:
+                 traceback: Optional[TracebackType]):
         self.close()
 
     def flush(self):
         pass
 
     @property
     def closed(self):
@@ -257,15 +257,15 @@
         self.buf = None
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type: Optional[Type[BaseException]],
                  exc_value: Optional[BaseException],
-                 traceback: Optional[TracebackType]) -> bool:
+                 traceback: Optional[TracebackType]):
         self.close()
 
     @property
     def closed(self):
         return self.buf is None
 
     def isatty(self):
@@ -429,23 +429,23 @@
                 obj = io.BufferedWriter(obj)
 
         else:
             raise RuntimeError(f'Unknown option: {mode}')
 
         return obj
 
-    def list(self, prefix: str = "", recursive=False, detail=False):
+    def list(self, prefix: Optional[str] = "", recursive=False, detail=False):
         '''List all objects (and prefixes)
 
         Although there is not concept of directory in AWS S3 API,
         common prefixes shows up like directories.
 
         '''
         self._checkfork()
-        key = os.path.join(self.cwd, prefix)
+        key = os.path.join(self.cwd, "" if prefix is None else prefix)
         key = _normalize_key(key)
         if key == '.':
             key = ''
         elif key != '' and not key.endswith('/'):
             key += '/'
         if '/../' in key or key.startswith('..'):
             raise ValueError('Invalid S3 key: {} as {}'.format(prefix, key))
```

### Comparing `pfio-2.5.1/pfio/v2/zip.py` & `pfio-2.6.0/pfio/v2/zip.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import io
 import logging
 import os
 import zipfile
 from datetime import datetime
+from typing import Optional
 
 from pfio.cache.sparse_file import MPCachedWrapper
 
 from .fs import FS, FileStat
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.StreamHandler())
@@ -162,15 +163,15 @@
             actual_path = path + '/'
         else:
             raise FileNotFoundError(
                 "{} is not found".format(path))
 
         return ZipFileStat(self.zipobj.getinfo(actual_path))
 
-    def list(self, path_or_prefix: str = "", recursive=False,
+    def list(self, path_or_prefix: Optional[str] = "", recursive=False,
              detail=False):
         self._checkfork()
 
         if path_or_prefix:
             path_or_prefix = os.path.join(self.cwd,
                                           os.path.normpath(path_or_prefix))
             # cannot move beyond root
@@ -192,14 +193,15 @@
                 # such kind of zip can be made with "zip -D"
                 raise FileNotFoundError(
                     "{} is not found".format(path_or_prefix))
 
         if recursive:
             for info in self.zipobj.infolist():
                 name = info.filename
+                assert path_or_prefix is not None
                 if name.startswith(path_or_prefix):
                     name = name[len(path_or_prefix):].strip("/")
                     if name:
                         if detail:
                             yield ZipFileStat(info)
                         else:
                             yield name
@@ -256,7 +258,11 @@
                 or file_path + "/" in namelist)
 
     def rename(self, *args):
         raise io.UnsupportedOperation
 
     def remove(self, file_path, recursive=False):
         raise io.UnsupportedOperation
+
+
+def _open_zip(fs, file_path, mode, **kwargs) -> Zip:
+    return Zip(fs, file_path, mode, **kwargs)
```

### Comparing `pfio-2.5.1/pfio.egg-info/PKG-INFO` & `pfio-2.6.0/pfio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: pfio
-Version: 2.5.1
+Version: 2.6.0
 Summary: PFN IO library
 Home-page: http://github.com/pfnet/pfio
 Author: Tianqi Xu, Kota Uenishi
 Author-email: tianqi@preferred.jp, kota@preferred.jp
 Keywords: filesystem hdfs chainer development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Filesystems
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: bench
+Provides-Extra: hdfs
 License-File: LICENSE
 
 ## PFIO
 
 PFIO is an IO abstraction library developed by PFN, optimized for deep
 learning training with batteries included. It supports
 
@@ -33,15 +32,15 @@
 - IO performance tracing and metrics stats, and
 - Fileset container utilities to save metadata.
 
 
 ## Dependency
 
 - HDFS client and libhdfs for HDFS access
-- CPython >= 3.6
+- CPython >= 3.8
 
 ## Installation and Document build
 
 Installation
 
 ```shell
 $ git clone https://github.com/pfnet/pfio.git
@@ -52,34 +51,27 @@
 Documentation
 ```sh
 $ cd pfio/docs
 $ make html
 $ open build/html/index.html
 ```
 
-Test
-```sh
-$ cd pfio
-$ pip install .[test]
-$ pytest tests/
-```
-
 ## How to use
 
 Please refer to the [official document](https://pfio.readthedocs.io) for more information about the usage.
 
 ## Release
 
 Check [the official document](https://packaging.python.org/tutorials/packaging-projects/) for latest release procedure.
 
 Run tests locally:
 
 ```sh
-$ pip install --user -e .[test]
-$ pytest
+$ pip install tox
+$ tox
 ```
 
 Bump version numbers in `pfio/version.py` .
 
 Push and open a pull request to invoke CI. Once CI passed and the pull request merged,
 tag a release:
```

### Comparing `pfio-2.5.1/pfio.egg-info/SOURCES.txt` & `pfio-2.6.0/pfio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pfio-2.5.1/setup.py` & `pfio-2.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,32 +35,31 @@
 
         'Intended Audience :: Developers',
 
         'License :: OSI Approved :: MIT License',
         'Operating System :: POSIX',
         'Operating System :: POSIX :: Linux',
 
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
 
         'Topic :: System :: Filesystems',
     ],
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     package_data={'pfio': package_data},
     extras_require={
-        'test': ['pytest', 'flake8', 'autopep8', 'parameterized', 'isort', 'moto[server]', 'numpy'],
+        'test': ['pytest', 'flake8', 'autopep8', 'parameterized', 'isort', 'moto[server]', 'numpy', 'mypy'],
         # When updating doc deps, docs/requirements.txt should be updated too
         'doc': ['sphinx', 'sphinx_rtd_theme'],
         'bench': ['numpy>=1.19.5', 'torch>=1.9.0', 'Pillow<=8.2.0'],
+        'hdfs': ['pyarrow>=6.0.0'],
     },
-    python_requires=">=3.7",
     # When updating install requires, docs/requirements.txt should be updated too
-    install_requires=['pyarrow>=6.0.0', 'boto3', 'deprecation', 'urllib3'],
+    install_requires=['boto3', 'deprecation', 'urllib3'],
     include_package_data=True,
     zip_safe=False,
 
     keywords='filesystem hdfs chainer development',
 )
```

