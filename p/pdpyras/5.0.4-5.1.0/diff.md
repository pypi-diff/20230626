# Comparing `tmp/pdpyras-5.0.4.tar.gz` & `tmp/pdpyras-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdpyras-5.0.4.tar", last modified: Wed Jun  7 20:41:28 2023, max compression
+gzip compressed data, was "pdpyras-5.1.0.tar", last modified: Mon Jun 26 16:41:32 2023, max compression
```

## Comparing `pdpyras-5.0.4.tar` & `pdpyras-5.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-06-07 20:41:28.642223 pdpyras-5.0.4/
--rw-r--r--   0 demitri    (503) staff       (20)     1053 2023-05-01 18:31:04.000000 pdpyras-5.0.4/LICENSE
--rw-r--r--   0 demitri    (503) staff       (20)      374 2023-06-07 20:41:28.642088 pdpyras-5.0.4/PKG-INFO
--rw-r--r--   0 demitri    (503) staff       (20)     4792 2023-05-17 22:04:20.000000 pdpyras-5.0.4/README.rst
-drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-06-07 20:41:28.641909 pdpyras-5.0.4/pdpyras.egg-info/
--rw-r--r--   0 demitri    (503) staff       (20)      374 2023-06-07 20:41:28.000000 pdpyras-5.0.4/pdpyras.egg-info/PKG-INFO
--rw-r--r--   0 demitri    (503) staff       (20)      192 2023-06-07 20:41:28.000000 pdpyras-5.0.4/pdpyras.egg-info/SOURCES.txt
--rw-r--r--   0 demitri    (503) staff       (20)        1 2023-06-07 20:41:28.000000 pdpyras-5.0.4/pdpyras.egg-info/dependency_links.txt
--rw-r--r--   0 demitri    (503) staff       (20)       29 2023-06-07 20:41:28.000000 pdpyras-5.0.4/pdpyras.egg-info/requires.txt
--rw-r--r--   0 demitri    (503) staff       (20)        8 2023-06-07 20:41:28.000000 pdpyras-5.0.4/pdpyras.egg-info/top_level.txt
--rw-r--r--   0 demitri    (503) staff       (20)    87112 2023-06-07 20:38:03.000000 pdpyras-5.0.4/pdpyras.py
--rw-r--r--   0 demitri    (503) staff       (20)       38 2023-06-07 20:41:28.642270 pdpyras-5.0.4/setup.cfg
--rw-r--r--   0 demitri    (503) staff       (20)      657 2023-06-07 20:38:03.000000 pdpyras-5.0.4/setup.py
+drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-06-26 16:41:32.338811 pdpyras-5.1.0/
+-rw-r--r--   0 demitri    (503) staff       (20)     1053 2023-05-01 18:31:04.000000 pdpyras-5.1.0/LICENSE
+-rw-r--r--   0 demitri    (503) staff       (20)      374 2023-06-26 16:41:32.338665 pdpyras-5.1.0/PKG-INFO
+-rw-r--r--   0 demitri    (503) staff       (20)     4792 2023-05-17 22:04:20.000000 pdpyras-5.1.0/README.rst
+drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-06-26 16:41:32.338465 pdpyras-5.1.0/pdpyras.egg-info/
+-rw-r--r--   0 demitri    (503) staff       (20)      374 2023-06-26 16:41:32.000000 pdpyras-5.1.0/pdpyras.egg-info/PKG-INFO
+-rw-r--r--   0 demitri    (503) staff       (20)      192 2023-06-26 16:41:32.000000 pdpyras-5.1.0/pdpyras.egg-info/SOURCES.txt
+-rw-r--r--   0 demitri    (503) staff       (20)        1 2023-06-26 16:41:32.000000 pdpyras-5.1.0/pdpyras.egg-info/dependency_links.txt
+-rw-r--r--   0 demitri    (503) staff       (20)       29 2023-06-26 16:41:32.000000 pdpyras-5.1.0/pdpyras.egg-info/requires.txt
+-rw-r--r--   0 demitri    (503) staff       (20)        8 2023-06-26 16:41:32.000000 pdpyras-5.1.0/pdpyras.egg-info/top_level.txt
+-rw-r--r--   0 demitri    (503) staff       (20)    82928 2023-06-26 16:39:56.000000 pdpyras-5.1.0/pdpyras.py
+-rw-r--r--   0 demitri    (503) staff       (20)       38 2023-06-26 16:41:32.338862 pdpyras-5.1.0/setup.cfg
+-rw-r--r--   0 demitri    (503) staff       (20)      657 2023-06-26 16:39:56.000000 pdpyras-5.1.0/setup.py
```

### Comparing `pdpyras-5.0.4/LICENSE` & `pdpyras-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdpyras-5.0.4/README.rst` & `pdpyras-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pdpyras-5.0.4/pdpyras.py` & `pdpyras-5.1.0/pdpyras.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Libraries from PyPI
 import requests
 from deprecation import deprecated, DeprecatedWarning
 from urllib3.exceptions import HTTPError, PoolError
 from requests.exceptions import RequestException
 
-__version__ = '5.0.4'
+__version__ = '5.1.0'
 
 #######################
 ### CLIENT DEFAULTS ###
 #######################
 ITERATION_LIMIT = 1e4
 """
 The maximum position of a result in classic pagination.
@@ -486,46 +486,14 @@
     elif not (url.startswith('http://') or url.startswith('https://')):
         return base_url.rstrip('/') + "/" + url.lstrip('/')
     else:
         raise URLError(
             f"URL {url} does not start with the API base URL {base_url}"
         )
 
-@deprecated(deprecated_in='5.0.0', removed_in='5.1.0',
-        current_version=__version__, details='Use canonical_path instead ' \
-            'to identify and classify URLs.')
-def tokenize_url_path(url, baseurl='https://api.pagerduty.com'):
-    """Return a tuple of path nodes.
-
-    This function is the implementation of URL parsing logic from versions
-    previous to v5.0.0. It is based on assumptions of patterns that are no
-    longer universal in REST API v2 but were once much more common.
-    """
-    urlnparams = url.split('#')[0].split('?')
-    url_nodes = urlnparams[0].lstrip('/').split('/')
-    path_index = 0
-    invalid_url = ValueError('Invalid API resource URL: '+url[:99])
-    if url.startswith(baseurl):
-        path_index = 3
-    elif url.startswith('http') and url_nodes[0].endswith(':'):
-        raise invalid_url
-    if len(url_nodes) - path_index < 1:
-        raise invalid_url
-    path_nodes = tuple(url_nodes[path_index:])
-    if '' in path_nodes:
-        raise invalid_url
-    tokenized_nodes = [path_nodes[0]]
-    if len(path_nodes) >= 3:
-        tokenized_nodes.extend(('{id}', path_nodes[2]))
-    final_node_type = '{id}'
-    if len(path_nodes)%2 == 1:
-        final_node_type = '{index}'
-    tokenized_nodes.append(final_node_type)
-    return tuple(tokenized_nodes)
-
 #######################
 ### ENTITY WRAPPING ###
 #######################
 
 def entity_wrappers(method: str, path: str):
     """
     Obtains entity wrapping information for a given endpoint (path and method)
@@ -663,24 +631,14 @@
     """
     doc = method.__doc__
     def call(self, url, **kw):
         return successful_response(method(self, url, **kw))
     call.__doc__ = doc
     return call
 
-@deprecated(deprecated_in='5.0.0', removed_in='5.1.0',
-    current_version=__version__, details='Use wrapped_entities instead.')
-def resource_envelope(method):
-    """
-    Convenience and consistency decorator for HTTP verb functions.
-
-    DEPRECATED. Use wrapped_entities instead.
-    """
-    return wrapped_entities(method)
-
 def resource_url(method):
     """
     API call decorator that allows passing a resource dict as the path/URL
 
     Most resources returned by the API will contain a ``self`` attribute that is
     the URL of the resource itself.
 
@@ -795,19 +753,14 @@
         return f"{endpoint}: Success (status {r.status_code}) but an " \
             f"expectation still failed{context_msg}"
 
 def last_4(secret: str):
     """Returns an abbreviation of the input"""
     return '*'+str(secret)[-4:]
 
-@deprecated(deprecated_in='5.0.0', removed_in='5.1.0',
-        current_version=__version__, details='Use singular_name instead.')
-def object_type(r_name):
-    return singular_name(r_name)
-
 def plural_name(obj_type: str):
     """
     Pluralizes a name, i.e. the API name from the ``type`` property
 
     :param obj_type:
         The object type, i.e. ``user`` or ``user_reference``
     :returns: The name of the resource, i.e. the last part of the URL for the
@@ -819,24 +772,14 @@
         obj_type = obj_type[:obj_type.index('_reference')]
     if obj_type.endswith('y'):
         # Because English
         return obj_type[:-1]+'ies'
     else:
         return obj_type+'s'
 
-@deprecated(deprecated_in='5.0.0', removed_in='5.1.0',
-        current_version=__version__, details='Use successful_response instead.')
-def raise_on_error(r):
-    return successful_response(r)
-
-@deprecated(deprecated_in='5.0.0', removed_in='5.1.0',
-        current_version=__version__, details='Use plural_name instead.')
-def resource_name(obj_type):
-    return plural_name(obj_type)
-
 def singular_name(r_name: str):
     """
     Singularizes a name, i.e. for the entity wrapper in a POST request
 
     :para r_name:
         The "resource" name, i.e. "escalation_policies", a plural noun that
         forms the part of the canonical path identifying what kind of resource
@@ -922,16 +865,14 @@
       any other HTTP methods.
 
     :param api_key:
         REST API access token to use for HTTP requests
     :param debug:
         Sets :attr:`print_debug`. Set to True to enable verbose command line
         output.
-    :param name:
-        Deprecated in v5.0.0; will be removed in v5.1.0.
     :type token: str
     :type debug: bool
     """
 
     log = None
     """
     A ``logging.Logger`` object for logging messages. By default it is
@@ -1010,18 +951,15 @@
     """
     This is the value sent to `Requests`_ as the ``timeout`` parameter that
     determines the TCP read timeout.
     """
 
     url = ""
 
-    def __init__(self, api_key: str, name=None, debug=False):
-        if name is not None:
-            deprecated_kwarg('name', 'It has no effect and will be removed ' \
-                'in v5.1.0.')
+    def __init__(self, api_key: str, debug=False):
         self.parent = super(PDSession, self)
         self.parent.__init__()
         self.api_key = api_key
         self.log = logging.getLogger(__name__)
         self.print_debug = debug
         self.retry = {}
 
@@ -1181,17 +1119,18 @@
         while True:
             try:
                 response = self.parent.request(method, full_url, **req_kw)
                 self.postprocess(response)
             except (HTTPError, PoolError, RequestException) as e:
                 network_attempts += 1
                 if network_attempts > self.max_network_attempts:
-                    raise PDClientError(f"{endpoint}: Non-transient network " \
+                    error_msg = f"{endpoint}: Non-transient network " \
                         'error; exceeded maximum number of attempts ' \
-                        f"({self.max_network_attempts}) to connect to the API.")
+                        f"({self.max_network_attempts}) to connect to the API."
+                    raise PDClientError(error_msg) from e
                 sleep_timer *= self.cooldown_factor()
                 self.log.warning(
                     "%s: HTTP or network error: %s. retrying in %g seconds.",
                     endpoint, e.__class__.__name__, sleep_timer)
                 time.sleep(sleep_timer)
                 continue
 
@@ -1232,29 +1171,14 @@
                     "(...%s) may be invalid or deactivated."%self.trunc_key,
                     response)
             else:
                 # All went according to plan.
                 return response
 
     @property
-    @deprecated(deprecated_in='5.0.0', removed_in='5.1.0',
-        current_version=__version__)
-    def raise_if_http_error(self):
-        """
-        (DEPRECATED) Raise an exception in iteration if there is a HTTP error.
-        """
-        return True
-
-    @raise_if_http_error.setter
-    @deprecated(deprecated_in='5.0.0', removed_in='5.1.0',
-        current_version=__version__)
-    def raise_if_http_error(self, val: bool):
-        pass
-
-    @property
     def stagger_cooldown(self):
         """
         Randomizing factor for wait times between retries during rate limiting.
 
         If set to number greater than 0, the sleep time for rate limiting will
         (for each successive sleep) be adjusted by a factor of one plus a
         uniformly-distributed random number between 0 and 1 times this number,
@@ -1521,40 +1445,46 @@
         response = self.post('/v2/change/enqueue', json=event)
         response_body = try_decoding(successful_response(
             response,
             context="submitting change event",
         ))
         return response_body.get("id", None)
 
-    def submit(self, summary, source=None, custom_details=None, links=None):
+    def submit(self, summary, source=None, custom_details=None, links=None,
+            timestamp=None):
         """
         Submit an incident change
 
         :param summary:
             Summary / brief description of the change.
         :param source:
             A human-readable name identifying the source of the change.
         :param custom_details:
             The ``payload.custom_details`` property of the payload.
         :param links:
             Set the ``links`` property of the event.
+        :param timestamp:
+            Specifies an event timestamp. Must be an ISO8601-format date/time.
         :type summary: str
         :type source: str
         :type custom_details: dict
         :type links: list
+        :type timestamp: str
         :rtype: str
         """
         local_var = locals()['custom_details']
         if not (local_var is None or isinstance(local_var, dict)):
             raise ValueError("custom_details must be a dict")
+        if timestamp is None:
+            timestamp = self.event_timestamp
         event = {
                 'routing_key': self.api_key,
                 'payload': {
                     'summary': summary,
-                    'timestamp': self.event_timestamp,
+                    'timestamp': timestamp,
                     }
                 }
         if isinstance(source, str):
             event['payload']['source'] = source
         if isinstance(custom_details, dict):
             event['payload']['custom_details'] = custom_details
         if links:
@@ -1569,16 +1499,14 @@
     Implements the most generic and oft-implemented aspects of PagerDuty's REST
     API v2 as an opinionated wrapper of `requests.Session`_.
 
     Inherits from :class:`PDSession`.
 
     :param api_key:
         REST API access token to use for HTTP requests
-    :param name:
-        Deprecated and has no effect as of v5.0.0
     :param default_from:
         The default email address to use in the ``From`` header when making
         API calls using an account-level API access key.
     :param auth_type:
         The type of credential in use. If authenticating with an OAuth access
         token, this must be set to ``oauth2`` or ``bearer``.
     :param debug:
@@ -1608,20 +1536,20 @@
     """
 
     permitted_methods = ('GET', 'POST', 'PUT', 'DELETE')
 
     url = 'https://api.pagerduty.com'
     """Base URL of the REST API"""
 
-    def __init__(self, api_key, name=None, default_from=None,
+    def __init__(self, api_key, default_from=None,
             auth_type='token', debug=False):
         self.api_call_counts = {}
         self.api_time = {}
         self.auth_type = auth_type
-        super(APISession, self).__init__(api_key, name=name, debug=debug)
+        super(APISession, self).__init__(api_key, debug=debug)
         self.default_from = default_from
         self.headers.update({
             'Accept': 'application/vnd.pagerduty+json;version=2',
         })
 
     def after_set_api_key(self):
         self._subdomain = None
@@ -1738,16 +1666,16 @@
         # When determining uniqueness, web/the API is largely case-insensitive:
         simplify = lambda s: s.lower()
         search_term = simplify(query)
         equiv = lambda s: simplify(s[attribute]) == search_term
         obj_iter = self.iter_all(resource, params=query_params)
         return next(iter(filter(equiv, obj_iter)), None)
 
-    def iter_all(self, url, params=None, paginate=None, page_size=None,
-            item_hook=None, total=False):
+    def iter_all(self, url, params=None, page_size=None, item_hook=None,
+            total=False):
         """
         Iterator for the contents of an index endpoint or query.
 
         Automatically paginates and yields the results in each page, until all
         matching results have been yielded or a HTTP error response is received.
 
         If the URL to use supports cursor-based pagintation, then this will
@@ -1759,21 +1687,14 @@
         yielded value will be an entry of the ``users`` array property in the
         response.
 
         :param url:
             The index endpoint URL to use.
         :param params:
             Additional URL parameters to include.
-        :param paginate:
-            In versions before v5.0.0, this could be set to False to disable
-            many of the features of numeric pagination. As of v5.0.0, this
-            keyword argument is deprecated and has no effect. The method can
-            still be used on endpoints that don't fully support pagination yet,
-            i.e. that don't return a ``more`` property in the response, although
-            it will raise a warning.
         :param page_size:
             If set, the ``page_size`` argument will override the
             ``default_page_size`` parameter on the session and set the ``limit``
             parameter to a custom value (default is 100), altering the number of
             pagination results. The actual number of results in the response
             will still take precedence, if it differs; this parameter and
             ``default_page_size`` only dictate what is requested of the API.
@@ -1791,17 +1712,14 @@
             a small performance advantage, as the API in this case does not have
             to compute the total count of results in the query.
         :type url: str
         :type params: dict or None
         :type page_size: int or None
         :type total: bool
         """
-        if paginate is not None:
-            deprecated_kwarg('paginate', details='It has no effect as of ' \
-                'v5.0.0 and will be removed in v5.1.0.')
         # Get entity wrapping and validate that the URL being requested is
         # likely to support pagination:
         path = canonical_path(self.url, url)
         endpoint = f"GET {path}"
         nodes = path.split('/')
         if is_path_param(nodes[-1]):
             # This is based on an as-yet universal pattern, but like classic
@@ -1894,31 +1812,25 @@
             for result in results:
                 n += 1
                 # Call a callable object for each item, i.e. to print progress:
                 if hasattr(item_hook, '__call__'):
                     item_hook(result, n, total_count)
                 yield result
 
-    def iter_cursor(self, url, attribute=None, params=None, item_hook=None):
+    def iter_cursor(self, url, params=None, item_hook=None):
         """
         Iterator for results from an endpoint using cursor-based pagination.
 
         :param url:
             The index endpoint URL to use.
-        :param attribute:
-            User-specified entity wrapper to use. Deprecated and has no effect
-            as of v5.0.0, and will be removed in v5.1.0.
         :param params:
             Query parameters to include in the request.
         :param item_hook:
             A callable object that accepts 3 positional arguments; see
         """
-        if attribute is not None:
-            deprecated_kwarg('attribute', details='It has no effect as of ' \
-                'v5.0.0 and will be removed in v5.1.0.')
         path = canonical_path(self.url, url)
         if path not in CURSOR_BASED_PAGINATION_PATHS:
             raise URLError(f"{path} does not support cursor-based pagination.")
         _, wrapper = entity_wrappers('GET', path)
         user_params = {}
         if isinstance(params, (dict, list)):
             # Override defaults with values given:
@@ -2078,25 +1990,14 @@
             headers['From'] = self.default_from
         if method in ('POST', 'PUT'):
             headers['Content-Type'] = 'application/json'
         if user_headers:
             headers.update(user_headers)
         return headers
 
-    @deprecated(deprecated_in='5.0.0', removed_in='5.1.0',
-        current_version=__version__, details='Use canonical_path to identify ' \
-            'REST API v2 URLs instead.')
-    def profiler_key(self, method, path, suffix=None):
-        """
-        Generates a fixed-format key to classify a request
-        """
-        my_suffix = "" if suffix is None else "#"+suffix
-        path_str = '/'.join(tokenize_url_path(path, baseurl=self.url))
-        return '%s:%s'%(method.lower(), path_str)+my_suffix
-
     @resource_url
     @requires_success
     def rdelete(self, resource, **kw) -> requests.Response:
         """
         Delete a resource.
 
         :param resource:
```

### Comparing `pdpyras-5.0.4/setup.py` & `pdpyras-5.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '5.0.4'
+__version__ = '5.1.0'
 
 if __name__ == '__main__':
     setup(
         name='pdpyras',
         description="PagerDuty Python REST API Sessions",
         long_description="A basic REST API client for PagerDuty based on Requests' Session class",
         py_modules=['pdpyras'],
```

