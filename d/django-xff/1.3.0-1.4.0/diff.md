# Comparing `tmp/django-xff-1.3.0.tar.gz` & `tmp/django-xff-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-xff-1.3.0.tar", last modified: Wed Jan  9 10:14:27 2019, max compression
+gzip compressed data, was "django-xff-1.4.0.tar", last modified: Mon Jun 26 17:29:05 2023, max compression
```

## Comparing `django-xff-1.3.0.tar` & `django-xff-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 ferrix     (501) staff       (20)        0 2019-01-09 10:14:27.000000 django-xff-1.3.0/
--rw-r--r--   0 ferrix     (501) staff       (20)     8443 2019-01-09 10:14:27.000000 django-xff-1.3.0/PKG-INFO
-drwxr-xr-x   0 ferrix     (501) staff       (20)        0 2019-01-09 10:14:27.000000 django-xff-1.3.0/xff/
--rw-r--r--   0 ferrix     (501) staff       (20)      471 2019-01-09 10:14:27.000000 django-xff-1.3.0/xff/_version.py
--rw-r--r--   0 ferrix     (501) staff       (20)        0 2015-11-17 10:47:09.000000 django-xff-1.3.0/xff/__init__.py
--rw-r--r--   0 ferrix     (501) staff       (20)     4869 2019-01-09 10:11:40.000000 django-xff-1.3.0/xff/middleware.py
--rw-r--r--   0 ferrix     (501) staff       (20)     1078 2015-11-16 07:01:45.000000 django-xff-1.3.0/LICENSE
-drwxr-xr-x   0 ferrix     (501) staff       (20)        0 2019-01-09 10:14:27.000000 django-xff-1.3.0/django_xff.egg-info/
--rw-r--r--   0 ferrix     (501) staff       (20)     8443 2019-01-09 10:14:27.000000 django-xff-1.3.0/django_xff.egg-info/PKG-INFO
--rw-r--r--   0 ferrix     (501) staff       (20)      311 2019-01-09 10:14:27.000000 django-xff-1.3.0/django_xff.egg-info/SOURCES.txt
--rw-r--r--   0 ferrix     (501) staff       (20)       46 2015-11-16 07:05:24.000000 django-xff-1.3.0/django_xff.egg-info/pbr.json
--rw-r--r--   0 ferrix     (501) staff       (20)       14 2019-01-09 10:14:27.000000 django-xff-1.3.0/django_xff.egg-info/requires.txt
--rw-r--r--   0 ferrix     (501) staff       (20)        4 2019-01-09 10:14:27.000000 django-xff-1.3.0/django_xff.egg-info/top_level.txt
--rw-r--r--   0 ferrix     (501) staff       (20)        1 2019-01-09 10:14:27.000000 django-xff-1.3.0/django_xff.egg-info/dependency_links.txt
--rw-r--r--   0 ferrix     (501) staff       (20)       81 2015-11-16 06:59:43.000000 django-xff-1.3.0/MANIFEST.in
--rwxr-xr-x   0 ferrix     (501) staff       (20)     1348 2019-01-09 07:40:56.000000 django-xff-1.3.0/setup.py
--rw-r--r--   0 ferrix     (501) staff       (20)      324 2019-01-09 10:14:27.000000 django-xff-1.3.0/setup.cfg
--rw-r--r--   0 ferrix     (501) staff       (20)    62474 2015-11-16 06:56:35.000000 django-xff-1.3.0/versioneer.py
--rw-r--r--   0 ferrix     (501) staff       (20)     6215 2015-11-18 04:56:28.000000 django-xff-1.3.0/README.rst
+drwxr-xr-x   0 ferrix     (501) staff       (20)        0 2023-06-26 17:29:05.028323 django-xff-1.4.0/
+-rw-r--r--   0 ferrix     (501) staff       (20)     1078 2023-06-26 17:14:16.000000 django-xff-1.4.0/LICENSE
+-rw-r--r--   0 ferrix     (501) staff       (20)       81 2023-06-26 17:14:16.000000 django-xff-1.4.0/MANIFEST.in
+-rw-r--r--   0 ferrix     (501) staff       (20)     7194 2023-06-26 17:29:05.028497 django-xff-1.4.0/PKG-INFO
+-rw-r--r--   0 ferrix     (501) staff       (20)     6559 2023-06-26 17:14:16.000000 django-xff-1.4.0/README.rst
+drwxr-xr-x   0 ferrix     (501) staff       (20)        0 2023-06-26 17:29:05.026489 django-xff-1.4.0/django_xff.egg-info/
+-rw-r--r--   0 ferrix     (501) staff       (20)     7194 2023-06-26 17:29:04.000000 django-xff-1.4.0/django_xff.egg-info/PKG-INFO
+-rw-r--r--   0 ferrix     (501) staff       (20)      307 2023-06-26 17:29:04.000000 django-xff-1.4.0/django_xff.egg-info/SOURCES.txt
+-rw-r--r--   0 ferrix     (501) staff       (20)        1 2023-06-26 17:29:04.000000 django-xff-1.4.0/django_xff.egg-info/dependency_links.txt
+-rw-r--r--   0 ferrix     (501) staff       (20)       14 2023-06-26 17:29:04.000000 django-xff-1.4.0/django_xff.egg-info/requires.txt
+-rw-r--r--   0 ferrix     (501) staff       (20)        4 2023-06-26 17:29:04.000000 django-xff-1.4.0/django_xff.egg-info/top_level.txt
+-rw-r--r--   0 ferrix     (501) staff       (20)      324 2023-06-26 17:29:05.029104 django-xff-1.4.0/setup.cfg
+-rwxr-xr-x   0 ferrix     (501) staff       (20)     1348 2023-06-26 17:14:16.000000 django-xff-1.4.0/setup.py
+drwxr-xr-x   0 ferrix     (501) staff       (20)        0 2023-06-26 17:29:05.026891 django-xff-1.4.0/tests/
+-rw-r--r--   0 ferrix     (501) staff       (20)    13378 2023-06-26 17:14:16.000000 django-xff-1.4.0/tests/test_middleware.py
+-rw-r--r--   0 ferrix     (501) staff       (20)    62474 2023-06-26 17:14:16.000000 django-xff-1.4.0/versioneer.py
+drwxr-xr-x   0 ferrix     (501) staff       (20)        0 2023-06-26 17:29:05.029373 django-xff-1.4.0/xff/
+-rw-r--r--   0 ferrix     (501) staff       (20)        0 2023-06-26 17:14:16.000000 django-xff-1.4.0/xff/__init__.py
+-rw-r--r--   0 ferrix     (501) staff       (20)      471 2023-06-26 17:29:05.029435 django-xff-1.4.0/xff/_version.py
+-rw-r--r--   0 ferrix     (501) staff       (20)     5196 2023-06-26 17:14:16.000000 django-xff-1.4.0/xff/middleware.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-xff-1.3.0/PKG-INFO` & `django-xff-1.4.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,217 +1,209 @@
-Metadata-Version: 1.1
-Name: django-xff
-Version: 1.3.0
-Summary: Django X-Forwarded-For Properly
-Home-page: https://github.com/ferrix/xff/
-Author: Ferrix Hovi
-Author-email: ferrix@codetry.fi
-License: MIT License
-Description: Django X-Forwarded-For Properly
-        -------------------------------
-        
-        The X-Forwarded-For header is used by many reverse proxies to pass the
-        IP addresses of the whole chain of hosts between client and application
-        server. The header looks something like this::
-        
-            X-Forwarded-For: 54.12.13.14, 192.168.2.0, 192.168.3.1
-        
-        This translates to::
-        
-            X-Forwarded-For: client, proxy1[, proxy2[...]]
-        
-        However it is just a header. Most default configurations simply append
-        to the header. It is trivial for a malicious client to deliver a header
-        in the initial request::
-        
-            X-Forwarded-For: phony, client
-        
-        What ``django-xff`` does
-        ========================
-        
-        This library provides a decent and configurable middleware to rewrite
-        the ``request.META['HTTP_REMOTE_ADDR']`` to the correct client IP.
-        
-        This is done by setting a depth of reverse proxies to be trusted alone.
-        The ``X-Forwarded-For`` header will additionally be sanitized from any
-        extraneous entries.
-        
-        By default, if the expected depth of proxies is 3, the ``client``
-        address will be used in all of these examples::
-        
-            X-Forwarded-For: phony, client, proxy1, proxy2
-            X-Forwarded-For: client, proxy1, proxy2
-            X-Forwarded-For: client, proxy
-        
-        Note:
-        
-         * Less proxies than expected is allowed by default, for varying lengths
-           of proxy chains, the longest is the only one that can be trusted.
-         * No header set is allowed by default and the library does nothing.
-        
-        What ``django-xff`` does not do
-        ===============================
-        
-        This library does not check the IP addresses of any proxies along the
-        path of the message.
-        
-        This library is unable to detect compromised proxies or any incoming
-        requests that have the right number addresses in the correct header.
-        
-        TODO
-        ====
-        
-         * Separate middleware that checks CIDR for the trusted proxies
-         * Separate middleware that checks exact IP addresses for proxies
-        
-        Configuration
-        =============
-        
-        Add the following to your Django ``settings.py`` module to enable this
-        middleware for two reverse proxies expected. The middlewares are
-        processed order of appearance. This middleware should go somewhere
-        near the top to avoid giving a potentially malicious user chances to
-        validate passwords with malformed requests::
-        
-            MIDDLEWARE_CLASSES = [
-               <a few middlewares here>
-               'xff.middleware.XForwardedForMiddleware',
-               <more middlewares here>
-            ]
-        
-            XFF_TRUSTED_PROXY_DEPTH = 2
-        
-        By default, no attempts are denied. There are several settings to send
-        a ``400`` (Bad Request) response to failing requests. Strict mode will
-        stop all failing requests::
-        
-            XFF_STRICT = True
-        
-        To prevent only the clearly malicious requests, use the following
-        instead::
-        
-            XFF_NO_SPOOFING = True
-        
-        To prevent requests that do not come through enough proxies, use the
-        following::
-        
-            XFF_ALWAYS_PROXY = True
-        
-        The previous setting implies a Bad Request when there is no
-        ``X-Forwarded-For`` header present. The following setting follows the
-        ``XFF_ALWAYS_PROXY`` and ``XFF_STRICT`` by default but can be set
-        independently::
-        
-            XFF_HEADER_REQUIRED = False
-        
-        Even in ``XFF_LOOSE_UNSAFE`` mode this will require the header::
-        
-            XFF_LOOSE_UNSAFE = True
-        
-        For an unsafe setting, in development possibly, you can trust that the
-        first entry is always correct and still get the assumed client IP in
-        the right place, use::
-        
-            XFF_LOOSE_UNSAFE = True
-        
-        If you want to keep the ``X-Forwarded-For`` header untouched even if
-        there are extra entries, use::
-        
-            XFF_CLEAN = False
-        
-        Whitelisting
-        ============
-        
-        In some cases requests from alternate request paths are to be expected.
-        The Amazon Elastic Loadbalancer healthcheck or other administrative
-        tasks need to be available even if they do not match the criteria.
-        
-        This library accepts URIs as regular expressions to be exempt for
-        checking. These will be exempt for any validation including
-        ``XFF_STRICT`` and ``XFF_HEADER_REQUIRED``.
-        
-        To define the whitelist::
-        
-            XFF_EXEMPT_URLS = [
-                r'^healthcheck/$',
-                r'^admin/',
-            ]
-        
-        This will allow calling ``/healthcheck/`` and ``/admin/*`` from anywhere.
-        It is a daft idea to allow everyone to access the admin site with less
-        requirements than the other parts of the site. For this reason it is
-        possible to respond with ``404`` (Not Found) when the request arrives
-        through the main entrance::
-        
-            XFF_EXEMPT_STEALTH = True
-        
-        This will assume that anything below ``XFF_TRUSTED_PROXY_DEPTH`` is
-        trusted. The method is naive, but effective.
-        
-        Logging
-        =======
-        
-        Dropped requests will be logged. This means that there will be plenty of
-        logs when the library is misconfigured or malicious things are taking
-        place. It is recommended to keep the logs for tracing in case of a real
-        attack. However they can be filtered from development by setting::
-        
-            LOGGING = {
-                'loggers': {
-                     'xff.middleware': {
-                          'handlers': ['null'],
-                          'propagate': False,
-                     },
-                 },
-            }
-        
-        Setting up
-        ==========
-        
-        It is recommended to enable the middleware with the assumed number of
-        proxies and investigating the logs. If the header is not present or the
-        middleware is not configured, there will be no log entries. If the logs
-        state that the depth is incorrect, it should be reduced. If all
-        requests are considered as spoofing, the depth should probably be
-        increased::
-        
-            MIDDLEWARE_CLASSES = [
-                'xff.middleware.XForwardedForMiddleware',
-                'django.contrib.sessions.middleware.SessionMiddleware',
-                'django.middleware.common.CommonMiddleware',
-                'django.contrib.auth.middleware.AuthenticationMiddleware',
-            ]
-        
-            XFF_TRUSTED_PROXY_DEPTH = 2
-        
-        When logs appear correct, control can be increased in increments::
-        
-            XFF_NO_SPOOFING = True
-        
-        Then::
-        
-            XFF_STRICT = True
-        
-        Defining exceptions is feasible with other flags set. The following
-        could be used behind an AWS Elastic Loadbalancer to prevent entry
-        without the proper header set but allow healthcheck to return
-        correctly. The stealth would also mask the same URI with a 404
-        error::
-        
-            XFF_TRUSTED_PROXY_DEPTH = 1
-            XFF_EXEMPT_URLS = [r'^health/]
-            XFF_REQUIRE_HEADER = True
-            XFF_EXEMPT_STEALTH = True
-        
-        In case there is a chain of reverse proxies, the healthcheck URI is
-        available for all layers except the last one.
-        
-Platform: UNKNOWN
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.8
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Django X-Forwarded-For Properly
+-------------------------------
+
+.. image:: https://travis-ci.org/ferrix/xff.svg?branch=master
+    :target: https://travis-ci.org/ferrix/xff
+.. image:: https://coveralls.io/repos/github/ferrix/xff/badge.svg
+    :target: https://coveralls.io/github/ferrix/xff
+
+
+The X-Forwarded-For header is used by many reverse proxies to pass the
+IP addresses of the whole chain of hosts between client and application
+server. The header looks something like this::
+
+    X-Forwarded-For: 54.12.13.14, 192.168.2.0, 192.168.3.1
+
+This translates to::
+
+    X-Forwarded-For: client, proxy1[, proxy2[...]]
+
+However it is just a header. Most default configurations simply append
+to the header. It is trivial for a malicious client to deliver a header
+in the initial request::
+
+    X-Forwarded-For: phony, client
+
+What ``django-xff`` does
+========================
+
+This library provides a decent and configurable middleware to rewrite
+the ``request.META['REMOTE_ADDR']`` to the correct client IP.
+
+This is done by setting a depth of reverse proxies to be trusted alone.
+The ``X-Forwarded-For`` header will additionally be sanitized from any
+extraneous entries.
+
+By default, if the expected depth of proxies is 3, the ``client``
+address will be used in all of these examples::
+
+    X-Forwarded-For: phony, client, proxy1, proxy2
+    X-Forwarded-For: client, proxy1, proxy2
+    X-Forwarded-For: client, proxy
+
+Note:
+
+ * Less proxies than expected is allowed by default, for varying lengths
+   of proxy chains, the longest is the only one that can be trusted.
+ * No header set is allowed by default and the library does nothing.
+
+What ``django-xff`` does not do
+===============================
+
+This library does not check the IP addresses of any proxies along the
+path of the message.
+
+This library is unable to detect compromised proxies or any incoming
+requests that have the right number addresses in the correct header.
+
+TODO
+====
+
+ * Separate middleware that checks CIDR for the trusted proxies
+ * Separate middleware that checks exact IP addresses for proxies
+
+Configuration
+=============
+
+Add the following to your Django ``settings.py`` module to enable this
+middleware for two reverse proxies expected. The middlewares are
+processed order of appearance. This middleware should go somewhere
+near the top to avoid giving a potentially malicious user chances to
+validate passwords with malformed requests::
+
+    MIDDLEWARE_CLASSES = [
+       <a few middlewares here>
+       'xff.middleware.XForwardedForMiddleware',
+       <more middlewares here>
+    ]
+
+    XFF_TRUSTED_PROXY_DEPTH = 2
+
+By default, no attempts are denied. There are several settings to send
+a ``400`` (Bad Request) response to failing requests. Strict mode will
+stop all failing requests::
+
+    XFF_STRICT = True
+
+To prevent only the clearly malicious requests, use the following
+instead::
+
+    XFF_NO_SPOOFING = True
+
+To prevent requests that do not come through enough proxies, use the
+following::
+
+    XFF_ALWAYS_PROXY = True
+
+The previous setting implies a Bad Request when there is no
+``X-Forwarded-For`` header present. The following setting follows the
+``XFF_ALWAYS_PROXY`` and ``XFF_STRICT`` by default but can be set
+independently::
+
+    XFF_HEADER_REQUIRED = False
+
+Even in ``XFF_LOOSE_UNSAFE`` mode this will require the header::
+
+    XFF_LOOSE_UNSAFE = True
+
+For an unsafe setting, in development possibly, you can trust that the
+first entry is always correct and still get the assumed client IP in
+the right place, use::
+
+    XFF_LOOSE_UNSAFE = True
+
+By default, this middleware rewrites ``REMOTE_ADDR``. To leave it
+untouched, use::
+
+    XFF_REWRITE_REMOTE_ADDR = False
+
+If you want to keep the ``X-Forwarded-For`` header untouched even if
+there are extra entries, use::
+
+    XFF_CLEAN = False
+
+Whitelisting
+============
+
+In some cases requests from alternate request paths are to be expected.
+The Amazon Elastic Loadbalancer healthcheck or other administrative
+tasks need to be available even if they do not match the criteria.
+
+This library accepts URIs as regular expressions to be exempt for
+checking. These will be exempt for any validation including
+``XFF_STRICT`` and ``XFF_HEADER_REQUIRED``.
+
+To define the whitelist::
+
+    XFF_EXEMPT_URLS = [
+        r'^healthcheck/$',
+        r'^admin/',
+    ]
+
+This will allow calling ``/healthcheck/`` and ``/admin/*`` from anywhere.
+It is a daft idea to allow everyone to access the admin site with less
+requirements than the other parts of the site. For this reason it is
+possible to respond with ``404`` (Not Found) when the request arrives
+through the main entrance::
+
+    XFF_EXEMPT_STEALTH = True
+
+This will assume that anything below ``XFF_TRUSTED_PROXY_DEPTH`` is
+trusted. The method is naive, but effective.
+
+Logging
+=======
+
+Dropped requests will be logged. This means that there will be plenty of
+logs when the library is misconfigured or malicious things are taking
+place. It is recommended to keep the logs for tracing in case of a real
+attack. However they can be filtered from development by setting::
+
+    LOGGING = {
+        'loggers': {
+             'xff.middleware': {
+                  'handlers': ['null'],
+                  'propagate': False,
+             },
+         },
+    }
+
+Setting up
+==========
+
+It is recommended to enable the middleware with the assumed number of
+proxies and investigating the logs. If the header is not present or the
+middleware is not configured, there will be no log entries. If the logs
+state that the depth is incorrect, it should be reduced. If all
+requests are considered as spoofing, the depth should probably be
+increased::
+
+    MIDDLEWARE_CLASSES = [
+        'xff.middleware.XForwardedForMiddleware',
+        'django.contrib.sessions.middleware.SessionMiddleware',
+        'django.middleware.common.CommonMiddleware',
+        'django.contrib.auth.middleware.AuthenticationMiddleware',
+    ]
+
+    XFF_TRUSTED_PROXY_DEPTH = 2
+
+When logs appear correct, control can be increased in increments::
+
+    XFF_NO_SPOOFING = True
+
+Then::
+
+    XFF_STRICT = True
+
+Defining exceptions is feasible with other flags set. The following
+could be used behind an AWS Elastic Loadbalancer to prevent entry
+without the proper header set but allow healthcheck to return
+correctly. The stealth would also mask the same URI with a 404
+error::
+
+    XFF_TRUSTED_PROXY_DEPTH = 1
+    XFF_EXEMPT_URLS = [r'^health/]
+    XFF_REQUIRE_HEADER = True
+    XFF_EXEMPT_STEALTH = True
+
+In case there is a chain of reverse proxies, the healthcheck URI is
+available for all layers except the last one.
```

### Comparing `django-xff-1.3.0/xff/middleware.py` & `django-xff-1.4.0/xff/middleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     cause a bad request to be sent on spoofed or wrongly routed requests.
     XFF_ALWAYS_PROXY will drop all requests with too little depth.
     XFF_NO_SPOOFING will drop connections with too many headers.
 
     This middleware will automatically clean the X-Forwarded-For header
     unless XFF_CLEAN = False is set.
 
+    By default, this middleware rewrites HTTP_REMOTE_ADDR. To leave it
+    untouched, set XFF_REWRITE_REMOTE_ADDR = False.
+
     XFF_LOOSE_UNSAFE = True will simply shut up and set the last in the
     stack.
 
     XFF_EXEMPT_URLS can be an iterable (eg. list) that defines URLs as
     regexps that will not be checked. XFF_EXEMPT_STEALTH = True will
     return a 404 when all proxies are present. This is nice for a
     healtcheck URL that is not for the public eye.
@@ -50,14 +53,16 @@
         self.loose = getattr(settings, 'XFF_LOOSE_UNSAFE', False)
         self.strict = getattr(settings, 'XFF_STRICT', False)
         self.always_proxy = getattr(settings, 'XFF_ALWAYS_PROXY', False)
         self.no_spoofing = getattr(settings, 'XFF_NO_SPOOFING', False)
         self.header_required = getattr(settings, 'XFF_HEADER_REQUIRED',
                                        (self.always_proxy or self.strict))
         self.clean = getattr(settings, 'XFF_CLEAN', True)
+        self.rewrite_remote = getattr(settings, 'XFF_REWRITE_REMOTE_ADDR',
+                                      True)
 
     def __call__(self, request):
         response = self.process_request(request)
         if not response:
             response = self.get_response(request)
         return response
 
@@ -73,15 +78,16 @@
             header = request.META['HTTP_X_FORWARDED_FOR']
             levels = [x.strip() for x in header.split(',')]
 
             if len(levels) >= depth and exempt and self.stealth:
                 return HttpResponseNotFound()
 
             if self.loose or exempt:
-                request.META['REMOTE_ADDR'] = levels[0]
+                if self.rewrite_remote:
+                    request.META['REMOTE_ADDR'] = levels[0]
                 return None
 
             if len(levels) != depth and self.strict:
                 logger.warning((
                     "Incorrect proxy depth in incoming request.\n" +
                     'Expected {} and got {} remote addresses in ' +
                     'X-Forwarded-For header.')
@@ -104,15 +110,16 @@
                 logger.info(
                     ('X-Forwarded-For spoof attempt with {} addresses when ' +
                      '{} expected. Full header: {}').format(
                          len(levels), depth, header))
                 if self.no_spoofing:
                     return HttpResponseBadRequest()
 
-            request.META['REMOTE_ADDR'] = levels[-1 * depth]
+            if self.rewrite_remote:
+                request.META['REMOTE_ADDR'] = levels[-1 * depth]
 
             if self.clean:
                 cleaned = ','.join(levels[-1 * depth:])
                 request.META['HTTP_X_FORWARDED_FOR'] = cleaned
 
         elif self.header_required and not (exempt or self.loose):
             logger.error(
```

### Comparing `django-xff-1.3.0/LICENSE` & `django-xff-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-xff-1.3.0/django_xff.egg-info/PKG-INFO` & `django-xff-1.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,217 +1,228 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-xff
-Version: 1.3.0
+Version: 1.4.0
 Summary: Django X-Forwarded-For Properly
 Home-page: https://github.com/ferrix/xff/
 Author: Ferrix Hovi
 Author-email: ferrix@codetry.fi
 License: MIT License
-Description: Django X-Forwarded-For Properly
-        -------------------------------
-        
-        The X-Forwarded-For header is used by many reverse proxies to pass the
-        IP addresses of the whole chain of hosts between client and application
-        server. The header looks something like this::
-        
-            X-Forwarded-For: 54.12.13.14, 192.168.2.0, 192.168.3.1
-        
-        This translates to::
-        
-            X-Forwarded-For: client, proxy1[, proxy2[...]]
-        
-        However it is just a header. Most default configurations simply append
-        to the header. It is trivial for a malicious client to deliver a header
-        in the initial request::
-        
-            X-Forwarded-For: phony, client
-        
-        What ``django-xff`` does
-        ========================
-        
-        This library provides a decent and configurable middleware to rewrite
-        the ``request.META['HTTP_REMOTE_ADDR']`` to the correct client IP.
-        
-        This is done by setting a depth of reverse proxies to be trusted alone.
-        The ``X-Forwarded-For`` header will additionally be sanitized from any
-        extraneous entries.
-        
-        By default, if the expected depth of proxies is 3, the ``client``
-        address will be used in all of these examples::
-        
-            X-Forwarded-For: phony, client, proxy1, proxy2
-            X-Forwarded-For: client, proxy1, proxy2
-            X-Forwarded-For: client, proxy
-        
-        Note:
-        
-         * Less proxies than expected is allowed by default, for varying lengths
-           of proxy chains, the longest is the only one that can be trusted.
-         * No header set is allowed by default and the library does nothing.
-        
-        What ``django-xff`` does not do
-        ===============================
-        
-        This library does not check the IP addresses of any proxies along the
-        path of the message.
-        
-        This library is unable to detect compromised proxies or any incoming
-        requests that have the right number addresses in the correct header.
-        
-        TODO
-        ====
-        
-         * Separate middleware that checks CIDR for the trusted proxies
-         * Separate middleware that checks exact IP addresses for proxies
-        
-        Configuration
-        =============
-        
-        Add the following to your Django ``settings.py`` module to enable this
-        middleware for two reverse proxies expected. The middlewares are
-        processed order of appearance. This middleware should go somewhere
-        near the top to avoid giving a potentially malicious user chances to
-        validate passwords with malformed requests::
-        
-            MIDDLEWARE_CLASSES = [
-               <a few middlewares here>
-               'xff.middleware.XForwardedForMiddleware',
-               <more middlewares here>
-            ]
-        
-            XFF_TRUSTED_PROXY_DEPTH = 2
-        
-        By default, no attempts are denied. There are several settings to send
-        a ``400`` (Bad Request) response to failing requests. Strict mode will
-        stop all failing requests::
-        
-            XFF_STRICT = True
-        
-        To prevent only the clearly malicious requests, use the following
-        instead::
-        
-            XFF_NO_SPOOFING = True
-        
-        To prevent requests that do not come through enough proxies, use the
-        following::
-        
-            XFF_ALWAYS_PROXY = True
-        
-        The previous setting implies a Bad Request when there is no
-        ``X-Forwarded-For`` header present. The following setting follows the
-        ``XFF_ALWAYS_PROXY`` and ``XFF_STRICT`` by default but can be set
-        independently::
-        
-            XFF_HEADER_REQUIRED = False
-        
-        Even in ``XFF_LOOSE_UNSAFE`` mode this will require the header::
-        
-            XFF_LOOSE_UNSAFE = True
-        
-        For an unsafe setting, in development possibly, you can trust that the
-        first entry is always correct and still get the assumed client IP in
-        the right place, use::
-        
-            XFF_LOOSE_UNSAFE = True
-        
-        If you want to keep the ``X-Forwarded-For`` header untouched even if
-        there are extra entries, use::
-        
-            XFF_CLEAN = False
-        
-        Whitelisting
-        ============
-        
-        In some cases requests from alternate request paths are to be expected.
-        The Amazon Elastic Loadbalancer healthcheck or other administrative
-        tasks need to be available even if they do not match the criteria.
-        
-        This library accepts URIs as regular expressions to be exempt for
-        checking. These will be exempt for any validation including
-        ``XFF_STRICT`` and ``XFF_HEADER_REQUIRED``.
-        
-        To define the whitelist::
-        
-            XFF_EXEMPT_URLS = [
-                r'^healthcheck/$',
-                r'^admin/',
-            ]
-        
-        This will allow calling ``/healthcheck/`` and ``/admin/*`` from anywhere.
-        It is a daft idea to allow everyone to access the admin site with less
-        requirements than the other parts of the site. For this reason it is
-        possible to respond with ``404`` (Not Found) when the request arrives
-        through the main entrance::
-        
-            XFF_EXEMPT_STEALTH = True
-        
-        This will assume that anything below ``XFF_TRUSTED_PROXY_DEPTH`` is
-        trusted. The method is naive, but effective.
-        
-        Logging
-        =======
-        
-        Dropped requests will be logged. This means that there will be plenty of
-        logs when the library is misconfigured or malicious things are taking
-        place. It is recommended to keep the logs for tracing in case of a real
-        attack. However they can be filtered from development by setting::
-        
-            LOGGING = {
-                'loggers': {
-                     'xff.middleware': {
-                          'handlers': ['null'],
-                          'propagate': False,
-                     },
-                 },
-            }
-        
-        Setting up
-        ==========
-        
-        It is recommended to enable the middleware with the assumed number of
-        proxies and investigating the logs. If the header is not present or the
-        middleware is not configured, there will be no log entries. If the logs
-        state that the depth is incorrect, it should be reduced. If all
-        requests are considered as spoofing, the depth should probably be
-        increased::
-        
-            MIDDLEWARE_CLASSES = [
-                'xff.middleware.XForwardedForMiddleware',
-                'django.contrib.sessions.middleware.SessionMiddleware',
-                'django.middleware.common.CommonMiddleware',
-                'django.contrib.auth.middleware.AuthenticationMiddleware',
-            ]
-        
-            XFF_TRUSTED_PROXY_DEPTH = 2
-        
-        When logs appear correct, control can be increased in increments::
-        
-            XFF_NO_SPOOFING = True
-        
-        Then::
-        
-            XFF_STRICT = True
-        
-        Defining exceptions is feasible with other flags set. The following
-        could be used behind an AWS Elastic Loadbalancer to prevent entry
-        without the proper header set but allow healthcheck to return
-        correctly. The stealth would also mask the same URI with a 404
-        error::
-        
-            XFF_TRUSTED_PROXY_DEPTH = 1
-            XFF_EXEMPT_URLS = [r'^health/]
-            XFF_REQUIRE_HEADER = True
-            XFF_EXEMPT_STEALTH = True
-        
-        In case there is a chain of reverse proxies, the healthcheck URI is
-        available for all layers except the last one.
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.8
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
+Django X-Forwarded-For Properly
+-------------------------------
+
+.. image:: https://travis-ci.org/ferrix/xff.svg?branch=master
+    :target: https://travis-ci.org/ferrix/xff
+.. image:: https://coveralls.io/repos/github/ferrix/xff/badge.svg
+    :target: https://coveralls.io/github/ferrix/xff
+
+
+The X-Forwarded-For header is used by many reverse proxies to pass the
+IP addresses of the whole chain of hosts between client and application
+server. The header looks something like this::
+
+    X-Forwarded-For: 54.12.13.14, 192.168.2.0, 192.168.3.1
+
+This translates to::
+
+    X-Forwarded-For: client, proxy1[, proxy2[...]]
+
+However it is just a header. Most default configurations simply append
+to the header. It is trivial for a malicious client to deliver a header
+in the initial request::
+
+    X-Forwarded-For: phony, client
+
+What ``django-xff`` does
+========================
+
+This library provides a decent and configurable middleware to rewrite
+the ``request.META['REMOTE_ADDR']`` to the correct client IP.
+
+This is done by setting a depth of reverse proxies to be trusted alone.
+The ``X-Forwarded-For`` header will additionally be sanitized from any
+extraneous entries.
+
+By default, if the expected depth of proxies is 3, the ``client``
+address will be used in all of these examples::
+
+    X-Forwarded-For: phony, client, proxy1, proxy2
+    X-Forwarded-For: client, proxy1, proxy2
+    X-Forwarded-For: client, proxy
+
+Note:
+
+ * Less proxies than expected is allowed by default, for varying lengths
+   of proxy chains, the longest is the only one that can be trusted.
+ * No header set is allowed by default and the library does nothing.
+
+What ``django-xff`` does not do
+===============================
+
+This library does not check the IP addresses of any proxies along the
+path of the message.
+
+This library is unable to detect compromised proxies or any incoming
+requests that have the right number addresses in the correct header.
+
+TODO
+====
+
+ * Separate middleware that checks CIDR for the trusted proxies
+ * Separate middleware that checks exact IP addresses for proxies
+
+Configuration
+=============
+
+Add the following to your Django ``settings.py`` module to enable this
+middleware for two reverse proxies expected. The middlewares are
+processed order of appearance. This middleware should go somewhere
+near the top to avoid giving a potentially malicious user chances to
+validate passwords with malformed requests::
+
+    MIDDLEWARE_CLASSES = [
+       <a few middlewares here>
+       'xff.middleware.XForwardedForMiddleware',
+       <more middlewares here>
+    ]
+
+    XFF_TRUSTED_PROXY_DEPTH = 2
+
+By default, no attempts are denied. There are several settings to send
+a ``400`` (Bad Request) response to failing requests. Strict mode will
+stop all failing requests::
+
+    XFF_STRICT = True
+
+To prevent only the clearly malicious requests, use the following
+instead::
+
+    XFF_NO_SPOOFING = True
+
+To prevent requests that do not come through enough proxies, use the
+following::
+
+    XFF_ALWAYS_PROXY = True
+
+The previous setting implies a Bad Request when there is no
+``X-Forwarded-For`` header present. The following setting follows the
+``XFF_ALWAYS_PROXY`` and ``XFF_STRICT`` by default but can be set
+independently::
+
+    XFF_HEADER_REQUIRED = False
+
+Even in ``XFF_LOOSE_UNSAFE`` mode this will require the header::
+
+    XFF_LOOSE_UNSAFE = True
+
+For an unsafe setting, in development possibly, you can trust that the
+first entry is always correct and still get the assumed client IP in
+the right place, use::
+
+    XFF_LOOSE_UNSAFE = True
+
+By default, this middleware rewrites ``REMOTE_ADDR``. To leave it
+untouched, use::
+
+    XFF_REWRITE_REMOTE_ADDR = False
+
+If you want to keep the ``X-Forwarded-For`` header untouched even if
+there are extra entries, use::
+
+    XFF_CLEAN = False
+
+Whitelisting
+============
+
+In some cases requests from alternate request paths are to be expected.
+The Amazon Elastic Loadbalancer healthcheck or other administrative
+tasks need to be available even if they do not match the criteria.
+
+This library accepts URIs as regular expressions to be exempt for
+checking. These will be exempt for any validation including
+``XFF_STRICT`` and ``XFF_HEADER_REQUIRED``.
+
+To define the whitelist::
+
+    XFF_EXEMPT_URLS = [
+        r'^healthcheck/$',
+        r'^admin/',
+    ]
+
+This will allow calling ``/healthcheck/`` and ``/admin/*`` from anywhere.
+It is a daft idea to allow everyone to access the admin site with less
+requirements than the other parts of the site. For this reason it is
+possible to respond with ``404`` (Not Found) when the request arrives
+through the main entrance::
+
+    XFF_EXEMPT_STEALTH = True
+
+This will assume that anything below ``XFF_TRUSTED_PROXY_DEPTH`` is
+trusted. The method is naive, but effective.
+
+Logging
+=======
+
+Dropped requests will be logged. This means that there will be plenty of
+logs when the library is misconfigured or malicious things are taking
+place. It is recommended to keep the logs for tracing in case of a real
+attack. However they can be filtered from development by setting::
+
+    LOGGING = {
+        'loggers': {
+             'xff.middleware': {
+                  'handlers': ['null'],
+                  'propagate': False,
+             },
+         },
+    }
+
+Setting up
+==========
+
+It is recommended to enable the middleware with the assumed number of
+proxies and investigating the logs. If the header is not present or the
+middleware is not configured, there will be no log entries. If the logs
+state that the depth is incorrect, it should be reduced. If all
+requests are considered as spoofing, the depth should probably be
+increased::
+
+    MIDDLEWARE_CLASSES = [
+        'xff.middleware.XForwardedForMiddleware',
+        'django.contrib.sessions.middleware.SessionMiddleware',
+        'django.middleware.common.CommonMiddleware',
+        'django.contrib.auth.middleware.AuthenticationMiddleware',
+    ]
+
+    XFF_TRUSTED_PROXY_DEPTH = 2
+
+When logs appear correct, control can be increased in increments::
+
+    XFF_NO_SPOOFING = True
+
+Then::
+
+    XFF_STRICT = True
+
+Defining exceptions is feasible with other flags set. The following
+could be used behind an AWS Elastic Loadbalancer to prevent entry
+without the proper header set but allow healthcheck to return
+correctly. The stealth would also mask the same URI with a 404
+error::
+
+    XFF_TRUSTED_PROXY_DEPTH = 1
+    XFF_EXEMPT_URLS = [r'^health/]
+    XFF_REQUIRE_HEADER = True
+    XFF_EXEMPT_STEALTH = True
+
+In case there is a chain of reverse proxies, the healthcheck URI is
+available for all layers except the last one.
```

### Comparing `django-xff-1.3.0/setup.py` & `django-xff-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-xff-1.3.0/versioneer.py` & `django-xff-1.4.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `django-xff-1.3.0/README.rst` & `django-xff-1.4.0/django_xff.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,35 @@
+Metadata-Version: 2.1
+Name: django-xff
+Version: 1.4.0
+Summary: Django X-Forwarded-For Properly
+Home-page: https://github.com/ferrix/xff/
+Author: Ferrix Hovi
+Author-email: ferrix@codetry.fi
+License: MIT License
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 1.8
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
 Django X-Forwarded-For Properly
 -------------------------------
 
+.. image:: https://travis-ci.org/ferrix/xff.svg?branch=master
+    :target: https://travis-ci.org/ferrix/xff
+.. image:: https://coveralls.io/repos/github/ferrix/xff/badge.svg
+    :target: https://coveralls.io/github/ferrix/xff
+
+
 The X-Forwarded-For header is used by many reverse proxies to pass the
 IP addresses of the whole chain of hosts between client and application
 server. The header looks something like this::
 
     X-Forwarded-For: 54.12.13.14, 192.168.2.0, 192.168.3.1
 
 This translates to::
@@ -17,15 +42,15 @@
 
     X-Forwarded-For: phony, client
 
 What ``django-xff`` does
 ========================
 
 This library provides a decent and configurable middleware to rewrite
-the ``request.META['HTTP_REMOTE_ADDR']`` to the correct client IP.
+the ``request.META['REMOTE_ADDR']`` to the correct client IP.
 
 This is done by setting a depth of reverse proxies to be trusted alone.
 The ``X-Forwarded-For`` header will additionally be sanitized from any
 extraneous entries.
 
 By default, if the expected depth of proxies is 3, the ``client``
 address will be used in all of these examples::
@@ -101,14 +126,19 @@
 
 For an unsafe setting, in development possibly, you can trust that the
 first entry is always correct and still get the assumed client IP in
 the right place, use::
 
     XFF_LOOSE_UNSAFE = True
 
+By default, this middleware rewrites ``REMOTE_ADDR``. To leave it
+untouched, use::
+
+    XFF_REWRITE_REMOTE_ADDR = False
+
 If you want to keep the ``X-Forwarded-For`` header untouched even if
 there are extra entries, use::
 
     XFF_CLEAN = False
 
 Whitelisting
 ============
```

