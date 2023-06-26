# Comparing `tmp/optipack-0.0.19.dev0.tar.gz` & `tmp/optipack-0.0.20.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optipack-0.0.19.dev0.tar", max compression
+gzip compressed data, was "optipack-0.0.20.dev0.tar", max compression
```

## Comparing `optipack-0.0.19.dev0.tar` & `optipack-0.0.20.dev0.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0     1072 2023-02-02 02:52:49.676807 optipack-0.0.19.dev0/LICENSE
--rw-r--r--   0        0        0      795 2023-02-22 03:50:53.157490 optipack-0.0.19.dev0/README.md
--rw-r--r--   0        0        0     8196 2023-02-09 02:34:16.755095 optipack-0.0.19.dev0/optipack/.DS_Store
--rw-r--r--   0        0        0      393 2023-02-23 04:45:57.676772 optipack-0.0.19.dev0/optipack/.config/app_start.yaml
--rw-r--r--   0        0        0     1152 2023-03-28 07:59:00.285290 optipack-0.0.19.dev0/optipack/.config/connection_config.yaml
--rw-r--r--   0        0        0     1105 2023-02-10 10:14:39.318351 optipack-0.0.19.dev0/optipack/.config/hyperparam_config.yaml
--rw-r--r--   0        0        0      182 2023-02-15 09:40:56.333654 optipack-0.0.19.dev0/optipack/.config/project_structure.yaml
--rw-r--r--   0        0        0      193 2023-02-10 10:47:35.669118 optipack-0.0.19.dev0/optipack/.config/run_config.yaml
--rw-r--r--   0        0        0      174 2023-04-11 04:35:43.491296 optipack-0.0.19.dev0/optipack/__init__.py
--rw-r--r--   0        0        0      487 2023-04-11 04:17:56.303032 optipack-0.0.19.dev0/optipack/__main__.py
--rw-r--r--   0        0        0     6148 2023-02-08 11:02:11.605877 optipack-0.0.19.dev0/optipack/asset/.DS_Store
--rw-r--r--   0        0        0    64098 2023-02-09 02:35:39.601968 optipack-0.0.19.dev0/optipack/asset/logo-large.png
--rw-r--r--   0        0        0    14305 2023-02-09 02:35:39.602667 optipack-0.0.19.dev0/optipack/asset/logo-small.png
--rw-r--r--   0        0        0      473 2023-02-10 10:23:56.503936 optipack-0.0.19.dev0/optipack/asset/message.txt
--rw-r--r--   0        0        0       98 2023-02-10 12:04:37.999291 optipack-0.0.19.dev0/optipack/asset/tree_vis.yaml
--rw-r--r--   0        0        0     1216 2023-03-20 02:22:23.786659 optipack-0.0.19.dev0/optipack/cli.py
--rw-r--r--   0        0        0      257 2023-04-19 04:49:17.885432 optipack-0.0.19.dev0/optipack/core/automl/builder/__init__.py
--rw-r--r--   0        0        0     3380 2023-04-05 08:46:46.918861 optipack-0.0.19.dev0/optipack/core/automl/builder/base.py
--rw-r--r--   0        0        0     2963 2023-04-19 04:50:11.565658 optipack-0.0.19.dev0/optipack/core/automl/builder/data_builder.py
--rw-r--r--   0        0        0     1252 2023-04-19 04:50:50.124725 optipack-0.0.19.dev0/optipack/core/automl/builder/metric_builder.py
--rw-r--r--   0        0        0     2100 2023-04-19 04:51:13.529341 optipack-0.0.19.dev0/optipack/core/automl/builder/model_builder.py
--rw-r--r--   0        0        0       51 2023-04-19 04:52:13.961098 optipack-0.0.19.dev0/optipack/core/automl/runner/__init__.py
--rw-r--r--   0        0        0      984 2023-04-06 08:45:17.640576 optipack-0.0.19.dev0/optipack/core/automl/runner/base.py
--rw-r--r--   0        0        0        0 2023-04-04 02:51:40.046557 optipack-0.0.19.dev0/optipack/core/automl/runner/evaluator_runner.py
--rw-r--r--   0        0        0        0 2023-04-04 02:51:40.046843 optipack-0.0.19.dev0/optipack/core/automl/runner/runner_config.py
--rw-r--r--   0        0        0      181 2023-04-06 08:45:17.641026 optipack-0.0.19.dev0/optipack/core/automl/runner/trainer_runner.py
--rw-r--r--   0        0        0     1012 2023-04-07 10:48:16.828004 optipack-0.0.19.dev0/optipack/core/fileio/reader_misc.py
--rw-r--r--   0        0        0     8407 2023-04-21 08:52:22.061222 optipack-0.0.19.dev0/optipack/core/fileio/storage_io.py
--rw-r--r--   0        0        0      741 2023-04-07 08:35:16.155017 optipack-0.0.19.dev0/optipack/core/fileio/writer_misc.py
--rw-r--r--   0        0        0      140 2023-04-19 04:41:50.728393 optipack-0.0.19.dev0/optipack/core/logger/__init__.py
--rw-r--r--   0        0        0      746 2023-04-11 04:01:15.541303 optipack-0.0.19.dev0/optipack/core/logger/base.py
--rw-r--r--   0        0        0      396 2023-03-29 11:10:16.995306 optipack-0.0.19.dev0/optipack/core/logger/logger.cfg
--rw-r--r--   0        0        0     1893 2023-04-20 10:49:19.728342 optipack-0.0.19.dev0/optipack/core/logger/otp_logger.py
--rw-r--r--   0        0        0     1076 2023-04-19 08:02:11.226814 optipack-0.0.19.dev0/optipack/core/manager/automl_manager.py
--rw-r--r--   0        0        0     3745 2023-04-19 08:02:42.526653 optipack-0.0.19.dev0/optipack/core/manager/automodel_manager.py
--rw-r--r--   0        0        0      554 2023-04-19 08:03:49.436991 optipack-0.0.19.dev0/optipack/core/manager/run_manager.py
--rw-r--r--   0        0        0     2251 2023-03-20 10:11:52.420417 optipack-0.0.19.dev0/optipack/core/typing.py
--rw-r--r--   0        0        0      143 2023-04-19 08:04:07.778785 optipack-0.0.19.dev0/optipack/core/visualizer/__init__.py
--rw-r--r--   0        0        0      250 2023-03-30 10:37:47.836408 optipack-0.0.19.dev0/optipack/core/visualizer/base.py
--rw-r--r--   0        0        0     4272 2023-04-19 08:27:30.465768 optipack-0.0.19.dev0/optipack/core/visualizer/otp_visualizer.py
--rw-r--r--   0        0        0     1040 2023-04-19 08:04:46.367924 optipack-0.0.19.dev0/optipack/internal_utils/file_util.py
--rw-r--r--   0        0        0     3775 2023-03-21 10:03:49.090579 optipack-0.0.19.dev0/optipack/internal_utils/terminal_util.py
--rw-r--r--   0        0        0      155 2023-04-10 10:17:01.113759 optipack-0.0.19.dev0/optipack/sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 05:14:38.498269 optipack-0.0.19.dev0/optipack/sdk/optipack_env_controller.py
--rw-r--r--   0        0        0     1062 2023-04-19 04:45:25.414500 optipack-0.0.19.dev0/optipack/sdk/optipack_init.py
--rw-r--r--   0        0        0     4111 2023-04-20 11:09:12.936344 optipack-0.0.19.dev0/optipack/sdk/optipack_logger.py
--rw-r--r--   0        0        0     6091 2023-04-19 04:46:45.842724 optipack-0.0.19.dev0/optipack/sdk/optipack_project_generator.py
--rw-r--r--   0        0        0      158 2023-02-23 08:07:04.463928 optipack-0.0.19.dev0/optipack/sdk/optipack_run.py
--rw-r--r--   0        0        0      249 2023-04-19 04:47:24.388598 optipack-0.0.19.dev0/optipack/sdk/optipack_utils.py
--rw-r--r--   0        0        0      513 2023-04-21 08:58:04.734461 optipack-0.0.19.dev0/pyproject.toml
--rw-r--r--   0        0        0     1939 1970-01-01 00:00:00.000000 optipack-0.0.19.dev0/setup.py
--rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 optipack-0.0.19.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-08 14:29:07.547953 optipack-0.0.20.dev0/LICENSE
+-rw-r--r--   0        0        0      795 2023-03-14 16:25:39.367108 optipack-0.0.20.dev0/README.md
+-rw-r--r--   0        0        0     8196 2023-02-12 08:00:08.555189 optipack-0.0.20.dev0/optipack/.DS_Store
+-rw-r--r--   0        0        0      393 2023-02-12 08:00:08.555189 optipack-0.0.20.dev0/optipack/.config/app_start.yaml
+-rw-r--r--   0        0        0     1152 2023-03-28 17:28:13.803023 optipack-0.0.20.dev0/optipack/.config/connection_config.yaml
+-rw-r--r--   0        0        0     1105 2023-02-12 08:00:08.555189 optipack-0.0.20.dev0/optipack/.config/hyperparam_config.yaml
+-rw-r--r--   0        0        0      182 2023-02-20 15:50:16.092520 optipack-0.0.20.dev0/optipack/.config/project_structure.yaml
+-rw-r--r--   0        0        0      193 2023-02-12 08:00:08.555189 optipack-0.0.20.dev0/optipack/.config/run_config.yaml
+-rw-r--r--   0        0        0      174 2023-04-18 16:18:01.492301 optipack-0.0.20.dev0/optipack/__init__.py
+-rw-r--r--   0        0        0      487 2023-04-18 16:18:01.492301 optipack-0.0.20.dev0/optipack/__main__.py
+-rw-r--r--   0        0        0     6148 2023-02-08 14:29:07.547953 optipack-0.0.20.dev0/optipack/asset/.DS_Store
+-rw-r--r--   0        0        0    64098 2023-02-08 14:29:07.547953 optipack-0.0.20.dev0/optipack/asset/logo-large.png
+-rw-r--r--   0        0        0    14305 2023-02-08 17:18:12.009951 optipack-0.0.20.dev0/optipack/asset/logo-small.png
+-rw-r--r--   0        0        0      473 2023-02-12 08:00:08.555189 optipack-0.0.20.dev0/optipack/asset/message.txt
+-rw-r--r--   0        0        0       98 2023-02-12 08:00:08.555189 optipack-0.0.20.dev0/optipack/asset/tree_vis.yaml
+-rw-r--r--   0        0        0     1216 2023-03-22 14:26:02.273126 optipack-0.0.20.dev0/optipack/cli.py
+-rw-r--r--   0        0        0      257 2023-05-04 17:37:54.829442 optipack-0.0.20.dev0/optipack/core/automl/builder/__init__.py
+-rw-r--r--   0        0        0     3380 2023-04-05 15:20:42.035494 optipack-0.0.20.dev0/optipack/core/automl/builder/base.py
+-rw-r--r--   0        0        0     3057 2023-06-21 20:18:00.078771 optipack-0.0.20.dev0/optipack/core/automl/builder/data_builder.py
+-rw-r--r--   0        0        0     1252 2023-05-04 17:37:54.832775 optipack-0.0.20.dev0/optipack/core/automl/builder/metric_builder.py
+-rw-r--r--   0        0        0     2100 2023-05-04 17:37:54.832775 optipack-0.0.20.dev0/optipack/core/automl/builder/model_builder.py
+-rw-r--r--   0        0        0       51 2023-05-04 17:37:54.832775 optipack-0.0.20.dev0/optipack/core/automl/runner/__init__.py
+-rw-r--r--   0        0        0      984 2023-04-05 18:08:56.353628 optipack-0.0.20.dev0/optipack/core/automl/runner/base.py
+-rw-r--r--   0        0        0        0 2023-03-22 14:26:02.273126 optipack-0.0.20.dev0/optipack/core/automl/runner/evaluator_runner.py
+-rw-r--r--   0        0        0        0 2023-04-03 18:00:46.073318 optipack-0.0.20.dev0/optipack/core/automl/runner/runner_config.py
+-rw-r--r--   0        0        0      181 2023-04-05 18:06:10.590604 optipack-0.0.20.dev0/optipack/core/automl/runner/trainer_runner.py
+-rw-r--r--   0        0        0     1012 2023-04-10 15:39:44.777137 optipack-0.0.20.dev0/optipack/core/fileio/reader_misc.py
+-rw-r--r--   0        0        0     8409 2023-05-04 17:37:54.832775 optipack-0.0.20.dev0/optipack/core/fileio/storage_io.py
+-rw-r--r--   0        0        0      741 2023-04-10 15:39:44.777137 optipack-0.0.20.dev0/optipack/core/fileio/writer_misc.py
+-rw-r--r--   0        0        0      140 2023-05-04 17:37:54.832775 optipack-0.0.20.dev0/optipack/core/logger/__init__.py
+-rw-r--r--   0        0        0      746 2023-04-18 16:18:01.492301 optipack-0.0.20.dev0/optipack/core/logger/base.py
+-rw-r--r--   0        0        0      394 2023-05-04 18:26:42.010803 optipack-0.0.20.dev0/optipack/core/logger/logger.cfg
+-rw-r--r--   0        0        0     1893 2023-05-04 17:37:54.832775 optipack-0.0.20.dev0/optipack/core/logger/otp_logger.py
+-rw-r--r--   0        0        0     1076 2023-05-04 17:37:54.832775 optipack-0.0.20.dev0/optipack/core/manager/automl_manager.py
+-rw-r--r--   0        0        0     3745 2023-05-04 17:37:54.832775 optipack-0.0.20.dev0/optipack/core/manager/automodel_manager.py
+-rw-r--r--   0        0        0      554 2023-05-04 17:37:54.832775 optipack-0.0.20.dev0/optipack/core/manager/run_manager.py
+-rw-r--r--   0        0        0     2317 2023-06-21 20:17:20.122296 optipack-0.0.20.dev0/optipack/core/typing.py
+-rw-r--r--   0        0        0      143 2023-05-04 17:37:54.832775 optipack-0.0.20.dev0/optipack/core/visualizer/__init__.py
+-rw-r--r--   0        0        0      250 2023-03-30 19:34:48.986473 optipack-0.0.20.dev0/optipack/core/visualizer/base.py
+-rw-r--r--   0        0        0     4532 2023-06-21 20:15:38.202794 optipack-0.0.20.dev0/optipack/core/visualizer/otp_visualizer.py
+-rw-r--r--   0        0        0     1040 2023-05-04 17:37:54.832775 optipack-0.0.20.dev0/optipack/internal_utils/file_util.py
+-rw-r--r--   0        0        0     3784 2023-06-26 18:46:22.081269 optipack-0.0.20.dev0/optipack/internal_utils/terminal_util.py
+-rw-r--r--   0        0        0      155 2023-04-18 16:17:34.715345 optipack-0.0.20.dev0/optipack/sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-12 08:00:08.555189 optipack-0.0.20.dev0/optipack/sdk/optipack_env_controller.py
+-rw-r--r--   0        0        0     1062 2023-05-04 17:37:54.832775 optipack-0.0.20.dev0/optipack/sdk/optipack_init.py
+-rw-r--r--   0        0        0     4110 2023-05-04 19:37:41.621086 optipack-0.0.20.dev0/optipack/sdk/optipack_logger.py
+-rw-r--r--   0        0        0     6091 2023-05-04 17:37:54.836109 optipack-0.0.20.dev0/optipack/sdk/optipack_project_generator.py
+-rw-r--r--   0        0        0      158 2023-03-14 16:25:39.430441 optipack-0.0.20.dev0/optipack/sdk/optipack_run.py
+-rw-r--r--   0        0        0      249 2023-05-04 17:37:54.836109 optipack-0.0.20.dev0/optipack/sdk/optipack_utils.py
+-rw-r--r--   0        0        0      535 2023-06-21 20:35:44.311136 optipack-0.0.20.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 optipack-0.0.20.dev0/PKG-INFO
```

### Comparing `optipack-0.0.19.dev0/LICENSE` & `optipack-0.0.20.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/README.md` & `optipack-0.0.20.dev0/README.md`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/.DS_Store` & `optipack-0.0.20.dev0/optipack/.DS_Store`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/.config/connection_config.yaml` & `optipack-0.0.20.dev0/optipack/.config/connection_config.yaml`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/.config/hyperparam_config.yaml` & `optipack-0.0.20.dev0/optipack/.config/hyperparam_config.yaml`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/asset/.DS_Store` & `optipack-0.0.20.dev0/optipack/asset/.DS_Store`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/asset/logo-large.png` & `optipack-0.0.20.dev0/optipack/asset/logo-large.png`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/asset/logo-small.png` & `optipack-0.0.20.dev0/optipack/asset/logo-small.png`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/cli.py` & `optipack-0.0.20.dev0/optipack/cli.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/core/automl/builder/base.py` & `optipack-0.0.20.dev0/optipack/core/automl/builder/base.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/core/automl/builder/data_builder.py` & `optipack-0.0.20.dev0/optipack/core/automl/builder/data_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,19 @@
             name = 'torch-data-builder-logger', 
             log_dir = './.otp_log/'
         )
         super().__init__(mode = mode, cfg = cfg, logger=logger)
         self.dataset_cls = None
 
     def split(self, dataset, val_ratio = 0.1, seed = 123): 
-        import torch
-        from torch.utils.data import random_split
+        try: 
+            import torch
+            from torch.utils.data import random_split
+        except: 
+            raise ImportError('Missing torch library')
 
         splitted = random_split(list(dataset), [val_ratio, 1-val_ratio], torch.Generator().manual_seed(seed))
         return splitted[0], splitted[1]
 
     def build_dataset(self, set_type: str ):
         try:
             if not self.dataset_cls:
```

### Comparing `optipack-0.0.19.dev0/optipack/core/automl/builder/metric_builder.py` & `optipack-0.0.20.dev0/optipack/core/automl/builder/metric_builder.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/core/automl/builder/model_builder.py` & `optipack-0.0.20.dev0/optipack/core/automl/builder/model_builder.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/core/automl/runner/base.py` & `optipack-0.0.20.dev0/optipack/core/automl/runner/base.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/core/fileio/reader_misc.py` & `optipack-0.0.20.dev0/optipack/core/fileio/reader_misc.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/core/fileio/storage_io.py` & `optipack-0.0.20.dev0/optipack/core/fileio/storage_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     # @abstractmethod
     # def write(self):
     #     pass
 
 class MongoDBStore(Storage):
     def __init__(self, storage_name: str, **kwargs) -> None:
-        super().__init__(storage_name, kwargs)
+        super().__init__(storage_name, **kwargs)
         self._validate()
         self.connection_string = f'mongodb://{self.username}:{self.password}@{self.host}/{self.db_name}/'
         self._connect()
         if self.db_name: 
             self.get_database(self.db_name)
         if self.db and self.collection_name: 
             self.get_collection(self.collection_name)
```

### Comparing `optipack-0.0.19.dev0/optipack/core/fileio/writer_misc.py` & `optipack-0.0.20.dev0/optipack/core/fileio/writer_misc.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/core/logger/base.py` & `optipack-0.0.20.dev0/optipack/core/logger/base.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/core/logger/otp_logger.py` & `optipack-0.0.20.dev0/optipack/core/logger/otp_logger.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/core/manager/automl_manager.py` & `optipack-0.0.20.dev0/optipack/core/manager/automl_manager.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/core/manager/automodel_manager.py` & `optipack-0.0.20.dev0/optipack/core/manager/automodel_manager.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/core/manager/run_manager.py` & `optipack-0.0.20.dev0/optipack/core/manager/run_manager.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/core/typing.py` & `optipack-0.0.20.dev0/optipack/core/typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-import torch
 import numpy as np
 import matplotlib
 from abc import ABC
+try: 
+    import torch
+except: 
+    raise ImportError('Missing torch library')
 
 class OtpDataType(ABC):
     def __init__(self, item) -> None:
         self._item = item
 
     def __str__(self) -> str:
         return self.__name__
```

### Comparing `optipack-0.0.19.dev0/optipack/core/visualizer/otp_visualizer.py` & `optipack-0.0.20.dev0/optipack/core/visualizer/otp_visualizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     RuntimeError: _description_
     NotImplementedError: _description_
 """
 
 from optipack.core.visualizer.base import BaseVisualizer
 from fastcore.dispatch import *
 from optipack import typing
+from threading import current_thread
 
 
 class TensorboardVisualizer(BaseVisualizer):
     """Tensorboard that maps with normal logger
         Supported visualization: 
             - scalar
             - image
@@ -23,34 +24,39 @@
 
     def __init__(self,
                  name: str,
                  root_dir: str,
                  run_folder: str= '',
                  **kwargs
                  ) -> None:
-        from torch.utils.tensorboard import SummaryWriter
+        
+        try: 
+            from torch.utils.tensorboard import SummaryWriter
+        except: 
+            raise ImportError('Missing Torch library')
         # the folder will be changed when optipack tracker is coded
         super().__init__(name, root_dir, run_folder)
         log_path = self.__create_log_dir(**kwargs)
         self.__writer = SummaryWriter(log_path)
+        self.verbose = True
 
     def __create_log_dir(self, **kwargs):
         import os
         dirs = ['tensorboard']
         if 'directory_list' in kwargs:
             dirs += kwargs['directory_list']
         else:
             dirs.append(self.run_folder)
         log_path = self.root_dir
         try:
             for d in dirs:
                 if not os.path.exists(log_path):
                     os.mkdir(log_path)
                 log_path = os.path.join(log_path, d)
-
+            print(f'Created tb log_path {log_path}')
             return log_path
         except:
             raise NotADirectoryError(f'{log_path} is unreachable.')
 
     def log_metric(
         self,
         title: str,
@@ -64,17 +70,18 @@
             self._step = step
         except Exception as e:
             raise RuntimeError(
                 f'Error {e} happened while processing keys and metrics')
 
         try:
             executor = ThreadPoolExecutor()
-            wait([executor.submit(self._log_tb, [m, metrics[m]])
-                  for m in metrics
+            futures = wait([executor.submit(self._log_tb, k,v)
+                  for k,v in metrics.items()
                   ])
+            print(futures)
             self.__writer.flush()
             executor.shutdown()
         except Exception as e:
             raise RuntimeError(
                 f'Error {e} happened while attempting threading execution')
 
     @typedispatch
@@ -109,15 +116,15 @@
                  run_folder: str) -> None:
         raise NotImplementedError('Waiting to be implemented :)')
 
 
 if __name__ == '__main__':
     import PIL
     import numpy as np
-    img = PIL.Image.open('asset/image/logo.png')
+    img = PIL.Image.open('optipack/asset/logo-large.png')
     np_arr = np.asarray(img)
 
     tb_vis = TensorboardVisualizer(
         name='tb-logger', root_dir='./log', run_folder='test-tb')
 
     from timeit import timeit
     time = timeit(str(
```

### Comparing `optipack-0.0.19.dev0/optipack/internal_utils/file_util.py` & `optipack-0.0.20.dev0/optipack/internal_utils/file_util.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/internal_utils/terminal_util.py` & `optipack-0.0.20.dev0/optipack/internal_utils/terminal_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             output = output + f'[on rgb({r},{g},{b})] [/]'
 
         output = output + '\n'
 
     return output
 
 def start_cli():
-    from core.fileio.reader_misc import read_text
+    from optipack.core.fileio.reader_misc import read_text
 
     terminal_size = os.get_terminal_size()
     logo_path = os.environ.get('LARGE_LOGO_PATH')
     scale = 1.0
     if terminal_size[0]<90:
         logo_path = os.environ.get('SMALL_LOGO_PATH')
         scale = 0.5
```

### Comparing `optipack-0.0.19.dev0/optipack/sdk/optipack_init.py` & `optipack-0.0.20.dev0/optipack/sdk/optipack_init.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/optipack/sdk/optipack_logger.py` & `optipack-0.0.20.dev0/optipack/sdk/optipack_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 class OptipackLogger(logging.LoggerAdapter):
     def __init__(self,
                  name: str,
                  logger: str = 'file',
                  visualizer: str = '',
                  log_dir: str = '.',
                  extra: Mapping[str, object] = {},
-                 logger_kwargs: dict = {'level': logging.DEBUG},
-                 visualizer_kwargs: dict = {'root_dir':'', 'run_folder': '', 'directory_list': {}}
+                 logger_kwargs: dict = {'level': logging.INFO},
+                 visualizer_kwargs: dict = {'root_dir':'', 'run_folder': '', 'directory_list': []}
                  ) -> None:
         '''Logger adapter that connect logger and visualizer.
 
         Args:
             name (str): logger's name. .log file will have the same name.
             logger (str, optional): type of logger, including "console","file". Defaults to "file".
             visualizer (str, optional): type of visualizer, including "tensorboard", "aim", "". Defaults to "" when no visualizer is chosen.
```

### Comparing `optipack-0.0.19.dev0/optipack/sdk/optipack_project_generator.py` & `optipack-0.0.20.dev0/optipack/sdk/optipack_project_generator.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.19.dev0/PKG-INFO` & `optipack-0.0.20.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: optipack
-Version: 0.0.19.dev0
+Version: 0.0.20.dev0
 Summary: The optimal ML package
 Author: indigoYoshimaru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (==9.4.0)
+Requires-Dist: fastcore (>=1.5,<2.0)
 Requires-Dist: fs-gcsfs (>=1.5.1,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: protobuf (>=3.20.2,<4.0.0)
 Requires-Dist: pyyaml (==6.0)
 Requires-Dist: rich (==13.3.1)
-Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 ![optipack](asset/image/logo.png)
 
 # What optipack do: 
 - Workspace management:
```

