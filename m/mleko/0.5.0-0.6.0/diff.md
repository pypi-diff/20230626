# Comparing `tmp/mleko-0.5.0.tar.gz` & `tmp/mleko-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-0.5.0.tar", max compression
+gzip compressed data, was "mleko-0.6.0.tar", max compression
```

## Comparing `mleko-0.5.0.tar` & `mleko-0.6.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1073 2023-06-17 16:53:35.711108 mleko-0.5.0/LICENSE
--rw-r--r--   0        0        0     2561 2023-06-17 16:53:35.711108 mleko-0.5.0/README.md
--rw-r--r--   0        0        0     1323 2023-06-17 16:54:05.835472 mleko-0.5.0/mleko/__init__.py
--rw-r--r--   0        0        0      584 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/__init__.py
--rw-r--r--   0        0        0    11493 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/cache_mixin.py
--rw-r--r--   0        0        0      805 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/fingerprinters/__init__.py
--rw-r--r--   0        0        0     1167 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/fingerprinters/base_fingerprinter.py
--rw-r--r--   0        0        0     2843 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/fingerprinters/csv_fingerprinter.py
--rw-r--r--   0        0        0     1233 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
--rw-r--r--   0        0        0      398 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/format/__init__.py
--rw-r--r--   0        0        0     1938 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/format/vaex_cache_format_mixin.py
--rw-r--r--   0        0        0     5974 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/lru_cache_mixin.py
--rw-r--r--   0        0        0      740 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/__init__.py
--rw-r--r--   0        0        0      491 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/convert/__init__.py
--rw-r--r--   0        0        0     1435 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/convert/base_converter.py
--rw-r--r--   0        0        0    11577 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/convert/csv_to_vaex_converter.py
--rw-r--r--   0        0        0     1613 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/feature_select/__init__.py
--rw-r--r--   0        0        0     5884 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/feature_select/base_feature_selector.py
--rw-r--r--   0        0        0     5188 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/feature_select/composite_feature_selector.py
--rw-r--r--   0        0        0     4990 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/feature_select/invariance_feature_selector.py
--rw-r--r--   0        0        0     5255 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
--rw-r--r--   0        0        0     7080 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
--rw-r--r--   0        0        0     5585 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/feature_select/variance_feature_selector.py
--rw-r--r--   0        0        0      877 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/ingest/__init__.py
--rw-r--r--   0        0        0     2261 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/ingest/base_ingester.py
--rw-r--r--   0        0        0    18020 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/ingest/kaggle_ingester.py
--rw-r--r--   0        0        0     9637 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/ingest/s3_ingester.py
--rw-r--r--   0        0        0      679 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/split/__init__.py
--rw-r--r--   0        0        0     1394 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/split/base_splitter.py
--rw-r--r--   0        0        0     3815 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/split/expression_splitter.py
--rw-r--r--   0        0        0     5934 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/split/random_splitter.py
--rw-r--r--   0        0        0     1611 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/transform/__init__.py
--rw-r--r--   0        0        0     3073 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/transform/base_transformer.py
--rw-r--r--   0        0        0     4424 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/transform/composite_transformer.py
--rw-r--r--   0        0        0     4389 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/transform/frequency_encoder_transformer.py
--rw-r--r--   0        0        0     4021 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/transform/label_encoder_transformer.py
--rw-r--r--   0        0        0     3677 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/transform/max_abs_scaler_transformer.py
--rw-r--r--   0        0        0     4053 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/transform/min_max_scaler_transformer.py
--rw-r--r--   0        0        0      644 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1420 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     4496 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     3595 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      697 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     2359 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/steps/convert_step.py
--rw-r--r--   0        0        0     2179 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/steps/feature_select_step.py
--rw-r--r--   0        0        0     2141 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/steps/ingest_step.py
--rw-r--r--   0        0        0     2248 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/steps/split_step.py
--rw-r--r--   0        0        0     2088 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/steps/transform_step.py
--rw-r--r--   0        0        0        0 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/py.typed
--rw-r--r--   0        0        0      765 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/utils/__init__.py
--rw-r--r--   0        0        0     4497 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     3430 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/utils/decorators.py
--rw-r--r--   0        0        0      742 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0     1413 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/utils/tqdm_helpers.py
--rw-r--r--   0        0        0     2836 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/utils/vaex_helpers.py
--rw-r--r--   0        0        0     2839 2023-06-17 16:54:05.887472 mleko-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 mleko-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-26 21:28:47.298938 mleko-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2561 2023-06-26 21:28:47.298938 mleko-0.6.0/README.md
+-rw-r--r--   0        0        0     1323 2023-06-26 21:29:23.071188 mleko-0.6.0/mleko/__init__.py
+-rw-r--r--   0        0        0      584 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    13234 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/cache_mixin.py
+-rw-r--r--   0        0        0      805 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/fingerprinters/__init__.py
+-rw-r--r--   0        0        0     1167 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/fingerprinters/base_fingerprinter.py
+-rw-r--r--   0        0        0     2843 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/fingerprinters/csv_fingerprinter.py
+-rw-r--r--   0        0        0     1233 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
+-rw-r--r--   0        0        0      398 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/format/__init__.py
+-rw-r--r--   0        0        0     1938 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/format/vaex_cache_format_mixin.py
+-rw-r--r--   0        0        0     6957 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/cache/lru_cache_mixin.py
+-rw-r--r--   0        0        0      740 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/convert/__init__.py
+-rw-r--r--   0        0        0     1530 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/convert/base_converter.py
+-rw-r--r--   0        0        0    11709 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/convert/csv_to_vaex_converter.py
+-rw-r--r--   0        0        0     1613 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/feature_select/__init__.py
+-rw-r--r--   0        0        0     5979 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/feature_select/base_feature_selector.py
+-rw-r--r--   0        0        0     5332 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/feature_select/composite_feature_selector.py
+-rw-r--r--   0        0        0     5134 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/feature_select/invariance_feature_selector.py
+-rw-r--r--   0        0        0     5387 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
+-rw-r--r--   0        0        0     7212 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
+-rw-r--r--   0        0        0     5717 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/feature_select/variance_feature_selector.py
+-rw-r--r--   0        0        0      877 2023-06-26 21:28:47.298938 mleko-0.6.0/mleko/dataset/ingest/__init__.py
+-rw-r--r--   0        0        0     2261 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/ingest/base_ingester.py
+-rw-r--r--   0        0        0    18020 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/ingest/kaggle_ingester.py
+-rw-r--r--   0        0        0     9637 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/ingest/s3_ingester.py
+-rw-r--r--   0        0        0      679 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/split/__init__.py
+-rw-r--r--   0        0        0     1489 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/split/base_splitter.py
+-rw-r--r--   0        0        0     3947 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/split/expression_splitter.py
+-rw-r--r--   0        0        0     6066 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/split/random_splitter.py
+-rw-r--r--   0        0        0     1611 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/transform/__init__.py
+-rw-r--r--   0        0        0     3168 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/transform/base_transformer.py
+-rw-r--r--   0        0        0     4556 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/transform/composite_transformer.py
+-rw-r--r--   0        0        0     4521 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/transform/frequency_encoder_transformer.py
+-rw-r--r--   0        0        0     4153 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/transform/label_encoder_transformer.py
+-rw-r--r--   0        0        0     3809 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/transform/max_abs_scaler_transformer.py
+-rw-r--r--   0        0        0     4185 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/dataset/transform/min_max_scaler_transformer.py
+-rw-r--r--   0        0        0      644 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1420 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     4496 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3711 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      697 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     2482 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/steps/convert_step.py
+-rw-r--r--   0        0        0     2302 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/steps/feature_select_step.py
+-rw-r--r--   0        0        0     2148 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/steps/ingest_step.py
+-rw-r--r--   0        0        0     2372 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/steps/split_step.py
+-rw-r--r--   0        0        0     2211 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/pipeline/steps/transform_step.py
+-rw-r--r--   0        0        0        0 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/py.typed
+-rw-r--r--   0        0        0      765 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     4497 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     3430 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/utils/decorators.py
+-rw-r--r--   0        0        0      742 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0     1413 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/utils/tqdm_helpers.py
+-rw-r--r--   0        0        0     2836 2023-06-26 21:28:47.302938 mleko-0.6.0/mleko/utils/vaex_helpers.py
+-rw-r--r--   0        0        0     2839 2023-06-26 21:29:23.175189 mleko-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 mleko-0.6.0/PKG-INFO
```

### Comparing `mleko-0.5.0/LICENSE` & `mleko-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/README.md` & `mleko-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/__init__.py` & `mleko-0.6.0/mleko/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 Each subpackage is designed to be modular and extensible, making it easy to customize and adapt the library to a wide
 range of model building processes and requirements.
 """
 from __future__ import annotations
 
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
```

### Comparing `mleko-0.5.0/mleko/cache/__init__.py` & `mleko-0.6.0/mleko/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/cache/cache_mixin.py` & `mleko-0.6.0/mleko/cache/cache_mixin.py`

 * *Files 13% similar despite different names*

```diff
@@ -95,32 +95,42 @@
         self._cache_file_suffix = cache_file_suffix
         self._cache_type_name = self._find_cache_type_name(self.__class__)
 
     def _cached_execute(
         self,
         lambda_func: Callable[[], Any],
         cache_keys: list[Hashable | tuple[Any, BaseFingerprinter]],
+        cache_group: str | None = None,
         force_recompute: bool = False,
     ) -> Any:
         """Executes the given function, caching the results based on the provided cache keys and fingerprints.
 
+        Warning:
+            The cache group is used to group related cache keys together to prevent collisions between cache keys
+            originating from the same method. For example, if a method is called during the training and testing
+            phases of a machine learning pipeline, the cache keys for the training and testing phases should be
+            using different cache groups to prevent collisions between the cache keys for the two phases. Otherwise,
+            the later cache keys might overwrite the earlier cache entries.
+
         Args:
             lambda_func: A lambda function to execute.
             cache_keys: A list of cache keys that can be a mix of hashable values and tuples containing a value and a
                 BaseFingerprinter instance for generating fingerprints.
+            cache_group: A string representing the cache group, used to group related cache keys together when methods
+                are called independently.
             force_recompute: A boolean indicating whether to force recompute the result and update the cache, even if a
                 cached result is available.
 
         Returns:
             The result of executing the given function. If a cached result is available and `force_recompute` is False,
             the cached result will be returned instead of recomputing the result.
         """
         frame_qualname = get_frame_qualname(inspect.stack()[1])
         class_method_name = ".".join(frame_qualname.split(".")[-2:])
-        cache_key = self._compute_cache_key(cache_keys, frame_qualname)
+        cache_key = self._compute_cache_key(cache_keys, class_method_name, cache_group)
 
         if not force_recompute:
             output = self._load_from_cache(cache_key)
             if output is not None:
                 logger.info(
                     f"\033[32mCache Hit\033[0m ({self._cache_type_name}) {class_method_name}: Using cached output."
                 )
@@ -135,42 +145,60 @@
             )
 
         output = lambda_func()
         self._save_to_cache(cache_key, output)
         return self._load_from_cache(cache_key)
 
     def _compute_cache_key(
-        self, cache_keys: list[Hashable | tuple[Any, BaseFingerprinter]], frame_qualname: str
+        self,
+        cache_keys: list[Hashable | tuple[Any, BaseFingerprinter]],
+        class_method_name: str,
+        cache_group: str | None = None,
     ) -> str:
         """Computes the cache key based on the provided cache keys and the calling function's fully qualified name.
 
         Args:
             cache_keys: A list of cache keys that can be a mix of hashable values and tuples containing a value and a
                 BaseFingerprinter instance for generating fingerprints.
-            frame_qualname: The fully qualified name of the cached function stack frame.
+            class_method_name: A string of format "class.method" for class methods or "module.function" for
+                functions, representing the fully qualified name of the calling function or method.
+            cache_group: A string representing the cache group.
+
+        Raises:
+            ValueError: If the computed cache key is too long.
 
         Returns:
             A string representing the computed cache key, which is the MD5 hash of the fully qualified name of the
             calling function or method, along with the fingerprints of the provided cache keys.
         """
         values_to_hash: list[Hashable] = []
 
         for key in cache_keys:
             if isinstance(key, tuple) and len(key) == 2 and isinstance(key[1], BaseFingerprinter):
                 value, fingerprinter = key
                 values_to_hash.append(fingerprinter.fingerprint(value))
             else:
                 values_to_hash.append(key)
 
-        data = pickle.dumps((frame_qualname, values_to_hash))
-
-        class_method_name = ".".join(frame_qualname.split(".")[-2:])
-        cache_key = f"{class_method_name}.{hashlib.md5(data).hexdigest()}"
+        data = pickle.dumps(values_to_hash)
+        cache_key_prefix = class_method_name
+        if cache_group is not None:
+            cache_key_prefix = f"{cache_key_prefix}.{cache_group}"
+
+        cache_key = f"{cache_key_prefix}.{hashlib.md5(data).hexdigest()}"
+        if len(cache_key) + 1 + len(self._cache_file_suffix) > 255:
+            raise ValueError(
+                f"The computed cache key is too long ({len(cache_key) + len(self._cache_file_suffix)} chars)."
+                "The maximum length of a cache key is 255 chars, and given the current class, the maximum "
+                "length of the provided cache_group is "
+                f"{255 - len(cache_key_prefix) - 32 - 1 - len(self._cache_file_suffix)} chars."
+                "Please reduce the length of the cache_group."
+            )
 
-        return cache_key
+        return f"{cache_key_prefix}.{hashlib.md5(data).hexdigest()}"
 
     def _read_cache_file(self, cache_file_path: Path) -> Any:
         """Reads the cache file from the specified path and returns the deserialized data.
 
         This method can be overridden in subclasses to customize the cache loading process.
 
         Args:
```

### Comparing `mleko-0.5.0/mleko/cache/fingerprinters/__init__.py` & `mleko-0.6.0/mleko/cache/fingerprinters/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/cache/fingerprinters/base_fingerprinter.py` & `mleko-0.6.0/mleko/cache/fingerprinters/base_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/cache/fingerprinters/csv_fingerprinter.py` & `mleko-0.6.0/mleko/cache/fingerprinters/csv_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/cache/fingerprinters/vaex_fingerprinter.py` & `mleko-0.6.0/mleko/cache/fingerprinters/vaex_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/cache/format/vaex_cache_format_mixin.py` & `mleko-0.6.0/mleko/cache/format/vaex_cache_format_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/cache/lru_cache_mixin.py` & `mleko-0.6.0/mleko/cache/lru_cache_mixin.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 rarely accessed and have not been accessed recently are evicted first as the cache fills up. The cache entries
 are stored in the cache directory, and the cache is trimmed if needed when cold starting the cache.
 """
 from __future__ import annotations
 
 import inspect
 import re
-from collections import OrderedDict
+from collections import OrderedDict, defaultdict
 from pathlib import Path
 from typing import Any
 
 from mleko.utils.custom_logger import CustomLogger
 
 from .cache_mixin import CacheMixin, get_frame_qualname
 
@@ -65,67 +65,85 @@
             >>> my_class.my_method(3)
             9 # This is cached
             >>> my_class.my_method(4)
             16 # This is not cached, and the cache is full so the least recently used entry is evicted (x = 2)
         """
         super().__init__(cache_directory, cache_file_suffix)
         self._cache_size = cache_size
-        self._cache: OrderedDict[str, bool] = OrderedDict()
+        self._cache: dict[str, OrderedDict[str, bool]] = defaultdict(OrderedDict)
         self._load_cache_from_disk()
 
     def _load_cache_from_disk(self) -> None:
         """Loads the cache entries from the cache directory and initializes the LRU cache.
 
         Cache entries are ordered by their modification time, and the cache is trimmed if needed.
         """
         frame_qualname = get_frame_qualname(inspect.stack()[2])
         class_name = frame_qualname.split(".")[-2]
-        file_name_pattern = rf"{class_name}\.[a-zA-Z_][a-zA-Z0-9_]*\.[a-fA-F\d]{{32}}"
+        file_name_pattern = rf"{class_name}\.([a-zA-Z_][a-zA-Z0-9_]*)(\.[a-zA-Z_][a-zA-Z0-9_]*)?\.[a-fA-F\d]{{32}}"
+
         cache_files = [
             f
             for f in self._cache_directory.glob(f"*.{self._cache_file_suffix}")
             if re.search(file_name_pattern, str(f.stem))
         ]
         ordered_cache_files = sorted(cache_files, key=lambda x: x.stat().st_mtime)
+
         for cache_file in ordered_cache_files:
             cache_key_match = re.search(file_name_pattern, cache_file.stem)
-            cache_key = cache_key_match.group(0)  # type: ignore
-            if cache_key not in self._cache:
-                if len(self._cache) >= self._cache_size:
-                    oldest_key = next(iter(self._cache))
-                    del self._cache[oldest_key]
-                    for file in self._cache_directory.glob(f"{oldest_key}*.{self._cache_file_suffix}"):
-                        file.unlink()
-                self._cache[cache_key] = True
+            if cache_key_match:
+                method_name, cache_group = cache_key_match.groups()
+                group_identifier = method_name + cache_group if cache_group else method_name
+                cache_key = cache_key_match.group(0)
+
+                if cache_key not in self._cache[group_identifier]:
+                    if len(self._cache[group_identifier]) >= self._cache_size:
+                        oldest_key = next(iter(self._cache[group_identifier]))
+                        del self._cache[group_identifier][oldest_key]
+                        for file in self._cache_directory.glob(f"{oldest_key}*.{self._cache_file_suffix}"):
+                            file.unlink()
+
+                    self._cache[group_identifier][cache_key] = True
 
     def _load_from_cache(self, cache_key: str) -> Any | None:
         """Loads data from the cache based on the provided cache key and updates the LRU cache.
 
         Args:
             cache_key: A string representing the cache key.
 
         Returns:
             The cached data if it exists, or None if there is no data for the given cache key.
         """
-        if cache_key in self._cache:
-            self._cache.move_to_end(cache_key)
-        return super()._load_from_cache(cache_key)
+        for group_identifier in self._cache.keys():
+            if cache_key in self._cache[group_identifier]:
+                self._cache[group_identifier].move_to_end(cache_key)
+            return super()._load_from_cache(cache_key)
+        return None
 
     def _save_to_cache(self, cache_key: str, output: Any) -> None:
         """Saves the given data to the cache using the provided cache key, updating the LRU cache accordingly.
 
         If the cache reaches its maximum size, the least recently used entry will be evicted.
 
         Args:
             cache_key: A string representing the cache key.
             output: The data to be saved to the cache.
         """
-        if cache_key not in self._cache:
-            if len(self._cache) >= self._cache_size:
-                oldest_key = next(iter(self._cache))
-                del self._cache[oldest_key]
-                for file in self._cache_directory.glob(f"{oldest_key}*.{self._cache_file_suffix}"):
-                    file.unlink()
-            self._cache[cache_key] = True
-        else:
-            self._cache.move_to_end(cache_key)
-        super()._save_to_cache(cache_key, output)
+        cache_key_match = re.match(
+            r"[a-zA-Z_][a-zA-Z0-9_]*\.([a-zA-Z_][a-zA-Z0-9_]*)(\.[a-zA-Z_][a-zA-Z0-9_]*)?\.[a-fA-F\d]{32}", cache_key
+        )
+        if cache_key_match:
+            method_name, cache_group = cache_key_match.groups()
+            group_identifier = method_name + cache_group if cache_group else method_name
+
+            if cache_key not in self._cache[group_identifier]:
+                if len(self._cache[group_identifier]) >= self._cache_size:
+                    oldest_key = next(iter(self._cache[group_identifier]))
+                    del self._cache[group_identifier][oldest_key]
+                    for file in self._cache_directory.glob(f"{oldest_key}*.{self._cache_file_suffix}"):
+                        file.unlink()
+
+                self._cache[group_identifier][cache_key] = True
+            else:
+                self._cache[group_identifier].move_to_end(cache_key)
+
+            super()._save_to_cache(cache_key, output)
```

### Comparing `mleko-0.5.0/mleko/dataset/__init__.py` & `mleko-0.6.0/mleko/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/dataset/convert/base_converter.py` & `mleko-0.6.0/mleko/dataset/convert/base_converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,21 @@
         Args:
             cache_directory: The directory to store the cache in.
             cache_size: The maximum number of cache entries.
         """
         LRUCacheMixin.__init__(self, cache_directory, self._cache_file_suffix, cache_size)
 
     @abstractmethod
-    def convert(self, file_paths: list[Path] | list[str], force_recompute: bool = False) -> vaex.DataFrame:
+    def convert(
+        self, file_paths: list[Path] | list[str], cache_group: str | None = None, force_recompute: bool = False
+    ) -> vaex.DataFrame:
         """Abstract method to convert the input file paths to the desired output format.
 
         Args:
             file_paths: A list of input file paths to be converted.
+            cache_group: The cache group to use.
             force_recompute: If set to True, forces recomputation and ignores the cache.
 
         Returns:
             The resulting DataFrame after conversion.
         """
         raise NotImplementedError
```

### Comparing `mleko-0.5.0/mleko/dataset/convert/csv_to_vaex_converter.py` & `mleko-0.6.0/mleko/dataset/convert/csv_to_vaex_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,28 +113,31 @@
         self._na_values = tuple(na_values)
         self._true_values = tuple(true_values)
         self._false_values = tuple(false_values)
         self._downcast_float = downcast_float
         self._num_workers = num_workers
         self._random_state = random_state
 
-    def convert(self, file_paths: list[Path] | list[str], force_recompute: bool = False) -> vaex.DataFrame:
+    def convert(
+        self, file_paths: list[Path] | list[str], cache_group: str | None = None, force_recompute: bool = False
+    ) -> vaex.DataFrame:
         """Converts a list of CSV files to Arrow format and returns a `vaex` dataframe joined from the converted data.
 
         The method takes care of caching, and results will be reused accordingly unless `force_recompute`
         is set to True. The resulting dataframe is a `vaex` DataFrame joined from the converted data.
         The conversion is done in chunks to optimize parallel processing.
 
         Note:
             Will read the first `100,000/len(file_paths)` rows of each file to determine if the file is the same as the
             one in the cache. If the file is the same, the cache will be used. Otherwise, the file will be converted
             and the cache will be updated.
 
         Args:
             file_paths: A list of file paths to be converted.
+            cache_group: The cache group to use.
             force_recompute: If set to True, forces recomputation and ignores the cache.
 
         Returns:
             The resulting dataframe with the combined converted data.
         """
         return self._cached_execute(
             lambda_func=lambda: self._convert(file_paths),
@@ -145,14 +148,15 @@
                 self._drop_columns,
                 self._na_values,
                 self._true_values,
                 self._false_values,
                 self._downcast_float,
                 (file_paths, CSVFingerprinter(n_rows=100_000 // len(file_paths))),
             ],
+            cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
     @staticmethod
     def _convert_csv_file_to_arrow(
         file_path: Path | str,
         output_directory: Path,
```

### Comparing `mleko-0.5.0/mleko/dataset/feature_select/__init__.py` & `mleko-0.6.0/mleko/dataset/feature_select/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/dataset/feature_select/base_feature_selector.py` & `mleko-0.6.0/mleko/dataset/feature_select/base_feature_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,19 +61,22 @@
             logger.error(error_msg)
             raise ValueError(error_msg)
 
         self._features: tuple[str, ...] | None = tuple(features) if features is not None else None
         self._ignore_features: tuple[str, ...] = tuple(ignore_features) if ignore_features is not None else tuple()
 
     @abstractmethod
-    def select_features(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> vaex.DataFrame:
+    def select_features(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> vaex.DataFrame:
         """Selects features from the given DataFrame.
 
         Args:
             dataframe: DataFrame from which to select features.
+            cache_group: The cache group to use.
             force_recompute: Whether to force the feature selector to recompute its output, even if it already exists.
 
         Raises:
             NotImplementedError: Must be implemented in the child class that inherits from `BaseFeatureSelector`.
 
         Returns:
             A DataFrame with the selected features.
```

### Comparing `mleko-0.5.0/mleko/dataset/feature_select/composite_feature_selector.py` & `mleko-0.6.0/mleko/dataset/feature_select/composite_feature_selector.py`

 * *Files 9% similar despite different names*

```diff
@@ -74,27 +74,31 @@
             7    8    None
             8    9    None
             9   10    None
         """
         super().__init__(cache_directory, None, None, cache_size)
         self._feature_selectors = tuple(feature_selectors)
 
-    def select_features(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> vaex.DataFrame:
+    def select_features(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> vaex.DataFrame:
         """Selects the features from the DataFrame.
 
         Args:
             dataframe: DataFrame from which the features will be selected.
+            cache_group: The cache group to use for caching.
             force_recompute: If True, the features will be recomputed even if they are cached.
 
         Returns:
             DataFrame with the selected features.
         """
         return self._cached_execute(
             lambda_func=lambda: self._select_features(dataframe),
             cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
+            cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
     def _select_features(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
         """Selects the features from the DataFrame.
 
         Args:
```

### Comparing `mleko-0.5.0/mleko/dataset/feature_select/invariance_feature_selector.py` & `mleko-0.6.0/mleko/dataset/feature_select/invariance_feature_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,30 +62,34 @@
             ... )
             >>> df_selected = selector.select_features(df)
             >>> df_selected.get_column_names()
             ['a', 'c', 'd']
         """
         super().__init__(cache_directory, features, ignore_features, cache_size)
 
-    def select_features(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> vaex.DataFrame:
+    def select_features(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> vaex.DataFrame:
         """Selects features based on invariance.
 
         Args:
             dataframe: The DataFrame to select features from.
+            cache_group: The cache group to use for caching.
             force_recompute: Whether to force recompute the selected features.
 
         Returns:
             The DataFrame with the selected features.
         """
         return self._cached_execute(
             lambda_func=lambda: self._select_features(dataframe),
             cache_keys=[
                 self._fingerprint(),
                 (dataframe, VaexFingerprinter()),
             ],
+            cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
     def _select_features(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
         """Selects features based on invariance.
 
         Args:
```

### Comparing `mleko-0.5.0/mleko/dataset/feature_select/missing_rate_feature_selector.py` & `mleko-0.6.0/mleko/dataset/feature_select/missing_rate_feature_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,29 +65,33 @@
             ...     missing_rate_threshold=0.3,
             ... ).select_features(df).get_column_names()
             ['a', 'b']
         """
         super().__init__(cache_directory, features, ignore_features, cache_size)
         self._missing_rate_threshold = missing_rate_threshold
 
-    def select_features(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> vaex.DataFrame:
+    def select_features(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> vaex.DataFrame:
         """Selects features based on the missing rate.
 
         Will cache the result of the feature selection.
 
         Args:
             dataframe: The DataFrame to select features from.
+            cache_group: The cache group to use.
             force_recompute: Whether to force recompute the feature selection.
 
         Returns:
             The DataFrame with the selected features.
         """
         return self._cached_execute(
             lambda_func=lambda: self._select_features(dataframe),
             cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
+            cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
     def _select_features(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
         """Selects features based on the missing rate.
 
         Args:
```

### Comparing `mleko-0.5.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py` & `mleko-0.6.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,27 +68,31 @@
             >>> selected_features = feature_selector.select_features(df)
             >>> selected_features.get_column_names()
             ['a', 'c']
         """
         super().__init__(cache_directory, features, ignore_features, cache_size)
         self._correlation_threshold = correlation_threshold
 
-    def select_features(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> vaex.DataFrame:
+    def select_features(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> vaex.DataFrame:
         """Selects features based on the Pearson correlation.
 
         Args:
             dataframe: The DataFrame to select features from.
+            cache_group: The cache group to use.
             force_recompute: Whether to force recompute the selected features.
 
         Returns:
             The DataFrame with the selected features.
         """
         return self._cached_execute(
             lambda_func=lambda: self._select_features(dataframe),
             cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
+            cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
     def _select_features(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
         """Selects features based on the Pearson correlation.
 
         Args:
```

### Comparing `mleko-0.5.0/mleko/dataset/feature_select/variance_feature_selector.py` & `mleko-0.6.0/mleko/dataset/feature_select/variance_feature_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,30 +68,34 @@
             >>> df_selected = selector.select_features(df)
             >>> df_selected.get_column_names()
             ['a', 'c', 'd']
         """
         super().__init__(cache_directory, features, ignore_features, cache_size)
         self._variance_threshold = variance_threshold
 
-    def select_features(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> vaex.DataFrame:
+    def select_features(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> vaex.DataFrame:
         """Selects features based on the variance.
 
         Args:
             dataframe: The DataFrame to select features from.
+            cache_group: The cache group to use.
             force_recompute: Whether to force recompute the selected features.
 
         Returns:
             The DataFrame with the selected features.
         """
         return self._cached_execute(
             lambda_func=lambda: self._select_features(dataframe),
             cache_keys=[
                 self._fingerprint(),
                 (dataframe, VaexFingerprinter()),
             ],
+            cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
     def _select_features(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
         """Selects features based on the variance.
 
         Args:
```

### Comparing `mleko-0.5.0/mleko/dataset/ingest/__init__.py` & `mleko-0.6.0/mleko/dataset/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/dataset/ingest/base_ingester.py` & `mleko-0.6.0/mleko/dataset/ingest/base_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/dataset/ingest/kaggle_ingester.py` & `mleko-0.6.0/mleko/dataset/ingest/kaggle_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/dataset/ingest/s3_ingester.py` & `mleko-0.6.0/mleko/dataset/ingest/s3_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/dataset/split/__init__.py` & `mleko-0.6.0/mleko/dataset/split/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/dataset/split/base_splitter.py` & `mleko-0.6.0/mleko/dataset/split/base_splitter.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,18 +22,21 @@
         Args:
             cache_directory: The target directory where the split dataframes are to be saved.
             cache_size: The maximum number of cache entries.
         """
         LRUCacheMixin.__init__(self, cache_directory, self._cache_file_suffix, cache_size)
 
     @abstractmethod
-    def split(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> tuple[vaex.DataFrame, vaex.DataFrame]:
+    def split(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> tuple[vaex.DataFrame, vaex.DataFrame]:
         """Abstract method to split the given dataframe into two parts.
 
         Args:
             dataframe: The dataframe to be split.
+            cache_group: The cache group to use.
             force_recompute: Forces recomputation if True, otherwise reads from the cache if available.
 
         Returns:
             A tuple containing the split dataframes.
         """
         raise NotImplementedError
```

### Comparing `mleko-0.5.0/mleko/dataset/split/expression_splitter.py` & `mleko-0.6.0/mleko/dataset/split/expression_splitter.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,30 +57,34 @@
             >>> df_test
                 #    x    y
                 0    1    4
         """
         super().__init__(cache_directory, cache_size)
         self._expression = expression
 
-    def split(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> tuple[vaex.DataFrame, vaex.DataFrame]:
+    def split(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> tuple[vaex.DataFrame, vaex.DataFrame]:
         """Split the given dataframe into two parts.
 
         Args:
             dataframe: The dataframe to be split.
+            cache_group: The cache group to use.
             force_recompute: Forces recomputation if True, otherwise reads from the cache if available.
 
         Returns:
             A tuple containing the split dataframes.
         """
         return self._cached_execute(  # type: ignore
             lambda_func=lambda: self._split(dataframe),
             cache_keys=[
                 self._expression,
                 (dataframe, VaexFingerprinter()),
             ],
+            cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
     def _split(self, dataframe: vaex.DataFrame) -> tuple[vaex.DataFrame, vaex.DataFrame]:
         """Split the given dataframe into two parts.
 
         Args:
```

### Comparing `mleko-0.5.0/mleko/dataset/split/random_splitter.py` & `mleko-0.6.0/mleko/dataset/split/random_splitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,37 +74,41 @@
         """
         super().__init__(cache_directory, cache_size)
         self._idx2_size = [split / sum(data_split) for split in data_split][1]
         self._shuffle = shuffle
         self._stratify = stratify
         self._random_state = random_state
 
-    def split(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> tuple[vaex.DataFrame, vaex.DataFrame]:
+    def split(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> tuple[vaex.DataFrame, vaex.DataFrame]:
         """Split the given dataframe into two parts.
 
         Splits the dataframe into train and test sets according to the proportions, shuffle,
         stratification, and random state provided during initializing the splitter. Will read from the cache if
         available, unless `force_recompute=True`.
 
         Args:
             dataframe: The dataframe to be split.
+            cache_group: The cache group to use.
             force_recompute: Whether to force recompute the split, even if the cache is available.
 
         Returns:
             A tuple containing the split dataframes.
         """
         return self._cached_execute(  # type: ignore
             lambda_func=lambda: self._split(dataframe),
             cache_keys=[
                 self._idx2_size,
                 self._shuffle,
                 self._stratify,
                 self._random_state,
                 (dataframe, VaexFingerprinter()),
             ],
+            cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
     def _split(self, dataframe: vaex.DataFrame) -> tuple[vaex.DataFrame, vaex.DataFrame]:
         """Split the given dataframe into two parts.
 
         Args:
```

### Comparing `mleko-0.5.0/mleko/dataset/transform/__init__.py` & `mleko-0.6.0/mleko/dataset/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/dataset/transform/base_transformer.py` & `mleko-0.6.0/mleko/dataset/transform/base_transformer.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,19 +36,22 @@
             features: List of feature names to be used by the transformer.
             cache_size: The maximum number of cache entries to keep in the cache.
         """
         LRUCacheMixin.__init__(self, cache_directory, self._cache_file_suffix, cache_size)
         self._features: tuple[str, ...] = tuple(features)
 
     @abstractmethod
-    def transform(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> vaex.DataFrame:
+    def transform(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> vaex.DataFrame:
         """Transfigures the specified features in the DataFrame.
 
         Args:
             dataframe: DataFrame to be transformed.
+            cache_group: The cache group to use.
             force_recompute: Whether to force the transformation to be recomputed even if the result is cached.
 
         Raises:
             NotImplementedError: Must be implemented by subclasses.
 
         Returns:
             Transformed DataFrame.
```

### Comparing `mleko-0.5.0/mleko/dataset/transform/composite_transformer.py` & `mleko-0.6.0/mleko/dataset/transform/composite_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,27 +70,31 @@
             [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
             >>> df["b"].tolist()
             [0.4, 0.4, 0.4, 0.4, nan, nan, nan, nan, nan, nan]
         """
         super().__init__(cache_directory, [], cache_size)
         self._transformers = tuple(transformers)
 
-    def transform(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> vaex.DataFrame:
+    def transform(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> vaex.DataFrame:
         """Transforms the DataFrame using the transformers in the order they are specified.
 
         Args:
             dataframe: The DataFrame to transform.
+            cache_group: The cache group to use.
             force_recompute: Whether to force the recomputation of the transformation.
 
         Returns:
             The transformed DataFrame.
         """
         return self._cached_execute(
             lambda_func=lambda: self._transform(dataframe),
             cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
+            cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
     def _transform(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
         """Returns the transformed DataFrame.
 
         Args:
```

### Comparing `mleko-0.5.0/mleko/dataset/transform/frequency_encoder_transformer.py` & `mleko-0.6.0/mleko/dataset/transform/frequency_encoder_transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,29 +63,33 @@
             [0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1]
             >>> df["b"].tolist()
             [0.4, 0.4, 0.4, 0.4, nan, nan, nan, nan, nan, nan]
         """
         super().__init__(cache_directory, features, cache_size)
         self._unseen_strategy = unseen_strategy
 
-    def transform(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> vaex.DataFrame:
+    def transform(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> vaex.DataFrame:
         """Transforms the features in the DataFrame using frequency encoding.
 
         Will cache the resulting DataFrame in the cache directory.
 
         Args:
             dataframe: The DataFrame to transform.
+            cache_group: The cache group to use.
             force_recompute: Whether to force recomputing the transformation.
 
         Returns:
             The transformed DataFrame.
         """
         return self._cached_execute(
             lambda_func=lambda: self._transform(dataframe),
             cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
+            cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
     def _transform(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
         """Transforms the features in the DataFrame using frequency encoding.
 
         Args:
```

### Comparing `mleko-0.5.0/mleko/dataset/transform/label_encoder_transformer.py` & `mleko-0.6.0/mleko/dataset/transform/label_encoder_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,29 +61,33 @@
             [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
             >>> df["b"].tolist()
             [1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
         """
         super().__init__(cache_directory, features, cache_size)
         self._allow_unseen = allow_unseen
 
-    def transform(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> vaex.DataFrame:
+    def transform(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> vaex.DataFrame:
         """Transforms the features of the given DataFrame using label encoding.
 
         Will cache the resulting DataFrame in the cache directory.
 
         Args:
             dataframe: The DataFrame to transform.
+            cache_group: The cache group to use.
             force_recompute: Whether to force recomputation of the transformation.
 
         Returns:
             The transformed DataFrame.
         """
         return self._cached_execute(
             lambda_func=lambda: self._transform(dataframe),
             cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
+            cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
     def _transform(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
         """Transforms the features of the given DataFrame using label encoding.
 
         Args:
```

### Comparing `mleko-0.5.0/mleko/dataset/transform/max_abs_scaler_transformer.py` & `mleko-0.6.0/mleko/dataset/transform/max_abs_scaler_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,29 +56,33 @@
             >>> df["a"].tolist()
             [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]
             >>> df["b"].tolist()
             [-0.2, -0.4, -0.6, -0.8, -1.0, 0.0, 0.2, 0.4, 0.6, 0.8]
         """
         super().__init__(cache_directory, features, cache_size)
 
-    def transform(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> vaex.DataFrame:
+    def transform(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> vaex.DataFrame:
         """Transforms the features in the DataFrame using maximum absolute scaling.
 
         Will cache the resulting DataFrame in the cache directory.
 
         Args:
             dataframe: The DataFrame to transform.
+            cache_group: The cache group to use.
             force_recompute: Whether to force recomputing the transformation.
 
         Returns:
             The transformed DataFrame.
         """
         return self._cached_execute(
             lambda_func=lambda: self._transform(dataframe),
             cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
+            cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
     def _transform(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
         """Transforms the features in the DataFrame using maximum absolute scaling.
 
         Args:
```

### Comparing `mleko-0.5.0/mleko/dataset/transform/min_max_scaler_transformer.py` & `mleko-0.6.0/mleko/dataset/transform/min_max_scaler_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,29 +62,33 @@
             >>> df["b"].tolist()
             [-0.2, -0.4, -0.6, -0.8, -1.0, 0.0, 0.2, 0.4, 0.6, 0.8]
         """
         super().__init__(cache_directory, features, cache_size)
         self._min_value = min_value
         self._max_value = max_value
 
-    def transform(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> vaex.DataFrame:
+    def transform(
+        self, dataframe: vaex.DataFrame, cache_group: str | None = None, force_recompute: bool = False
+    ) -> vaex.DataFrame:
         """Transforms the features in the DataFrame using min max scaling.
 
         Will cache the resulting DataFrame in the cache directory.
 
         Args:
             dataframe: The DataFrame to transform.
+            cache_group: The cache group to use.
             force_recompute: Whether to force recomputing the transformation.
 
         Returns:
             The transformed DataFrame.
         """
         return self._cached_execute(
             lambda_func=lambda: self._transform(dataframe),
             cache_keys=[self._fingerprint(), (dataframe, VaexFingerprinter())],
+            cache_group=cache_group,
             force_recompute=force_recompute,
         )
 
     def _transform(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
         """Transforms the features in the DataFrame using min max scaling.
 
         Args:
```

### Comparing `mleko-0.5.0/mleko/pipeline/__init__.py` & `mleko-0.6.0/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/pipeline/data_container.py` & `mleko-0.6.0/mleko/pipeline/data_container.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/pipeline/pipeline.py` & `mleko-0.6.0/mleko/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/pipeline/pipeline_step.py` & `mleko-0.6.0/mleko/pipeline/pipeline_step.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,25 +27,28 @@
     """Number of inputs expected by the PipelineStep."""
 
     _num_outputs: int
     """Number of outputs expected by the PipelineStep."""
 
     def __init__(
         self,
-        inputs: list[str] | tuple[str, ...] | tuple[()] = (),
-        outputs: list[str] | tuple[str, ...] | tuple[()] = (),
+        inputs: list[str] | tuple[str, ...] | tuple[()],
+        outputs: list[str] | tuple[str, ...] | tuple[()],
+        cache_group: str | None,
     ) -> None:
         """Initialize a new PipelineStep with the provided input and output keys.
 
         Args:
             inputs: List or tuple of input keys expected by this step.
             outputs: List or tuple of output keys produced by this step.
+            cache_group: The cache group to use.
         """
-        self.inputs = tuple(inputs)
-        self.outputs = tuple(outputs)
+        self._inputs = tuple(inputs)
+        self._outputs = tuple(outputs)
+        self._cache_group = cache_group
 
         self._validate_inputs()
         self._validate_outputs()
 
     @abstractmethod
     def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
         """Execute the data processing operation associated with this pipeline step.
@@ -68,18 +71,18 @@
 
     def _validate_inputs(self) -> None:
         """Check the input keys for compliance with this step's requirements.
 
         Raises:
             ValueError: If the PipelineStep has an invalid number of inputs.
         """
-        if len(self.inputs) != self._num_inputs:
+        if len(self._inputs) != self._num_inputs:
             raise ValueError(f"{self.__class__.__name__} must have exactly {self._num_inputs} input(s).")
 
     def _validate_outputs(self) -> None:
         """Check the output keys for compliance with this step's requirements.
 
         Raises:
             ValueError: If the PipelineStep has an invalid number of outputs.
         """
-        if len(self.outputs) != self._num_outputs:
+        if len(self._outputs) != self._num_outputs:
             raise ValueError(f"{self.__class__.__name__} must have exactly {self._num_outputs} output(s).")
```

### Comparing `mleko-0.5.0/mleko/pipeline/steps/__init__.py` & `mleko-0.6.0/mleko/pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/pipeline/steps/convert_step.py` & `mleko-0.6.0/mleko/pipeline/steps/convert_step.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,23 +24,25 @@
 
     @auto_repr
     def __init__(
         self,
         converter: BaseConverter,
         inputs: list[str] | tuple[str, ...] | tuple[()] = (),
         outputs: list[str] | tuple[str, ...] | tuple[()] = (),
+        cache_group: str | None = None,
     ) -> None:
         """Initialize the ConvertStep with the specified data converter.
 
         Args:
             converter: The DataConverter responsible for handling data format conversion.
             inputs: List or tuple of input keys expected by this step.
             outputs: List or tuple of output keys produced by this step.
+            cache_group: The cache group to use.
         """
-        super().__init__(inputs, outputs)
+        super().__init__(inputs, outputs, cache_group)
         self._converter = converter
 
     def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
         """Perform data format conversion using the configured converter.
 
         Args:
             data_container: Contains a list of file Paths to be converted.
@@ -48,14 +50,14 @@
 
         Raises:
             ValueError: If data container contains invalid data - not a list of Paths.
 
         Returns:
             A DataContainer containing the converted data as a vaex dataframe.
         """
-        file_paths = data_container.data[self.inputs[0]]
+        file_paths = data_container.data[self._inputs[0]]
         if not isinstance(file_paths, list) or not all(isinstance(e, Path) for e in file_paths):
             raise ValueError
 
-        df = self._converter.convert(file_paths, force_recompute)
-        data_container.data[self.outputs[0]] = df
+        df = self._converter.convert(file_paths, self._cache_group, force_recompute)
+        data_container.data[self._outputs[0]] = df
         return data_container
```

### Comparing `mleko-0.5.0/mleko/pipeline/steps/feature_select_step.py` & `mleko-0.6.0/mleko/pipeline/steps/feature_select_step.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,23 +20,25 @@
 
     @auto_repr
     def __init__(
         self,
         feature_selector: BaseFeatureSelector,
         inputs: list[str] | tuple[str, ...] | tuple[()] = (),
         outputs: list[str] | tuple[str, ...] | tuple[()] = (),
+        cache_group: str | None = None,
     ) -> None:
         """Initialize the FeatureSelectStep with the specified feature selector.
 
         Args:
             feature_selector: The FeatureSelector responsible for handling feature selection.
             inputs: List or tuple of input keys expected by this step.
             outputs: List or tuple of output keys produced by this step.
+            cache_group: The cache group to use.
         """
-        super().__init__(inputs, outputs)
+        super().__init__(inputs, outputs, cache_group)
         self._feature_selector = feature_selector
 
     def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
         """Perform feature selection using the configured feature selector.
 
         Args:
             data_container: Contains the input DataFrame.
@@ -44,14 +46,14 @@
 
         Raises:
             ValueError: If data container contains invalid data - not a vaex DataFrame.
 
         Returns:
             A DataContainer containing the selected features as a vaex DataFrame.
         """
-        dataframe = data_container.data[self.inputs[0]]
+        dataframe = data_container.data[self._inputs[0]]
         if not isinstance(dataframe, DataFrame):
             raise ValueError
 
-        df = self._feature_selector.select_features(dataframe, force_recompute)
-        data_container.data[self.outputs[0]] = df
+        df = self._feature_selector.select_features(dataframe, self._cache_group, force_recompute)
+        data_container.data[self._outputs[0]] = df
         return data_container
```

### Comparing `mleko-0.5.0/mleko/pipeline/steps/ingest_step.py` & `mleko-0.6.0/mleko/pipeline/steps/ingest_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,23 +31,23 @@
         """Initialize the IngestStep with the specified data source.
 
         Args:
             ingester: The data source from which to fetch the data, a BaseIngester instance.
             inputs: List or tuple of input keys expected by this step.
             outputs: List or tuple of output keys produced by this step.
         """
-        super().__init__(inputs, outputs)
+        super().__init__(inputs, outputs, None)
         self._ingester = ingester
 
     def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
         """Fetch data from the configured data source and return a DataContainer with fetched files.
 
         Args:
             data_container: Input data for this step's processing operation.
             force_recompute: Whether to force the step to recompute its output, even if it already exists.
 
         Returns:
             DataContainer: A DataContainer containing a list of fetched files.
         """
         files = self._ingester.fetch_data(force_recompute)
-        data_container.data[self.outputs[0]] = files
+        data_container.data[self._outputs[0]] = files
         return data_container
```

### Comparing `mleko-0.5.0/mleko/pipeline/steps/split_step.py` & `mleko-0.6.0/mleko/pipeline/steps/split_step.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,23 +24,25 @@
 
     @auto_repr
     def __init__(
         self,
         splitter: BaseSplitter,
         inputs: list[str] | tuple[str, ...] | tuple[()] = (),
         outputs: list[str] | tuple[str, ...] | tuple[()] = (),
+        cache_group: str | None = None,
     ) -> None:
         """Initialize the SplitStep with the specified data splitter.
 
         Args:
             splitter: The DataSplitter responsible for handling data splitting.
             inputs: List or tuple of input keys expected by this step.
             outputs: List or tuple of output keys produced by this step.
+            cache_group: The cache group to use.
         """
-        super().__init__(inputs, outputs)
+        super().__init__(inputs, outputs, cache_group)
         self._splitter = splitter
 
     def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
         """Perform data splitting using the configured splitter.
 
         Args:
             data_container: Contains the DataFrame to be split.
@@ -48,15 +50,15 @@
 
         Raises:
             ValueError: If data container contains invalid data - not a vaex DataFrame.
 
         Returns:
             A DataContainer containing the split data as two vaex DataFrames.
         """
-        dataframe = data_container.data[self.inputs[0]]
+        dataframe = data_container.data[self._inputs[0]]
         if not isinstance(dataframe, DataFrame):
             raise ValueError
 
-        df1, df2 = self._splitter.split(dataframe, force_recompute)
-        data_container.data[self.outputs[0]] = df1
-        data_container.data[self.outputs[1]] = df2
+        df1, df2 = self._splitter.split(dataframe, self._cache_group, force_recompute)
+        data_container.data[self._outputs[0]] = df1
+        data_container.data[self._outputs[1]] = df2
         return data_container
```

### Comparing `mleko-0.5.0/mleko/pipeline/steps/transform_step.py` & `mleko-0.6.0/mleko/pipeline/steps/transform_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,23 +20,25 @@
 
     @auto_repr
     def __init__(
         self,
         transformer: BaseTransformer,
         inputs: list[str] | tuple[str, ...] | tuple[()] = (),
         outputs: list[str] | tuple[str, ...] | tuple[()] = (),
+        cache_group: str | None = None,
     ) -> None:
         """Initialize the TransformStep with the specified transformer.
 
         Args:
             transformer: The Transformer responsible for handling feature transformation.
             inputs: List or tuple of input keys expected by this step.
             outputs: List or tuple of output keys produced by this step.
+            cache_group: The cache group to use.
         """
-        super().__init__(inputs, outputs)
+        super().__init__(inputs, outputs, cache_group)
         self._transformer = transformer
 
     def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
         """Perform transformation using the configured transformer.
 
         Args:
             data_container: Contains the input DataFrame.
@@ -44,14 +46,14 @@
 
         Raises:
             ValueError: If data container contains invalid data - not a vaex DataFrame.
 
         Returns:
             A DataContainer containing the selected features as a vaex DataFrame.
         """
-        dataframe = data_container.data[self.inputs[0]]
+        dataframe = data_container.data[self._inputs[0]]
         if not isinstance(dataframe, DataFrame):
             raise ValueError
 
-        df = self._transformer.transform(dataframe, force_recompute)
-        data_container.data[self.outputs[0]] = df
+        df = self._transformer.transform(dataframe, self._cache_group, force_recompute)
+        data_container.data[self._outputs[0]] = df
         return data_container
```

### Comparing `mleko-0.5.0/mleko/utils/__init__.py` & `mleko-0.6.0/mleko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/utils/custom_logger.py` & `mleko-0.6.0/mleko/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/utils/decorators.py` & `mleko-0.6.0/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/utils/file_helpers.py` & `mleko-0.6.0/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/utils/tqdm_helpers.py` & `mleko-0.6.0/mleko/utils/tqdm_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/mleko/utils/vaex_helpers.py` & `mleko-0.6.0/mleko/utils/vaex_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.5.0/pyproject.toml` & `mleko-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "0.5.0"
+version = "0.6.0"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ErikBavenstrand/mleko"
 repository = "https://github.com/ErikBavenstrand/mleko"
 documentation = "https://mleko.readthedocs.io"
```

### Comparing `mleko-0.5.0/PKG-INFO` & `mleko-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 0.5.0
+Version: 0.6.0
 Summary: ML-Ekosystem
 Home-page: https://github.com/ErikBavenstrand/mleko
 License: MIT
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: Development Status :: 3 - Alpha
```

