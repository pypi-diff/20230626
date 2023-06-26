# Comparing `tmp/hcube-0.9.0.tar.gz` & `tmp/hcube-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcube-0.9.0.tar", max compression
+gzip compressed data, was "hcube-0.9.1.tar", max compression
```

## Comparing `hcube-0.9.0.tar` & `hcube-0.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      484 2021-11-08 11:53:41.418642 hcube-0.9.0/LICENSE
--rw-r--r--   0        0        0        0 2022-07-14 15:51:23.797365 hcube-0.9.0/hcube/__init__.py
--rw-r--r--   0        0        0        0 2022-07-14 15:51:23.797365 hcube-0.9.0/hcube/api/__init__.py
--rw-r--r--   0        0        0     1525 2023-01-10 08:38:59.631056 hcube-0.9.0/hcube/api/backend.py
--rw-r--r--   0        0        0       90 2022-07-14 15:51:23.797365 hcube-0.9.0/hcube/api/exceptions.py
--rw-r--r--   0        0        0        0 2022-07-14 15:51:23.797365 hcube-0.9.0/hcube/api/models/__init__.py
--rw-r--r--   0        0        0     2481 2023-01-03 09:57:18.665105 hcube-0.9.0/hcube/api/models/aggregation.py
--rw-r--r--   0        0        0     2689 2023-01-03 09:57:18.669105 hcube-0.9.0/hcube/api/models/cube.py
--rw-r--r--   0        0        0     2539 2023-01-03 09:57:18.669105 hcube-0.9.0/hcube/api/models/dimensions.py
--rw-r--r--   0        0        0     2278 2023-01-10 16:47:28.918188 hcube-0.9.0/hcube/api/models/filters.py
--rw-r--r--   0        0        0     3814 2022-12-14 09:14:57.081839 hcube-0.9.0/hcube/api/models/materialized_views.py
--rw-r--r--   0        0        0     1172 2023-01-03 09:57:18.669105 hcube-0.9.0/hcube/api/models/metrics.py
--rw-r--r--   0        0        0      449 2022-07-14 15:51:23.797365 hcube-0.9.0/hcube/api/models/ordering.py
--rw-r--r--   0        0        0    10153 2023-01-10 17:00:46.483194 hcube-0.9.0/hcube/api/models/query.py
--rw-r--r--   0        0        0     1796 2022-07-14 15:51:23.801365 hcube-0.9.0/hcube/api/models/transforms.py
--rw-r--r--   0        0        0        0 2022-07-14 15:51:23.801365 hcube-0.9.0/hcube/backends/__init__.py
--rw-r--r--   0        0        0      235 2023-01-05 06:55:20.652782 hcube-0.9.0/hcube/backends/clickhouse/__init__.py
--rw-r--r--   0        0        0    27163 2023-01-10 17:00:46.475194 hcube-0.9.0/hcube/backends/clickhouse/backend.py
--rw-r--r--   0        0        0     4047 2023-01-10 08:38:59.631056 hcube-0.9.0/hcube/backends/clickhouse/dictionaries.py
--rw-r--r--   0        0        0      391 2023-01-05 06:55:20.652782 hcube-0.9.0/hcube/backends/clickhouse/indexes.py
--rw-r--r--   0        0        0      691 2023-01-05 06:55:20.652782 hcube-0.9.0/hcube/backends/clickhouse/utils.py
--rw-r--r--   0        0        0     7944 2023-01-10 17:01:05.587409 hcube-0.9.0/hcube/backends/naive.py
--rw-r--r--   0        0        0    11480 2023-01-10 17:00:46.487194 hcube-0.9.0/hcube/backends/postgres.py
--rw-r--r--   0        0        0      160 2022-12-02 17:08:57.302861 hcube-0.9.0/hcube/settings.py
--rw-r--r--   0        0        0      694 2023-01-10 17:02:44.024519 hcube-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      862 2023-01-10 17:03:09.927907 hcube-0.9.0/setup.py
--rw-r--r--   0        0        0      635 2023-01-10 17:03:09.928119 hcube-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      484 2021-11-16 07:14:52.570187 hcube-0.9.1/LICENSE
+-rw-r--r--   0        0        0        0 2022-06-08 14:43:30.613812 hcube-0.9.1/hcube/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-08 14:43:30.613812 hcube-0.9.1/hcube/api/__init__.py
+-rw-r--r--   0        0        0     1525 2023-01-09 11:49:00.010470 hcube-0.9.1/hcube/api/backend.py
+-rw-r--r--   0        0        0       90 2022-06-08 14:43:30.613812 hcube-0.9.1/hcube/api/exceptions.py
+-rw-r--r--   0        0        0        0 2022-06-08 14:43:30.613812 hcube-0.9.1/hcube/api/models/__init__.py
+-rw-r--r--   0        0        0     2481 2023-01-04 07:20:23.388035 hcube-0.9.1/hcube/api/models/aggregation.py
+-rw-r--r--   0        0        0     2689 2023-01-04 07:20:23.388035 hcube-0.9.1/hcube/api/models/cube.py
+-rw-r--r--   0        0        0     2783 2023-01-11 15:45:27.117738 hcube-0.9.1/hcube/api/models/dimensions.py
+-rw-r--r--   0        0        0     2809 2023-01-11 15:45:27.117738 hcube-0.9.1/hcube/api/models/filters.py
+-rw-r--r--   0        0        0     3814 2023-01-04 07:20:23.388035 hcube-0.9.1/hcube/api/models/materialized_views.py
+-rw-r--r--   0        0        0     1172 2023-01-04 07:20:23.388035 hcube-0.9.1/hcube/api/models/metrics.py
+-rw-r--r--   0        0        0      449 2022-06-08 14:43:30.613812 hcube-0.9.1/hcube/api/models/ordering.py
+-rw-r--r--   0        0        0    10206 2023-01-11 15:45:27.117738 hcube-0.9.1/hcube/api/models/query.py
+-rw-r--r--   0        0        0     1796 2022-06-08 14:43:30.613812 hcube-0.9.1/hcube/api/models/transforms.py
+-rw-r--r--   0        0        0        0 2022-06-08 14:43:30.613812 hcube-0.9.1/hcube/backends/__init__.py
+-rw-r--r--   0        0        0      235 2023-01-04 15:26:28.788715 hcube-0.9.1/hcube/backends/clickhouse/__init__.py
+-rw-r--r--   0        0        0    27460 2023-01-11 15:45:27.121738 hcube-0.9.1/hcube/backends/clickhouse/backend.py
+-rw-r--r--   0        0        0     4554 2023-01-11 15:45:27.121738 hcube-0.9.1/hcube/backends/clickhouse/dictionaries.py
+-rw-r--r--   0        0        0      391 2023-01-04 15:26:28.788715 hcube-0.9.1/hcube/backends/clickhouse/indexes.py
+-rw-r--r--   0        0        0      691 2023-01-04 15:26:28.788715 hcube-0.9.1/hcube/backends/clickhouse/utils.py
+-rw-r--r--   0        0        0     8063 2023-01-11 15:45:27.121738 hcube-0.9.1/hcube/backends/naive.py
+-rw-r--r--   0        0        0    12020 2023-01-11 15:45:27.121738 hcube-0.9.1/hcube/backends/postgres.py
+-rw-r--r--   0        0        0      160 2023-01-04 07:20:23.388035 hcube-0.9.1/hcube/settings.py
+-rw-r--r--   0        0        0      694 2023-01-11 15:45:27.121738 hcube-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      862 2023-01-11 15:45:49.176577 hcube-0.9.1/setup.py
+-rw-r--r--   0        0        0      635 2023-01-11 15:45:49.176734 hcube-0.9.1/PKG-INFO
```

### Comparing `hcube-0.9.0/hcube/api/backend.py` & `hcube-0.9.1/hcube/api/backend.py`

 * *Files identical despite different names*

### Comparing `hcube-0.9.0/hcube/api/models/aggregation.py` & `hcube-0.9.1/hcube/api/models/aggregation.py`

 * *Files identical despite different names*

### Comparing `hcube-0.9.0/hcube/api/models/cube.py` & `hcube-0.9.1/hcube/api/models/cube.py`

 * *Files identical despite different names*

### Comparing `hcube-0.9.0/hcube/api/models/dimensions.py` & `hcube-0.9.1/hcube/api/models/dimensions.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,7 +87,17 @@
         if value is None:
             return None
         if isinstance(value, datetime):
             return value
         if isinstance(value, date):
             return datetime(value.year, value.month, value.day)
         return datetime.fromisoformat(value)
+
+
+class ArrayDimension(Dimension):
+
+    _type = list
+    default = []
+
+    def __init__(self, name: Optional[str] = None, null: bool = False, dimension: Dimension = None):
+        super().__init__(name, null)
+        self.dimension = dimension
```

### Comparing `hcube-0.9.0/hcube/api/models/filters.py` & `hcube-0.9.1/hcube/api/models/filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import abc
 from enum import Enum
 from typing import Any, Union
 
-from hcube.api.models.dimensions import Dimension
+from hcube.api.models.dimensions import ArrayDimension, Dimension
+from hcube.api.models.transforms import Transform
 
 
 class Filter(abc.ABC):
     def __init__(self, dimension: Dimension):
         self.dimension = dimension
 
 
@@ -62,14 +63,29 @@
 
     def __init__(self, dimension: Dimension, values: [str], case_sensitive: bool = True):
         super().__init__(dimension)
         self.values = list(values)
         self.case_sensitive = case_sensitive
 
 
+class OverlapFilter(Filter):
+    """
+    Describes overlap between two arrays.
+    """
+
+    def __init__(self, dimension: Dimension, values: list):
+        if not isinstance(dimension, (ArrayDimension, Transform)):
+            raise ValueError(
+                "OverlapFilter can only be used with ArrayDimension or a Transform, "
+                "'{}' given".format(dimension)
+            )
+        super().__init__(dimension)
+        self.values = list(values)
+
+
 class Wrapper:
     """
     This is helper class wrapping one filter shorthand.
     """
 
     def __init__(self, **named_filters):
         if len(named_filters) > 1:
```

### Comparing `hcube-0.9.0/hcube/api/models/materialized_views.py` & `hcube-0.9.1/hcube/api/models/materialized_views.py`

 * *Files identical despite different names*

### Comparing `hcube-0.9.0/hcube/api/models/metrics.py` & `hcube-0.9.1/hcube/api/models/metrics.py`

 * *Files identical despite different names*

### Comparing `hcube-0.9.0/hcube/api/models/query.py` & `hcube-0.9.1/hcube/api/models/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ComparisonType,
     EqualityFilter,
     Filter,
     FilterCombinator,
     IsNullFilter,
     ListFilter,
     NegativeListFilter,
+    OverlapFilter,
     SubstringFilter,
     SubstringMultiValueFilter,
     Wrapper,
 )
 from hcube.api.models.metrics import Metric
 from hcube.api.models.ordering import OrderDirection, OrderSpec
 from hcube.api.models.transforms import Transform
@@ -26,14 +27,15 @@
     Describes a cube query - i. e. filters, groups, aggregations and ordering
     """
 
     FILTER_SHORTHANDS = {
         "in": ListFilter,
         "isnull": IsNullFilter,
         "not_in": NegativeListFilter,
+        "overlap": OverlapFilter,
     }
 
     def __init__(self, cube: Type["Cube"]):  # noqa - cannot import Cube - circular import
         self.cube = cube
         self.filters: List[Filter] = []
         self.aggregations: List[Aggregation] = []
         self.groups: List[Dimension] = []
```

### Comparing `hcube-0.9.0/hcube/api/models/transforms.py` & `hcube-0.9.1/hcube/api/models/transforms.py`

 * *Files identical despite different names*

### Comparing `hcube-0.9.0/hcube/backends/clickhouse/backend.py` & `hcube-0.9.1/hcube/backends/clickhouse/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,28 +13,30 @@
     AggregationOp,
     ArrayAgg,
     Count,
     Sum,
 )
 from hcube.api.models.cube import Cube
 from hcube.api.models.dimensions import (
+    ArrayDimension,
     DateDimension,
     DateTimeDimension,
     Dimension,
     IntDimension,
     StringDimension,
 )
 from hcube.api.models.filters import (
     ComparisonFilter,
     EqualityFilter,
     Filter,
     IsNullFilter,
     ListFilter,
     NegativeListFilter,
     Or,
+    OverlapFilter,
     SubstringFilter,
     SubstringMultiValueFilter,
 )
 from hcube.api.models.materialized_views import AggregatingMaterializedView
 from hcube.api.models.metrics import FloatMetric, IntMetric, Metric
 from hcube.api.models.query import CubeQuery
 from hcube.api.models.transforms import (
@@ -416,14 +418,16 @@
             fn = "positionUTF8" if fltr.case_sensitive else "positionCaseInsensitiveUTF8"
             return f"{fn}({fltr.dimension.name}, %({key})s) > 0", {key: fltr.value}
         if isinstance(fltr, SubstringMultiValueFilter):
             fn = (
                 "multiSearchAnyUTF8" if fltr.case_sensitive else "multiSearchAnyCaseInsensitiveUTF8"
             )
             return f"{fn}({fltr.dimension.name}, %({key})s)", {key: fltr.values}
+        if isinstance(fltr, OverlapFilter):
+            return f"hasAny({fltr.dimension.name}, %({key})s)", {key: fltr.values}
         raise ValueError(f"unsupported filter {fltr.__class__}")
 
     @classmethod
     def _agg_name(cls, agg: Aggregation) -> str:
         if agg.op in (AggregationOp.SUM, AggregationOp.COUNT, AggregationOp.MAX, AggregationOp.MIN):
             # CH aggregations return 0 by default, but we want None to be compatible with other
             # backends, most notably standard SQL
@@ -499,15 +503,18 @@
             f"{partition_part} "
             f"{settings_part};"
         )
         logger.debug(command)
         with self.pool.get_client() as client:
             client.execute(command)
 
-    def _ch_type(self, dimension: Union[Dimension, Metric]):
+    def _ch_type(self, dimension: Union[Dimension, Metric]) -> str:
+        if isinstance(dimension, ArrayDimension):
+            subtype = self._ch_type(dimension.dimension)
+            return f"Array({subtype})"
         for dim_cls, ch_type in self.dimension_type_map:
             if isinstance(dimension, (IntDimension, IntMetric)):
                 sign = "U" if not dimension.signed else ""
                 ch_type = f"{sign}{ch_type}{dimension.bits}"
             if isinstance(dimension, dim_cls):
                 if hasattr(dimension, "null") and dimension.null:
                     return f"Nullable({ch_type})"
@@ -606,18 +613,19 @@
             select = (
                 f"transform({transform.dimension.name}, {key_array}, {value_array}) "
                 f"AS {transform.name}"
             )
             return transform.name, select
         if isinstance(transform, StoredMappingTransform):
             select = (
-                f"dictGetOrDefault('{self.database}.{transform.mapping_name}', "
+                f"dictGet('{self.database}.{transform.mapping_name}', "
                 f"'{transform.mapping_field}', "
-                f"toUInt64({transform.dimension.name}), {transform.dimension.name}) "
-                f"AS {transform.name}"
+                f"toUInt64({transform.dimension.name})) AS {transform.name}"
             )
             return transform.name, select
         raise ValueError(f"Unsupported transform {transform.__class__} in the clickhouse backend")
 
     def _drop_table(self, cube: Type[Cube]):
         with self.pool.get_client() as client:
-            client.execute(f"DROP TABLE IF EXISTS {self.database}.{self.cube_to_table_name(cube)}")
+            client.execute(
+                f"DROP TABLE IF EXISTS {self.database}.{self.cube_to_table_name(cube)} SYNC"
+            )
```

### Comparing `hcube-0.9.0/hcube/backends/clickhouse/dictionaries.py` & `hcube-0.9.1/hcube/backends/clickhouse/dictionaries.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,41 +20,48 @@
         """
 
 
 class PostgresqlSource(DataSource):
     def __init__(
         self,
         database,
-        table,
+        table=None,
+        query=None,
         host="localhost",
         port=5432,
         user="postgres",
         password="",
         invalidate_query=None,
     ):
         super().__init__()
         self.host = host
         self.port = port
         self.database = database
         self.user = user
         self.password = password
         self.table = table
+        self.query = query
         self.invalidate_query = invalidate_query
+        if not bool(self.table) ^ bool(self.query):
+            raise ValueError("Either table or query must be specified, but not both.")
 
     def definition_sql(self):
         invalidate_query = ""
         if self.invalidate_query:
             invalidate_query = f"invalidate_query '{self.invalidate_query}'"
+        # self.table and self.query are mutually exclusive, which is already enforced in
+        # the constructor, so we can rely on the fact that only one of them is set.
+        table_part = f"table '{self.table}'" if self.table else f"query '{self.query}'"
         return f"""SOURCE(POSTGRESQL(
             port {self.port}
             host '{self.host}'
             user '{self.user}'
             password '{self.password}'
             db '{self.database}'
-            table '{self.table}'
+            {table_part}
             {invalidate_query}
         ))"""
 
 
 class ClickhouseSource(DataSource):
     def __init__(self, database, table, host="localhost", port=9000, user="default", password=""):
         super().__init__()
@@ -82,16 +89,17 @@
     type: str
     expression: Optional[str] = None
     null_value: str = "NULL"
     injective: bool = False
 
     def definition_sql(self):
         expression = f"EXPRESSION {self.expression}" if self.expression else ""
+        default = f"DEFAULT {self.null_value}" if self.null_value else ""
         return (
-            f"{self.name} {self.type} DEFAULT {self.null_value} {expression} "
+            f"{self.name} {self.type} {default} {expression} "
             f"{'INJECTIVE' if self.injective else ''}"
         )
 
 
 class DictionaryDefinition:
     def __init__(
         self,
@@ -137,8 +145,8 @@
             "lifetime_min": self.lifetime_min,
             "lifetime_max": self.lifetime_max,
         }
         return hashlib.blake2b(json.dumps(data).encode("utf-8"), digest_size=32).hexdigest()
 
     def drop_sql(self, database=None):
         db_part = f"{database}." if database else ""
-        return f"DROP DICTIONARY IF EXISTS {db_part}{self.name}"
+        return f"DROP DICTIONARY IF EXISTS {db_part}{self.name} SYNC"
```

### Comparing `hcube-0.9.0/hcube/backends/clickhouse/utils.py` & `hcube-0.9.1/hcube/backends/clickhouse/utils.py`

 * *Files identical despite different names*

### Comparing `hcube-0.9.0/hcube/backends/naive.py` & `hcube-0.9.1/hcube/backends/naive.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     ComparisonType,
     EqualityFilter,
     Filter,
     IsNullFilter,
     ListFilter,
     NegativeListFilter,
     Or,
+    OverlapFilter,
     SubstringFilter,
     SubstringMultiValueFilter,
 )
 from hcube.api.models.ordering import OrderDirection, OrderSpec
 from hcube.api.models.query import CubeQuery
 from hcube.api.models.transforms import ExplicitMappingTransform
 from hcube.settings import GlobalSettings
@@ -147,14 +148,16 @@
             else:
                 return fltr.value.lower() in value.lower()
         if isinstance(fltr, SubstringMultiValueFilter):
             if fltr.case_sensitive:
                 return any(v in value for v in fltr.values)
             else:
                 return any(v.lower() in value.lower() for v in fltr.values)
+        if isinstance(fltr, OverlapFilter):
+            return any(v in fltr.values for v in value)
         raise ValueError(f"unsupported filter {fltr}")
 
     @classmethod
     def _aggregate(cls, op: AggregationOp, base, value):
         if op == AggregationOp.COUNT:
             return base + 1
         elif op == AggregationOp.SUM:
```

### Comparing `hcube-0.9.0/hcube/backends/postgres.py` & `hcube-0.9.1/hcube/backends/postgres.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 from decouple import config
 
 from hcube.api.backend import CubeBackend
 from hcube.api.exceptions import ConfigurationError
 from hcube.api.models.aggregation import AggregationOp, ArrayAgg, Count
 from hcube.api.models.cube import Cube
 from hcube.api.models.dimensions import (
+    ArrayDimension,
     DateDimension,
     DateTimeDimension,
     Dimension,
     IntDimension,
     StringDimension,
 )
 from hcube.api.models.filters import (
     ComparisonFilter,
     EqualityFilter,
     Filter,
     IsNullFilter,
     ListFilter,
     NegativeListFilter,
     Or,
+    OverlapFilter,
     SubstringFilter,
     SubstringMultiValueFilter,
 )
 from hcube.api.models.metrics import FloatMetric, IntMetric, Metric
 from hcube.api.models.query import CubeQuery
 from hcube.settings import GlobalSettings
 
@@ -248,14 +250,16 @@
             op = "LIKE" if fltr.case_sensitive else "ILIKE"
             return f"{fltr.dimension.name} {op} %({key})s", {key: f"%{fltr.value}%"}
         if isinstance(fltr, SubstringMultiValueFilter):
             op = "LIKE" if fltr.case_sensitive else "ILIKE"
             return " OR ".join(
                 f"{fltr.dimension.name} {op} %({key}_{i})s" for i in range(len(fltr.values))
             ), {f"{key}_{i}": f"%{value}%" for i, value in enumerate(fltr.values)}
+        if isinstance(fltr, OverlapFilter):
+            return f"{fltr.dimension.name} && %({key})s", {key: fltr.values}
         raise ValueError(f"unsupported filter {fltr.__class__}")
 
     def _agg_name(self, agg: AggregationOp):
         if agg in (AggregationOp.SUM, AggregationOp.COUNT, AggregationOp.MAX, AggregationOp.MIN):
             return agg.name
         if agg == AggregationOp.ARRAY:
             return "ARRAY_AGG"
@@ -275,14 +279,22 @@
             for dim in list(cube._dimensions.values()) + list(cube._metrics.values())
         ]
         field_part = ", ".join(fields)
         command = f"CREATE TABLE IF NOT EXISTS {self.schema}.{name} ({field_part})"
         logger.debug(command)
         self._execute(command)
 
-    def _ch_type(self, dimension: Union[Dimension, Metric]):
+    def _ch_type(self, dimension: Union[Dimension, Metric]) -> str:
+        a, b = self._ch_type_parts(dimension)
+        return f"{a} {b}" if b else a
+
+    def _ch_type_parts(self, dimension: Union[Dimension, Metric]) -> (str, str):
+        if isinstance(dimension, ArrayDimension):
+            subtype, _subnull = self._ch_type_parts(dimension.dimension)
+            # we ignore the null definition
+            return f"{subtype}[]", ""
         for dim_cls, ch_type in self.dimension_type_map:
             if isinstance(dimension, dim_cls):
                 if hasattr(dimension, "null") and dimension.null:
-                    return ch_type
-                return f"{ch_type} NOT NULL"
+                    return ch_type, ""
+                return ch_type, "NOT NULL"
         raise ValueError("unsupported dimension: %s", dimension.__class__)
```

### Comparing `hcube-0.9.0/pyproject.toml` & `hcube-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hcube"
-version = "0.9.0"
+version = "0.9.1"
 description = "HCube is a simple ORM for working with hyper-cube OLAP data stored in various backends."
 authors = ["Beda Kosata <beda@bigdigdata.com>"]
 license = "WTFPL"
 include = [
     "LICENSE",
 ]
```

### Comparing `hcube-0.9.0/setup.py` & `hcube-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ['clickhouse-driver>=0.2.4,<0.3.0',
  'clickhouse-pool>=0.5.3,<0.6.0',
  'psycopg2-binary>=2.9.5,<3.0.0',
  'python-decouple>=3.5,<4.0']
 
 setup_kwargs = {
     'name': 'hcube',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'HCube is a simple ORM for working with hyper-cube OLAP data stored in various backends.',
     'long_description': None,
     'author': 'Beda Kosata',
     'author_email': 'beda@bigdigdata.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `hcube-0.9.0/PKG-INFO` & `hcube-0.9.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcube
-Version: 0.9.0
+Version: 0.9.1
 Summary: HCube is a simple ORM for working with hyper-cube OLAP data stored in various backends.
 License: WTFPL
 Author: Beda Kosata
 Author-email: beda@bigdigdata.com
 Requires-Python: >=3.8.8,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

