# Comparing `tmp/3D-registration-0.4.1.tar.gz` & `tmp/3D-registration-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3D-registration-0.4.1.tar", last modified: Tue Jan 31 09:40:06 2023, max compression
+gzip compressed data, was "3D-registration-0.4.3.tar", last modified: Mon Jun 26 15:46:09 2023, max compression
```

## Comparing `3D-registration-0.4.1.tar` & `3D-registration-0.4.3.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-01-31 09:40:06.186325 3D-registration-0.4.1/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     4462 2023-01-31 09:40:06.186398 3D-registration-0.4.1/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)     3237 2023-01-30 13:23:51.000000 3D-registration-0.4.1/README.md
--rw-r--r--   0 leo.guignard   (501) staff       (20)      574 2023-01-31 09:39:28.000000 3D-registration-0.4.1/pyproject.toml
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1835 2023-01-31 09:40:06.186754 3D-registration-0.4.1/setup.cfg
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-01-31 09:40:06.180231 3D-registration-0.4.1/src/
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-01-31 09:40:06.181460 3D-registration-0.4.1/src/3D_registration.egg-info/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     4462 2023-01-31 09:40:06.000000 3D-registration-0.4.1/src/3D_registration.egg-info/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1045 2023-01-31 09:40:06.000000 3D-registration-0.4.1/src/3D_registration.egg-info/SOURCES.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-01-31 09:40:06.000000 3D-registration-0.4.1/src/3D_registration.egg-info/dependency_links.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)      136 2023-01-31 09:40:06.000000 3D-registration-0.4.1/src/3D_registration.egg-info/entry_points.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)      115 2023-01-31 09:40:06.000000 3D-registration-0.4.1/src/3D_registration.egg-info/requires.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       21 2023-01-31 09:40:06.000000 3D-registration-0.4.1/src/3D_registration.egg-info/top_level.txt
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-01-31 09:40:06.182372 3D-registration-0.4.1/src/IO/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     3418 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/IO/IO.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)       71 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/IO/__init__.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)      901 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/IO/folder.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)      704 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/IO/h5.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)     7725 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/IO/inrimage.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1038 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/IO/klb.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)     7047 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/IO/spatial_image.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    21167 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/IO/tif.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-01-31 09:40:06.182752 3D-registration-0.4.1/src/registrationtools/
--rw-r--r--   0 leo.guignard   (501) staff       (20)      543 2023-01-31 09:39:28.000000 3D-registration-0.4.1/src/registrationtools/__init__.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-01-31 09:40:06.180468 3D-registration-0.4.1/src/registrationtools/data/
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-01-31 09:40:06.182892 3D-registration-0.4.1/src/registrationtools/data/JSON_spatial/
--rw-r--r--   0 leo.guignard   (501) staff       (20)      560 2022-12-01 16:01:34.000000 3D-registration-0.4.1/src/registrationtools/data/JSON_spatial/test1.json
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-01-31 09:40:06.183640 3D-registration-0.4.1/src/registrationtools/data/JSON_time/
--rw-r--r--   0 leo.guignard   (501) staff       (20)      466 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/registrationtools/data/JSON_time/test1.json
--rw-r--r--   0 leo.guignard   (501) staff       (20)      469 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/registrationtools/data/JSON_time/test2.json
--rw-r--r--   0 leo.guignard   (501) staff       (20)      500 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/registrationtools/data/JSON_time/test3.json
--rw-r--r--   0 leo.guignard   (501) staff       (20)      380 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/registrationtools/data/JSON_time/test4.json
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-01-31 09:40:06.186096 3D-registration-0.4.1/src/registrationtools/data/images/
--rw-r--r--   0 leo.guignard   (501) staff       (20)    72160 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/registrationtools/data/images/t0.tiff
--rw-r--r--   0 leo.guignard   (501) staff       (20)    72161 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/registrationtools/data/images/t1.tiff
--rw-r--r--   0 leo.guignard   (501) staff       (20)    72161 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/registrationtools/data/images/t2.tiff
--rw-r--r--   0 leo.guignard   (501) staff       (20)    72161 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/registrationtools/data/images/t3.tiff
--rw-r--r--   0 leo.guignard   (501) staff       (20)    72161 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/registrationtools/data/images/t4.tiff
--rw-r--r--   0 leo.guignard   (501) staff       (20)    72161 2022-11-23 11:15:09.000000 3D-registration-0.4.1/src/registrationtools/data/images/t5.tiff
--rw-r--r--   0 leo.guignard   (501) staff       (20)    32549 2023-01-31 09:08:03.000000 3D-registration-0.4.1/src/registrationtools/spatial_registration.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    45858 2023-01-31 09:08:03.000000 3D-registration-0.4.1/src/registrationtools/time_registration.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-26 15:46:09.021240 3D-registration-0.4.3/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     4894 2023-06-26 15:46:09.021308 3D-registration-0.4.3/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     3669 2023-01-31 15:38:37.000000 3D-registration-0.4.3/README.md
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      574 2023-06-26 15:44:06.000000 3D-registration-0.4.3/pyproject.toml
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1843 2023-06-26 15:46:09.021689 3D-registration-0.4.3/setup.cfg
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-26 15:46:09.014491 3D-registration-0.4.3/src/
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-26 15:46:09.015692 3D-registration-0.4.3/src/3D_registration.egg-info/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     4894 2023-06-26 15:46:09.000000 3D-registration-0.4.3/src/3D_registration.egg-info/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1076 2023-06-26 15:46:09.000000 3D-registration-0.4.3/src/3D_registration.egg-info/SOURCES.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-06-26 15:46:09.000000 3D-registration-0.4.3/src/3D_registration.egg-info/dependency_links.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      136 2023-06-26 15:46:09.000000 3D-registration-0.4.3/src/3D_registration.egg-info/entry_points.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      122 2023-06-26 15:46:09.000000 3D-registration-0.4.3/src/3D_registration.egg-info/requires.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       21 2023-06-26 15:46:09.000000 3D-registration-0.4.3/src/3D_registration.egg-info/top_level.txt
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-26 15:46:09.016686 3D-registration-0.4.3/src/IO/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     3292 2023-01-31 10:08:26.000000 3D-registration-0.4.3/src/IO/IO.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       71 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/IO/__init__.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      901 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/IO/folder.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      704 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/IO/h5.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     7725 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/IO/inrimage.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1038 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/IO/klb.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     7047 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/IO/spatial_image.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     4508 2023-06-26 15:25:15.000000 3D-registration-0.4.3/src/IO/tif.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-26 15:46:09.017205 3D-registration-0.4.3/src/registrationtools/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      564 2023-06-26 15:44:06.000000 3D-registration-0.4.3/src/registrationtools/__init__.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-26 15:46:09.014726 3D-registration-0.4.3/src/registrationtools/data/
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-26 15:46:09.017342 3D-registration-0.4.3/src/registrationtools/data/JSON_spatial/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      560 2022-12-01 16:01:34.000000 3D-registration-0.4.3/src/registrationtools/data/JSON_spatial/test1.json
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-26 15:46:09.018629 3D-registration-0.4.3/src/registrationtools/data/JSON_time/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      466 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/registrationtools/data/JSON_time/test1.json
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      469 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/registrationtools/data/JSON_time/test2.json
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      500 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/registrationtools/data/JSON_time/test3.json
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      380 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/registrationtools/data/JSON_time/test4.json
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-06-26 15:46:09.020999 3D-registration-0.4.3/src/registrationtools/data/images/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    72160 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/registrationtools/data/images/t0.tiff
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    72161 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/registrationtools/data/images/t1.tiff
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    72161 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/registrationtools/data/images/t2.tiff
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    72161 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/registrationtools/data/images/t3.tiff
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    72161 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/registrationtools/data/images/t4.tiff
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    72161 2022-11-23 11:15:09.000000 3D-registration-0.4.3/src/registrationtools/data/images/t5.tiff
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    34030 2023-06-26 15:23:14.000000 3D-registration-0.4.3/src/registrationtools/spatial_registration.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    47246 2023-06-26 15:23:14.000000 3D-registration-0.4.3/src/registrationtools/time_registration.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    15345 2023-06-26 15:25:25.000000 3D-registration-0.4.3/src/registrationtools/utils.py
```

### Comparing `3D-registration-0.4.1/PKG-INFO` & `3D-registration-0.4.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3D-registration
-Version: 0.4.1
+Version: 0.4.3
 Summary: Some scripts to register images in space and time
 Home-page: https://github.com/GuignardLab/registration-tools
 Author: Léo Guignard
 Author-email: leo.guignard@univ-amu.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/GuignardLab/registration-tools/issues
 Project-URL: Documentation, https://github.com/GuignardLab/registration-tools#README.md
@@ -60,14 +60,25 @@
 
     pip install 3D-registration
 
 Or, if you want the latest version, by specifying the git repository:
 
     pip install git+https://github.com/GuignardLab/registration-tools.git
 
+### Troubleshooting
+- Windows:
+
+    If you are trying to run the script on Windows you might need to install `pthreadvse2.dll`. 
+
+    It can be found there: https://www.pconlife.com/viewfileinfo/pthreadvse2-dll/ . Make sure to download the version that matches your operating system (32 or 64 bits, most likely 64).
+
+- MacOs:
+
+    As there are no M1 binaries available yet, please use rosetta or install an intel version of conda.
+
 ## Usage
 
 Most of the description on how to use the two scripts is described in the [manual] (Note that the installation part is quite outdated, the remaining is ok).
 
 That being said, once installed, one can run either of the scripts from anywhere in a terminal by typing:
 
     time-registration
```

### Comparing `3D-registration-0.4.1/README.md` & `3D-registration-0.4.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,25 @@
 
     pip install 3D-registration
 
 Or, if you want the latest version, by specifying the git repository:
 
     pip install git+https://github.com/GuignardLab/registration-tools.git
 
+### Troubleshooting
+- Windows:
+
+    If you are trying to run the script on Windows you might need to install `pthreadvse2.dll`. 
+
+    It can be found there: https://www.pconlife.com/viewfileinfo/pthreadvse2-dll/ . Make sure to download the version that matches your operating system (32 or 64 bits, most likely 64).
+
+- MacOs:
+
+    As there are no M1 binaries available yet, please use rosetta or install an intel version of conda.
+
 ## Usage
 
 Most of the description on how to use the two scripts is described in the [manual] (Note that the installation part is quite outdated, the remaining is ok).
 
 That being said, once installed, one can run either of the scripts from anywhere in a terminal by typing:
 
     time-registration
```

### Comparing `3D-registration-0.4.1/pyproject.toml` & `3D-registration-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 line-length = 79
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.bumpver]
-current_version = "0.4.1"
+current_version = "0.4.3"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `3D-registration-0.4.1/setup.cfg` & `3D-registration-0.4.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = 3D-registration
-version = 0.4.1
+version = 0.4.3
 description = Some scripts to register images in space and time
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GuignardLab/registration-tools
 author = Léo Guignard
 author_email = leo.guignard@univ-amu.fr
 license = MIT
@@ -34,14 +34,15 @@
 	scipy
 	statsmodels
 	h5py
 	tifffile
 	importlib-resources
 	matplotlib
 	transforms3d
+	ensure
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 
 [options.entry_points]
 console_scripts =
```

### Comparing `3D-registration-0.4.1/src/3D_registration.egg-info/PKG-INFO` & `3D-registration-0.4.3/src/3D_registration.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3D-registration
-Version: 0.4.1
+Version: 0.4.3
 Summary: Some scripts to register images in space and time
 Home-page: https://github.com/GuignardLab/registration-tools
 Author: Léo Guignard
 Author-email: leo.guignard@univ-amu.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/GuignardLab/registration-tools/issues
 Project-URL: Documentation, https://github.com/GuignardLab/registration-tools#README.md
@@ -60,14 +60,25 @@
 
     pip install 3D-registration
 
 Or, if you want the latest version, by specifying the git repository:
 
     pip install git+https://github.com/GuignardLab/registration-tools.git
 
+### Troubleshooting
+- Windows:
+
+    If you are trying to run the script on Windows you might need to install `pthreadvse2.dll`. 
+
+    It can be found there: https://www.pconlife.com/viewfileinfo/pthreadvse2-dll/ . Make sure to download the version that matches your operating system (32 or 64 bits, most likely 64).
+
+- MacOs:
+
+    As there are no M1 binaries available yet, please use rosetta or install an intel version of conda.
+
 ## Usage
 
 Most of the description on how to use the two scripts is described in the [manual] (Note that the installation part is quite outdated, the remaining is ok).
 
 That being said, once installed, one can run either of the scripts from anywhere in a terminal by typing:
 
     time-registration
```

### Comparing `3D-registration-0.4.1/src/3D_registration.egg-info/SOURCES.txt` & `3D-registration-0.4.3/src/3D_registration.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/IO/inrimage.py
 src/IO/klb.py
 src/IO/spatial_image.py
 src/IO/tif.py
 src/registrationtools/__init__.py
 src/registrationtools/spatial_registration.py
 src/registrationtools/time_registration.py
+src/registrationtools/utils.py
 src/registrationtools/data/JSON_spatial/test1.json
 src/registrationtools/data/JSON_time/test1.json
 src/registrationtools/data/JSON_time/test2.json
 src/registrationtools/data/JSON_time/test3.json
 src/registrationtools/data/JSON_time/test4.json
 src/registrationtools/data/images/t0.tiff
 src/registrationtools/data/images/t1.tiff
```

### Comparing `3D-registration-0.4.1/src/IO/IO.py` & `3D-registration-0.4.3/src/IO/IO.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,16 +58,14 @@
     if ext == ".gz":
         root, ext = splitext(root)
         ext = ext.lower()
     if ext == ".inr":
         return read_inrimage(filename)
     elif ext in [".tif", ".tiff"]:
         return read_tif(filename)
-    elif ext in [".npz", ".npy"]:
-        return load(filename)
     elif ext in [".h5", ".hdf5"]:
         return read_h5(filename)
     elif ext == ".klb":
         return read_klb(filename, SP_im)
     elif isdir(filename):
         return read_folder(filename, parallel)
 
@@ -102,15 +100,13 @@
     # is2D = img.shape[2] == 1
     ext = ext.lower()
     if ext == ".gz":
         root, ext = splitext(root)
         ext = ext.lower()
     if ext == ".inr":
         write_inrimage(filename, img)
-    elif ext in [".npz", ".npy"]:
-        save(filename, img)
     elif ext in [".tiff", ".tif"]:
         write_tif(filename, img)
     elif ext == ".klb":
         write_klb(filename, img)
     elif ext in [".h5", ".hdf5"]:
         write_h5(filename, img)
```

### Comparing `3D-registration-0.4.1/src/IO/folder.py` & `3D-registration-0.4.3/src/IO/folder.py`

 * *Files identical despite different names*

### Comparing `3D-registration-0.4.1/src/IO/h5.py` & `3D-registration-0.4.3/src/IO/h5.py`

 * *Files identical despite different names*

### Comparing `3D-registration-0.4.1/src/IO/inrimage.py` & `3D-registration-0.4.3/src/IO/inrimage.py`

 * *Files identical despite different names*

### Comparing `3D-registration-0.4.1/src/IO/klb.py` & `3D-registration-0.4.3/src/IO/klb.py`

 * *Files identical despite different names*

### Comparing `3D-registration-0.4.1/src/IO/spatial_image.py` & `3D-registration-0.4.3/src/IO/spatial_image.py`

 * *Files identical despite different names*

### Comparing `3D-registration-0.4.1/src/registrationtools/__init__.py` & `3D-registration-0.4.3/src/registrationtools/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-__version__ = "0.4.1"
+__version__ = "0.4.3"
 
 from .time_registration import TimeRegistration, time_registration
 from .spatial_registration import SpatialRegistration, spatial_registration
+from .utils import *
 import sys
 
 if 8 < sys.version_info.minor:
     import importlib.resources as importlib_resources
 
     pkg = importlib_resources.files("registrationtools") / "data"
 else:
```

### Comparing `3D-registration-0.4.1/src/registrationtools/data/JSON_spatial/test1.json` & `3D-registration-0.4.3/src/registrationtools/data/JSON_spatial/test1.json`

 * *Files identical despite different names*

### Comparing `3D-registration-0.4.1/src/registrationtools/data/images/t0.tiff` & `3D-registration-0.4.3/src/registrationtools/data/images/t0.tiff`

 * *Files identical despite different names*

### Comparing `3D-registration-0.4.1/src/registrationtools/data/images/t1.tiff` & `3D-registration-0.4.3/src/registrationtools/data/images/t1.tiff`

 * *Files identical despite different names*

### Comparing `3D-registration-0.4.1/src/registrationtools/data/images/t2.tiff` & `3D-registration-0.4.3/src/registrationtools/data/images/t2.tiff`

 * *Files identical despite different names*

### Comparing `3D-registration-0.4.1/src/registrationtools/data/images/t3.tiff` & `3D-registration-0.4.3/src/registrationtools/data/images/t3.tiff`

 * *Files identical despite different names*

### Comparing `3D-registration-0.4.1/src/registrationtools/data/images/t4.tiff` & `3D-registration-0.4.3/src/registrationtools/data/images/t4.tiff`

 * *Files identical despite different names*

### Comparing `3D-registration-0.4.1/src/registrationtools/data/images/t5.tiff` & `3D-registration-0.4.3/src/registrationtools/data/images/t5.tiff`

 * *Files identical despite different names*

### Comparing `3D-registration-0.4.1/src/registrationtools/spatial_registration.py` & `3D-registration-0.4.3/src/registrationtools/spatial_registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,31 +122,41 @@
                 else:
                     param_dict[k] = v
 
         # Default parameters
         self.param_dict = param_dict
         self.init_trsfs = [[], [], []]
         self.path_to_bin = ""
-        self.registration_depth = 3
+        self.registration_depth_start = 6
+        self.registration_depth_end = 3
         self.init_trsf_real_unit = True
         self.image_interpolation = "linear"
         self.apply_trsf = True
         self.compute_trsf = True
         self.test_init = False
         self.begin = None
         self.end = None
         self.trsf_types = []
-        self.time_tag = "TM"
+        self.time_tag = None
         self.bdv_unit = "microns"
         self.bdv_voxel_size = None
         self.do_bdv = 0
         self.flo_im_sizes = None
         self.copy_ref = False
         self.bbox_out = False
 
+        if "registration_depth" in param_dict:
+            self.__dict__["registration_depth_start"] = 6
+            self.__dict__["registration_depth_end"] = param_dict[
+                "registration_depth"
+            ]
+        elif not "registration_depth_start" in param_dict:
+            self.__dict__["registration_depth_start"] = 6
+            self.__dict__["registration_depth_end"] = 3
+
         self.__dict__.update(param_dict)
         self.ref_voxel = tuple(self.ref_voxel)
         self.flo_voxels = [tuple(vox) for vox in self.flo_voxels]
         self.out_voxel = tuple(self.out_voxel)
         self.origin_file_name = file_name
         self.path_to_bin = os.path.join(self.path_to_bin, "")
         if 0 < len(self.path_to_bin) and not os.path.exists(self.path_to_bin):
@@ -363,32 +373,39 @@
             p.trsf_paths = [os.path.split(pi)[0] for pi in p.flo_outs]
             p.trsf_names = ["A{a:d}-{trsf:s}.trsf" for _ in p.flo_outs]
         else:
             formated_paths = []
             p.trsf_names = []
             for pi in p.trsf_paths:
                 path, n = os.path.split(pi)
+                if os.path.splitext(n)[-1] == "":
+                    n = ""
+                    path = pi
+                    if not os.path.exists(path):
+                        os.makedirs(path)
                 if n == "":
                     n = "A{a:d}-{trsf:s}.trsf"
                 elif not "{a:" in n:
                     if not "{trsf:" in n:
                         n += "{a:d}-{trsf:s}.trsf"
                     else:
                         n += "{a:d}.trsf"
                 elif not "{trsf:" in n:
                     n += "{trsf:s}.trsf"
                 formated_paths += [path]
                 p.trsf_names += [n]
             p.trsf_paths = formated_paths
-        if p.begin is None:
+        if p.time_tag is not None:
             s = p.ref_A.find(p.time_tag) + len(p.time_tag)
             e = s
             while p.ref_A[e].isdigit() and e < len(p.ref_A):
                 e += 1
             p.begin = p.end = int(p.ref_A[s:e])
+        else:
+            p.begin = p.end = None
         if p.flo_im_sizes is None:
             p.flo_im_sizes = []
             for im_p in p.flo_As:
                 p.flo_im_sizes.append(imread(im_p).shape)
         if (
             not hasattr(p, "ref_im_size") or p.ref_im_size is None
         ) and p.flo_im_sizes is not None:
@@ -513,16 +530,20 @@
                         p.path_to_bin
                         + "blockmatching -ref "
                         + p.ref_A.format(t=p.begin)
                         + " -flo "
                         + flo_A.format(t=p.begin)
                         + " -reference-voxel %f %f %f" % p.ref_voxel
                         + " -floating-voxel %f %f %f" % flo_voxel
-                        + " -trsf-type %s -py-hl 6 -py-ll %d"
-                        % (trsf_type, p.registration_depth)
+                        + " -trsf-type %s -py-hl %d -py-ll %d"
+                        % (
+                            trsf_type,
+                            p.registration_depth_start,
+                            p.registration_depth_end,
+                        )
                         + init_trsf_command
                         + " -res-trsf "
                         + res_trsf
                         + " -composition-with-initial",
                         shell=True,
                     )
                 trsf_type = p.trsf_types[-1]
@@ -542,16 +563,20 @@
                     p.path_to_bin
                     + "blockmatching -ref "
                     + p.ref_A.format(t=p.begin)
                     + " -flo "
                     + flo_A.format(t=p.begin)
                     + " -reference-voxel %f %f %f" % p.ref_voxel
                     + " -floating-voxel %f %f %f" % flo_voxel
-                    + " -trsf-type %s -py-hl 6 -py-ll %d"
-                    % (trsf_type, p.registration_depth)
+                    + " -trsf-type %s -py-hl %d -py-ll %d"
+                    % (
+                        trsf_type,
+                        p.registration_depth_start,
+                        p.registration_depth_end,
+                    )
                     + init_trsf_command
                     + " -res-trsf "
                     + res_trsf
                     +  # ' -res-voxel-trsf ' + res_voxel_trsf + \
                     # ' -res ' + flo_out +\
                     " -composition-with-initial",
                     shell=True,
@@ -580,21 +605,24 @@
         im = SpatialImage(np.ones(im_shape, dtype=np.uint8))
         im.voxelsize = p.ref_voxel
         template = os.path.join(trsf_path, "tmp.tif")
         res_t = "template.tif"
         imsave(template, im)
         identity = np.identity(4)
 
-        where_a = trsf_name.find("{a:d}")
-        no_a = (trsf_name[:where_a] + trsf_name[where_a + 5 :]).format(
-            trsf=trsf_type
-        )
-        trsf_name_only_a = no_a[:where_a] + "{a:d}" + no_a[where_a:]
-        trsf_fmt = os.path.join(trsf_path, trsf_name_only_a)
+        if p.test_init:
+            trsf_name_only_a = "A{a:d}-init.trsf"
+        else:
+            where_a = trsf_name.find("{a:d}")
+            no_a = (trsf_name[:where_a] + trsf_name[where_a + 5 :]).format(
+                trsf=trsf_type
+            )
+            trsf_name_only_a = no_a[:where_a] + "{a:d}" + no_a[where_a:]
 
+        trsf_fmt = os.path.join(trsf_path, trsf_name_only_a)
         trsf_fmt_no_flo = trsf_fmt.replace("{a:d}", "%d")
         new_trsf_fmt = ".".join(trsf_fmt.split(".")[:-1]) + "-padded.txt"
         new_trsf_fmt_no_flo = new_trsf_fmt.replace("{a:d}", "%d")
         np.savetxt(trsf_fmt.format(a=0, trsf=trsf_type), identity)
 
         call(
             p.path_to_bin
@@ -605,29 +633,39 @@
             + " -template "
             + template
             + " -res "
             + new_trsf_fmt_no_flo
             + " -res-t "
             + os.path.join(trsf_path, res_t)
             + " "
-            + " -trsf-type %s -vs %f %f %f" % ((trsf_type,) + out_voxel),
+            + " -trsf-type %s" % (trsf_type),
             shell=True,
         )
         template = os.path.join(trsf_path, res_t)
         return new_trsf_fmt, template
 
     def apply_trsf(self, p, t=None):
         """
         Apply the transformation according to `trsf_parameters`
 
         Args:
             p (trsf_parameters): parameters for the transformation
         """
         if p.bbox_out:
             trsf_fmt, template = self.pad_trsfs(p, t)
+            if p.out_voxel != p.ref_voxel:
+                before, after = os.path.splitext(template)
+                old_template = template
+                template = "".join((before, ".final_template", after))
+                call(
+                    p.path_to_bin
+                    + f"applyTrsf {old_template} {template} "
+                    + "-vs %f %f %f" % p.out_voxel,
+                    shell=True,
+                )
             A0_trsf = (
                 " -trsf " + trsf_fmt.format(a=0) + " -template " + template
             )
         else:
             A0_trsf = ""
         if p.out_voxel != p.ref_voxel or p.bbox_out:
             call(
```

### Comparing `3D-registration-0.4.1/src/registrationtools/time_registration.py` & `3D-registration-0.4.3/src/registrationtools/time_registration.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,18 +265,17 @@
         self.origin_file_name = file_name
 
         if (
             0 < len(self.projection_path)
             and self.projection_path[-1] != os.path.sep
         ):
             self.projection_path = self.projection_path + os.path.sep
-        if 0 < len(self.path_to_data) and self.path_to_data[-1] != os.path.sep:
-            self.path_to_data = self.path_to_data + os.path.sep
-        if 0 < len(self.trsf_folder) and self.trsf_folder[-1] != os.path.sep:
-            self.trsf_folder = self.trsf_folder + os.path.sep
+
+        self.path_to_data = os.path.join(self.path_to_data, "")
+        self.trsf_folder = os.path.join(self.trsf_folder, "")
         self.path_to_bin = os.path.join(self.path_to_bin, "")
         if 0 < len(self.path_to_bin) and not os.path.exists(self.path_to_bin):
             print("Binary path could not be found, will try with global call")
             self.path_to_bin = ""
 
 
 class TimeRegistration:
@@ -614,22 +613,33 @@
     def prepare_paths(p: trsf_parameters):
         """
         Prepare the paths in a format that is usable by the algorithm
 
         Args:
             p (trsf_parameters): parameter object
         """
+        image_formats = [
+            ".tiff",
+            ".tif",
+            ".inr",
+            ".gz",
+            ".klb",
+            ".h5",
+            ".hdf5",
+        ]
         ### Check the file names and folders:
         p.im_ext = p.file_name.split(".")[-1]  # Image type
         p.A0 = os.path.join(p.path_to_data, p.file_name)  # Image path
         # Output format
         if p.output_format is not None:
+            # If the output format is a file alone
             if os.path.split(p.output_format)[0] == "":
                 p.A0_out = os.path.join(p.path_to_data, p.output_format)
-            elif os.path.split(p.output_format)[1] == "":
+            # If the output format is a folder alone
+            elif not os.path.splitext(p.output_format)[-1] in image_formats:
                 p.A0_out = os.path.join(p.output_format, p.file_name)
             else:
                 p.A0_out = p.output_format
         else:
             p.A0_out = os.path.join(
                 p.path_to_data,
                 p.file_name.replace(p.im_ext, p.suffix + "." + p.im_ext),
@@ -894,36 +904,66 @@
                 -1:-4:-1
             ]
             template = p.A0.format(t=p.ref_TP)
         else:
             X, Y, Z = imread(p.A0.format(t=p.ref_TP)).shape
             template = p.A0.format(t=p.ref_TP)
 
+        if p.voxel_size != p.voxel_size_out:
+            before, after = os.path.splitext(template)
+            old_template = template
+            template = "".join((before, ".final_template", after))
+            call(
+                p.path_to_bin
+                + f"applyTrsf {old_template} {template} "
+                + "-vs %f %f %f" % p.voxel_size_out,
+                shell=True,
+            )
+            X, Y, Z = imread(template).shape
+
         xy_proj = np.zeros((X, Y, len(p.time_points)), dtype=np.uint16)
         xz_proj = np.zeros((X, Z, len(p.time_points)), dtype=np.uint16)
         yz_proj = np.zeros((Y, Z, len(p.time_points)), dtype=np.uint16)
         for i, t in enumerate(sorted(p.time_points)):
             folder_tmp = os.path.split(p.A0_out.format(t=t))[0]
             if not os.path.exists(folder_tmp):
                 os.makedirs(folder_tmp)
             call(
                 p.path_to_bin
-                + "applyTrsf '%s' '%s' -trsf "
+                + "applyTrsf %s %s -trsf "
                 % (p.A0.format(t=t), p.A0_out.format(t=t))
                 + os.path.join(
                     p.trsf_folder, trsf_fmt.format(flo=t, ref=p.ref_TP)
                 )
                 + " -template "
                 + template
                 + " -floating-voxel %f %f %f " % p.voxel_size
                 + " -reference-voxel %f %f %f " % p.voxel_size_out
                 + " -interpolation %s" % p.image_interpolation,
                 shell=True,
             )
-            im = imread(p.A0_out.format(t=t))
+            try:
+                im = imread(p.A0_out.format(t=t))
+            except Exception as e:
+                # print("applyTrsf failed at t=",str(t),", retrying now")
+                call(
+                    p.path_to_bin
+                    + "applyTrsf %s %s -trsf "
+                    % (p.A0.format(t=t), p.A0_out.format(t=t))
+                    + os.path.join(
+                        p.trsf_folder, trsf_fmt.format(flo=t, ref=p.ref_TP)
+                    )
+                    + " -template "
+                    + template
+                    + " -floating-voxel %f %f %f " % p.voxel_size
+                    + " -reference-voxel %f %f %f " % p.voxel_size_out
+                    + " -interpolation %s" % p.image_interpolation,
+                    shell=True,
+                )
+                im = imread(p.A0_out.format(t=t))
             if p.projection_path is not None:
                 xy_proj[..., i] = SpatialImage(np.max(im, axis=2))
                 xz_proj[..., i] = SpatialImage(np.max(im, axis=1))
                 yz_proj[..., i] = SpatialImage(np.max(im, axis=0))
         if p.projection_path is not None:
             if not os.path.exists(p.projection_path):
                 os.makedirs(p.projection_path)
@@ -1140,15 +1180,14 @@
             self.do_ViewRegistration(ViewRegistrations, p, t)
 
         with open(p.out_bdv, "w") as f:
             f.write(self.prettify(SpimData))
             f.close()
 
     def plot_transformations(self, p: trsf_parameters):
-
         trsf_fmt = "t{flo:06d}-{ref:06d}.txt"
         if p.lowess:
             trsf_fmt = "t{flo:06d}-{ref:06d}-filtered.txt"
         if p.trsf_interpolation:
             trsf_fmt = "t{flo:06d}-{ref:06d}-interpolated.txt"
         if p.padding:
             trsf_fmt = "t{flo:06d}-{ref:06d}-padded.txt"
@@ -1198,15 +1237,14 @@
         Start the Spatial registration after having informed the parameter files
         """
         for p in self.params:
             try:
                 print("Starting experiment")
                 print(p)
                 self.prepare_paths(p)
-
                 if p.compute_trsf:
                     self.compute_trsfs(p)
                 if p.plot_trsf:
                     self.plot_transformations(p)
                 if p.apply_trsf and p.trsf_type != "vectorfield":
                     self.apply_trsf(p)
                 if p.do_bdv:
```

