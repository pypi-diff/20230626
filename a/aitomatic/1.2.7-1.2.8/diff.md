# Comparing `tmp/aitomatic-1.2.7.tar.gz` & `tmp/aitomatic-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aitomatic-1.2.7.tar", last modified: Tue May 23 00:25:13 2023, max compression
+gzip compressed data, was "aitomatic-1.2.8.tar", last modified: Mon Jun 26 07:26:32 2023, max compression
```

## Comparing `aitomatic-1.2.7.tar` & `aitomatic-1.2.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-23 00:25:13.231569 aitomatic-1.2.7/
--rw-r--r--   0 hungvo     (501) staff       (20)     1065 2023-02-15 03:11:17.000000 aitomatic-1.2.7/LICENSE
--rw-r--r--   0 hungvo     (501) staff       (20)       36 2023-02-24 03:49:01.000000 aitomatic-1.2.7/MANIFEST.in
--rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-05-23 00:25:13.232165 aitomatic-1.2.7/PKG-INFO
--rw-r--r--   0 hungvo     (501) staff       (20)     4051 2023-05-08 07:01:50.000000 aitomatic-1.2.7/README.md
--rw-r--r--   0 hungvo     (501) staff       (20)       85 2023-02-15 03:11:17.000000 aitomatic-1.2.7/pyproject.toml
--rw-r--r--   0 hungvo     (501) staff       (20)       87 2023-05-08 07:01:50.000000 aitomatic-1.2.7/requirements.txt
--rw-r--r--   0 hungvo     (501) staff       (20)      714 2023-05-23 00:25:13.233625 aitomatic-1.2.7/setup.cfg
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-23 00:25:13.175027 aitomatic-1.2.7/src/
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-23 00:25:13.186465 aitomatic-1.2.7/src/aitomatic/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.2.7/src/aitomatic/__init__.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-23 00:25:13.209156 aitomatic-1.2.7/src/aitomatic/api/
--rw-r--r--   0 hungvo     (501) staff       (20)     1203 2023-05-04 14:19:17.000000 aitomatic-1.2.7/src/aitomatic/api/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)     8726 2023-05-23 00:24:16.000000 aitomatic-1.2.7/src/aitomatic/api/build.py
--rw-r--r--   0 hungvo     (501) staff       (20)     6120 2023-05-04 14:19:17.000000 aitomatic-1.2.7/src/aitomatic/api/client.py
--rw-r--r--   0 hungvo     (501) staff       (20)       54 2023-02-24 03:49:01.000000 aitomatic-1.2.7/src/aitomatic/api/exceptions.py
--rw-r--r--   0 hungvo     (501) staff       (20)     7673 2023-05-04 14:19:17.000000 aitomatic-1.2.7/src/aitomatic/api/model_params.py
--rw-r--r--   0 hungvo     (501) staff       (20)     4333 2023-05-04 14:19:17.000000 aitomatic-1.2.7/src/aitomatic/api/tuning_utils.py
--rw-r--r--   0 hungvo     (501) staff       (20)    15755 2023-05-16 01:46:06.000000 aitomatic-1.2.7/src/aitomatic/api/web_model.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-23 00:25:13.222824 aitomatic-1.2.7/src/aitomatic/dsl/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.2.7/src/aitomatic/dsl/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3778 2023-02-24 03:49:01.000000 aitomatic-1.2.7/src/aitomatic/dsl/arl_conclusions.py
--rw-r--r--   0 hungvo     (501) staff       (20)     8933 2023-02-24 03:49:01.000000 aitomatic-1.2.7/src/aitomatic/dsl/arl_features.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3690 2023-05-04 14:19:17.000000 aitomatic-1.2.7/src/aitomatic/dsl/arl_handler.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3463 2023-02-24 03:49:01.000000 aitomatic-1.2.7/src/aitomatic/dsl/arl_rules.py
--rw-r--r--   0 hungvo     (501) staff       (20)     1040 2023-05-16 01:46:06.000000 aitomatic-1.2.7/src/aitomatic/dsl/utils.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-23 00:25:13.228942 aitomatic-1.2.7/src/aitomatic/objects/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-04-25 08:41:40.000000 aitomatic-1.2.7/src/aitomatic/objects/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)      531 2023-05-04 14:19:17.000000 aitomatic-1.2.7/src/aitomatic/objects/dataset.py
--rw-r--r--   0 hungvo     (501) staff       (20)     1563 2023-05-04 14:19:17.000000 aitomatic-1.2.7/src/aitomatic/objects/model.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-05-23 00:25:13.191145 aitomatic-1.2.7/src/aitomatic.egg-info/
--rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-05-23 00:25:13.000000 aitomatic-1.2.7/src/aitomatic.egg-info/PKG-INFO
--rw-r--r--   0 hungvo     (501) staff       (20)      799 2023-05-23 00:25:13.000000 aitomatic-1.2.7/src/aitomatic.egg-info/SOURCES.txt
--rw-r--r--   0 hungvo     (501) staff       (20)        1 2023-05-23 00:25:13.000000 aitomatic-1.2.7/src/aitomatic.egg-info/dependency_links.txt
--rw-r--r--   0 hungvo     (501) staff       (20)       78 2023-05-23 00:25:13.000000 aitomatic-1.2.7/src/aitomatic.egg-info/requires.txt
--rw-r--r--   0 hungvo     (501) staff       (20)       10 2023-05-23 00:25:13.000000 aitomatic-1.2.7/src/aitomatic.egg-info/top_level.txt
--rw-r--r--   0 hungvo     (501) staff       (20)        6 2023-05-23 00:24:58.000000 aitomatic-1.2.7/version.txt
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-26 07:26:32.383148 aitomatic-1.2.8/
+-rw-r--r--   0 hungvo     (501) staff       (20)     1065 2023-02-15 03:11:17.000000 aitomatic-1.2.8/LICENSE
+-rw-r--r--   0 hungvo     (501) staff       (20)       36 2023-02-24 03:49:01.000000 aitomatic-1.2.8/MANIFEST.in
+-rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-06-26 07:26:32.383542 aitomatic-1.2.8/PKG-INFO
+-rw-r--r--   0 hungvo     (501) staff       (20)     4051 2023-05-08 07:01:50.000000 aitomatic-1.2.8/README.md
+-rw-r--r--   0 hungvo     (501) staff       (20)       85 2023-02-15 03:11:17.000000 aitomatic-1.2.8/pyproject.toml
+-rw-r--r--   0 hungvo     (501) staff       (20)       87 2023-05-08 07:01:50.000000 aitomatic-1.2.8/requirements.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)      714 2023-06-26 07:26:32.384819 aitomatic-1.2.8/setup.cfg
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-26 07:26:32.356311 aitomatic-1.2.8/src/
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-26 07:26:32.364301 aitomatic-1.2.8/src/aitomatic/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.2.8/src/aitomatic/__init__.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-26 07:26:32.375019 aitomatic-1.2.8/src/aitomatic/api/
+-rw-r--r--   0 hungvo     (501) staff       (20)     1203 2023-05-04 14:19:17.000000 aitomatic-1.2.8/src/aitomatic/api/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     8843 2023-06-26 07:24:53.000000 aitomatic-1.2.8/src/aitomatic/api/build.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     6120 2023-05-04 14:19:17.000000 aitomatic-1.2.8/src/aitomatic/api/client.py
+-rw-r--r--   0 hungvo     (501) staff       (20)       54 2023-02-24 03:49:01.000000 aitomatic-1.2.8/src/aitomatic/api/exceptions.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     7673 2023-05-04 14:19:17.000000 aitomatic-1.2.8/src/aitomatic/api/model_params.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     4333 2023-05-04 14:19:17.000000 aitomatic-1.2.8/src/aitomatic/api/tuning_utils.py
+-rw-r--r--   0 hungvo     (501) staff       (20)    15820 2023-06-26 07:24:20.000000 aitomatic-1.2.8/src/aitomatic/api/web_model.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-26 07:26:32.379384 aitomatic-1.2.8/src/aitomatic/dsl/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.2.8/src/aitomatic/dsl/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3778 2023-02-24 03:49:01.000000 aitomatic-1.2.8/src/aitomatic/dsl/arl_conclusions.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     8933 2023-02-24 03:49:01.000000 aitomatic-1.2.8/src/aitomatic/dsl/arl_features.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3690 2023-05-04 14:19:17.000000 aitomatic-1.2.8/src/aitomatic/dsl/arl_handler.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3463 2023-02-24 03:49:01.000000 aitomatic-1.2.8/src/aitomatic/dsl/arl_rules.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     1040 2023-05-16 01:46:06.000000 aitomatic-1.2.8/src/aitomatic/dsl/utils.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-26 07:26:32.382213 aitomatic-1.2.8/src/aitomatic/objects/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-04-25 08:41:40.000000 aitomatic-1.2.8/src/aitomatic/objects/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)      531 2023-05-04 14:19:17.000000 aitomatic-1.2.8/src/aitomatic/objects/dataset.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     1563 2023-05-04 14:19:17.000000 aitomatic-1.2.8/src/aitomatic/objects/model.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-26 07:26:32.367013 aitomatic-1.2.8/src/aitomatic.egg-info/
+-rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-06-26 07:26:32.000000 aitomatic-1.2.8/src/aitomatic.egg-info/PKG-INFO
+-rw-r--r--   0 hungvo     (501) staff       (20)      799 2023-06-26 07:26:32.000000 aitomatic-1.2.8/src/aitomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)        1 2023-06-26 07:26:32.000000 aitomatic-1.2.8/src/aitomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)       78 2023-06-26 07:26:32.000000 aitomatic-1.2.8/src/aitomatic.egg-info/requires.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)       10 2023-06-26 07:26:32.000000 aitomatic-1.2.8/src/aitomatic.egg-info/top_level.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)        6 2023-06-26 07:25:05.000000 aitomatic-1.2.8/version.txt
```

### Comparing `aitomatic-1.2.7/LICENSE` & `aitomatic-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.7/PKG-INFO` & `aitomatic-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitomatic
-Version: 1.2.7
+Version: 1.2.8
 Summary: aitomatic library to interact with Aitomatic product
 Home-page: https://github.com/aitomatic/aitomatic-cli
 Author: Pham Hoang Tuan
 Author-email: tuan@aitomatic.com
 Project-URL: Bug Tracker, https://github.com/aitomatic/aitomatic-cli/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aitomatic-1.2.7/README.md` & `aitomatic-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.7/setup.cfg` & `aitomatic-1.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.7/src/aitomatic/api/__init__.py` & `aitomatic-1.2.8/src/aitomatic/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.7/src/aitomatic/api/build.py` & `aitomatic-1.2.8/src/aitomatic/api/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,28 +161,34 @@
         try:
             model_info = self.project.get_model_info(model_name)
             return model_info.status.lower()
         except Exception as e:
             print("Checking model status, e =", e)
             return "training"
 
-    def wait_for_tuning_to_complete(self, model_df: pd.DataFrame, sleep_time: int = 30):
+    def wait_for_tuning_to_complete(
+        self,
+        model_df: pd.DataFrame,
+        file_path: str = "tuning.parquet",
+        sleep_time: int = 30,
+    ):
         print("Waiting for training jobs to complete")
         while True:
             for i, row in model_df.iterrows():
                 model_name = row["model_name"]
                 status = self.check_model_status(model_name)
                 model_df.loc[i, "status"] = status
 
             success_length = len(model_df[model_df["status"] == "success"])
             error_length = len(model_df[model_df["status"] == "error"])
             df_length = len(model_df)
             print(
                 f"Waiting for training jobs to complete: [{success_length} success, {error_length} error, {df_length} total]"
             )
+            model_df.to_parquet(file_path)
             if model_df["status"].isin(["training"]).any():
                 time.sleep(sleep_time)
             else:
                 break
         return model_df
 
     def get_metadata(seft, data: Dataset, mapping_column: dict):
```

### Comparing `aitomatic-1.2.7/src/aitomatic/api/client.py` & `aitomatic-1.2.8/src/aitomatic/api/client.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.7/src/aitomatic/api/model_params.py` & `aitomatic-1.2.8/src/aitomatic/api/model_params.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.7/src/aitomatic/api/tuning_utils.py` & `aitomatic-1.2.8/src/aitomatic/api/tuning_utils.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.7/src/aitomatic/api/web_model.py` & `aitomatic-1.2.8/src/aitomatic/api/web_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     Class for making inference calls with models served via the Aitomatic Wed API
 
     Ex:
     model = WebModel(API_TOKEN, "MyModelName").load_params()
     predictions = model.predict({'X': MyDataFrame})
     """
 
-    data_key = 'X'
-    output_key = 'predictions'
+    data_key = "X"
+    output_key = "predictions"
 
     def __init__(
         self,
         model_name: str,
         api_token: str = None,
         project_name: str = None,
         chunk_size: int = 1024,
@@ -41,44 +41,44 @@
         Initialize remote model
 
         :param api_token: Aitomatic API Access Token
         :param model_name: name of the model being used
         :param chunk_size: size to chunk inference calls in kb
         """
         if api_token is None:
-            api_token = os.getenv('AITOMATIC_API_TOKEN')
+            api_token = os.getenv("AITOMATIC_API_TOKEN")
 
         if project_name is None:
-            project_name = os.getenv('AITOMATIC_PROJECT_NAME')
-            project_id = os.getenv('AITOMATIC_PROJECT_ID')
+            project_name = os.getenv("AITOMATIC_PROJECT_NAME")
+            project_id = os.getenv("AITOMATIC_PROJECT_ID")
         else:
             project_id = get_project_id(project_name, api_token=api_token)
 
         self.project_name = project_name
         self.project_id = project_id
         self.model_name = model_name
         self.api_token = api_token
         self.chunk_size = chunk_size * 1024  # convert from kb to bytes
-        self.model_version = 'latest'
+        self.model_version = "latest"
         self.headers = {
-            'access-token': self.api_token,
-            'Content-Type': 'application/json',
-            'accept': 'application/json',
+            "access-token": self.api_token,
+            "Content-Type": "application/json",
+            "accept": "application/json",
         }
         self.init_endpoints()
 
     def init_endpoints(self):
         self.MODEL_API_ROOT, self.CLIENT_API_ROOT = get_api_root()
-        self.MODELS_ENDPOINT = f'{self.MODEL_API_ROOT}/models'
-        self.PREDICTION_ENDPOINT = f'{self.MODEL_API_ROOT}/inferencing'
-        self.METADATA_ENDPOINT = f'{self.MODELS_ENDPOINT}/metadata'
-        self.METRICS_ENDPOINT = f'{self.MODELS_ENDPOINT}/metrics'
+        self.MODELS_ENDPOINT = f"{self.MODEL_API_ROOT}/models"
+        self.PREDICTION_ENDPOINT = f"{self.MODEL_API_ROOT}/inferencing"
+        self.METADATA_ENDPOINT = f"{self.MODELS_ENDPOINT}/metadata"
+        self.METRICS_ENDPOINT = f"{self.MODELS_ENDPOINT}/metrics"
 
-        self.KNOWLEDGE_DETAIL = lambda id_: f'{self.CLIENT_API_ROOT}/knowledges/' + id_
-        self.DATA_DETAIL = lambda id_: f'{self.CLIENT_API_ROOT}/data/' + id_
+        self.KNOWLEDGE_DETAIL = lambda id_: f"{self.CLIENT_API_ROOT}/knowledges/" + id_
+        self.DATA_DETAIL = lambda id_: f"{self.CLIENT_API_ROOT}/data/" + id_
 
     def batch_predict(self, input_data: Dict) -> Dict:
         """
         Chunks data in input_data['X'] and does prediction in batches
         """
         # TODO: Make this more versatile to it slices all large data in input
         # data, not just 'X' ... maybe
@@ -88,16 +88,16 @@
         size = sys.getsizeof(X)
         items = self.count_items(X)
         chunk_max = self.chunk_size
         spi = size / items
         N = int(chunk_max / spi) - 1
         total_batches = int(np.ceil(items / N))
         logger.info(
-            f'data size too large. Running inference in chunks of '
-            f'{chunk_max /1024} kb or {N} data points'
+            f"data size too large. Running inference in chunks of "
+            f"{chunk_max /1024} kb or {N} data points"
         )
         out = []
         for Xi in tqdm(self.slice_data(X, N), total=total_batches):
             pred = self.predict({self.data_key: Xi, **Xother})[self.output_key]
             out.append(pred)
 
         predictions = self.merge_items(out, type(X))
@@ -114,21 +114,21 @@
         elif dtype == np.ndarray:
             return np.concatenate(items)
         elif dtype == list:
             return list(chain.from_iterable(items))
         elif dtype == pd.DataFrame or dtype == pd.Series:
             return pd.concat(items, axis=0)
         else:
-            raise NotImplementedError(f'Data type {str(type)} not supported')
+            raise NotImplementedError(f"Data type {str(type)} not supported")
 
     def count_items(self, X: Union[np.ndarray, pd.Series, pd.DataFrame, Dict, List]):
         """
         Count items in dataset
         """
-        if hasattr(X, 'shape'):
+        if hasattr(X, "shape"):
             return X.shape[0]
 
         return len(X)
 
     def slice_data(self, X, N):
         """
         Iterate over slices of data with pieces of size N
@@ -176,57 +176,57 @@
         # user the same input type that they put in
 
         # TODO: remove this, after resolving API input format
         types_dict[self.output_key] = type(input_data[self.data_key])
 
         # Create web request dicts
         request_data = {
-            'project_name': self.project_name,
-            'model_name': self.model_name,
-            'model_version': self.model_version,
-            'input_data': json_data,
+            "project_name": self.project_name,
+            "model_name": self.model_name,
+            "model_version": self.model_version,
+            "input_data": json_data,
         }
 
         # Convert data to json str (NpEncoder allows numpy array conversion)
         request_data = json.dumps(request_data, cls=NpEncoder)
 
         # Make web request
         resp = requests.post(
             self.PREDICTION_ENDPOINT, headers=self.headers, data=request_data
         )
 
         # Handle request errors
         if resp.status_code != 200:
-            err = f'{resp.status_code}: {resp.content}'
+            err = f"{resp.status_code}: {resp.content}"
             raise ConnectionError(err)
 
         resp_content = json.loads(resp.content)
         # resp_data = resp_content['result']
         resp_data = resp_content
-        result_file_path = resp_content['result_file_path']
+        result_file_path = resp_content["result_file_path"]
 
         # Convert response back to correct types
         # predictions format to match input_data['X'] format/types
-        predictions = convert_json_to_data(resp_data['result'], types_dict)
+        predictions = convert_json_to_data(resp_data["result"], types_dict)
 
         return predictions
 
     def process(self, input_data: Dict) -> Dict:
         """
         Implement logic to generate prediction from data
         """
         return self.predict(input_data=input_data)
 
     def persist(self, version: str) -> str:
         raise NotImplementedError()
 
-    def load_params(self, *args, **kwargs) -> 'WebModel':
+    def load_params(self, *args, **kwargs) -> "WebModel":
         return self.load(*args, **kwargs)
 
-    def load(self, version: str = 'latest') -> 'WebModel':
+    def load(self, version: str = "latest") -> "WebModel":
         """
         load model parameters for usage
 
         :param version: (optional) version of the model to load, defaults to
         latest
         """
         self.model_version = version
@@ -234,28 +234,28 @@
         # TODO: Make API call to get model stats & metrics, uncomment below
         # when API implemented
 
         resp = requests.get(
             self.METADATA_ENDPOINT,
             headers=self.headers,
             params={
-                'project_name': self.project_name,
-                'model_name': self.model_name,
-                'model_version': version,
+                "project_name": self.project_name,
+                "model_name": self.model_name,
+                "model_version": version,
             },
         )
 
         # Handle request errors
         if resp.status_code != 200:
-            err = f'{resp.status_code}: {resp.content}'
+            err = f"{resp.status_code}: {resp.content}"
             raise ConnectionError(err)
 
         resp_data = json.loads(resp.content)
-        self.stats = resp_data['result']['stats']
-        self.metrics = resp_data['result']['metrics']
+        self.stats = resp_data["result"]["stats"]
+        self.metrics = resp_data["result"]["metrics"]
 
         manager = ProjectManager(
             project_name=self.project_name, api_token=self.api_token
         )
         self.model_info = manager.get_model_info(self.model_name)
         self.knowledge = manager.get_knowledge(
             self.model_info.structured_knowledge_name
@@ -272,26 +272,26 @@
 
         ml_params_builder = MLParamBuilder()
 
         # generate combination of model_params
 
         for key in model_params.keys():
             model_ranges, _ = generate_train_hyperparams(model_params[key])
-            model_params[key]['tuning_ranges'] = [
+            model_params[key]["tuning_ranges"] = [
                 ml_params_builder.build_with_type(model_type=key, **model)
                 for model in model_ranges
             ]
 
         ranges = []
         for ml_model in current_ml_model_params:
-            if not model_params[ml_model.get('type')]:
+            if not model_params[ml_model.get("type")]:
                 # if model types not configured, use current hyperparams
                 ranges.append([ml_model])
                 continue
-            ranges.append(model_params[ml_model.get('type')]['tuning_ranges'])
+            ranges.append(model_params[ml_model.get("type")]["tuning_ranges"])
         return [list(item) for item in list(product(*ranges))]
 
     def tune_with_hyperparams(
         self, tuning_params: List[Any], base_name: str = None, data_name: str = None
     ):
         model_builder = ModelBuilder()
         if not base_name:
@@ -308,69 +308,69 @@
             metadata=self.model_info.metadata,
         )
 
         return model_df
 
     def _save_metrics(self):
         payload = {
-            'project_name': self.project_name,
-            'model_name': self.model_name,
-            'model_version': self.model_version,
-            'metrics': self.metrics,
+            "project_name": self.project_name,
+            "model_name": self.model_name,
+            "model_version": self.model_version,
+            "metrics": self.metrics,
         }
         resp = requests.post(self.METRICS_ENDPOINT, headers=self.headers, json=payload)
 
         if resp.status_code != 200:
-            err = f'{resp.status_code}: {resp.content}'
+            err = f"{resp.status_code}: {resp.content}"
             raise ConnectionError(err)
 
     def log_metrics(self, key, value):
         self.metrics[key] = value
         self._save_metrics()
 
     @staticmethod
     def get_model_names(api_token=None, project_name=None):
         if project_name is None:
-            project_id = os.getenv('AITOMATIC_PROJECT_ID')
+            project_id = os.getenv("AITOMATIC_PROJECT_ID")
         else:
             project_id = get_project_id(project_name, api_token=api_token)
 
         if api_token is None:
-            api_token = os.getenv('AITOMATIC_API_TOKEN')
+            api_token = os.getenv("AITOMATIC_API_TOKEN")
 
         _, client_api = get_api_root()
-        url = f'{client_api}/{project_id}/models'
+        url = f"{client_api}/{project_id}/models"
 
         headers = {
-            'authorization': api_token,
-            'Content-Type': 'application/json',
-            'accept': 'application/json',
+            "authorization": api_token,
+            "Content-Type": "application/json",
+            "accept": "application/json",
         }
         resp = requests.get(url, headers=headers)
 
         # Handle request errors
         if resp.status_code != 200:
-            err = f'{resp.status_code}: {resp.content}'
+            err = f"{resp.status_code}: {resp.content}"
             raise ConnectionError(err)
 
         resp_content = json.loads(resp.content)
-        return [x['name'] for x in resp_content]
+        return [x["name"] for x in resp_content]
 
 
 def convert_data_to_json(input_data: Dict) -> Tuple[Dict, Dict]:
     """
     Converts input data to json str for web request.
     Supports dict, pandas DataFrame, pandas Series and numpy arrays
     """
     # This segment is here when passing input_data['X'] instead of input_data
     # TODO: remove this after API is updated
     if isinstance(input_data, (pd.DataFrame, pd.Series)):
-        return json.loads(input_data.to_json()), {'predictions': type(input_data)}
-    elif isinstance(input_data, (dict, np.ndarray)) and 'X' not in input_data:
-        return input_data, {'predictions': type(input_data)}
+        return json.loads(input_data.to_json()), {"predictions": type(input_data)}
+    elif isinstance(input_data, (dict, np.ndarray)) and "X" not in input_data:
+        return input_data, {"predictions": type(input_data)}
 
     out_data = {}
     types_dict = {}
     for k, v in input_data.items():
         types_dict[k] = type(v)
         if isinstance(v, (pd.DataFrame, pd.Series)):
             out_data[k] = json.loads(v.to_json())
@@ -379,19 +379,19 @@
             out_data[k] = v
         elif isinstance(v, np.ndarray):
             # Convert later using JSONEncoder NpEncoder
             out_data[k] = v
         else:
             out_data[k] = v
 
-        if k.lower() in ['x', 'x_train', 'x_test']:
-            types_dict['predictions'] = type(v)
+        if k.lower() in ["x", "x_train", "x_test"]:
+            types_dict["predictions"] = type(v)
 
-    if 'predictions' not in types_dict.keys():
-        types_dict['predictions'] = pd.DataFrame
+    if "predictions" not in types_dict.keys():
+        types_dict["predictions"] = pd.DataFrame
 
     # out_json = json.dumps(out_data, cls=NpEncoder)
     return out_data, types_dict
 
 
 def convert_json_to_data(json_data: Dict, types_dict: Dict) -> Dict:
     """
@@ -404,15 +404,15 @@
         json_data = json.loads(json_data)
 
     for k, v in json_data.items():
         goal_type = types_dict.get(k, pd.DataFrame)
         if goal_type == pd.DataFrame or goal_type == pd.Series:
             out_data[k] = goal_type(eval(v))
         elif goal_type == np.ndarray:
-            out_data[k] = np.array(v, dtype='O')
+            out_data[k] = np.array(v, dtype="O")
         else:
             out_data[k] = v
 
     return out_data
 
 
 class NpEncoder(json.JSONEncoder):
@@ -442,20 +442,22 @@
     ml_ranges = model.generate_ml_model_params(
         model.model_info.ml_models, ml_tuning_params
     )
 
     # build conclusion threshold tuning ranges
     conclusion_threshold_ranges, _ = generate_train_hyperparams(conclusion_tuning_range)
 
-    TUNING_RANGES = {'threshold': conclusion_threshold_ranges, 'ml_models': ml_ranges}
+    TUNING_RANGES = {"threshold": conclusion_threshold_ranges, "ml_models": ml_ranges}
     tuning_params, _ = generate_train_hyperparams(TUNING_RANGES)
 
     builder = ModelBuilder()
-    base_name = f'{prefix} - {base_model}'
+    base_name = f"{prefix} - {base_model}"
     model_df = model.tune_with_hyperparams(tuning_params, base_name=base_name)
     try:
         model_df.to_parquet(output_model_df_path)
     except Exception as e:
-        print(f'Failed to save model_df to {output_model_df_path}')
+        print(f"Failed to save model_df to {output_model_df_path}")
         print(e)
     if wait_for_tuning_to_complete:
-        builder.wait_for_tuning_to_complete(model_df, 10)
+        builder.wait_for_tuning_to_complete(
+            model_df, file_path=output_model_df_path, sleep_time=10
+        )
```

### Comparing `aitomatic-1.2.7/src/aitomatic/dsl/arl_conclusions.py` & `aitomatic-1.2.8/src/aitomatic/dsl/arl_conclusions.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.7/src/aitomatic/dsl/arl_features.py` & `aitomatic-1.2.8/src/aitomatic/dsl/arl_features.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.7/src/aitomatic/dsl/arl_handler.py` & `aitomatic-1.2.8/src/aitomatic/dsl/arl_handler.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.7/src/aitomatic/dsl/arl_rules.py` & `aitomatic-1.2.8/src/aitomatic/dsl/arl_rules.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.7/src/aitomatic/dsl/utils.py` & `aitomatic-1.2.8/src/aitomatic/dsl/utils.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.7/src/aitomatic/objects/dataset.py` & `aitomatic-1.2.8/src/aitomatic/objects/dataset.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.7/src/aitomatic/objects/model.py` & `aitomatic-1.2.8/src/aitomatic/objects/model.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.7/src/aitomatic.egg-info/PKG-INFO` & `aitomatic-1.2.8/src/aitomatic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitomatic
-Version: 1.2.7
+Version: 1.2.8
 Summary: aitomatic library to interact with Aitomatic product
 Home-page: https://github.com/aitomatic/aitomatic-cli
 Author: Pham Hoang Tuan
 Author-email: tuan@aitomatic.com
 Project-URL: Bug Tracker, https://github.com/aitomatic/aitomatic-cli/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aitomatic-1.2.7/src/aitomatic.egg-info/SOURCES.txt` & `aitomatic-1.2.8/src/aitomatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

