# Comparing `tmp/openweathersdk-0.1.0.tar.gz` & `tmp/openweathersdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openweathersdk-0.1.0.tar", last modified: Sun Jun 25 21:55:03 2023, max compression
+gzip compressed data, was "openweathersdk-0.2.0.tar", last modified: Sun Jun 25 22:08:20 2023, max compression
```

## Comparing `openweathersdk-0.1.0.tar` & `openweathersdk-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-06-25 21:55:03.407273 openweathersdk-0.1.0/
--rw-r--r--   0 marcus    (1000) marcus    (1000)      318 2023-06-25 21:55:03.407273 openweathersdk-0.1.0/PKG-INFO
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-06-25 21:55:03.407273 openweathersdk-0.1.0/openweathersdk/
--rw-r--r--   0 marcus    (1000) marcus    (1000)     3108 2023-06-25 21:45:00.000000 openweathersdk-0.1.0/openweathersdk/OpenWeatherMap.py
--rw-r--r--   0 marcus    (1000) marcus    (1000)        0 2023-06-25 21:50:49.000000 openweathersdk-0.1.0/openweathersdk/__init__.py
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-06-25 21:55:03.407273 openweathersdk-0.1.0/openweathersdk.egg-info/
--rw-r--r--   0 marcus    (1000) marcus    (1000)      318 2023-06-25 21:55:03.000000 openweathersdk-0.1.0/openweathersdk.egg-info/PKG-INFO
--rw-r--r--   0 marcus    (1000) marcus    (1000)      220 2023-06-25 21:55:03.000000 openweathersdk-0.1.0/openweathersdk.egg-info/SOURCES.txt
--rw-r--r--   0 marcus    (1000) marcus    (1000)        1 2023-06-25 21:55:03.000000 openweathersdk-0.1.0/openweathersdk.egg-info/dependency_links.txt
--rw-r--r--   0 marcus    (1000) marcus    (1000)       15 2023-06-25 21:55:03.000000 openweathersdk-0.1.0/openweathersdk.egg-info/top_level.txt
--rw-r--r--   0 marcus    (1000) marcus    (1000)       38 2023-06-25 21:55:03.407273 openweathersdk-0.1.0/setup.cfg
--rw-r--r--   0 marcus    (1000) marcus    (1000)      425 2023-06-25 21:43:12.000000 openweathersdk-0.1.0/setup.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-06-25 22:08:20.825017 openweathersdk-0.2.0/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      655 2023-06-25 22:08:20.825017 openweathersdk-0.2.0/PKG-INFO
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-06-25 22:08:20.825017 openweathersdk-0.2.0/openweathersdk/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)     3108 2023-06-25 21:45:00.000000 openweathersdk-0.2.0/openweathersdk/OpenWeatherMap.py
+-rw-r--r--   0 marcus    (1000) marcus    (1000)        0 2023-06-25 21:50:49.000000 openweathersdk-0.2.0/openweathersdk/__init__.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2023-06-25 22:08:20.825017 openweathersdk-0.2.0/openweathersdk.egg-info/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      655 2023-06-25 22:08:20.000000 openweathersdk-0.2.0/openweathersdk.egg-info/PKG-INFO
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      220 2023-06-25 22:08:20.000000 openweathersdk-0.2.0/openweathersdk.egg-info/SOURCES.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)        1 2023-06-25 22:08:20.000000 openweathersdk-0.2.0/openweathersdk.egg-info/dependency_links.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)       15 2023-06-25 22:08:20.000000 openweathersdk-0.2.0/openweathersdk.egg-info/top_level.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)       38 2023-06-25 22:08:20.825017 openweathersdk-0.2.0/setup.cfg
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      755 2023-06-25 22:08:10.000000 openweathersdk-0.2.0/setup.py
```

### Comparing `openweathersdk-0.1.0/openweathersdk/OpenWeatherMap.py` & `openweathersdk-0.2.0/openweathersdk/OpenWeatherMap.py`

 * *Files identical despite different names*

