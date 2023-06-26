# Comparing `tmp/superpoint_superglue_deployment-0.0.2.tar.gz` & `tmp/superpoint_superglue_deployment-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpoint_superglue_deployment-0.0.2.tar", last modified: Sat Jun 24 17:15:53 2023, max compression
+gzip compressed data, was "superpoint_superglue_deployment-0.0.3.tar", last modified: Mon Jun 26 14:46:19 2023, max compression
```

## Comparing `superpoint_superglue_deployment-0.0.2.tar` & `superpoint_superglue_deployment-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:15:53.674005 superpoint_superglue_deployment-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-24 17:15:49.000000 superpoint_superglue_deployment-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-24 17:15:53.674005 superpoint_superglue_deployment-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-24 17:15:49.000000 superpoint_superglue_deployment-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-24 17:15:49.000000 superpoint_superglue_deployment-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-24 17:15:49.000000 superpoint_superglue_deployment-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-24 17:15:53.674005 superpoint_superglue_deployment-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-24 17:15:49.000000 superpoint_superglue_deployment-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:15:53.674005 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-24 17:15:49.000000 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:15:53.674005 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/core/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-24 17:15:49.000000 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-24 17:15:49.000000 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-24 17:15:49.000000 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-06-24 17:15:49.000000 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/superglue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-24 17:15:49.000000 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/superglue_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-06-24 17:15:49.000000 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/superpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-24 17:15:49.000000 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/superpoint_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-24 17:15:49.000000 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:15:53.674005 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-24 17:15:53.000000 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-24 17:15:53.000000 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 17:15:53.000000 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-24 17:15:53.000000 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 17:15:53.000000 superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:46:19.279251 superpoint_superglue_deployment-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-26 14:46:19.279251 superpoint_superglue_deployment-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 14:46:19.279251 superpoint_superglue_deployment-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:46:19.279251 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:46:19.279251 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/superglue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/superglue_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/superpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/superpoint_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 14:46:14.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:46:19.279251 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-26 14:46:19.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-26 14:46:19.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:46:19.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 14:46:19.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 14:46:19.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 14:46:19.000000 superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment.egg-info/top_level.txt
```

### Comparing `superpoint_superglue_deployment-0.0.2/PKG-INFO` & `superpoint_superglue_deployment-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpoint_superglue_deployment
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/xmba15/superpoint_superglue_deployment
 Author: Ba Tran
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -101,14 +101,20 @@
 <p align="center">
   <img src="https://raw.githubusercontent.com/xmba15/superpoint_superglue_deployment/master/docs/images/matched_image.jpg" alt="matched image sample">
 </p>
 
 - [Notebook with detailed sample code for SuperPoint](notebooks/demo_superpoint.ipynb)
 - [Notebook with detailed sample code for SuperGlue](notebooks/demo_superglue.ipynb)
 
+- Command line to test matching two images after installing the library
+
+```bash
+match_two_images --query_path [path/to/query/image] --ref_path [path/to/reference/image] --use_gpu
+```
+
 ## 🎛 Development environment
 
 ---
 
 ```bash
 mamba env create --file environment.yml
 mamba activate superpoint_superglue_deployment
```

### Comparing `superpoint_superglue_deployment-0.0.2/README.md` & `superpoint_superglue_deployment-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,20 @@
 <p align="center">
   <img src="https://raw.githubusercontent.com/xmba15/superpoint_superglue_deployment/master/docs/images/matched_image.jpg" alt="matched image sample">
 </p>
 
 - [Notebook with detailed sample code for SuperPoint](notebooks/demo_superpoint.ipynb)
 - [Notebook with detailed sample code for SuperGlue](notebooks/demo_superglue.ipynb)
 
+- Command line to test matching two images after installing the library
+
+```bash
+match_two_images --query_path [path/to/query/image] --ref_path [path/to/reference/image] --use_gpu
+```
+
 ## 🎛 Development environment
 
 ---
 
 ```bash
 mamba env create --file environment.yml
 mamba activate superpoint_superglue_deployment
```

### Comparing `superpoint_superglue_deployment-0.0.2/setup.py` & `superpoint_superglue_deployment-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,12 +31,17 @@
             "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
         ],
         packages=find_packages(exclude=["tests"]),
         install_requires=_INSTALL_REQUIRES,
+        entry_points={
+            "console_scripts": [
+                "match_two_images=superpoint_superglue_deployment.__main__:main",
+            ]
+        },
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/matcher.py` & `superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/matcher.py`

 * *Files identical despite different names*

### Comparing `superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/superglue.py` & `superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/superglue.py`

 * *Files identical despite different names*

### Comparing `superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/superglue_handler.py` & `superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/superglue_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,27 +110,31 @@
     def match(
         self,
         query_pred: Dict[str, torch.Tensor],
         ref_pred: Dict[str, torch.Tensor],
         query_shape: Tuple[int, int],
         ref_shape: Tuple[int, int],
     ) -> List[cv2.DMatch]:
+        num_query_kpts = query_pred["keypoints"][0].size()[0]
+        num_ref_kpts = ref_pred["keypoints"][0].size()[0]
         pred = self.run(
             query_pred,
             ref_pred,
             query_shape,
             ref_shape,
         )
-        query_indices = pred["matches0"].cpu().numpy().squeeze(0)
-        ref_indices = pred["matches1"].cpu().numpy().squeeze(0)
+        matches0_to_1 = pred["matches0"].cpu().numpy().squeeze(0)
         query_matching_scores = pred["matching_scores0"].cpu().numpy().squeeze(0)
+        valid = matches0_to_1 > -1
 
         del pred
-        matched_query_indices = np.where(query_indices > -1)[0]
-        matched_ref_indices = np.where(ref_indices > -1)[0]
+
+        matched_query_indices = np.arange(num_query_kpts)[valid]
+        matched_ref_indices = np.arange(num_ref_kpts)[matches0_to_1[valid]]
+
         matches = [
             cv2.DMatch(
                 _distance=1 - query_matching_scores[matched_query_idx],
                 _queryIdx=matched_query_idx,
                 _trainIdx=matched_ref_idx,
             )
             for matched_query_idx, matched_ref_idx in zip(matched_query_indices, matched_ref_indices)
```

### Comparing `superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/superpoint.py` & `superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/superpoint.py`

 * *Files identical despite different names*

### Comparing `superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment/superpoint_handler.py` & `superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment/superpoint_handler.py`

 * *Files identical despite different names*

### Comparing `superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment.egg-info/PKG-INFO` & `superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpoint-superglue-deployment
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/xmba15/superpoint_superglue_deployment
 Author: Ba Tran
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -101,14 +101,20 @@
 <p align="center">
   <img src="https://raw.githubusercontent.com/xmba15/superpoint_superglue_deployment/master/docs/images/matched_image.jpg" alt="matched image sample">
 </p>
 
 - [Notebook with detailed sample code for SuperPoint](notebooks/demo_superpoint.ipynb)
 - [Notebook with detailed sample code for SuperGlue](notebooks/demo_superglue.ipynb)
 
+- Command line to test matching two images after installing the library
+
+```bash
+match_two_images --query_path [path/to/query/image] --ref_path [path/to/reference/image] --use_gpu
+```
+
 ## 🎛 Development environment
 
 ---
 
 ```bash
 mamba env create --file environment.yml
 mamba activate superpoint_superglue_deployment
```

### Comparing `superpoint_superglue_deployment-0.0.2/superpoint_superglue_deployment.egg-info/SOURCES.txt` & `superpoint_superglue_deployment-0.0.3/superpoint_superglue_deployment.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 superpoint_superglue_deployment/__init__.py
+superpoint_superglue_deployment/__main__.py
 superpoint_superglue_deployment/matcher.py
 superpoint_superglue_deployment/superglue.py
 superpoint_superglue_deployment/superglue_handler.py
 superpoint_superglue_deployment/superpoint.py
 superpoint_superglue_deployment/superpoint_handler.py
 superpoint_superglue_deployment/version.py
 superpoint_superglue_deployment.egg-info/PKG-INFO
 superpoint_superglue_deployment.egg-info/SOURCES.txt
 superpoint_superglue_deployment.egg-info/dependency_links.txt
+superpoint_superglue_deployment.egg-info/entry_points.txt
 superpoint_superglue_deployment.egg-info/requires.txt
 superpoint_superglue_deployment.egg-info/top_level.txt
 superpoint_superglue_deployment/core/__init__.py
 superpoint_superglue_deployment/core/utils.py
```

