# Comparing `tmp/glfw-2.6.0.tar.gz` & `tmp/glfw-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glfw-2.6.0.tar", last modified: Fri Jun 23 17:39:50 2023, max compression
+gzip compressed data, was "glfw-2.6.1.tar", last modified: Mon Jun 26 18:43:34 2023, max compression
```

## Comparing `glfw-2.6.0.tar` & `glfw-2.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 17:39:50.106509 glfw-2.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     3372 2023-06-23 17:39:34.000000 glfw-2.6.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-23 17:39:34.000000 glfw-2.6.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-23 17:39:34.000000 glfw-2.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5018 2023-06-23 17:39:50.106509 glfw-2.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4302 2023-06-23 17:39:34.000000 glfw-2.6.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 17:39:50.105509 glfw-2.6.0/glfw/
--rw-rw-rw-   0 root         (0) root         (0)    19575 2023-06-23 17:39:34.000000 glfw-2.6.0/glfw/GLFW.py
--rw-rw-rw-   0 root         (0) root         (0)   115553 2023-06-23 17:39:34.000000 glfw-2.6.0/glfw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6556 2023-06-23 17:39:34.000000 glfw-2.6.0/glfw/library.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 17:39:50.106509 glfw-2.6.0/glfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5018 2023-06-23 17:39:50.000000 glfw-2.6.0/glfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2023-06-23 17:39:50.000000 glfw-2.6.0/glfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 17:39:50.000000 glfw-2.6.0/glfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-23 17:39:50.000000 glfw-2.6.0/glfw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 17:39:50.000000 glfw-2.6.0/glfw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 17:39:50.106509 glfw-2.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1369 2023-06-23 17:39:34.000000 glfw-2.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 18:43:34.533474 glfw-2.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)     3494 2023-06-26 18:43:21.000000 glfw-2.6.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-26 18:43:21.000000 glfw-2.6.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-26 18:43:21.000000 glfw-2.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5312 2023-06-26 18:43:34.533474 glfw-2.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4596 2023-06-26 18:43:21.000000 glfw-2.6.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 18:43:34.532474 glfw-2.6.1/glfw/
+-rw-rw-rw-   0 root         (0) root         (0)    19575 2023-06-26 18:43:21.000000 glfw-2.6.1/glfw/GLFW.py
+-rw-rw-rw-   0 root         (0) root         (0)   115553 2023-06-26 18:43:21.000000 glfw-2.6.1/glfw/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7054 2023-06-26 18:43:21.000000 glfw-2.6.1/glfw/library.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 18:43:34.533474 glfw-2.6.1/glfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5312 2023-06-26 18:43:34.000000 glfw-2.6.1/glfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      241 2023-06-26 18:43:34.000000 glfw-2.6.1/glfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 18:43:34.000000 glfw-2.6.1/glfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-26 18:43:34.000000 glfw-2.6.1/glfw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-26 18:43:34.000000 glfw-2.6.1/glfw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 18:43:34.534474 glfw-2.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-06-26 18:43:21.000000 glfw-2.6.1/setup.py
```

### Comparing `glfw-2.6.0/CHANGELOG.md` & `glfw-2.6.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 For information on changes in GLFW itself, see the [GLFW version history](https://www.glfw.org/changelog.html).
 
+## [2.6.1] - 2023-06-23
+- Revert changes made in 2.6.0
+- Do not search for GLFW library when running in a frozen library
+
 ## [2.6.0] - 2023-06-23
 - Use multiprocessing for library version detection on non-Windows systems
 
 ## [2.5.9] - 2023-04-01
 - Fixed package version in CHANGELOG.md and glfw/__init__.py
 
 ## [2.5.8] - 2023-04-01
```

### Comparing `glfw-2.6.0/LICENSE.txt` & `glfw-2.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `glfw-2.6.0/PKG-INFO` & `glfw-2.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glfw
-Version: 2.6.0
+Version: 2.6.1
 Summary: A ctypes-based wrapper for GLFW3.
 Home-page: https://github.com/FlorianRhiem/pyGLFW
 Author: Florian Rhiem
 Author-email: florian.rhiem@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -90,14 +90,21 @@
 `compiling GLFW from source <http://www.glfw.org/docs/latest/compile.html>`__
 (use ``-DBUILD_SHARED_LIBS=ON``).
 
 pyGLFW will search for the library in a list of search paths (including those
 in ``LD_LIBRARY_PATH``). If you want to use a specific library, you can set
 the ``PYGLFW_LIBRARY`` environment variable to its path.
 
+cx_Freeze / PyInstaller
+~~~~~~~~~~~~~~~~~~~~~~~
+
+pyGLFW is unable to dynamically search for the GLFW library on non-Windows platforms if
+running in an executable frozen with cx_Freeze or PyInstaller, so a path to the library
+must be provided using the ``PYGLFW_LIBRARY`` environment variable.
+
 Development Version
 ~~~~~~~~~~~~~~~~~~~
 
 If you are using the development version of GLFW and would like to use wrappers
 for currently unreleased macros and functions, you can instead install:
 
 .. code:: sh
```

### Comparing `glfw-2.6.0/README.rst` & `glfw-2.6.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,21 @@
 `compiling GLFW from source <http://www.glfw.org/docs/latest/compile.html>`__
 (use ``-DBUILD_SHARED_LIBS=ON``).
 
 pyGLFW will search for the library in a list of search paths (including those
 in ``LD_LIBRARY_PATH``). If you want to use a specific library, you can set
 the ``PYGLFW_LIBRARY`` environment variable to its path.
 
+cx_Freeze / PyInstaller
+~~~~~~~~~~~~~~~~~~~~~~~
+
+pyGLFW is unable to dynamically search for the GLFW library on non-Windows platforms if
+running in an executable frozen with cx_Freeze or PyInstaller, so a path to the library
+must be provided using the ``PYGLFW_LIBRARY`` environment variable.
+
 Development Version
 ~~~~~~~~~~~~~~~~~~~
 
 If you are using the development version of GLFW and would like to use wrappers
 for currently unreleased macros and functions, you can instead install:
 
 .. code:: sh
```

### Comparing `glfw-2.6.0/glfw/GLFW.py` & `glfw-2.6.1/glfw/GLFW.py`

 * *Files identical despite different names*

### Comparing `glfw-2.6.0/glfw/__init__.py` & `glfw-2.6.1/glfw/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import print_function
 from __future__ import division
 from __future__ import unicode_literals
 
 __author__ = 'Florian Rhiem (florian.rhiem@gmail.com)'
 __copyright__ = 'Copyright (c) 2013-2023 Florian Rhiem'
 __license__ = 'MIT'
-__version__ = '2.6.0'
+__version__ = '2.6.1'
 
 # By default, GLFW errors will be handled by a pre-defined error callback.
 # Depending on the value of ERROR_REPORTING, this callback will:
 # - Raise a GLFWError exception, if ERROR_REPORTING is 'raise', 'exception'
 #   or True.
 # - Issue a GLFWError warning, if ERROR_REPORTING is 'warn' or 'warning'.
 # - Log on debug level using the 'glfw' logger, if ERROR_REPORTING is 'log'.
```

### Comparing `glfw-2.6.0/glfw/library.py` & `glfw-2.6.1/glfw/library.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from __future__ import print_function
 from __future__ import division
 from __future__ import unicode_literals
 
 import ctypes
 import os
 import glob
-import multiprocessing
 import sys
 import subprocess
 import textwrap
 
 
 def _find_library_candidates(library_names,
                              library_file_extensions,
@@ -62,50 +61,66 @@
             library_versions.append((version, filename))
 
     if not library_versions:
         return None
     library_versions.sort()
     return ctypes.CDLL(library_versions[-1][1])
 
-def _glfw_get_version_helper(filename, queue):
-    """
-    Queries the library version tuple and puts it in a queue.
-    """
-    try:
-        library_handle = ctypes.CDLL(filename)
-    except OSError:
-        return
-    major_value = ctypes.c_int(0)
-    major = ctypes.pointer(major_value)
-    minor_value = ctypes.c_int(0)
-    minor = ctypes.pointer(minor_value)
-    rev_value = ctypes.c_int(0)
-    rev = ctypes.pointer(rev_value)
-    if hasattr(library_handle, 'glfwGetVersion'):
-        library_handle.glfwGetVersion(major, minor, rev)
-        version = (major_value.value,
-                   minor_value.value,
-                   rev_value.value)
-        queue.put(version)
 
 def _glfw_get_version(filename):
     """
     Queries and returns the library version tuple or None by using a
     subprocess.
     """
-    try:
-        context = multiprocessing.get_context('fork')
-        queue = context.Queue()
-        process = context.Process(target=_glfw_get_version_helper, args=(filename, queue))
-        process.start()
-        process.join()
-        if queue.empty():
-            return None
-        return queue.get()
-    except multiprocessing.ProcessError:
+    version_checker_source = '''
+        import sys
+        import ctypes
+
+        def get_version(library_handle):
+            """
+            Queries and returns the library version tuple or None.
+            """
+            major_value = ctypes.c_int(0)
+            major = ctypes.pointer(major_value)
+            minor_value = ctypes.c_int(0)
+            minor = ctypes.pointer(minor_value)
+            rev_value = ctypes.c_int(0)
+            rev = ctypes.pointer(rev_value)
+            if hasattr(library_handle, 'glfwGetVersion'):
+                library_handle.glfwGetVersion(major, minor, rev)
+                version = (major_value.value,
+                           minor_value.value,
+                           rev_value.value)
+                return version
+            else:
+                return None
+
+        try:
+            input_func = raw_input
+        except NameError:
+            input_func = input
+        filename = input_func().strip()
+
+        try:
+            library_handle = ctypes.CDLL(filename)
+        except OSError:
+            pass
+        else:
+            version = get_version(library_handle)
+            print(version)
+    '''
+
+    args = [sys.executable, '-c', textwrap.dedent(version_checker_source)]
+    process = subprocess.Popen(args, universal_newlines=True,
+                               stdin=subprocess.PIPE, stdout=subprocess.PIPE)
+    out = process.communicate(filename)[0]
+    out = out.strip()
+    if out:
+        return eval(out)
+    else:
         return None
 
 
 def _get_library_search_paths():
     """
     Returns a list of library search paths, considering of the current working
     directory, default paths and paths from environment variables.
@@ -173,10 +188,12 @@
 
     # try conda's default location on Windows
     if glfw is None:
         try:
             glfw = ctypes.CDLL(os.path.join(sys.prefix, 'Library', 'bin', 'glfw3.dll'))
         except OSError:
             pass
-else:
+elif not getattr(sys, "frozen", False):
     glfw = _load_library(['glfw', 'glfw3'], ['.so', '.dylib'],
                           _get_library_search_paths(), _glfw_get_version)
+else:
+    glfw = None
```

### Comparing `glfw-2.6.0/glfw.egg-info/PKG-INFO` & `glfw-2.6.1/glfw.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glfw
-Version: 2.6.0
+Version: 2.6.1
 Summary: A ctypes-based wrapper for GLFW3.
 Home-page: https://github.com/FlorianRhiem/pyGLFW
 Author: Florian Rhiem
 Author-email: florian.rhiem@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -90,14 +90,21 @@
 `compiling GLFW from source <http://www.glfw.org/docs/latest/compile.html>`__
 (use ``-DBUILD_SHARED_LIBS=ON``).
 
 pyGLFW will search for the library in a list of search paths (including those
 in ``LD_LIBRARY_PATH``). If you want to use a specific library, you can set
 the ``PYGLFW_LIBRARY`` environment variable to its path.
 
+cx_Freeze / PyInstaller
+~~~~~~~~~~~~~~~~~~~~~~~
+
+pyGLFW is unable to dynamically search for the GLFW library on non-Windows platforms if
+running in an executable frozen with cx_Freeze or PyInstaller, so a path to the library
+must be provided using the ``PYGLFW_LIBRARY`` environment variable.
+
 Development Version
 ~~~~~~~~~~~~~~~~~~~
 
 If you are using the development version of GLFW and would like to use wrappers
 for currently unreleased macros and functions, you can instead install:
 
 .. code:: sh
```

### Comparing `glfw-2.6.0/setup.py` & `glfw-2.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 setup_directory = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(setup_directory, 'README.rst')) as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='glfw',
-    version='2.6.0',
+    version='2.6.1',
     description='A ctypes-based wrapper for GLFW3.',
     long_description=long_description,
     url='https://github.com/FlorianRhiem/pyGLFW',
     author='Florian Rhiem',
     author_email='florian.rhiem@gmail.com',
     license='MIT',
     classifiers=[
```

