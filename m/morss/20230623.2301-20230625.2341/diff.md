# Comparing `tmp/morss-20230623.2301.tar.gz` & `tmp/morss-20230625.2341.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morss-20230623.2301.tar", last modified: Fri Jun 23 23:01:14 2023, max compression
+gzip compressed data, was "morss-20230625.2341.tar", last modified: Sun Jun 25 23:41:02 2023, max compression
```

## Comparing `morss-20230623.2301.tar` & `morss-20230625.2341.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:01:14.315560 morss-20230623.2301/
--rw-r--r--   0 root         (0) root         (0)    34523 2023-06-23 23:01:02.000000 morss-20230623.2301/LICENSE
--rw-r--r--   0 root         (0) root         (0)    17771 2023-06-23 23:01:14.315560 morss-20230623.2301/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17334 2023-06-23 23:01:02.000000 morss-20230623.2301/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:01:14.311560 morss-20230623.2301/morss/
--rw-r--r--   0 root         (0) root         (0)      869 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1352 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/__main__.py
--rw-r--r--   0 root         (0) root         (0)     3822 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/caching.py
--rw-r--r--   0 root         (0) root         (0)     4230 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/cli.py
--rw-r--r--   0 root         (0) root         (0)    22734 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/crawler.py
--rw-r--r--   0 root         (0) root         (0)     2938 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/feedify.ini
--rw-r--r--   0 root         (0) root         (0)    23557 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/feeds.py
--rw-r--r--   0 root         (0) root         (0)    12442 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/morss.py
--rw-r--r--   0 root         (0) root         (0)    11496 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/readabilite.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/util.py
--rw-r--r--   0 root         (0) root         (0)     8484 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/wsgi.py
--rwxr-xr-x   0 root         (0) root         (0)      822 2023-06-23 23:01:02.000000 morss-20230623.2301/morss-helper
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:01:14.315560 morss-20230623.2301/morss.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17771 2023-06-23 23:01:14.000000 morss-20230623.2301/morss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-23 23:01:14.000000 morss-20230623.2301/morss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 23:01:14.000000 morss-20230623.2301/morss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-23 23:01:14.000000 morss-20230623.2301/morss.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-23 23:01:14.000000 morss-20230623.2301/morss.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-23 23:01:14.000000 morss-20230623.2301/morss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 23:01:14.315560 morss-20230623.2301/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1240 2023-06-23 23:01:02.000000 morss-20230623.2301/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:01:14.315560 morss-20230623.2301/tests/
--rw-r--r--   0 root         (0) root         (0)     3516 2023-06-23 23:01:02.000000 morss-20230623.2301/tests/test_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-06-23 23:01:02.000000 morss-20230623.2301/tests/test_feeds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:01:14.315560 morss-20230623.2301/www/
--rw-r--r--   0 root         (0) root         (0)     1154 2023-06-23 23:01:02.000000 morss-20230623.2301/www/index.html
--rw-r--r--   0 root         (0) root         (0)      735 2023-06-23 23:01:02.000000 morss-20230623.2301/www/logo.svg
--rw-r--r--   0 root         (0) root         (0)     8258 2023-06-23 23:01:02.000000 morss-20230623.2301/www/sheet.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:41:02.696956 morss-20230625.2341/
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-06-25 23:40:52.000000 morss-20230625.2341/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    17665 2023-06-25 23:41:02.696956 morss-20230625.2341/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17228 2023-06-25 23:40:52.000000 morss-20230625.2341/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:41:02.692956 morss-20230625.2341/morss/
+-rw-r--r--   0 root         (0) root         (0)      869 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/caching.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/cli.py
+-rw-r--r--   0 root         (0) root         (0)    22734 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/crawler.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/feedify.ini
+-rw-r--r--   0 root         (0) root         (0)    23557 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/feeds.py
+-rw-r--r--   0 root         (0) root         (0)    12447 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/morss.py
+-rw-r--r--   0 root         (0) root         (0)    11496 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/readabilite.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/util.py
+-rw-r--r--   0 root         (0) root         (0)     8484 2023-06-25 23:40:52.000000 morss-20230625.2341/morss/wsgi.py
+-rwxr-xr-x   0 root         (0) root         (0)      822 2023-06-25 23:40:52.000000 morss-20230625.2341/morss-helper
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:41:02.696956 morss-20230625.2341/morss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17665 2023-06-25 23:41:02.000000 morss-20230625.2341/morss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-25 23:41:02.000000 morss-20230625.2341/morss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 23:41:02.000000 morss-20230625.2341/morss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-25 23:41:02.000000 morss-20230625.2341/morss.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-25 23:41:02.000000 morss-20230625.2341/morss.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-25 23:41:02.000000 morss-20230625.2341/morss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 23:41:02.696956 morss-20230625.2341/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-06-25 23:40:52.000000 morss-20230625.2341/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:41:02.696956 morss-20230625.2341/tests/
+-rw-r--r--   0 root         (0) root         (0)     3516 2023-06-25 23:40:52.000000 morss-20230625.2341/tests/test_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-06-25 23:40:52.000000 morss-20230625.2341/tests/test_feeds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 23:41:02.696956 morss-20230625.2341/www/
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-06-25 23:40:52.000000 morss-20230625.2341/www/index.html
+-rw-r--r--   0 root         (0) root         (0)      735 2023-06-25 23:40:52.000000 morss-20230625.2341/www/logo.svg
+-rw-r--r--   0 root         (0) root         (0)     8258 2023-06-25 23:40:52.000000 morss-20230625.2341/www/sheet.xsl
```

### Comparing `morss-20230623.2301/LICENSE` & `morss-20230625.2341/LICENSE`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/PKG-INFO` & `morss-20230625.2341/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morss
-Version: 20230623.2301
+Version: 20230625.2341
 Summary: Get full-text RSS feeds
 Home-page: http://morss.it/
 Author: pictuga
 Author-email: contact@pictuga.com
 License: AGPL v3
 Project-URL: Source, https://git.pictuga.com/pictuga/morss
 Project-URL: Bug Tracker, https://github.com/pictuga/morss/issues
@@ -93,17 +93,17 @@
 
 From git
 
 ```shell
 pip install git+https://git.pictuga.com/pictuga/morss.git#egg=morss[full]
 ```
 
-The full install includes all the cache backends. Otherwise, only in-memory and
-sqlite3 caches are available. The full install also includes gunicorn (for more
-efficient HTTP handling).
+The full install includes all the cache backends. Otherwise, only in-memory
+cache is available. The full install also includes gunicorn (for more efficient
+HTTP handling).
 
 The dependency `lxml` is fairly long to install (especially on Raspberry Pi, as
 C code needs to be compiled). If possible on your distribution, try installing
 it with the system package manager.
 
 ### Docker
 
@@ -365,33 +365,32 @@
 ```
 
 Using cache and passing arguments:
 
 ```python
 >>> import morss
 >>> url = 'http://feeds.bbci.co.uk/news/rss.xml'
->>> cache = '/tmp/morss-cache.db' # sqlite cache location
+>>> cache = '/tmp/morss-cache' # diskcache cache location
 >>> options = {'csv':True}
 >>> xml_string = morss.process(url, cache, options)
 >>> xml_string[:50]
 '{"title": "BBC News - Home", "desc": "The latest s'
 ```
 
 `morss.process` is actually a wrapper around simpler function. It's still
 possible to call the simpler functions, to have more control on what's happening
 under the hood.
 
 Doing it step-by-step:
 
 ```python
-import morss, morss.crawler
+import morss
 
 url = 'http://newspaper.example/feed.xml'
 options = morss.Options(csv=True) # arguments
-morss.crawler.sqlite_default = '/tmp/morss-cache.db' # sqlite cache location
 
 url, rss = morss.FeedFetch(url, options) # this only grabs the RSS feed
 rss = morss.FeedGather(rss, url, options) # this fills the feed and cleans it up
 
 output = morss.FeedFormat(rss, options, 'unicode') # formats final feed
 ```
```

### Comparing `morss-20230623.2301/README.md` & `morss-20230625.2341/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,17 @@
 
 From git
 
 ```shell
 pip install git+https://git.pictuga.com/pictuga/morss.git#egg=morss[full]
 ```
 
-The full install includes all the cache backends. Otherwise, only in-memory and
-sqlite3 caches are available. The full install also includes gunicorn (for more
-efficient HTTP handling).
+The full install includes all the cache backends. Otherwise, only in-memory
+cache is available. The full install also includes gunicorn (for more efficient
+HTTP handling).
 
 The dependency `lxml` is fairly long to install (especially on Raspberry Pi, as
 C code needs to be compiled). If possible on your distribution, try installing
 it with the system package manager.
 
 ### Docker
 
@@ -349,33 +349,32 @@
 ```
 
 Using cache and passing arguments:
 
 ```python
 >>> import morss
 >>> url = 'http://feeds.bbci.co.uk/news/rss.xml'
->>> cache = '/tmp/morss-cache.db' # sqlite cache location
+>>> cache = '/tmp/morss-cache' # diskcache cache location
 >>> options = {'csv':True}
 >>> xml_string = morss.process(url, cache, options)
 >>> xml_string[:50]
 '{"title": "BBC News - Home", "desc": "The latest s'
 ```
 
 `morss.process` is actually a wrapper around simpler function. It's still
 possible to call the simpler functions, to have more control on what's happening
 under the hood.
 
 Doing it step-by-step:
 
 ```python
-import morss, morss.crawler
+import morss
 
 url = 'http://newspaper.example/feed.xml'
 options = morss.Options(csv=True) # arguments
-morss.crawler.sqlite_default = '/tmp/morss-cache.db' # sqlite cache location
 
 url, rss = morss.FeedFetch(url, options) # this only grabs the RSS feed
 rss = morss.FeedGather(rss, url, options) # this fills the feed and cleans it up
 
 output = morss.FeedFormat(rss, options, 'unicode') # formats final feed
 ```
```

### Comparing `morss-20230623.2301/morss/__init__.py` & `morss-20230625.2341/morss/__init__.py`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/morss/__main__.py` & `morss-20230625.2341/morss/__main__.py`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/morss/caching.py` & `morss-20230625.2341/morss/caching.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,28 +100,15 @@
         return self.cache[key]
 
     def __setitem__(self, key, data):
         self.cache.set(key, data)
 
 
 if 'CACHE' in os.environ:
-    if os.environ['CACHE'] == 'mysql':
-        default_cache = MySQLCacheHandler(
-            user = os.getenv('MYSQL_USER'),
-            password = os.getenv('MYSQL_PWD'),
-            database = os.getenv('MYSQL_DB'),
-            host = os.getenv('MYSQL_HOST', 'localhost')
-        )
-
-    elif os.environ['CACHE'] == 'sqlite':
-        default_cache = SQLiteCache(
-            os.getenv('SQLITE_PATH', ':memory:')
-        )
-
-    elif os.environ['CACHE'] == 'redis':
+    if os.environ['CACHE'] == 'redis':
         default_cache = RedisCacheHandler(
             host = os.getenv('REDIS_HOST', 'localhost'),
             port = int(os.getenv('REDIS_PORT', 6379)),
             db = int(os.getenv('REDIS_DB', 0)),
             password = os.getenv('REDIS_PWD', None)
         )
```

### Comparing `morss-20230623.2301/morss/cli.py` & `morss-20230625.2341/morss/cli.py`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/morss/crawler.py` & `morss-20230625.2341/morss/crawler.py`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/morss/feedify.ini` & `morss-20230625.2341/morss/feedify.ini`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/morss/feeds.py` & `morss-20230625.2341/morss/feeds.py`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/morss/morss.py` & `morss-20230625.2341/morss/morss.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,13 +424,13 @@
 def process(url, cache=None, options=None):
     if not options:
         options = []
 
     options = Options(options)
 
     if cache:
-        caching.default_cache = caching.SQLiteCache(cache)
+        caching.default_cache = caching.DiskCacheHandler(cache)
 
     url, rss = FeedFetch(url, options)
     rss = FeedGather(rss, url, options)
 
     return FeedFormat(rss, options, 'unicode')
```

### Comparing `morss-20230623.2301/morss/readabilite.py` & `morss-20230625.2341/morss/readabilite.py`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/morss/util.py` & `morss-20230625.2341/morss/util.py`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/morss/wsgi.py` & `morss-20230625.2341/morss/wsgi.py`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/morss-helper` & `morss-20230625.2341/morss-helper`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/morss.egg-info/PKG-INFO` & `morss-20230625.2341/morss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morss
-Version: 20230623.2301
+Version: 20230625.2341
 Summary: Get full-text RSS feeds
 Home-page: http://morss.it/
 Author: pictuga
 Author-email: contact@pictuga.com
 License: AGPL v3
 Project-URL: Source, https://git.pictuga.com/pictuga/morss
 Project-URL: Bug Tracker, https://github.com/pictuga/morss/issues
@@ -93,17 +93,17 @@
 
 From git
 
 ```shell
 pip install git+https://git.pictuga.com/pictuga/morss.git#egg=morss[full]
 ```
 
-The full install includes all the cache backends. Otherwise, only in-memory and
-sqlite3 caches are available. The full install also includes gunicorn (for more
-efficient HTTP handling).
+The full install includes all the cache backends. Otherwise, only in-memory
+cache is available. The full install also includes gunicorn (for more efficient
+HTTP handling).
 
 The dependency `lxml` is fairly long to install (especially on Raspberry Pi, as
 C code needs to be compiled). If possible on your distribution, try installing
 it with the system package manager.
 
 ### Docker
 
@@ -365,33 +365,32 @@
 ```
 
 Using cache and passing arguments:
 
 ```python
 >>> import morss
 >>> url = 'http://feeds.bbci.co.uk/news/rss.xml'
->>> cache = '/tmp/morss-cache.db' # sqlite cache location
+>>> cache = '/tmp/morss-cache' # diskcache cache location
 >>> options = {'csv':True}
 >>> xml_string = morss.process(url, cache, options)
 >>> xml_string[:50]
 '{"title": "BBC News - Home", "desc": "The latest s'
 ```
 
 `morss.process` is actually a wrapper around simpler function. It's still
 possible to call the simpler functions, to have more control on what's happening
 under the hood.
 
 Doing it step-by-step:
 
 ```python
-import morss, morss.crawler
+import morss
 
 url = 'http://newspaper.example/feed.xml'
 options = morss.Options(csv=True) # arguments
-morss.crawler.sqlite_default = '/tmp/morss-cache.db' # sqlite cache location
 
 url, rss = morss.FeedFetch(url, options) # this only grabs the RSS feed
 rss = morss.FeedGather(rss, url, options) # this fills the feed and cleans it up
 
 output = morss.FeedFormat(rss, options, 'unicode') # formats final feed
 ```
```

### Comparing `morss-20230623.2301/setup.py` & `morss-20230625.2341/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         'Bug Tracker': 'https://github.com/pictuga/morss/issues',
     },
     license = 'AGPL v3',
     packages = [package_name],
     install_requires = ['lxml', 'bs4', 'python-dateutil', 'chardet'],
     extras_require = {
         'full': ['redis', 'diskcache', 'gunicorn', 'setproctitle'],
-        'dev': ['pylint', 'pytest', 'pytest-cov'],
+        'dev': ['pylint', 'pyenchant', 'pytest', 'pytest-cov'],
     },
     python_requires = '>=2.7',
     package_data = {package_name: ['feedify.ini']},
     data_files = [
         ('share/' + package_name, ['README.md', 'LICENSE']),
         ('share/' + package_name + '/www', glob('www/*.*')),
     ],
```

### Comparing `morss-20230623.2301/tests/test_crawler.py` & `morss-20230625.2341/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/tests/test_feeds.py` & `morss-20230625.2341/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/www/index.html` & `morss-20230625.2341/www/index.html`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/www/logo.svg` & `morss-20230625.2341/www/logo.svg`

 * *Files identical despite different names*

### Comparing `morss-20230623.2301/www/sheet.xsl` & `morss-20230625.2341/www/sheet.xsl`

 * *Files identical despite different names*

