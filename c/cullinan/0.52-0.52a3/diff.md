# Comparing `tmp/cullinan-0.52.tar.gz` & `tmp/cullinan-0.52a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cullinan-0.52.tar", last modified: Mon Jun 26 10:37:41 2023, max compression
+gzip compressed data, was "cullinan-0.52a3.tar", last modified: Mon Jun 19 18:46:59 2023, max compression
```

## Comparing `cullinan-0.52.tar` & `cullinan-0.52a3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:37:41.741738 cullinan-0.52/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-26 10:37:31.000000 cullinan-0.52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-26 10:37:41.741738 cullinan-0.52/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:37:41.741738 cullinan-0.52/cullinan/
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-26 10:37:31.000000 cullinan-0.52/cullinan/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    25100 2023-06-26 10:37:31.000000 cullinan-0.52/cullinan/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-26 10:37:31.000000 cullinan-0.52/cullinan/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-26 10:37:31.000000 cullinan-0.52/cullinan/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-26 10:37:31.000000 cullinan-0.52/cullinan/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-26 10:37:31.000000 cullinan-0.52/cullinan/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:37:41.741738 cullinan-0.52/cullinan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-26 10:37:41.000000 cullinan-0.52/cullinan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 10:37:41.000000 cullinan-0.52/cullinan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:37:41.000000 cullinan-0.52/cullinan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 10:37:41.000000 cullinan-0.52/cullinan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 10:37:41.000000 cullinan-0.52/cullinan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 10:37:41.741738 cullinan-0.52/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-26 10:37:31.000000 cullinan-0.52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:46:59.598644 cullinan-0.52a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-19 18:46:41.000000 cullinan-0.52a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-19 18:46:59.598644 cullinan-0.52a3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:46:59.598644 cullinan-0.52a3/cullinan/
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-19 18:46:41.000000 cullinan-0.52a3/cullinan/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25143 2023-06-19 18:46:41.000000 cullinan-0.52a3/cullinan/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-19 18:46:41.000000 cullinan-0.52a3/cullinan/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-19 18:46:41.000000 cullinan-0.52a3/cullinan/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-19 18:46:41.000000 cullinan-0.52a3/cullinan/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-19 18:46:41.000000 cullinan-0.52a3/cullinan/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:46:59.598644 cullinan-0.52a3/cullinan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-19 18:46:59.000000 cullinan-0.52a3/cullinan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-19 18:46:59.000000 cullinan-0.52a3/cullinan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 18:46:59.000000 cullinan-0.52a3/cullinan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 18:46:59.000000 cullinan-0.52a3/cullinan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 18:46:59.000000 cullinan-0.52a3/cullinan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 18:46:59.598644 cullinan-0.52a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-19 18:46:41.000000 cullinan-0.52a3/setup.py
```

### Comparing `cullinan-0.52/LICENSE` & `cullinan-0.52a3/LICENSE`

 * *Files identical despite different names*

### Comparing `cullinan-0.52/PKG-INFO` & `cullinan-0.52a3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cullinan
-Version: 0.52
+Version: 0.52a3
 Summary: Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application
 Home-page: https://github.com/plumeink/Cullinan
 Author: plumeink
 Author-email: official@plumeink.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Source, https://github.com/plumeink/Cullinan
 Project-URL: Wiki, https://github.com/plumeink/Cullinan/wiki
```

### Comparing `cullinan-0.52/cullinan/application.py` & `cullinan-0.52a3/cullinan/application.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.52/cullinan/controller.py` & `cullinan-0.52a3/cullinan/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,36 +56,38 @@
                 handler_list.append((url, servlet))
                 return servlet
 
     @staticmethod
     def add_url_ws(url: str, cls: Callable) -> object:
         servlet = type('Servlet' + url.replace('/', ''), (tornado.websocket.WebSocketHandler,),
                        {"set_instance_method": EncapsulationHandler.set_fragment_method})
-        setattr(servlet, 'service', service_list)
         if handler_list.__len__() == 0:
             for item in dir(cls):
                 if not item.startswith('__') and not item.endswith('__'):
                     servlet.set_instance_method(servlet, cls.__dict__[item])
                     servlet.f = types.MethodType(cls.__dict__[item], servlet)
             handler_list.append((url, servlet))
+            print(servlet)
             return servlet
         else:
             for item in handler_list:
                 if url == item[0]:
                     for i in dir(cls):
                         if not i.startswith('__') and not i.endswith('__'):
                             item[1].set_instance_method(item[1], cls.__dict__[i])
                             item[1].f = types.MethodType(cls.__dict__[i], item[1])
+                    print(servlet)
                     return item[1]
             else:
                 for item in dir(cls):
                     if not item.startswith('__') and not item.endswith('__'):
                         servlet.set_instance_method(servlet, cls.__dict__[item])
                         servlet.f = types.MethodType(cls.__dict__[item], servlet)
                 handler_list.append((url, servlet))
+                print(servlet)
                 return servlet
 
 
 class Handler(tornado.web.RequestHandler):
 
     def data_received(self, chunk):
         pass
```

### Comparing `cullinan-0.52/cullinan/dao.py` & `cullinan-0.52a3/cullinan/dao.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.52/cullinan/request.py` & `cullinan-0.52a3/cullinan/request.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.52/cullinan/service.py` & `cullinan-0.52a3/cullinan/service.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.52/cullinan.egg-info/PKG-INFO` & `cullinan-0.52a3/cullinan.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cullinan
-Version: 0.52
+Version: 0.52a3
 Summary: Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application
 Home-page: https://github.com/plumeink/Cullinan
 Author: plumeink
 Author-email: official@plumeink.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Source, https://github.com/plumeink/Cullinan
 Project-URL: Wiki, https://github.com/plumeink/Cullinan/wiki
```

### Comparing `cullinan-0.52/setup.py` & `cullinan-0.52a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.MD", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cullinan',
-    version='0.52',
+    version='0.52a3',
     packages=['cullinan'],
     description='Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application',
     author='plumeink',
     project_urls={
             'Source': 'https://github.com/plumeink/Cullinan',
             'Wiki': 'https://github.com/plumeink/Cullinan/wiki',
       },
```

