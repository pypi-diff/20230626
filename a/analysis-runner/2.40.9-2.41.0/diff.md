# Comparing `tmp/analysis-runner-2.40.9.tar.gz` & `tmp/analysis-runner-2.41.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysis-runner-2.40.9.tar", last modified: Fri Jun 23 06:40:32 2023, max compression
+gzip compressed data, was "analysis-runner-2.41.0.tar", last modified: Mon Jun 26 02:24:45 2023, max compression
```

## Comparing `analysis-runner-2.40.9.tar` & `analysis-runner-2.41.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:40:32.625113 analysis-runner-2.40.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-23 06:40:32.625113 analysis-runner-2.40.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:40:32.625113 analysis-runner-2.40.9/analysis_runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2125 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/cli_analysisrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/cli_cromwell.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    24334 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/cromwell.py
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/cromwell_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/dataproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:40:32.625113 analysis-runner-2.40.9/analysis_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-23 06:40:32.000000 analysis-runner-2.40.9/analysis_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-23 06:40:32.000000 analysis-runner-2.40.9/analysis_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 06:40:32.000000 analysis-runner-2.40.9/analysis_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 06:40:32.000000 analysis-runner-2.40.9/analysis_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 06:40:32.000000 analysis-runner-2.40.9/analysis_runner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 06:40:32.000000 analysis-runner-2.40.9/analysis_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 06:40:32.000000 analysis-runner-2.40.9/analysis_runner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 06:40:32.625113 analysis-runner-2.40.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:40:32.625113 analysis-runner-2.40.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/test/test_analysis_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:24:45.302737 analysis-runner-2.41.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-26 02:24:45.302737 analysis-runner-2.41.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:24:45.298737 analysis-runner-2.41.0/analysis_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/analysis_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/analysis_runner/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2125 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/analysis_runner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/analysis_runner/cli_analysisrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/analysis_runner/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/analysis_runner/cli_cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/analysis_runner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/analysis_runner/cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/analysis_runner/cromwell_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/analysis_runner/dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/analysis_runner/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/analysis_runner/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:24:45.302737 analysis-runner-2.41.0/analysis_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-26 02:24:45.000000 analysis-runner-2.41.0/analysis_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 02:24:45.000000 analysis-runner-2.41.0/analysis_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 02:24:45.000000 analysis-runner-2.41.0/analysis_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 02:24:45.000000 analysis-runner-2.41.0/analysis_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 02:24:45.000000 analysis-runner-2.41.0/analysis_runner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 02:24:45.000000 analysis-runner-2.41.0/analysis_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 02:24:45.000000 analysis-runner-2.41.0/analysis_runner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 02:24:45.302737 analysis-runner-2.41.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:24:45.302737 analysis-runner-2.41.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-26 02:24:42.000000 analysis-runner-2.41.0/test/test_analysis_runner.py
```

### Comparing `analysis-runner-2.40.9/LICENSE` & `analysis-runner-2.41.0/LICENSE`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.9/PKG-INFO` & `analysis-runner-2.41.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analysis-runner
-Version: 2.40.9
+Version: 2.41.0
 Summary: Analysis runner to help make analysis results reproducible
 Home-page: https://github.com/populationgenomics/analysis-runner
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `analysis-runner-2.40.9/README.md` & `analysis-runner-2.41.0/README.md`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.9/analysis_runner/cli.py` & `analysis-runner-2.41.0/analysis_runner/cli.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.9/analysis_runner/cli_analysisrunner.py` & `analysis-runner-2.41.0/analysis_runner/cli_analysisrunner.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.9/analysis_runner/cli_config.py` & `analysis-runner-2.41.0/analysis_runner/cli_config.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.9/analysis_runner/cli_cromwell.py` & `analysis-runner-2.41.0/analysis_runner/cli_cromwell.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.9/analysis_runner/constants.py` & `analysis-runner-2.41.0/analysis_runner/constants.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.9/analysis_runner/cromwell.py` & `analysis-runner-2.41.0/analysis_runner/cromwell.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,14 +128,15 @@
     cwd: Optional[str],
     libs: List[str],
     output_prefix: str,
     labels: Dict[str, str] = None,
     input_dict: Optional[Dict[str, Any]] = None,
     input_paths: List[str] = None,
     project: Optional[str] = None,
+    copy_outputs_to_gcp: bool = True,
 ):
     """
     Run a cromwell workflow, and return a Batch.ResourceFile
     that contains the workflow ID
     """
 
     def get_cromwell_key(dataset, access_level):
@@ -173,30 +174,36 @@
             _project = get_config()['workflow']['dataset_gcp_project']
         else:
             _project = get_project_id_from_service_account_email(service_account_email)
 
     if not service_account_email:
         raise ValueError("The service_account didn't contain an entry for client_email")
 
-    if access_level == 'test':
-        intermediate_dir = f'gs://cpg-{dataset}-test-tmp/cromwell'
-        workflow_output_dir = f'gs://cpg-{dataset}-test/{output_prefix}'
-    else:
-        intermediate_dir = f'gs://cpg-{dataset}-main-tmp/cromwell'
-        workflow_output_dir = f'gs://cpg-{dataset}-main/{output_prefix}'
+    # test/main should be implicit from the config
+    storage_config = get_config()['storage'][dataset]
+    intermediate_dir = os.path.join(storage_config['tmp'], 'cromwell')
+    workflow_output_dir = os.path.join(storage_config['default'], output_prefix)
+    logging_output_dir = os.path.join(
+        storage_config['analysis'], 'cromwell_logs', output_prefix
+    )
 
     workflow_options = {
         'user_service_account_json': service_account_json,
         'google_compute_service_account': service_account_email,
         'google_project': _project,
         'jes_gcs_root': intermediate_dir,
-        'final_workflow_outputs_dir': workflow_output_dir,
         'google_labels': google_labels,
+        'final_call_logs_dir': logging_output_dir,
+        'final_workflow_log_dir': logging_output_dir,
     }
 
+    # if required, export the workflow outputs to GCS
+    if copy_outputs_to_gcp:
+        workflow_options['final_workflow_outputs_dir'] = workflow_output_dir
+
     input_paths = input_paths or []
     if input_dict:
         tmp_input_json_path = '/tmp/inputs.json'
         job.command(f"echo '{json.dumps(input_dict)}' > {tmp_input_json_path}")
         input_paths.append(tmp_input_json_path)
 
     inputs_cli = []
@@ -242,14 +249,15 @@
     input_dict: Optional[Dict[str, Any]] = None,
     input_paths: List[str] = None,
     repo: Optional[str] = None,
     commit: Optional[str] = None,
     cwd: Optional[str] = None,
     driver_image: Optional[str] = None,
     project: Optional[str] = None,
+    copy_outputs_to_gcp: bool = True,
 ) -> tuple[Job, dict[str, Resource]]:
     """
     This function needs to know the structure of the outputs you
     want to collect. It currently only supports:
         - a single value, or
         - a list of values
 
@@ -257,14 +265,17 @@
         'hello.out': None, # single output
         'hello.outs': 5, # array output of length=5
     }
 
     If the starts with "gs://", we'll copy it as a resource file,
     otherwise write the value into a file which will be a batch resource.
 
+    If copy_outputs_to_gcp is True, the outputs will be copied to GCS.
+    Workflows may then choose to copy these outputs to a final destination.
+
     Returns a submit Job object, and a dict of output Resource objects.
     """
     _driver_image = driver_image or os.getenv('DRIVER_IMAGE')
 
     submit_job = b.new_job(f'{job_prefix}_submit')
     submit_job.image(_driver_image)
     prepare_git_job(
@@ -282,14 +293,15 @@
         cwd=cwd,
         libs=libs,
         output_prefix=output_prefix,
         input_dict=input_dict,
         input_paths=input_paths,
         labels=labels,
         project=project,
+        copy_outputs_to_gcp=copy_outputs_to_gcp,
     )
 
     outputs_dict = watch_workflow_and_get_output(
         b,
         job_prefix=job_prefix,
         workflow_id_file=workflow_id_file,
         outputs_to_collect=outputs_to_collect,
```

### Comparing `analysis-runner-2.40.9/analysis_runner/cromwell_model.py` & `analysis-runner-2.41.0/analysis_runner/cromwell_model.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.9/analysis_runner/dataproc.py` & `analysis-runner-2.41.0/analysis_runner/dataproc.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.9/analysis_runner/git.py` & `analysis-runner-2.41.0/analysis_runner/git.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.9/analysis_runner/util.py` & `analysis-runner-2.41.0/analysis_runner/util.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.9/analysis_runner.egg-info/PKG-INFO` & `analysis-runner-2.41.0/analysis_runner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analysis-runner
-Version: 2.40.9
+Version: 2.41.0
 Summary: Analysis runner to help make analysis results reproducible
 Home-page: https://github.com/populationgenomics/analysis-runner
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `analysis-runner-2.40.9/analysis_runner.egg-info/SOURCES.txt` & `analysis-runner-2.41.0/analysis_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.9/setup.py` & `analysis-runner-2.41.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     with open(filename, encoding='utf-8') as f:
         return f.read()
 
 
 setuptools.setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='2.40.9',
+    version='2.41.0',
     description='Analysis runner to help make analysis results reproducible',
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/{PKG}',
     license='MIT',
     packages=['analysis_runner'],
     include_package_data=True,
```

### Comparing `analysis-runner-2.40.9/test/test_analysis_runner.py` & `analysis-runner-2.41.0/test/test_analysis_runner.py`

 * *Files identical despite different names*

