# Comparing `tmp/th2_grpc_sim-4.2.0.dev4312583252.tar.gz` & `tmp/th2_grpc_sim-5.0.0.dev5376623916.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_sim-4.2.0.dev4312583252.tar", last modified: Thu Mar  2 09:39:55 2023, max compression
+gzip compressed data, was "dist/th2_grpc_sim-5.0.0.dev5376623916.tar", last modified: Mon Jun 26 09:43:26 2023, max compression
```

## Comparing `th2_grpc_sim-4.2.0.dev4312583252.tar` & `th2_grpc_sim-5.0.0.dev5376623916.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-03-02 09:39:11.000000 th2_grpc_sim-4.2.0.dev4312583252/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-03-02 09:39:12.000000 th2_grpc_sim-4.2.0.dev4312583252/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4569 2023-03-02 09:39:11.000000 th2_grpc_sim-4.2.0.dev4312583252/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-03-02 09:39:11.000000 th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim/sim.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim/sim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     4355 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim/sim_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     7291 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim/sim_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-03-02 09:39:40.000000 th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim/sim_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      391 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-03-02 09:39:55.000000 th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-06-26 09:42:34.000000 th2_grpc_sim-5.0.0.dev5376623916/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-26 09:42:35.000000 th2_grpc_sim-5.0.0.dev5376623916/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-06-26 09:42:34.000000 th2_grpc_sim-5.0.0.dev5376623916/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-06-26 09:42:34.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4355 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     7291 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-26 09:43:06.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim.egg-info/top_level.txt
```

### Comparing `th2_grpc_sim-4.2.0.dev4312583252/PKG-INFO` & `th2_grpc_sim-5.0.0.dev5376623916/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_sim
-Version: 4.2.0.dev4312583252
+Version: 5.0.0.dev5376623916
 Summary: th2_grpc_sim
 Home-page: https://github.com/th2-net/th2-grpc-sim
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC sim library
```

### Comparing `th2_grpc_sim-4.2.0.dev4312583252/README.md` & `th2_grpc_sim-5.0.0.dev5376623916/README.md`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-4.2.0.dev4312583252/setup.py` & `th2_grpc_sim-5.0.0.dev5376623916/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.strict_mode = False
 
     def finalize_options(self):
         pass
 
     def run(self):
         proto_path = os.path.abspath('src/main/proto')
-        gen_path = os.path.abspath('src/gen/main/python')
+        gen_path = os.path.abspath('build/generated/source/proto/main/services/python')
 
         if not os.path.exists(gen_path):
             os.makedirs(gen_path)
 
         proto_files = []
         for root, _, files in os.walk(proto_path):
             for filename in files:
@@ -68,16 +68,15 @@
 
 
 class CustomDist(sdist):
 
     def run(self):
         copy_tree(f'src/main/proto/{package_name}', package_name)
 
-        copy_tree(f'src/gen/main/python/{package_name}', package_name)
-        copy_tree(f'src/gen/main/services/python/{package_name}', package_name)
+        copy_tree(f'build/generated/source/proto/main/services/python/{package_name}', package_name)
         Path(f'{package_name}/__init__.py').touch()
         Path(f'{package_name}/py.typed').touch()
 
         def make_packages(root_dir):
             for path in Path(root_dir).iterdir():
                 if path.is_dir():
                     path.joinpath('__init__.py').touch()
@@ -117,15 +116,15 @@
     long_description_content_type='text/markdown',
     author='TH2-devs',
     author_email='th2-devs@exactprosystems.com',
     url='https://github.com/th2-net/th2-grpc-sim',
     license='Apache License 2.0',
     python_requires='>=3.7',
     install_requires=[
-        'th2-grpc-common>=3,<4',
+        'th2-grpc-common>=4,<5',
         'mypy-protobuf==3.2'
     ],
     packages=packages,
     package_data=package_data,
     cmdclass={
         'generate': ProtoGenerator,
         'sdist': CustomDist
```

### Comparing `th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim/sim.proto` & `th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim/sim_pb2.py` & `th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim/sim_pb2.pyi` & `th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim/sim_pb2_grpc.py` & `th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim/sim_service.py` & `th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-4.2.0.dev4312583252/th2_grpc_sim.egg-info/PKG-INFO` & `th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-sim
-Version: 4.2.0.dev4312583252
+Version: 5.0.0.dev5376623916
 Summary: th2_grpc_sim
 Home-page: https://github.com/th2-net/th2-grpc-sim
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC sim library
```

