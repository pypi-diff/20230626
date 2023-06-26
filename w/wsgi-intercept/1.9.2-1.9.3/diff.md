# Comparing `tmp/wsgi_intercept-1.9.2.tar.gz` & `tmp/wsgi_intercept-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wsgi_intercept-1.9.2.tar", last modified: Wed Feb  5 11:15:55 2020, max compression
+gzip compressed data, was "wsgi_intercept-1.9.3.tar", last modified: Thu Jan 13 14:38:37 2022, max compression
```

## Comparing `wsgi_intercept-1.9.2.tar` & `wsgi_intercept-1.9.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2020-02-05 11:15:55.000000 wsgi_intercept-1.9.2/
--rw-r--r--   0 cdent      (503) staff       (20)     1094 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/LICENSE
--rw-r--r--   0 cdent      (503) staff       (20)       50 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/MANIFEST.in
--rw-r--r--   0 cdent      (503) staff       (20)     1010 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/Makefile
--rw-r--r--   0 cdent      (503) staff       (20)     7275 2020-02-05 11:15:55.000000 wsgi_intercept-1.9.2/PKG-INFO
--rw-r--r--   0 cdent      (503) staff       (20)     5138 2020-02-05 11:15:50.000000 wsgi_intercept-1.9.2/README
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2020-02-05 11:15:55.000000 wsgi_intercept-1.9.2/docs/
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/docs/.gitignore
--rw-r--r--   0 cdent      (503) staff       (20)     6794 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/docs/Makefile
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2020-02-05 11:15:55.000000 wsgi_intercept-1.9.2/docs/_static/
--rw-r--r--   0 cdent      (503) staff       (20)        0 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/docs/_static/.gitignore
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2020-02-05 11:15:55.000000 wsgi_intercept-1.9.2/docs/_templates/
--rw-r--r--   0 cdent      (503) staff       (20)        0 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/docs/_templates/.gitignore
--rw-r--r--   0 cdent      (503) staff       (20)    10608 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/docs/conf.py
--rw-r--r--   0 cdent      (503) staff       (20)     1239 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/docs/http_client.rst
--rw-r--r--   0 cdent      (503) staff       (20)      920 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/docs/httplib2.rst
--rw-r--r--   0 cdent      (503) staff       (20)      352 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/docs/index.rst
--rw-r--r--   0 cdent      (503) staff       (20)      586 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/docs/interceptor.rst
--rw-r--r--   0 cdent      (503) staff       (20)      639 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/docs/requests.rst
--rw-r--r--   0 cdent      (503) staff       (20)      780 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/docs/urllib.rst
--rw-r--r--   0 cdent      (503) staff       (20)      671 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/docs/urllib3.rst
--rw-r--r--   0 cdent      (503) staff       (20)      133 2020-02-05 11:15:55.000000 wsgi_intercept-1.9.2/setup.cfg
--rw-r--r--   0 cdent      (503) staff       (20)     1433 2020-02-05 11:13:22.000000 wsgi_intercept-1.9.2/setup.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2020-02-05 11:15:55.000000 wsgi_intercept-1.9.2/wsgi_intercept/
--rw-r--r--   0 cdent      (503) staff       (20)    22301 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     1692 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/_urllib3.py
--rw-r--r--   0 cdent      (503) staff       (20)     1234 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/http_client_intercept.py
--rw-r--r--   0 cdent      (503) staff       (20)     1962 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/httplib2_intercept.py
--rw-r--r--   0 cdent      (503) staff       (20)     3771 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/interceptor.py
--rw-r--r--   0 cdent      (503) staff       (20)      588 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/requests_intercept.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2020-02-05 11:15:55.000000 wsgi_intercept-1.9.2/wsgi_intercept/tests/
--rw-r--r--   0 cdent      (503) staff       (20)      230 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/tests/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     2224 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/tests/install.py
--rw-r--r--   0 cdent      (503) staff       (20)     2812 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/tests/test_http_client.py
--rw-r--r--   0 cdent      (503) staff       (20)     2809 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/tests/test_httplib2.py
--rw-r--r--   0 cdent      (503) staff       (20)     9817 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/tests/test_interceptor.py
--rw-r--r--   0 cdent      (503) staff       (20)      926 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/tests/test_module_interceptor.py
--rw-r--r--   0 cdent      (503) staff       (20)     3869 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/tests/test_requests.py
--rw-r--r--   0 cdent      (503) staff       (20)     2655 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/tests/test_response_headers.py
--rw-r--r--   0 cdent      (503) staff       (20)     2783 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/tests/test_urllib.py
--rw-r--r--   0 cdent      (503) staff       (20)     3668 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/tests/test_urllib3.py
--rw-r--r--   0 cdent      (503) staff       (20)     4834 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/tests/test_wsgi_compliance.py
--rw-r--r--   0 cdent      (503) staff       (20)     1145 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/tests/wsgi_app.py
--rw-r--r--   0 cdent      (503) staff       (20)      521 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/urllib3_intercept.py
--rw-r--r--   0 cdent      (503) staff       (20)     1309 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.2/wsgi_intercept/urllib_intercept.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2020-02-05 11:15:55.000000 wsgi_intercept-1.9.2/wsgi_intercept.egg-info/
--rw-r--r--   0 cdent      (503) staff       (20)     7275 2020-02-05 11:15:55.000000 wsgi_intercept-1.9.2/wsgi_intercept.egg-info/PKG-INFO
--rw-r--r--   0 cdent      (503) staff       (20)     1200 2020-02-05 11:15:55.000000 wsgi_intercept-1.9.2/wsgi_intercept.egg-info/SOURCES.txt
--rw-r--r--   0 cdent      (503) staff       (20)        1 2020-02-05 11:15:55.000000 wsgi_intercept-1.9.2/wsgi_intercept.egg-info/dependency_links.txt
--rw-r--r--   0 cdent      (503) staff       (20)       83 2020-02-05 11:15:55.000000 wsgi_intercept-1.9.2/wsgi_intercept.egg-info/requires.txt
--rw-r--r--   0 cdent      (503) staff       (20)       15 2020-02-05 11:15:55.000000 wsgi_intercept-1.9.2/wsgi_intercept.egg-info/top_level.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-01-13 14:38:37.431850 wsgi_intercept-1.9.3/
+-rw-r--r--   0 cdent      (503) staff       (20)     1094 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/LICENSE
+-rw-r--r--   0 cdent      (503) staff       (20)       50 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/MANIFEST.in
+-rw-r--r--   0 cdent      (503) staff       (20)     1010 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/Makefile
+-rw-r--r--   0 cdent      (503) staff       (20)     6174 2022-01-13 14:38:37.432129 wsgi_intercept-1.9.3/PKG-INFO
+-rw-r--r--   0 cdent      (503) staff       (20)     5138 2022-01-13 14:38:34.000000 wsgi_intercept-1.9.3/README
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-01-13 14:38:37.404283 wsgi_intercept-1.9.3/docs/
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/docs/.gitignore
+-rw-r--r--   0 cdent      (503) staff       (20)     6794 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/docs/Makefile
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-01-13 14:38:37.404618 wsgi_intercept-1.9.3/docs/_static/
+-rw-r--r--   0 cdent      (503) staff       (20)        0 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/docs/_static/.gitignore
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-01-13 14:38:37.404923 wsgi_intercept-1.9.3/docs/_templates/
+-rw-r--r--   0 cdent      (503) staff       (20)        0 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/docs/_templates/.gitignore
+-rw-r--r--   0 cdent      (503) staff       (20)    10608 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/docs/conf.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1239 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/docs/http_client.rst
+-rw-r--r--   0 cdent      (503) staff       (20)      920 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/docs/httplib2.rst
+-rw-r--r--   0 cdent      (503) staff       (20)      352 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/docs/index.rst
+-rw-r--r--   0 cdent      (503) staff       (20)      586 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/docs/interceptor.rst
+-rw-r--r--   0 cdent      (503) staff       (20)      639 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/docs/requests.rst
+-rw-r--r--   0 cdent      (503) staff       (20)      780 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/docs/urllib.rst
+-rw-r--r--   0 cdent      (503) staff       (20)      671 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/docs/urllib3.rst
+-rw-r--r--   0 cdent      (503) staff       (20)      133 2022-01-13 14:38:37.433057 wsgi_intercept-1.9.3/setup.cfg
+-rw-r--r--   0 cdent      (503) staff       (20)     1433 2022-01-13 14:34:50.000000 wsgi_intercept-1.9.3/setup.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-01-13 14:38:37.407834 wsgi_intercept-1.9.3/wsgi_intercept/
+-rw-r--r--   0 cdent      (503) staff       (20)    22301 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1788 2022-01-13 14:31:38.000000 wsgi_intercept-1.9.3/wsgi_intercept/_urllib3.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1234 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/http_client_intercept.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1962 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/httplib2_intercept.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3771 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/interceptor.py
+-rw-r--r--   0 cdent      (503) staff       (20)      588 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/requests_intercept.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-01-13 14:38:37.431426 wsgi_intercept-1.9.3/wsgi_intercept/tests/
+-rw-r--r--   0 cdent      (503) staff       (20)      230 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/tests/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2224 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/tests/install.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2812 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/tests/test_http_client.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2809 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/tests/test_httplib2.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9817 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/tests/test_interceptor.py
+-rw-r--r--   0 cdent      (503) staff       (20)      926 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/tests/test_module_interceptor.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3869 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/tests/test_requests.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2655 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/tests/test_response_headers.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2783 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/tests/test_urllib.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3668 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/tests/test_urllib3.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4834 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/tests/test_wsgi_compliance.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1145 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/tests/wsgi_app.py
+-rw-r--r--   0 cdent      (503) staff       (20)      521 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/urllib3_intercept.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1309 2020-02-05 11:08:46.000000 wsgi_intercept-1.9.3/wsgi_intercept/urllib_intercept.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-01-13 14:38:37.409638 wsgi_intercept-1.9.3/wsgi_intercept.egg-info/
+-rw-r--r--   0 cdent      (503) staff       (20)     6174 2022-01-13 14:38:37.000000 wsgi_intercept-1.9.3/wsgi_intercept.egg-info/PKG-INFO
+-rw-r--r--   0 cdent      (503) staff       (20)     1200 2022-01-13 14:38:37.000000 wsgi_intercept-1.9.3/wsgi_intercept.egg-info/SOURCES.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        1 2022-01-13 14:38:37.000000 wsgi_intercept-1.9.3/wsgi_intercept.egg-info/dependency_links.txt
+-rw-r--r--   0 cdent      (503) staff       (20)       83 2022-01-13 14:38:37.000000 wsgi_intercept-1.9.3/wsgi_intercept.egg-info/requires.txt
+-rw-r--r--   0 cdent      (503) staff       (20)       15 2022-01-13 14:38:37.000000 wsgi_intercept-1.9.3/wsgi_intercept.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wsgi_intercept-1.9.2/LICENSE` & `wsgi_intercept-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/Makefile` & `wsgi_intercept-1.9.3/Makefile`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/PKG-INFO` & `wsgi_intercept-1.9.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,155 +1,15 @@
 Metadata-Version: 2.1
 Name: wsgi_intercept
-Version: 1.9.2
+Version: 1.9.3
 Summary: wsgi_intercept installs a WSGI application in place of a real URI for testing.
 Home-page: http://pypi.python.org/pypi/wsgi_intercept
 Author: Titus Brown, Kumar McMillan, Chris Dent, Sasha Hart
 Author-email: cdent@peermore.com
 License: MIT License
-Description: Installs a WSGI application in place of a real host for testing.
-        
-        Introduction
-        ============
-        
-        Testing a WSGI application sometimes involves starting a server at a
-        local host and port, then pointing your test code to that address.
-        Instead, this library lets you intercept calls to any specific host/port
-        combination and redirect them into a `WSGI application`_ importable by
-        your test program. Thus, you can avoid spawning multiple processes or
-        threads to test your Web app.
-        
-        Supported Libaries
-        ==================
-        
-        ``wsgi_intercept`` works with a variety of HTTP clients in Python 2.7,
-        3.5 and beyond, and in pypy.
-        
-        * urllib2
-        * urllib.request
-        * httplib
-        * http.client
-        * httplib2
-        * requests
-        * urllib3
-        
-        How Does It Work?
-        =================
-        
-        ``wsgi_intercept`` works by replacing ``httplib.HTTPConnection`` with a
-        subclass, ``wsgi_intercept.WSGI_HTTPConnection``. This class then
-        redirects specific server/port combinations into a WSGI application by
-        emulating a socket. If no intercept is registered for the host and port
-        requested, those requests are passed on to the standard handler.
-        
-        The easiest way to use an intercept is to import an appropriate subclass
-        of ``~wsgi_intercept.interceptor.Interceptor`` and use that as a
-        context manager over web requests that use the library associated with
-        the subclass. For example::
-        
-            import httplib2
-            from wsgi_intercept.interceptor import Httplib2Interceptor
-            from mywsgiapp import app
-        
-            def load_app():
-                return app
-        
-            http = httplib2.Http()
-            with Httplib2Interceptor(load_app, host='example.com', port=80) as url:
-                response, content = http.request('%s%s' % (url, '/path'))
-                assert response.status == 200
-        
-        The interceptor class may aslo be used directly to install intercepts.
-        See the module documentation for more information.
-        
-        Older versions required that the functions ``add_wsgi_intercept(host,
-        port, app_create_fn, script_name='')`` and ``remove_wsgi_intercept(host,port)``
-        be used to specify which URLs should be redirected into what applications.
-        These methods are still available, but the ``Interceptor`` classes are likely
-        easier to use for most use cases.
-        
-        .. note:: ``app_create_fn`` is a *function object* returning a WSGI
-                  application; ``script_name`` becomes ``SCRIPT_NAME`` in the WSGI
-                  app's environment, if set.
-        
-        .. note:: If ``http_proxy`` or ``https_proxy`` is set in the environment
-                  this can cause difficulties with some of the intercepted libraries.
-                  If requests or urllib is being used, these will raise an exception
-                  if one of those variables is set.
-        
-        .. note:: If ``wsgi_intercept.STRICT_RESPONSE_HEADERS`` is set to ``True``
-                  then response headers sent by an application will be checked to
-                  make sure they are of the type ``str`` native to the version of
-                  Python, as required by pep 3333. The default is ``False`` (to
-                  preserve backwards compatibility)
-        
-        
-        Install
-        =======
-        
-        ::
-        
-            pip install -U wsgi_intercept
-        
-        Packages Intercepted
-        ====================
-        
-        Unfortunately each of the HTTP client libraries use their own specific
-        mechanism for making HTTP call-outs, so individual implementations are
-        needed. At this time there are implementations for ``httplib2``,
-        ``urllib3`` and ``requests`` in both Python 2 and 3, ``urllib2`` and
-        ``httplib`` in Python 2 and ``urllib.request`` and ``http.client``
-        in Python 3.
-        
-        If you are using Python 2 and need support for a different HTTP
-        client, require a version of ``wsgi_intercept<0.6``. Earlier versions
-        include support for ``webtest``, ``webunit`` and ``zope.testbrowser``.
-        
-        The best way to figure out how to use interception is to inspect
-        `the tests`_. More comprehensive documentation available upon
-        request.
-        
-        .. _the tests: https://github.com/cdent/wsgi-intercept/tree/master/test
-        
-        
-        History
-        =======
-        
-        Pursuant to Ian Bicking's `"best Web testing framework"`_ post, Titus
-        Brown put together an `in-process HTTP-to-WSGI interception mechanism`_
-        for his own Web testing system, twill. Because the mechanism is pretty
-        generic -- it works at the httplib level -- Titus decided to try adding
-        it into all of the *other* Python Web testing frameworks.
-        
-        The Python 2 version of wsgi-intercept was the result. Kumar McMillan
-        later took over maintenance.
-        
-        The current version is tested with Python 2.7, 3.5-3.8, and pypy and pypy3.
-        It was assembled by `Chris Dent`_. Testing and documentation improvements
-        from `Sasha Hart`_.
-        
-        .. _"best Web testing framework":
-             http://blog.ianbicking.org/best-of-the-web-app-test-frameworks.html
-        .. _in-process HTTP-to-WSGI interception mechanism:
-             http://www.advogato.org/person/titus/diary.html?start=119
-        .. _WSGI application: http://www.python.org/peps/pep-3333.html
-        .. _Chris Dent: https://github.com/cdent
-        .. _Sasha Hart: https://github.com/sashahart
-        
-        Project Home
-        ============
-        
-        This project lives on `GitHub`_. Please submit all bugs, patches,
-        failing tests, et cetera using the Issue Tracker.
-        
-        Additional documentation is available on `Read The Docs`_.
-        
-        .. _GitHub: http://github.com/cdent/wsgi-intercept
-        .. _Read The Docs: http://wsgi-intercept.readthedocs.org/en/latest/
-        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -158,7 +18,150 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: testing
 Provides-Extra: docs
+License-File: LICENSE
+
+Installs a WSGI application in place of a real host for testing.
+
+Introduction
+============
+
+Testing a WSGI application sometimes involves starting a server at a
+local host and port, then pointing your test code to that address.
+Instead, this library lets you intercept calls to any specific host/port
+combination and redirect them into a `WSGI application`_ importable by
+your test program. Thus, you can avoid spawning multiple processes or
+threads to test your Web app.
+
+Supported Libaries
+==================
+
+``wsgi_intercept`` works with a variety of HTTP clients in Python 2.7,
+3.5 and beyond, and in pypy.
+
+* urllib2
+* urllib.request
+* httplib
+* http.client
+* httplib2
+* requests
+* urllib3
+
+How Does It Work?
+=================
+
+``wsgi_intercept`` works by replacing ``httplib.HTTPConnection`` with a
+subclass, ``wsgi_intercept.WSGI_HTTPConnection``. This class then
+redirects specific server/port combinations into a WSGI application by
+emulating a socket. If no intercept is registered for the host and port
+requested, those requests are passed on to the standard handler.
+
+The easiest way to use an intercept is to import an appropriate subclass
+of ``~wsgi_intercept.interceptor.Interceptor`` and use that as a
+context manager over web requests that use the library associated with
+the subclass. For example::
+
+    import httplib2
+    from wsgi_intercept.interceptor import Httplib2Interceptor
+    from mywsgiapp import app
+
+    def load_app():
+        return app
+
+    http = httplib2.Http()
+    with Httplib2Interceptor(load_app, host='example.com', port=80) as url:
+        response, content = http.request('%s%s' % (url, '/path'))
+        assert response.status == 200
+
+The interceptor class may aslo be used directly to install intercepts.
+See the module documentation for more information.
+
+Older versions required that the functions ``add_wsgi_intercept(host,
+port, app_create_fn, script_name='')`` and ``remove_wsgi_intercept(host,port)``
+be used to specify which URLs should be redirected into what applications.
+These methods are still available, but the ``Interceptor`` classes are likely
+easier to use for most use cases.
+
+.. note:: ``app_create_fn`` is a *function object* returning a WSGI
+          application; ``script_name`` becomes ``SCRIPT_NAME`` in the WSGI
+          app's environment, if set.
+
+.. note:: If ``http_proxy`` or ``https_proxy`` is set in the environment
+          this can cause difficulties with some of the intercepted libraries.
+          If requests or urllib is being used, these will raise an exception
+          if one of those variables is set.
+
+.. note:: If ``wsgi_intercept.STRICT_RESPONSE_HEADERS`` is set to ``True``
+          then response headers sent by an application will be checked to
+          make sure they are of the type ``str`` native to the version of
+          Python, as required by pep 3333. The default is ``False`` (to
+          preserve backwards compatibility)
+
+
+Install
+=======
+
+::
+
+    pip install -U wsgi_intercept
+
+Packages Intercepted
+====================
+
+Unfortunately each of the HTTP client libraries use their own specific
+mechanism for making HTTP call-outs, so individual implementations are
+needed. At this time there are implementations for ``httplib2``,
+``urllib3`` and ``requests`` in both Python 2 and 3, ``urllib2`` and
+``httplib`` in Python 2 and ``urllib.request`` and ``http.client``
+in Python 3.
+
+If you are using Python 2 and need support for a different HTTP
+client, require a version of ``wsgi_intercept<0.6``. Earlier versions
+include support for ``webtest``, ``webunit`` and ``zope.testbrowser``.
+
+The best way to figure out how to use interception is to inspect
+`the tests`_. More comprehensive documentation available upon
+request.
+
+.. _the tests: https://github.com/cdent/wsgi-intercept/tree/master/test
+
+
+History
+=======
+
+Pursuant to Ian Bicking's `"best Web testing framework"`_ post, Titus
+Brown put together an `in-process HTTP-to-WSGI interception mechanism`_
+for his own Web testing system, twill. Because the mechanism is pretty
+generic -- it works at the httplib level -- Titus decided to try adding
+it into all of the *other* Python Web testing frameworks.
+
+The Python 2 version of wsgi-intercept was the result. Kumar McMillan
+later took over maintenance.
+
+The current version is tested with Python 2.7, 3.5-3.8, and pypy and pypy3.
+It was assembled by `Chris Dent`_. Testing and documentation improvements
+from `Sasha Hart`_.
+
+.. _"best Web testing framework":
+     http://blog.ianbicking.org/best-of-the-web-app-test-frameworks.html
+.. _in-process HTTP-to-WSGI interception mechanism:
+     http://www.advogato.org/person/titus/diary.html?start=119
+.. _WSGI application: http://www.python.org/peps/pep-3333.html
+.. _Chris Dent: https://github.com/cdent
+.. _Sasha Hart: https://github.com/sashahart
+
+Project Home
+============
+
+This project lives on `GitHub`_. Please submit all bugs, patches,
+failing tests, et cetera using the Issue Tracker.
+
+Additional documentation is available on `Read The Docs`_.
+
+.. _GitHub: http://github.com/cdent/wsgi-intercept
+.. _Read The Docs: http://wsgi-intercept.readthedocs.org/en/latest/
+
+
```

### Comparing `wsgi_intercept-1.9.2/README` & `wsgi_intercept-1.9.3/README`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/docs/Makefile` & `wsgi_intercept-1.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/docs/conf.py` & `wsgi_intercept-1.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/docs/http_client.rst` & `wsgi_intercept-1.9.3/docs/http_client.rst`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/docs/httplib2.rst` & `wsgi_intercept-1.9.3/docs/httplib2.rst`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/docs/interceptor.rst` & `wsgi_intercept-1.9.3/docs/interceptor.rst`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/docs/requests.rst` & `wsgi_intercept-1.9.3/docs/requests.rst`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/docs/urllib.rst` & `wsgi_intercept-1.9.3/docs/urllib.rst`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/docs/urllib3.rst` & `wsgi_intercept-1.9.3/docs/urllib3.rst`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/setup.py` & `wsgi_intercept-1.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from setuptools import setup, find_packages
 
-VERSION = '1.9.2'
+VERSION = '1.9.3'
 
 CLASSIFIERS = """
 Environment :: Web Environment
 Intended Audience :: Developers
 License :: OSI Approved :: MIT License
 Operating System :: OS Independent
 Programming Language :: Python :: 2
```

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/__init__.py` & `wsgi_intercept-1.9.3/wsgi_intercept/__init__.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/_urllib3.py` & `wsgi_intercept-1.9.3/wsgi_intercept/_urllib3.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,27 @@
                           HTTPConnection, HTTPSConnection):
 
     class HTTP_WSGIInterceptor(WSGI_HTTPConnection, HTTPConnection):
         def __init__(self, *args, **kwargs):
             if 'strict' in kwargs and sys.version_info > (3, 0):
                 kwargs.pop('strict')
             kwargs.pop('socket_options', None)
+            kwargs.pop('server_hostname', None)
             WSGI_HTTPConnection.__init__(self, *args, **kwargs)
             HTTPConnection.__init__(self, *args, **kwargs)
 
     class HTTPS_WSGIInterceptor(WSGI_HTTPSConnection, HTTPSConnection):
         is_verified = True
 
         def __init__(self, *args, **kwargs):
             if 'strict' in kwargs and sys.version_info > (3, 0):
                 kwargs.pop('strict')
             kwargs.pop('socket_options', None)
             kwargs.pop('key_password', None)
+            kwargs.pop('server_hostname', None)
             WSGI_HTTPSConnection.__init__(self, *args, **kwargs)
             HTTPSConnection.__init__(self, *args, **kwargs)
 
     def install():
         if 'http_proxy' in os.environ or 'https_proxy' in os.environ:
             raise RuntimeError(
                 'http_proxy or https_proxy set in environment, please unset')
```

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/http_client_intercept.py` & `wsgi_intercept-1.9.3/wsgi_intercept/http_client_intercept.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/httplib2_intercept.py` & `wsgi_intercept-1.9.3/wsgi_intercept/httplib2_intercept.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/interceptor.py` & `wsgi_intercept-1.9.3/wsgi_intercept/interceptor.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/requests_intercept.py` & `wsgi_intercept-1.9.3/wsgi_intercept/requests_intercept.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/tests/install.py` & `wsgi_intercept-1.9.3/wsgi_intercept/tests/install.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/tests/test_http_client.py` & `wsgi_intercept-1.9.3/wsgi_intercept/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/tests/test_httplib2.py` & `wsgi_intercept-1.9.3/wsgi_intercept/tests/test_httplib2.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/tests/test_interceptor.py` & `wsgi_intercept-1.9.3/wsgi_intercept/tests/test_interceptor.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/tests/test_module_interceptor.py` & `wsgi_intercept-1.9.3/wsgi_intercept/tests/test_module_interceptor.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/tests/test_requests.py` & `wsgi_intercept-1.9.3/wsgi_intercept/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/tests/test_response_headers.py` & `wsgi_intercept-1.9.3/wsgi_intercept/tests/test_response_headers.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/tests/test_urllib.py` & `wsgi_intercept-1.9.3/wsgi_intercept/tests/test_urllib.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/tests/test_urllib3.py` & `wsgi_intercept-1.9.3/wsgi_intercept/tests/test_urllib3.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/tests/test_wsgi_compliance.py` & `wsgi_intercept-1.9.3/wsgi_intercept/tests/test_wsgi_compliance.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/tests/wsgi_app.py` & `wsgi_intercept-1.9.3/wsgi_intercept/tests/wsgi_app.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/urllib3_intercept.py` & `wsgi_intercept-1.9.3/wsgi_intercept/urllib3_intercept.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept/urllib_intercept.py` & `wsgi_intercept-1.9.3/wsgi_intercept/urllib_intercept.py`

 * *Files identical despite different names*

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept.egg-info/PKG-INFO` & `wsgi_intercept-1.9.3/wsgi_intercept.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,155 +1,15 @@
 Metadata-Version: 2.1
 Name: wsgi-intercept
-Version: 1.9.2
+Version: 1.9.3
 Summary: wsgi_intercept installs a WSGI application in place of a real URI for testing.
 Home-page: http://pypi.python.org/pypi/wsgi_intercept
 Author: Titus Brown, Kumar McMillan, Chris Dent, Sasha Hart
 Author-email: cdent@peermore.com
 License: MIT License
-Description: Installs a WSGI application in place of a real host for testing.
-        
-        Introduction
-        ============
-        
-        Testing a WSGI application sometimes involves starting a server at a
-        local host and port, then pointing your test code to that address.
-        Instead, this library lets you intercept calls to any specific host/port
-        combination and redirect them into a `WSGI application`_ importable by
-        your test program. Thus, you can avoid spawning multiple processes or
-        threads to test your Web app.
-        
-        Supported Libaries
-        ==================
-        
-        ``wsgi_intercept`` works with a variety of HTTP clients in Python 2.7,
-        3.5 and beyond, and in pypy.
-        
-        * urllib2
-        * urllib.request
-        * httplib
-        * http.client
-        * httplib2
-        * requests
-        * urllib3
-        
-        How Does It Work?
-        =================
-        
-        ``wsgi_intercept`` works by replacing ``httplib.HTTPConnection`` with a
-        subclass, ``wsgi_intercept.WSGI_HTTPConnection``. This class then
-        redirects specific server/port combinations into a WSGI application by
-        emulating a socket. If no intercept is registered for the host and port
-        requested, those requests are passed on to the standard handler.
-        
-        The easiest way to use an intercept is to import an appropriate subclass
-        of ``~wsgi_intercept.interceptor.Interceptor`` and use that as a
-        context manager over web requests that use the library associated with
-        the subclass. For example::
-        
-            import httplib2
-            from wsgi_intercept.interceptor import Httplib2Interceptor
-            from mywsgiapp import app
-        
-            def load_app():
-                return app
-        
-            http = httplib2.Http()
-            with Httplib2Interceptor(load_app, host='example.com', port=80) as url:
-                response, content = http.request('%s%s' % (url, '/path'))
-                assert response.status == 200
-        
-        The interceptor class may aslo be used directly to install intercepts.
-        See the module documentation for more information.
-        
-        Older versions required that the functions ``add_wsgi_intercept(host,
-        port, app_create_fn, script_name='')`` and ``remove_wsgi_intercept(host,port)``
-        be used to specify which URLs should be redirected into what applications.
-        These methods are still available, but the ``Interceptor`` classes are likely
-        easier to use for most use cases.
-        
-        .. note:: ``app_create_fn`` is a *function object* returning a WSGI
-                  application; ``script_name`` becomes ``SCRIPT_NAME`` in the WSGI
-                  app's environment, if set.
-        
-        .. note:: If ``http_proxy`` or ``https_proxy`` is set in the environment
-                  this can cause difficulties with some of the intercepted libraries.
-                  If requests or urllib is being used, these will raise an exception
-                  if one of those variables is set.
-        
-        .. note:: If ``wsgi_intercept.STRICT_RESPONSE_HEADERS`` is set to ``True``
-                  then response headers sent by an application will be checked to
-                  make sure they are of the type ``str`` native to the version of
-                  Python, as required by pep 3333. The default is ``False`` (to
-                  preserve backwards compatibility)
-        
-        
-        Install
-        =======
-        
-        ::
-        
-            pip install -U wsgi_intercept
-        
-        Packages Intercepted
-        ====================
-        
-        Unfortunately each of the HTTP client libraries use their own specific
-        mechanism for making HTTP call-outs, so individual implementations are
-        needed. At this time there are implementations for ``httplib2``,
-        ``urllib3`` and ``requests`` in both Python 2 and 3, ``urllib2`` and
-        ``httplib`` in Python 2 and ``urllib.request`` and ``http.client``
-        in Python 3.
-        
-        If you are using Python 2 and need support for a different HTTP
-        client, require a version of ``wsgi_intercept<0.6``. Earlier versions
-        include support for ``webtest``, ``webunit`` and ``zope.testbrowser``.
-        
-        The best way to figure out how to use interception is to inspect
-        `the tests`_. More comprehensive documentation available upon
-        request.
-        
-        .. _the tests: https://github.com/cdent/wsgi-intercept/tree/master/test
-        
-        
-        History
-        =======
-        
-        Pursuant to Ian Bicking's `"best Web testing framework"`_ post, Titus
-        Brown put together an `in-process HTTP-to-WSGI interception mechanism`_
-        for his own Web testing system, twill. Because the mechanism is pretty
-        generic -- it works at the httplib level -- Titus decided to try adding
-        it into all of the *other* Python Web testing frameworks.
-        
-        The Python 2 version of wsgi-intercept was the result. Kumar McMillan
-        later took over maintenance.
-        
-        The current version is tested with Python 2.7, 3.5-3.8, and pypy and pypy3.
-        It was assembled by `Chris Dent`_. Testing and documentation improvements
-        from `Sasha Hart`_.
-        
-        .. _"best Web testing framework":
-             http://blog.ianbicking.org/best-of-the-web-app-test-frameworks.html
-        .. _in-process HTTP-to-WSGI interception mechanism:
-             http://www.advogato.org/person/titus/diary.html?start=119
-        .. _WSGI application: http://www.python.org/peps/pep-3333.html
-        .. _Chris Dent: https://github.com/cdent
-        .. _Sasha Hart: https://github.com/sashahart
-        
-        Project Home
-        ============
-        
-        This project lives on `GitHub`_. Please submit all bugs, patches,
-        failing tests, et cetera using the Issue Tracker.
-        
-        Additional documentation is available on `Read The Docs`_.
-        
-        .. _GitHub: http://github.com/cdent/wsgi-intercept
-        .. _Read The Docs: http://wsgi-intercept.readthedocs.org/en/latest/
-        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -158,7 +18,150 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: testing
 Provides-Extra: docs
+License-File: LICENSE
+
+Installs a WSGI application in place of a real host for testing.
+
+Introduction
+============
+
+Testing a WSGI application sometimes involves starting a server at a
+local host and port, then pointing your test code to that address.
+Instead, this library lets you intercept calls to any specific host/port
+combination and redirect them into a `WSGI application`_ importable by
+your test program. Thus, you can avoid spawning multiple processes or
+threads to test your Web app.
+
+Supported Libaries
+==================
+
+``wsgi_intercept`` works with a variety of HTTP clients in Python 2.7,
+3.5 and beyond, and in pypy.
+
+* urllib2
+* urllib.request
+* httplib
+* http.client
+* httplib2
+* requests
+* urllib3
+
+How Does It Work?
+=================
+
+``wsgi_intercept`` works by replacing ``httplib.HTTPConnection`` with a
+subclass, ``wsgi_intercept.WSGI_HTTPConnection``. This class then
+redirects specific server/port combinations into a WSGI application by
+emulating a socket. If no intercept is registered for the host and port
+requested, those requests are passed on to the standard handler.
+
+The easiest way to use an intercept is to import an appropriate subclass
+of ``~wsgi_intercept.interceptor.Interceptor`` and use that as a
+context manager over web requests that use the library associated with
+the subclass. For example::
+
+    import httplib2
+    from wsgi_intercept.interceptor import Httplib2Interceptor
+    from mywsgiapp import app
+
+    def load_app():
+        return app
+
+    http = httplib2.Http()
+    with Httplib2Interceptor(load_app, host='example.com', port=80) as url:
+        response, content = http.request('%s%s' % (url, '/path'))
+        assert response.status == 200
+
+The interceptor class may aslo be used directly to install intercepts.
+See the module documentation for more information.
+
+Older versions required that the functions ``add_wsgi_intercept(host,
+port, app_create_fn, script_name='')`` and ``remove_wsgi_intercept(host,port)``
+be used to specify which URLs should be redirected into what applications.
+These methods are still available, but the ``Interceptor`` classes are likely
+easier to use for most use cases.
+
+.. note:: ``app_create_fn`` is a *function object* returning a WSGI
+          application; ``script_name`` becomes ``SCRIPT_NAME`` in the WSGI
+          app's environment, if set.
+
+.. note:: If ``http_proxy`` or ``https_proxy`` is set in the environment
+          this can cause difficulties with some of the intercepted libraries.
+          If requests or urllib is being used, these will raise an exception
+          if one of those variables is set.
+
+.. note:: If ``wsgi_intercept.STRICT_RESPONSE_HEADERS`` is set to ``True``
+          then response headers sent by an application will be checked to
+          make sure they are of the type ``str`` native to the version of
+          Python, as required by pep 3333. The default is ``False`` (to
+          preserve backwards compatibility)
+
+
+Install
+=======
+
+::
+
+    pip install -U wsgi_intercept
+
+Packages Intercepted
+====================
+
+Unfortunately each of the HTTP client libraries use their own specific
+mechanism for making HTTP call-outs, so individual implementations are
+needed. At this time there are implementations for ``httplib2``,
+``urllib3`` and ``requests`` in both Python 2 and 3, ``urllib2`` and
+``httplib`` in Python 2 and ``urllib.request`` and ``http.client``
+in Python 3.
+
+If you are using Python 2 and need support for a different HTTP
+client, require a version of ``wsgi_intercept<0.6``. Earlier versions
+include support for ``webtest``, ``webunit`` and ``zope.testbrowser``.
+
+The best way to figure out how to use interception is to inspect
+`the tests`_. More comprehensive documentation available upon
+request.
+
+.. _the tests: https://github.com/cdent/wsgi-intercept/tree/master/test
+
+
+History
+=======
+
+Pursuant to Ian Bicking's `"best Web testing framework"`_ post, Titus
+Brown put together an `in-process HTTP-to-WSGI interception mechanism`_
+for his own Web testing system, twill. Because the mechanism is pretty
+generic -- it works at the httplib level -- Titus decided to try adding
+it into all of the *other* Python Web testing frameworks.
+
+The Python 2 version of wsgi-intercept was the result. Kumar McMillan
+later took over maintenance.
+
+The current version is tested with Python 2.7, 3.5-3.8, and pypy and pypy3.
+It was assembled by `Chris Dent`_. Testing and documentation improvements
+from `Sasha Hart`_.
+
+.. _"best Web testing framework":
+     http://blog.ianbicking.org/best-of-the-web-app-test-frameworks.html
+.. _in-process HTTP-to-WSGI interception mechanism:
+     http://www.advogato.org/person/titus/diary.html?start=119
+.. _WSGI application: http://www.python.org/peps/pep-3333.html
+.. _Chris Dent: https://github.com/cdent
+.. _Sasha Hart: https://github.com/sashahart
+
+Project Home
+============
+
+This project lives on `GitHub`_. Please submit all bugs, patches,
+failing tests, et cetera using the Issue Tracker.
+
+Additional documentation is available on `Read The Docs`_.
+
+.. _GitHub: http://github.com/cdent/wsgi-intercept
+.. _Read The Docs: http://wsgi-intercept.readthedocs.org/en/latest/
+
+
```

### Comparing `wsgi_intercept-1.9.2/wsgi_intercept.egg-info/SOURCES.txt` & `wsgi_intercept-1.9.3/wsgi_intercept.egg-info/SOURCES.txt`

 * *Files identical despite different names*

