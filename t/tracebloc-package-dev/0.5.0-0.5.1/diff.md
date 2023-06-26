# Comparing `tmp/tracebloc_package-dev-0.5.0.tar.gz` & `tmp/tracebloc_package-dev-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.5.0.tar", last modified: Thu Jun 22 04:59:11 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.5.1.tar", last modified: Mon Jun 26 09:32:28 2023, max compression
```

## Comparing `tracebloc_package-dev-0.5.0.tar` & `tracebloc_package-dev-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-22 04:59:11.330904 tracebloc_package-dev-0.5.0/
--rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.0/LICENSE.txt
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-22 04:59:11.330985 tracebloc_package-dev-0.5.0/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.0/README.md
--rw-r--r--   0 hasan      (501) staff       (20)       78 2023-06-22 04:59:11.331298 tracebloc_package-dev-0.5.0/setup.cfg
--rw-r--r--   0 hasan      (501) staff       (20)      949 2023-06-22 04:56:54.000000 tracebloc_package-dev-0.5.0/setup.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-22 04:59:11.329692 tracebloc_package-dev-0.5.0/tracebloc_package/
--rw-r--r--   0 hasan      (501) staff       (20)       67 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.0/tracebloc_package/__init__.py
--rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.0/tracebloc_package/check_parameters.py
--rw-r--r--   0 hasan      (501) staff       (20)    24369 2023-06-21 10:23:04.000000 tracebloc_package-dev-0.5.0/tracebloc_package/functional_test.py
--rw-r--r--   0 hasan      (501) staff       (20)    61149 2023-06-09 12:24:04.000000 tracebloc_package-dev-0.5.0/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-03-23 11:28:43.000000 tracebloc_package-dev-0.5.0/tracebloc_package/messages.py
--rw-r--r--   0 hasan      (501) staff       (20)    10936 2023-06-21 10:23:04.000000 tracebloc_package-dev-0.5.0/tracebloc_package/upload.py
--rw-r--r--   0 hasan      (501) staff       (20)    10427 2023-06-09 12:24:04.000000 tracebloc_package-dev-0.5.0/tracebloc_package/user.py
--rw-r--r--   0 hasan      (501) staff       (20)     6712 2023-06-21 10:23:04.000000 tracebloc_package-dev-0.5.0/tracebloc_package/utils.py
--rw-r--r--   0 hasan      (501) staff       (20)     3200 2023-06-09 12:24:04.000000 tracebloc_package-dev-0.5.0/tracebloc_package/weights.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-22 04:59:11.330748 tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-22 04:59:11.000000 tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      591 2023-06-22 04:59:11.000000 tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-22 04:59:11.000000 tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-22 04:59:11.000000 tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 hasan      (501) staff       (20)      119 2023-06-22 04:59:11.000000 tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 hasan      (501) staff       (20)       18 2023-06-22 04:59:11.000000 tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-26 09:32:28.833543 tracebloc_package-dev-0.5.1/
+-rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.1/LICENSE.txt
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-26 09:32:28.833623 tracebloc_package-dev-0.5.1/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.1/README.md
+-rw-r--r--   0 hasan      (501) staff       (20)       78 2023-06-26 09:32:28.833845 tracebloc_package-dev-0.5.1/setup.cfg
+-rw-r--r--   0 hasan      (501) staff       (20)      949 2023-06-23 11:35:27.000000 tracebloc_package-dev-0.5.1/setup.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-26 09:32:28.832588 tracebloc_package-dev-0.5.1/tracebloc_package/
+-rw-r--r--   0 hasan      (501) staff       (20)       67 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.1/tracebloc_package/__init__.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.1/tracebloc_package/check_parameters.py
+-rw-r--r--   0 hasan      (501) staff       (20)    24334 2023-06-23 11:37:55.000000 tracebloc_package-dev-0.5.1/tracebloc_package/functional_test.py
+-rw-r--r--   0 hasan      (501) staff       (20)    61330 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.1/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.1/tracebloc_package/messages.py
+-rw-r--r--   0 hasan      (501) staff       (20)    10936 2023-06-23 10:56:15.000000 tracebloc_package-dev-0.5.1/tracebloc_package/upload.py
+-rw-r--r--   0 hasan      (501) staff       (20)    10427 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.1/tracebloc_package/user.py
+-rw-r--r--   0 hasan      (501) staff       (20)     6712 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.1/tracebloc_package/utils.py
+-rw-r--r--   0 hasan      (501) staff       (20)     3200 2023-06-09 12:24:04.000000 tracebloc_package-dev-0.5.1/tracebloc_package/weights.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-26 09:32:28.833420 tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-26 09:32:28.000000 tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      591 2023-06-26 09:32:28.000000 tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-26 09:32:28.000000 tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-26 09:32:28.000000 tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 hasan      (501) staff       (20)      119 2023-06-26 09:32:28.000000 tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 hasan      (501) staff       (20)       18 2023-06-26 09:32:28.000000 tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.5.0/LICENSE.txt` & `tracebloc_package-dev-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.0/PKG-INFO` & `tracebloc_package-dev-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.5.0
+Version: 0.5.1
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-dev-0.5.0/setup.py` & `tracebloc_package-dev-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.5.0",
+    version="0.5.1",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.5.0/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.5.1/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.0/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.5.1/tracebloc_package/functional_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,16 +447,15 @@
         try:
             self.is_model_supported()
             self.check_original_model_channels()
             self.layer_instance_check()
             self.small_training_loop()
             self.message = "all check passed"
         except Exception as e:  # pragma: no cover
-            if self.message == "":
-                self.message = f"Model checks failed with error as {e}"
+            self.message = f"\nModel checks failed with error as {e}"
             return False, self.message
         return True, self.message
 
     def model_func_checks(self):
         # check if model is eligible
         eligible, message = self.is_model_eligible()
         if not eligible:
@@ -609,12 +608,12 @@
             self.progress_bar.update(2)
             self.small_training_loop()
             self.average_weights()
             self.load_averaged_weights()
             self.message = "all check passed"
             eligible = True
         except Exception as e:  # pragma: no cover
-            self.message = f"Model checks failed with error as {e}"
+            self.message = f"\nModel checks failed with error as {e}"
             eligible = False
         if not eligible:
             return eligible, self.message, None, self.progress_bar  # pragma: no cover
         return eligible, self.message, self.model_name, self.progress_bar
```

### Comparing `tracebloc_package-dev-0.5.0/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.5.1/tracebloc_package/linkModelDataSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         self.__image_shape = image_size
         self.__image_type = "rgb"
         self.__optimizer = "sgd"
         self.__totalDatasetSize = totalDatasetSize
         self.__trainingDatasetSize = totalDatasetSize
         self.__trainingClasses = class_names
         self.__subdataset = {}
+        self.__images_per_edge = {}
         self.__lossFunction = {TYPE: STANDARD, VALUE: "mse"}
         self.__learningRate = {TYPE: CONSTANT, VALUE: 0.001}
         self.__seed = False
         self.__total_images = total_images
         self.__num_classes = num_classes
         self.__class_names = class_names
         self.__batchSize = self.__default_batchSize(batchsize)
@@ -229,15 +230,16 @@
             content = json.loads(body_unicode)
             if re.status_code == 200:
                 self.__total_images = content["total_images_per_edge"]
                 self.__validation_split = self.__default_validation_split()
                 self.__images_per_class = json.dumps(
                     training_dataset
                 )  # assign images count for sub-dataset
-            # else:
+                self.__images_per_edge = json.dumps(content["total_images_per_edge"])
+                # else:
             #     self.__print_error(content['message'])
 
     def __update_image_model(self):
         """
         change image type and size data as user choice in model file provided by user
         """
         header = {"Authorization": f"Token {self.__token}"}
@@ -1405,14 +1407,15 @@
             "name": self.__name,
             "modelType": self.__modelType,
             "category": self.__category,
             "upperboundTime": self.__upperboundTime,
             "callbacks": self.__callbacks,
             "pre_trained_weights": self.__weights,
             "subdataset": self.__subdataset,
+            "images_per_edge": self.__images_per_edge,
             "images_per_class": self.__images_per_class,
             "image_shape": self.__image_shape,
             "image_type": self.__image_type,
             "framework": self.__framework,
         }
 
         return parameters
```

### Comparing `tracebloc_package-dev-0.5.0/tracebloc_package/messages.py` & `tracebloc_package-dev-0.5.1/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.0/tracebloc_package/upload.py` & `tracebloc_package-dev-0.5.1/tracebloc_package/upload.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.0/tracebloc_package/user.py` & `tracebloc_package-dev-0.5.1/tracebloc_package/user.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.0/tracebloc_package/utils.py` & `tracebloc_package-dev-0.5.1/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.0/tracebloc_package/weights.py` & `tracebloc_package-dev-0.5.1/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.5.0
+Version: 0.5.1
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

