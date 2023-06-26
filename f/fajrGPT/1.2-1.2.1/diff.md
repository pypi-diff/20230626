# Comparing `tmp/fajrGPT-1.2.tar.gz` & `tmp/fajrGPT-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.2.tar", last modified: Sun Jun 25 17:36:04 2023, max compression
+gzip compressed data, was "fajrGPT-1.2.1.tar", last modified: Mon Jun 26 03:52:56 2023, max compression
```

## Comparing `fajrGPT-1.2.tar` & `fajrGPT-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-25 17:36:04.499924 fajrGPT-1.2/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.2/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2944 2023-06-25 17:36:04.499758 fajrGPT-1.2/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.2/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-25 17:36:04.497516 fajrGPT-1.2/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.2/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-1.2/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)     8697 2023-06-25 17:34:53.000000 fajrGPT-1.2/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-25 17:36:04.499565 fajrGPT-1.2/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2944 2023-06-25 17:36:04.000000 fajrGPT-1.2/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-06-25 17:36:04.000000 fajrGPT-1.2/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-06-25 17:36:04.000000 fajrGPT-1.2/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-06-25 17:36:04.000000 fajrGPT-1.2/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-06-25 17:36:04.000000 fajrGPT-1.2/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-06-25 17:36:04.000000 fajrGPT-1.2/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-06-25 17:36:04.499962 fajrGPT-1.2/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1127 2023-06-25 17:35:52.000000 fajrGPT-1.2/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-26 03:52:56.192198 fajrGPT-1.2.1/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.2.1/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-06-26 03:52:56.192048 fajrGPT-1.2.1/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.2.1/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-26 03:52:56.190881 fajrGPT-1.2.1/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.2.1/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-1.2.1/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)     8699 2023-06-26 03:52:10.000000 fajrGPT-1.2.1/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-26 03:52:56.191871 fajrGPT-1.2.1/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-06-26 03:52:56.000000 fajrGPT-1.2.1/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-06-26 03:52:56.000000 fajrGPT-1.2.1/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-06-26 03:52:56.000000 fajrGPT-1.2.1/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-06-26 03:52:56.000000 fajrGPT-1.2.1/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-06-26 03:52:56.000000 fajrGPT-1.2.1/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-06-26 03:52:56.000000 fajrGPT-1.2.1/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-06-26 03:52:56.192237 fajrGPT-1.2.1/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-06-26 03:51:51.000000 fajrGPT-1.2.1/setup.py
```

### Comparing `fajrGPT-1.2/LICENSE` & `fajrGPT-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.2/PKG-INFO` & `fajrGPT-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.2
+Version: 1.2.1
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.2/README.md` & `fajrGPT-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.2/fajrGPT/quran_metadata.py` & `fajrGPT-1.2.1/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.2/fajrGPT/wake.py` & `fajrGPT-1.2.1/fajrGPT/wake.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     stop_audio()
 
     # return back to the main thread
     play_audio_thread.join()
 
 def convert_to_seconds(time_str):
     # Get the number and the time unit (h/m/s)
-    number = int(time_str[:-1])
+    number = float(time_str[:-1])
     unit = time_str[-1].lower()
 
     # Convert to seconds
     if unit == "h":
         return number * 60 * 60
     elif unit == "m":
         return number * 60
```

### Comparing `fajrGPT-1.2/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.2.1/fajrGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.2
+Version: 1.2.1
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.2/setup.py` & `fajrGPT-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.2",
+    version="1.2.1",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

