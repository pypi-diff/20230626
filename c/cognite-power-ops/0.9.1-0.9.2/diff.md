# Comparing `tmp/cognite_power_ops-0.9.1.tar.gz` & `tmp/cognite_power_ops-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_power_ops-0.9.1.tar", max compression
+gzip compressed data, was "cognite_power_ops-0.9.2.tar", max compression
```

## Comparing `cognite_power_ops-0.9.1.tar` & `cognite_power_ops-0.9.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    10758 2023-05-26 10:41:33.311287 cognite_power_ops-0.9.1/LICENSE
--rw-r--r--   0        0        0      250 2023-05-26 10:41:33.311287 cognite_power_ops-0.9.1/README.md
--rw-r--r--   0        0        0      192 2023-05-26 10:41:33.311287 cognite_power_ops-0.9.1/cognite/powerops/__init__.py
--rw-r--r--   0        0        0    10348 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/bootstrap.py
--rw-r--r--   0        0        0       23 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/case/__init__.py
--rw-r--r--   0        0        0     3869 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/case/case.py
--rw-r--r--   0        0        0       65 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/client/__init__.py
--rw-r--r--   0        0        0     6202 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/client/asset_apis.py
--rw-r--r--   0        0        0      601 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/client/config_client.py
--rw-r--r--   0        0        0        0 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/client/dm/__init__.py
--rw-r--r--   0        0        0     1857 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/client/dm/client.py
--rw-r--r--   0        0        0      895 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/client/dm/schema.graphql
--rw-r--r--   0        0        0     2037 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/client/dm/schema.py
--rw-r--r--   0        0        0     1883 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/client/dm_apis.py
--rw-r--r--   0        0        0     2281 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/client/powerops_client.py
--rw-r--r--   0        0        0     2990 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/client/shop_api.py
--rw-r--r--   0        0        0    33429 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/config.py
--rw-r--r--   0        0        0        0 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/__init__.py
--rw-r--r--   0        0        0     1220 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/asset_lists.py
--rw-r--r--   0        0        0    13238 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/cdf_resource_collection.py
--rw-r--r--   0        0        0     2513 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/common.py
--rw-r--r--   0        0        0      129 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/config_model.py
--rw-r--r--   0        0        0     3630 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/core.py
--rw-r--r--   0        0        0     2361 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/generator.py
--rw-r--r--   0        0        0    16336 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/plant.py
--rw-r--r--   0        0        0       99 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/price_area.py
--rw-r--r--   0        0        0     5114 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/reserve_scenario.py
--rw-r--r--   0        0        0      180 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/reservoirs.py
--rw-r--r--   0        0        0      163 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/shared.py
--rw-r--r--   0        0        0     2171 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/shop_file_config.py
--rw-r--r--   0        0        0     2815 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/shop_output_definition.py
--rw-r--r--   0        0        0     9189 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/time_series_mapping.py
--rw-r--r--   0        0        0     1144 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/data_classes/transformation.py
--rw-r--r--   0        0        0     1042 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/logger.py
--rw-r--r--   0        0        0     2070 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/main.py
--rw-r--r--   0        0        0        0 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/__init__.py
--rw-r--r--   0        0        0     1936 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/asset_types.py
--rw-r--r--   0        0        0     1323 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/cdf_auth.py
--rw-r--r--   0        0        0     2724 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/cdf_utils.py
--rw-r--r--   0        0        0      744 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/common.py
--rw-r--r--   0        0        0      324 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/constants.py
--rw-r--r--   0        0        0     3271 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/files.py
--rw-r--r--   0        0        0     5039 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/labels.py
--rw-r--r--   0        0        0     1766 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/mapping/mapping.py
--rw-r--r--   0        0        0     2609 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/mapping/static_mapping.py
--rw-r--r--   0        0        0     3165 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/powerops_asset_hierarchy.py
--rw-r--r--   0        0        0      718 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/powerops_status_events.py
--rw-r--r--   0        0        0     4495 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/relationship_types.py
--rw-r--r--   0        0        0    12598 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/resource_generation.py
--rw-r--r--   0        0        0     1495 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/utils/serializer.py
--rw-r--r--   0        0        0       22 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/cognite/powerops/version.py
--rw-r--r--   0        0        0     1516 2023-05-26 10:41:33.315287 cognite_power_ops-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 cognite_power_ops-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/LICENSE
+-rw-r--r--   0        0        0      250 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/README.md
+-rw-r--r--   0        0        0      192 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/__init__.py
+-rw-r--r--   0        0        0    10361 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/bootstrap.py
+-rw-r--r--   0        0        0       23 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/case/__init__.py
+-rw-r--r--   0        0        0     3869 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/case/case.py
+-rw-r--r--   0        0        0       65 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/client/__init__.py
+-rw-r--r--   0        0        0     6202 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/client/asset_apis.py
+-rw-r--r--   0        0        0      601 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/client/config_client.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/client/dm/__init__.py
+-rw-r--r--   0        0        0     1857 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/client/dm/client.py
+-rw-r--r--   0        0        0      895 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/client/dm/schema.graphql
+-rw-r--r--   0        0        0     2037 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/client/dm/schema.py
+-rw-r--r--   0        0        0     1883 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/client/dm_apis.py
+-rw-r--r--   0        0        0     2281 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/client/powerops_client.py
+-rw-r--r--   0        0        0     2990 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/client/shop_api.py
+-rw-r--r--   0        0        0    33429 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/config.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/__init__.py
+-rw-r--r--   0        0        0     1220 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/asset_lists.py
+-rw-r--r--   0        0        0    13238 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/cdf_resource_collection.py
+-rw-r--r--   0        0        0     2513 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/common.py
+-rw-r--r--   0        0        0      129 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/config_model.py
+-rw-r--r--   0        0        0     3630 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/core.py
+-rw-r--r--   0        0        0     2361 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/generator.py
+-rw-r--r--   0        0        0    16336 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/plant.py
+-rw-r--r--   0        0        0       99 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/price_area.py
+-rw-r--r--   0        0        0     5114 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/reserve_scenario.py
+-rw-r--r--   0        0        0      180 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/reservoirs.py
+-rw-r--r--   0        0        0      163 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/shared.py
+-rw-r--r--   0        0        0     2171 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/shop_file_config.py
+-rw-r--r--   0        0        0     2815 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/shop_output_definition.py
+-rw-r--r--   0        0        0     9189 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/time_series_mapping.py
+-rw-r--r--   0        0        0     1144 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/data_classes/transformation.py
+-rw-r--r--   0        0        0     1042 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/logger.py
+-rw-r--r--   0        0        0     2070 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/main.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/__init__.py
+-rw-r--r--   0        0        0     1936 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/asset_types.py
+-rw-r--r--   0        0        0     1323 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/cdf_auth.py
+-rw-r--r--   0        0        0     2724 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/cdf_utils.py
+-rw-r--r--   0        0        0      744 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/common.py
+-rw-r--r--   0        0        0      324 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/constants.py
+-rw-r--r--   0        0        0     3271 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/files.py
+-rw-r--r--   0        0        0     5039 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/labels.py
+-rw-r--r--   0        0        0     1766 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/mapping/mapping.py
+-rw-r--r--   0        0        0     2609 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/mapping/static_mapping.py
+-rw-r--r--   0        0        0     3165 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/powerops_asset_hierarchy.py
+-rw-r--r--   0        0        0      718 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/powerops_status_events.py
+-rw-r--r--   0        0        0     4495 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/relationship_types.py
+-rw-r--r--   0        0        0    12598 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/resource_generation.py
+-rw-r--r--   0        0        0     1495 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/utils/serializer.py
+-rw-r--r--   0        0        0       22 2023-05-30 08:49:13.694296 cognite_power_ops-0.9.2/cognite/powerops/version.py
+-rw-r--r--   0        0        0     1516 2023-05-30 08:49:13.698296 cognite_power_ops-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 cognite_power_ops-0.9.2/PKG-INFO
```

### Comparing `cognite_power_ops-0.9.1/LICENSE` & `cognite_power_ops-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/bootstrap.py` & `cognite_power_ops-0.9.2/cognite/powerops/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         else "https://shop-staging.az-inso-powerops.cognite.ai/submit-run"
     )
 
 
 def _load_config(path: Path) -> BootstrapConfig:
     config = BootstrapConfig.from_yamls(path)
     if os.environ.get("COGNITE_PROJECT"):
-        config.cdf.from_env()
+        config.cdf = config.cdf.from_env()
     return config
 
 
 def _transform(
     config: BootstrapConfig,
     path: Path,
     market: str = "Dayahead",
```

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/case/case.py` & `cognite_power_ops-0.9.2/cognite/powerops/case/case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/client/asset_apis.py` & `cognite_power_ops-0.9.2/cognite/powerops/client/asset_apis.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/client/config_client.py` & `cognite_power_ops-0.9.2/cognite/powerops/client/config_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/client/dm/client.py` & `cognite_power_ops-0.9.2/cognite/powerops/client/dm/client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/client/dm/schema.graphql` & `cognite_power_ops-0.9.2/cognite/powerops/client/dm/schema.graphql`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/client/dm/schema.py` & `cognite_power_ops-0.9.2/cognite/powerops/client/dm/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/client/dm_apis.py` & `cognite_power_ops-0.9.2/cognite/powerops/client/dm_apis.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/client/powerops_client.py` & `cognite_power_ops-0.9.2/cognite/powerops/client/powerops_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/client/shop_api.py` & `cognite_power_ops-0.9.2/cognite/powerops/client/shop_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/config.py` & `cognite_power_ops-0.9.2/cognite/powerops/config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/data_classes/asset_lists.py` & `cognite_power_ops-0.9.2/cognite/powerops/data_classes/asset_lists.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/data_classes/cdf_resource_collection.py` & `cognite_power_ops-0.9.2/cognite/powerops/data_classes/cdf_resource_collection.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/data_classes/common.py` & `cognite_power_ops-0.9.2/cognite/powerops/data_classes/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/data_classes/core.py` & `cognite_power_ops-0.9.2/cognite/powerops/data_classes/core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/data_classes/generator.py` & `cognite_power_ops-0.9.2/cognite/powerops/data_classes/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/data_classes/plant.py` & `cognite_power_ops-0.9.2/cognite/powerops/data_classes/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/data_classes/reserve_scenario.py` & `cognite_power_ops-0.9.2/cognite/powerops/data_classes/reserve_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/data_classes/shop_file_config.py` & `cognite_power_ops-0.9.2/cognite/powerops/data_classes/shop_file_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/data_classes/shop_output_definition.py` & `cognite_power_ops-0.9.2/cognite/powerops/data_classes/shop_output_definition.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/data_classes/time_series_mapping.py` & `cognite_power_ops-0.9.2/cognite/powerops/data_classes/time_series_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/data_classes/transformation.py` & `cognite_power_ops-0.9.2/cognite/powerops/data_classes/transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/logger.py` & `cognite_power_ops-0.9.2/cognite/powerops/logger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/main.py` & `cognite_power_ops-0.9.2/cognite/powerops/main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/utils/asset_types.py` & `cognite_power_ops-0.9.2/cognite/powerops/utils/asset_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/utils/cdf_auth.py` & `cognite_power_ops-0.9.2/cognite/powerops/utils/cdf_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/utils/cdf_utils.py` & `cognite_power_ops-0.9.2/cognite/powerops/utils/cdf_utils.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/utils/common.py` & `cognite_power_ops-0.9.2/cognite/powerops/utils/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/utils/files.py` & `cognite_power_ops-0.9.2/cognite/powerops/utils/files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/utils/labels.py` & `cognite_power_ops-0.9.2/cognite/powerops/utils/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/utils/mapping/mapping.py` & `cognite_power_ops-0.9.2/cognite/powerops/utils/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/utils/mapping/static_mapping.py` & `cognite_power_ops-0.9.2/cognite/powerops/utils/mapping/static_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/utils/powerops_asset_hierarchy.py` & `cognite_power_ops-0.9.2/cognite/powerops/utils/powerops_asset_hierarchy.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/utils/powerops_status_events.py` & `cognite_power_ops-0.9.2/cognite/powerops/utils/powerops_status_events.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/utils/relationship_types.py` & `cognite_power_ops-0.9.2/cognite/powerops/utils/relationship_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/utils/resource_generation.py` & `cognite_power_ops-0.9.2/cognite/powerops/utils/resource_generation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/cognite/powerops/utils/serializer.py` & `cognite_power_ops-0.9.2/cognite/powerops/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.9.1/pyproject.toml` & `cognite_power_ops-0.9.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-power-ops"
-version = "0.9.1"
+version = "0.9.2"
 description = "SDK for power markets operations on Cognite Data Fusion"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache 2.0"
 packages = [{include = "cognite", from = "."}]
 
 [tool.black]
```

### Comparing `cognite_power_ops-0.9.1/PKG-INFO` & `cognite_power_ops-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-power-ops
-Version: 0.9.1
+Version: 0.9.2
 Summary: SDK for power markets operations on Cognite Data Fusion
 License: Apache 2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

