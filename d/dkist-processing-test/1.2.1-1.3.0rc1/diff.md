# Comparing `tmp/dkist-processing-test-1.2.1.tar.gz` & `tmp/dkist-processing-test-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-test-1.2.1.tar", last modified: Wed May 17 18:59:44 2023, max compression
+gzip compressed data, was "dkist-processing-test-1.3.0rc1.tar", last modified: Mon Jun 26 20:05:43 2023, max compression
```

## Comparing `dkist-processing-test-1.2.1.tar` & `dkist-processing-test-1.3.0rc1.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 18:59:44.749658 dkist-processing-test-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     2417 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1977 2023-05-17 18:59:44.749658 dkist-processing-test-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2334 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 18:59:44.745658 dkist-processing-test-1.2.1/dkist_processing_test/
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 18:59:44.745658 dkist-processing-test-1.2.1/dkist_processing_test/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/models/parameters.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 18:59:44.749658 dkist-processing-test-1.2.1/dkist_processing_test/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/tasks/exercise_numba.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/tasks/fail.py
--rw-rw-rw-   0 root         (0) root         (0)     2407 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/tasks/fake_science.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/tasks/movie.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/tasks/noop.py
--rw-rw-rw-   0 root         (0) root         (0)     2293 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/tasks/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 18:59:44.749658 dkist-processing-test-1.2.1/dkist_processing_test/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2411 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    13624 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/tests/test_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 18:59:44.749658 dkist-processing-test-1.2.1/dkist_processing_test/workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4418 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/workflows/common_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/workflows/end_to_end.py
--rw-rw-rw-   0 root         (0) root         (0)      362 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/workflows/exercise_numba.py
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/workflows/fail.py
--rw-rw-rw-   0 root         (0) root         (0)      676 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/dkist_processing_test/workflows/noop.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 18:59:44.745658 dkist-processing-test-1.2.1/dkist_processing_test.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1977 2023-05-17 18:59:44.000000 dkist-processing-test-1.2.1/dkist_processing_test.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-05-17 18:59:44.000000 dkist-processing-test-1.2.1/dkist_processing_test.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-17 18:59:44.000000 dkist-processing-test-1.2.1/dkist_processing_test.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-17 18:59:44.000000 dkist-processing-test-1.2.1/dkist_processing_test.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-17 18:59:44.000000 dkist-processing-test-1.2.1/dkist_processing_test.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-05-17 18:59:44.749658 dkist-processing-test-1.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-05-17 18:59:36.000000 dkist-processing-test-1.2.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 20:05:43.465725 dkist-processing-test-1.3.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2417 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2023-06-26 20:05:43.465725 dkist-processing-test-1.3.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 20:05:43.461725 dkist-processing-test-1.3.0rc1/dkist_processing_test/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 20:05:43.465725 dkist-processing-test-1.3.0rc1/dkist_processing_test/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/models/parameters.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 20:05:43.465725 dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/exercise_numba.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/fail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3459 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/fake_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/movie.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/noop.py
+-rw-rw-rw-   0 root         (0) root         (0)     2293 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 20:05:43.465725 dkist-processing-test-1.3.0rc1/dkist_processing_test/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2411 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    16665 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/tests/test_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 20:05:43.465725 dkist-processing-test-1.3.0rc1/dkist_processing_test/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5060 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/workflows/common_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/workflows/end_to_end.py
+-rw-rw-rw-   0 root         (0) root         (0)      362 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/workflows/exercise_numba.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/workflows/fail.py
+-rw-rw-rw-   0 root         (0) root         (0)      676 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/workflows/noop.py
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test/workflows/trial_end_to_end.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 20:05:43.461725 dkist-processing-test-1.3.0rc1/dkist_processing_test.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2023-06-26 20:05:43.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-06-26 20:05:43.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-26 20:05:43.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-06-26 20:05:43.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-26 20:05:43.000000 dkist-processing-test-1.3.0rc1/dkist_processing_test.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-06-26 20:05:43.469725 dkist-processing-test-1.3.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-26 20:05:36.000000 dkist-processing-test-1.3.0rc1/setup.py
```

### Comparing `dkist-processing-test-1.2.1/.gitignore` & `dkist-processing-test-1.3.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.2.1/.pre-commit-config.yaml` & `dkist-processing-test-1.3.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.2.1/PKG-INFO` & `dkist-processing-test-1.3.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-test
-Version: 1.2.1
+Version: 1.3.0rc1
 Summary: Example Instrument code that is used by the DKIST Science Data Processing pipelines to test processing infrastructure.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-test/src/main/
 Author: NSO / AURA
 Author-email: dkistdc@nso.edu
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-processing-test-1.2.1/README.rst` & `dkist-processing-test-1.3.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.2.1/bitbucket-pipelines.yml` & `dkist-processing-test-1.3.0rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.2.1/dkist_processing_test/models/parameters.py` & `dkist-processing-test-1.3.0rc1/dkist_processing_test/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.2.1/dkist_processing_test/tasks/exercise_numba.py` & `dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/exercise_numba.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.2.1/dkist_processing_test/tasks/fake_science.py` & `dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/fake_science.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Fake science task
 """
 import numpy as np
 from astropy.io import fits
+from dkist_processing_common.codecs.fits import fits_array_encoder
+from dkist_processing_common.codecs.json import json_encoder
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tasks import WorkflowTaskBase
 from dkist_processing_common.tasks.mixin.fits import FitsDataMixin
 from dkist_processing_common.tasks.mixin.input_dataset import InputDatasetMixin
 
 from dkist_processing_test.models.parameters import TestParameters
 
@@ -26,17 +28,39 @@
             workflow_name=workflow_name,
             workflow_version=workflow_version,
         )
         self.parameters = TestParameters(self.input_dataset_parameters)
 
     def run(self):
         rng = np.random.default_rng()
-        count = 1  # keep a running count to increment the dsps repeat number
-        with self.apm_task_step("Looping over inputs"):
-            for path, hdu in self.fits_data_read_hdu(tags=Tag.input()):
+        with self.apm_task_step("Create debug frame"):
+            self.write(
+                data=np.arange(10), tags=[Tag.frame(), Tag.debug()], encoder=fits_array_encoder
+            )
+
+        with self.apm_task_step("Creating intermediate frame"):
+            self.write(
+                data=np.arange(5),
+                tags=[Tag.frame(), Tag.intermediate(), Tag.task("DUMMY")],
+                encoder=fits_array_encoder,
+            )
+
+        with self.apm_task_step("Creating unique frames"):
+            for _ in range(2):
+                self.write(data=np.arange(3), tags=["FOO", "BAR"], encoder=fits_array_encoder)
+
+            self.write(data={"test": "dictionary"}, tags=["BAZ"], encoder=json_encoder)
+
+        with self.apm_task_step("Creating frames that won't be used"):
+            self.write(data=b"123", tags=[Tag.intermediate(), Tag.task("NOT_USED")])
+            self.write(data=b"123", tags=["FOO"])
+
+        with self.apm_task_step("Loop over inputs"):
+            count = 1  # keep a running count to increment the dsps repeat number
+            for hdu in self.fits_data_read_hdu(tags=Tag.input()):
                 header = hdu.header
                 with self.apm_processing_step("Doing some calculations"):
                     header["DSPSNUM"] = count
                     data = hdu.data
 
                     # Just do some weird crap. We don't use the loaded random array directly so that we
                     # don't have to care that the shapes are the same as the "real" data.
```

### Comparing `dkist-processing-test-1.2.1/dkist_processing_test/tasks/movie.py` & `dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/movie.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Take each output frame, copy the header and data and write out
     as a movie frame
     """
 
     def run(self):
         for d in range(1, self.constants.num_dsps_repeats + 1):
             with self.apm_task_step(f"Workign on dsps repeat {d}"):
-                for path, hdu in self.fits_data_read_hdu(tags=[Tag.output(), Tag.dsps_repeat(d)]):
+                for hdu in self.fits_data_read_hdu(tags=[Tag.output(), Tag.dsps_repeat(d)]):
                     header = hdu.header
                     data = hdu.data
                     output_hdu = fits.PrimaryHDU(data=data, header=header)
                     output_hdul = fits.HDUList([output_hdu])
 
                     with self.apm_writing_step("Writing data"):
                         self.fits_data_write(
```

### Comparing `dkist-processing-test-1.2.1/dkist_processing_test/tasks/parse.py` & `dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.2.1/dkist_processing_test/tasks/write_l1.py` & `dkist-processing-test-1.3.0rc1/dkist_processing_test/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.2.1/dkist_processing_test/tests/conftest.py` & `dkist-processing-test-1.3.0rc1/dkist_processing_test/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.2.1/dkist_processing_test/tests/test_parameters.py` & `dkist-processing-test-1.3.0rc1/dkist_processing_test/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.2.1/dkist_processing_test/tests/test_tasks.py` & `dkist-processing-test-1.3.0rc1/dkist_processing_test/tests/test_tasks.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import json
 import logging
 from dataclasses import asdict
 from dataclasses import dataclass
 from datetime import datetime
 from random import randint
+from uuid import uuid4
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from dkist_data_simulator.spec122 import Spec122Dataset
 from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
@@ -20,14 +21,15 @@
 from dkist_processing_test.models.parameters import TestParameters
 from dkist_processing_test.tasks.exercise_numba import ExerciseNumba
 from dkist_processing_test.tasks.fail import FailTask
 from dkist_processing_test.tasks.fake_science import GenerateCalibratedData
 from dkist_processing_test.tasks.movie import AssembleTestMovie
 from dkist_processing_test.tasks.movie import MakeTestMovieFrames
 from dkist_processing_test.tasks.noop import NoOpTask
+from dkist_processing_test.tasks.trial_output_data import TransferTestTrialData
 from dkist_processing_test.tasks.write_l1 import WriteL1Data
 from dkist_processing_test.tests.conftest import generate_214_l0_fits_frame
 from dkist_processing_test.tests.conftest import S122Headers
 
 
 @dataclass
 class FakeConstantDb:
@@ -169,14 +171,19 @@
     calibrated_frame_paths = list(task.read(tags=[Tag.calibrated(), Tag.frame()]))
 
     # Verify frames
     assert len(calibrated_frame_paths) == number_of_frames
     for filepath in calibrated_frame_paths:
         assert filepath.exists()
 
+    # Verify debug frame was written
+    debug_frame_paths = list(task.read(tags=[Tag.debug(), Tag.frame()]))
+    assert len(debug_frame_paths) == 1
+    assert debug_frame_paths[0].exists()
+
 
 class CommonDataset(Spec122Dataset):
     def __init__(self):
         super().__init__(
             array_shape=(1, 10, 10),
             time_delta=1,
             dataset_shape=(2, 10, 10),
@@ -381,14 +388,94 @@
     task()
     movie_file = list(task.read(tags=[Tag.movie()]))
     logging.info(f"{movie_file=}")
     assert len(movie_file) == 1
     assert movie_file[0].exists()
 
 
+@pytest.fixture
+def trial_output_task(recipe_run_id, tmp_path, mocker):
+    mocker.patch(
+        "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient",
+        new=FakeGQLClient,
+    )
+    proposal_id = "test_proposal_id"
+    with TransferTestTrialData(
+        recipe_run_id=recipe_run_id,
+        workflow_name="workflow_name",
+        workflow_version="workflow_version",
+    ) as task:
+        task.scratch = WorkflowFileSystem(
+            recipe_run_id=recipe_run_id,
+            scratch_base_path=tmp_path,
+        )
+        task.constants._update({"PROPOSAL_ID": proposal_id})
+
+        file_count = 0
+        # Write a debug frame
+        debug_file_obj = uuid4().hex.encode("utf8")
+        task.write(debug_file_obj, tags=[Tag.debug(), Tag.frame()])
+        file_count += 1
+
+        # Write an intermediate frame that we want to transfer
+        intermediate_keep_file_obj = uuid4().hex.encode("utf8")
+        task.write(
+            intermediate_keep_file_obj,
+            tags=[Tag.intermediate(), Tag.frame(), Tag.task("DUMMY")],
+        )
+        file_count += 1
+
+        # Write an intermediate frame that we don't want to transfer
+        intermediate_discard_file_obj = uuid4().hex.encode("utf8")
+        task.write(
+            intermediate_discard_file_obj,
+            tags=[Tag.intermediate(), Tag.frame(), Tag.task("WHO_CARES")],
+        )
+
+        # An output frame
+        output_file_obj = uuid4().hex.encode("utf8")
+        task.write(output_file_obj, tags=[Tag.output(), Tag.frame()])
+        file_count += 1
+
+        # Specifically tagged files
+        task.write(uuid4().hex.encode("utf8"), tags=[Tag.frame(), "FOO", "BAR"])
+        file_count += 1
+        task.write(uuid4().hex.encode("utf8"), tags=[Tag.frame(), "BAZ"])
+        file_count += 1
+
+        # This one won't get transferred
+        task.write(uuid4().hex.encode("utf8"), tags=[Tag.frame(), "FOO"])
+
+        yield task, file_count
+        task.scratch.purge()
+        task.constants._purge()
+
+
+def test_transfer_test_trial_data(trial_output_task, mocker):
+    """
+    Given: A TransferTestTrialData task with associated frames
+    When: Running the task and building the transfer list
+    Then: No errors occur and the transfer list has the correct number of items
+    """
+    task, expected_num_items = trial_output_task
+
+    mocker.patch(
+        "dkist_processing_common.tasks.mixin.globus.GlobusMixin.globus_transfer_scratch_to_object_store"
+    )
+    mocker.patch(
+        "dkist_processing_test.tasks.trial_output_data.TransferTestTrialData.remove_folder_objects"
+    )
+
+    # Just make sure the thing runs with no errors
+    task()
+
+    transfer_list = task.build_transfer_list()
+    assert len(transfer_list) == expected_num_items
+
+
 @pytest.fixture()
 def exercise_numba_task(recipe_run_id):
     with ExerciseNumba(
         recipe_run_id=recipe_run_id, workflow_name="ExerciseNumba", workflow_version="VX.Y"
     ) as task:
         yield task
```

### Comparing `dkist-processing-test-1.2.1/dkist_processing_test/workflows/common_tasks.py` & `dkist-processing-test-1.3.0rc1/dkist_processing_test/workflows/common_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 """
 from dkist_processing_common.tasks import AddDatasetReceiptAccount
 from dkist_processing_common.tasks import PublishCatalogAndQualityMessages
 from dkist_processing_common.tasks import QualityL1Metrics
 from dkist_processing_common.tasks import Teardown
 from dkist_processing_common.tasks import TransferL0Data
 from dkist_processing_common.tasks import TransferL1Data
+from dkist_processing_common.tasks import TrialTeardown
 from dkist_processing_core import Workflow
 
 from dkist_processing_test.tasks.fake_science import GenerateCalibratedData
 from dkist_processing_test.tasks.movie import AssembleTestMovie
 from dkist_processing_test.tasks.movie import MakeTestMovieFrames
 from dkist_processing_test.tasks.parse import ParseL0TestInputData
 from dkist_processing_test.tasks.quality import TestQualityL0Metrics
 from dkist_processing_test.tasks.quality import TestSubmitQuality
+from dkist_processing_test.tasks.trial_output_data import TransferTestTrialData
 from dkist_processing_test.tasks.write_l1 import WriteL1Data
 
 # TransferInputData Task
 transfer_input_data = Workflow(
     input_data="input",
     output_data="output",
     category="test",
@@ -113,14 +115,24 @@
     output_data="output",
     category="test",
     detail="transfer-output-data",
     workflow_package=__package__,
 )
 transfer_output_data.add_node(task=TransferL1Data, upstreams=None)
 
+# TransferTrialData Task
+transfer_trial_data = Workflow(
+    input_data="input",
+    output_data="output",
+    category="test",
+    detail="transfer-trial-data",
+    workflow_package=__package__,
+)
+transfer_trial_data.add_node(task=TransferTestTrialData, upstreams=None)
+
 # AddDatasetReceiptAccount Task
 add_dataset_receipt_account = Workflow(
     input_data="input",
     output_data="output",
     category="test",
     detail="add-dataset-receipt-account",
     workflow_package=__package__,
@@ -142,7 +154,17 @@
     input_data="input",
     output_data="output",
     category="test",
     detail="teardown",
     workflow_package=__package__,
 )
 teardown.add_node(task=Teardown, upstreams=None)
+
+# Trial Teardown Task
+teardown = Workflow(
+    input_data="input",
+    output_data="output",
+    category="test",
+    detail="trial-teardown",
+    workflow_package=__package__,
+)
+teardown.add_node(task=TrialTeardown, upstreams=None)
```

### Comparing `dkist-processing-test-1.2.1/dkist_processing_test/workflows/end_to_end.py` & `dkist-processing-test-1.3.0rc1/dkist_processing_test/workflows/end_to_end.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.2.1/dkist_processing_test/workflows/noop.py` & `dkist-processing-test-1.3.0rc1/dkist_processing_test/workflows/noop.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.2.1/dkist_processing_test.egg-info/PKG-INFO` & `dkist-processing-test-1.3.0rc1/dkist_processing_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-test
-Version: 1.2.1
+Version: 1.3.0rc1
 Summary: Example Instrument code that is used by the DKIST Science Data Processing pipelines to test processing infrastructure.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-test/src/main/
 Author: NSO / AURA
 Author-email: dkistdc@nso.edu
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-processing-test-1.2.1/dkist_processing_test.egg-info/SOURCES.txt` & `dkist-processing-test-1.3.0rc1/dkist_processing_test.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 dkist_processing_test/tasks/exercise_numba.py
 dkist_processing_test/tasks/fail.py
 dkist_processing_test/tasks/fake_science.py
 dkist_processing_test/tasks/movie.py
 dkist_processing_test/tasks/noop.py
 dkist_processing_test/tasks/parse.py
 dkist_processing_test/tasks/quality.py
+dkist_processing_test/tasks/trial_output_data.py
 dkist_processing_test/tasks/write_l1.py
 dkist_processing_test/tests/__init__.py
 dkist_processing_test/tests/conftest.py
 dkist_processing_test/tests/test_parameters.py
 dkist_processing_test/tests/test_tasks.py
 dkist_processing_test/tests/test_workflows.py
 dkist_processing_test/workflows/__init__.py
 dkist_processing_test/workflows/common_tasks.py
 dkist_processing_test/workflows/end_to_end.py
 dkist_processing_test/workflows/exercise_numba.py
 dkist_processing_test/workflows/fail.py
-dkist_processing_test/workflows/noop.py
+dkist_processing_test/workflows/noop.py
+dkist_processing_test/workflows/trial_end_to_end.py
```

### Comparing `dkist-processing-test-1.2.1/setup.cfg` & `dkist-processing-test-1.3.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 [options]
 python_requires = >=3.10
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 2.7.0
+	dkist-processing-common == 3.0.0rc9
 	dkist-header-validator == 3.0.5
 	dkist-fits-specifications == 3.6.0
 	numba == 0.56.0
 	astropy == 5.1.1
 	numpy == 1.22.4
 	dkist-spectral-lines == 1.0.0
```

