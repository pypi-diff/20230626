# Comparing `tmp/pyaogmaneo-2.0.7.tar.gz` & `tmp/pyaogmaneo-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.0.7.tar", last modified: Tue Jun 20 19:27:40 2023, max compression
+gzip compressed data, was "pyaogmaneo-2.0.8.tar", last modified: Mon Jun 26 20:10:26 2023, max compression
```

## Comparing `pyaogmaneo-2.0.7.tar` & `pyaogmaneo-2.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-20 19:27:40.737136 pyaogmaneo-2.0.7/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-20 19:27:40.737136 pyaogmaneo-2.0.7/CMake/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.0.7/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-06-20 19:25:57.000000 pyaogmaneo-2.0.7/CMakeLists.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.7/LICENSE.md
--rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.7/MANIFEST.in
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-20 19:27:40.737136 pyaogmaneo-2.0.7/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-05-18 17:15:10.000000 pyaogmaneo-2.0.7/README.md
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-20 19:27:40.737136 pyaogmaneo-2.0.7/pyaogmaneo.egg-info/
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-20 19:27:40.000000 pyaogmaneo-2.0.7/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-06-20 19:27:40.000000 pyaogmaneo-2.0.7/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-20 19:27:40.000000 pyaogmaneo-2.0.7/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2022-12-03 02:07:23.000000 pyaogmaneo-2.0.7/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-06-20 19:27:40.000000 pyaogmaneo-2.0.7/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.0.7/pyproject.toml
--rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-06-20 19:27:40.737136 pyaogmaneo-2.0.7/setup.cfg
--rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-06-20 19:26:10.000000 pyaogmaneo-2.0.7/setup.py
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-20 19:27:40.737136 pyaogmaneo-2.0.7/source/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-20 19:27:40.737136 pyaogmaneo-2.0.7/source/pyaogmaneo/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-09 23:28:26.000000 pyaogmaneo-2.0.7/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-09 23:43:55.000000 pyaogmaneo-2.0.7/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)    15208 2023-06-20 18:21:44.000000 pyaogmaneo-2.0.7/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     6938 2023-06-20 18:21:44.000000 pyaogmaneo-2.0.7/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     8183 2023-06-20 18:12:37.000000 pyaogmaneo-2.0.7/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-06-20 18:21:44.000000 pyaogmaneo-2.0.7/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     8969 2023-06-20 18:42:29.000000 pyaogmaneo-2.0.7/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-26 20:10:25.999165 pyaogmaneo-2.0.8/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-26 20:10:25.999165 pyaogmaneo-2.0.8/CMake/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.0.8/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-06-26 20:00:45.000000 pyaogmaneo-2.0.8/CMakeLists.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.8/LICENSE.md
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.8/MANIFEST.in
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-26 20:10:25.999165 pyaogmaneo-2.0.8/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-06-22 14:37:40.000000 pyaogmaneo-2.0.8/README.md
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-26 20:10:25.999165 pyaogmaneo-2.0.8/pyaogmaneo.egg-info/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-26 20:10:25.000000 pyaogmaneo-2.0.8/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-06-26 20:10:25.000000 pyaogmaneo-2.0.8/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-26 20:10:25.000000 pyaogmaneo-2.0.8/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2022-12-03 02:07:23.000000 pyaogmaneo-2.0.8/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-06-26 20:10:25.000000 pyaogmaneo-2.0.8/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.0.8/pyproject.toml
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-06-26 20:10:25.999165 pyaogmaneo-2.0.8/setup.cfg
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-06-26 20:01:06.000000 pyaogmaneo-2.0.8/setup.py
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-26 20:10:25.999165 pyaogmaneo-2.0.8/source/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-26 20:10:25.999165 pyaogmaneo-2.0.8/source/pyaogmaneo/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-22 14:37:40.000000 pyaogmaneo-2.0.8/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-22 14:37:40.000000 pyaogmaneo-2.0.8/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    15208 2023-06-26 18:24:52.000000 pyaogmaneo-2.0.8/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     6938 2023-06-26 18:24:52.000000 pyaogmaneo-2.0.8/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     8213 2023-06-26 18:24:52.000000 pyaogmaneo-2.0.8/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-06-26 18:24:52.000000 pyaogmaneo-2.0.8/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     8969 2023-06-26 18:24:52.000000 pyaogmaneo-2.0.8/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.0.7/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.0.8/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.7/CMakeLists.txt` & `pyaogmaneo-2.0.8/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG 97fd2822c76ba756acf79f0918c6d13b89f9bbe4
+        GIT_TAG 2e50df8cd14b68438cfb85acdbf3ec2496101034
     )
 
     FetchContent_GetProperties(AOgmaNeo)
 
     if(NOT AOgmaNeo_POPULATED)
         FetchContent_Populate(AOgmaNeo)
         add_subdirectory(${aogmaneo_SOURCE_DIR} ${aogmaneo_BINARY_DIR})
```

### Comparing `pyaogmaneo-2.0.7/LICENSE.md` & `pyaogmaneo-2.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.7/PKG-INFO` & `pyaogmaneo-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.0.7
+Version: 2.0.8
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.0.7/README.md` & `pyaogmaneo-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.7/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.0.8/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.0.7
+Version: 2.0.8
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.0.7/setup.py` & `pyaogmaneo-2.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.0.7",
+    version="2.0.8",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.0.7/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.0.8/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.7/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.0.8/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.7/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.0.8/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.7/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.0.8/source/pyaogmaneo/py_hierarchy.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.7/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.0.8/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -213,13 +213,13 @@
 
             int field_start = vld.size.z * (offset.y + diam * offset.x);
 
             for (int vc = 0; vc < vld.size.z; vc++) {
                 float w0 = vl.weights0[vc + wi_start];
                 float w1 = vl.weights1[vc + wi_start];
 
-                field[vc + field_start] = (w0 + w1) * 0.5f;
+                field[vc + vld.size.z * (offset.y + diam * offset.x)] = (w0 + w1) * 0.5f;
             }
         }
 
     return std::make_tuple(field, std::make_tuple(size.x, size.y, size.z));
 }
```

### Comparing `pyaogmaneo-2.0.7/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.0.8/source/pyaogmaneo/py_image_encoder.h`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 #pragma once
 
 #include "py_helpers.h"
 #include <aogmaneo/image_encoder.h>
 
 namespace pyaon {
-const int image_encoder_magic = 2111637;
+const int image_encoder_magic = 6221138;
 
 struct Image_Visible_Layer_Desc {
     std::tuple<int, int, int> size;
 
     int radius;
 
     Image_Visible_Layer_Desc(
```

### Comparing `pyaogmaneo-2.0.7/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.0.8/source/pyaogmaneo/py_module.cpp`

 * *Files identical despite different names*

