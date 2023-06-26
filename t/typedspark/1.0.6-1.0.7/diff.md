# Comparing `tmp/typedspark-1.0.6.tar.gz` & `tmp/typedspark-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedspark-1.0.6.tar", last modified: Fri Jun  2 20:00:28 2023, max compression
+gzip compressed data, was "typedspark-1.0.7.tar", last modified: Mon Jun 26 14:18:25 2023, max compression
```

## Comparing `typedspark-1.0.6.tar` & `typedspark-1.0.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:28.386178 typedspark-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 20:00:14.000000 typedspark-1.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-02 20:00:28.386178 typedspark-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-02 20:00:14.000000 typedspark-1.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-02 20:00:14.000000 typedspark-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 20:00:28.386178 typedspark-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-02 20:00:14.000000 typedspark-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:28.382177 typedspark-1.0.6/typedspark/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:28.386178 typedspark-1.0.6/typedspark/_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_core/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_core/column_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_core/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_core/validate_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:28.386178 typedspark-1.0.6/typedspark/_schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_schema/dlt_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_schema/get_schema_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_schema/get_schema_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_schema/structfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:28.386178 typedspark-1.0.6/typedspark/_transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_transforms/structtype_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_transforms/transform_to_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_transforms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:28.386178 typedspark-1.0.6/typedspark/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_utils/create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_utils/load_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/_utils/register_schema_to_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:14.000000 typedspark-1.0.6/typedspark/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:00:28.382177 typedspark-1.0.6/typedspark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-02 20:00:28.000000 typedspark-1.0.6/typedspark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-02 20:00:28.000000 typedspark-1.0.6/typedspark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 20:00:28.000000 typedspark-1.0.6/typedspark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-02 20:00:28.000000 typedspark-1.0.6/typedspark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 20:00:28.000000 typedspark-1.0.6/typedspark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:18:25.172863 typedspark-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 14:18:08.000000 typedspark-1.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-26 14:18:25.172863 typedspark-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-26 14:18:08.000000 typedspark-1.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-26 14:18:08.000000 typedspark-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:18:25.172863 typedspark-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-26 14:18:08.000000 typedspark-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:18:25.172863 typedspark-1.0.7/typedspark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:18:25.172863 typedspark-1.0.7/typedspark/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_core/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_core/column_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_core/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_core/validate_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:18:25.172863 typedspark-1.0.7/typedspark/_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_schema/dlt_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_schema/get_schema_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_schema/get_schema_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_schema/structfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:18:25.172863 typedspark-1.0.7/typedspark/_transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_transforms/structtype_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_transforms/transform_to_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_transforms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:18:25.172863 typedspark-1.0.7/typedspark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_utils/create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_utils/load_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/_utils/register_schema_to_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:18:08.000000 typedspark-1.0.7/typedspark/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:18:25.172863 typedspark-1.0.7/typedspark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-26 14:18:25.000000 typedspark-1.0.7/typedspark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-26 14:18:25.000000 typedspark-1.0.7/typedspark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:18:25.000000 typedspark-1.0.7/typedspark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 14:18:25.000000 typedspark-1.0.7/typedspark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 14:18:25.000000 typedspark-1.0.7/typedspark.egg-info/top_level.txt
```

### Comparing `typedspark-1.0.6/LICENSE.txt` & `typedspark-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.6/PKG-INFO` & `typedspark-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.0.6
+Version: 1.0.7
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
```

### Comparing `typedspark-1.0.6/README.rst` & `typedspark-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.6/pyproject.toml` & `typedspark-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.6/setup.py` & `typedspark-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.6/typedspark/__init__.py` & `typedspark-1.0.7/typedspark/__init__.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.6/typedspark/_core/column.py` & `typedspark-1.0.7/typedspark/_core/column.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Module containing classes and functions related to TypedSpark Columns."""
 
-from typing import Generic, Optional, TypeVar
+from typing import Generic, Optional, TypeVar, Union, get_args, get_origin
 
 from pyspark.sql import Column as SparkColumn
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.functions import col
 from pyspark.sql.types import DataType
 
+from typedspark._core.datatypes import StructType
+
 T = TypeVar("T", bound=DataType)
 
 
 class EmptyColumn(SparkColumn):
     """Column object to be instantiated when there is no active Spark session."""
 
     def __init__(self, *args, **kwargs) -> None:  # pragma: no cover
@@ -26,15 +28,16 @@
             a: Column[IntegerType]
             b: Column[StringType]
     """
 
     def __new__(
         cls,
         name: str,
-        dataframe: Optional[DataFrame] = None,
+        dtype: T,
+        parent: Union[DataFrame, "Column", None] = None,
         curid: Optional[int] = None,
     ):
         """``__new__()`` instantiates the object (prior to ``__init__()``).
 
         Here, we simply take the provided ``name``, create a pyspark
         ``Column`` object and cast it to a typedspark ``Column`` object.
         This allows us to bypass the pypsark ``Column`` constuctor in
@@ -42,27 +45,39 @@
         to access.
         """
         # pylint: disable=unused-argument
 
         column: SparkColumn
         if SparkSession.getActiveSession() is None:
             column = EmptyColumn()  # pragma: no cover
-        elif dataframe is None:
+        elif parent is None:
             column = col(name)
         else:
-            column = dataframe[name]
+            column = parent[name]
 
         column.__class__ = Column
         return column
 
     def __init__(
         self,
         name: str,
-        dataframe: Optional[DataFrame] = None,
+        dtype: T,
+        parent: Union[DataFrame, "Column", None] = None,
         curid: Optional[int] = None,
     ):
         # pylint: disable=unused-argument
         self.str = name
+        self._dtype = dtype
         self._curid = curid
 
     def __hash__(self) -> int:
         return hash((self.str, self._curid))
+
+    @property
+    def dtype(self) -> T:
+        """Get the datatype of the column, e.g. Column[IntegerType] -> IntegerType."""
+        dtype = self._dtype
+        if get_origin(dtype) == StructType:
+            dtype.schema = get_args(dtype)[0]  # type: ignore
+            dtype.schema._parent = self  # type: ignore
+
+        return dtype
```

### Comparing `typedspark-1.0.6/typedspark/_core/column_meta.py` & `typedspark-1.0.7/typedspark/_core/column_meta.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.6/typedspark/_core/dataset.py` & `typedspark-1.0.7/typedspark/_core/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         set after ``__new__()`` and ``__init__()`` are finished.
         """
         object.__setattr__(self, name, value)
 
         if name == "__orig_class__":
             orig_class_args = get_args(self.__orig_class__)
             if orig_class_args and issubclass(orig_class_args[0], Schema):
-                self._schema_annotations: Type[Schema] = get_args(value)[0]
+                self._schema_annotations: Type[Schema] = orig_class_args[0]
                 validate_schema(
                     self._schema_annotations.get_structtype(),
                     deepcopy(self.schema),
                     self._schema_annotations.get_schema_name(),
                 )
                 self._add_schema_metadata()
```

### Comparing `typedspark-1.0.6/typedspark/_core/datatypes.py` & `typedspark-1.0.7/typedspark/_core/datatypes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Here, we make our own definitions of ``MapType``, ``ArrayType`` and
 ``StructType`` in order to allow e.g. for ``ArrayType[StringType]``."""
 from __future__ import annotations
 
 from abc import ABC
-from typing import TYPE_CHECKING, Generic, TypeVar
+from typing import TYPE_CHECKING, Generic, Type, TypeVar
 
 from pyspark.sql.types import DataType
 
 if TYPE_CHECKING:  # pragma: no cover
     from typedspark._schema.schema import Schema
 
     _Schema = TypeVar("_Schema", bound=Schema)
@@ -33,14 +33,16 @@
             position: Column[StringType]
             salary: Column[LongType]
 
         class Person(Schema):
             job: Column[StructType[Job]]
     """
 
+    schema: Type[_Schema]
+
 
 class MapType(Generic[_KeyType, _ValueType], TypedSparkDataType):
     """Allows for type annotations such as.
 
     .. code-block:: python
 
         class Basket(Schema):
```

### Comparing `typedspark-1.0.6/typedspark/_core/validate_schema.py` & `typedspark-1.0.7/typedspark/_core/validate_schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.6/typedspark/_schema/get_schema_definition.py` & `typedspark-1.0.7/typedspark/_schema/get_schema_definition.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,31 +11,37 @@
     from typedspark._schema.schema import Schema
 
 
 def get_schema_definition_as_string(
     schema: Type[Schema],
     include_documentation: bool,
     generate_imports: bool,
+    add_subschemas: bool,
     class_name: str = "MyNewSchema",
 ) -> str:
     """Return the code for a given ``Schema`` as a string.
 
     Typically used when you load a dataset using
     ``load_dataset_from_table()`` in a notebook and you want to save the
     schema in your code base. When ``generate_imports`` is True, the
     required imports for the schema are included in the string.
     """
     imports = get_schema_imports(schema, include_documentation) if generate_imports else ""
-    schema_string = _build_schema_definition_string(schema, include_documentation, class_name)
+    schema_string = _build_schema_definition_string(
+        schema, include_documentation, add_subschemas, class_name
+    )
 
     return imports + schema_string
 
 
 def _build_schema_definition_string(
-    schema: Type[Schema], include_documentation: bool, class_name: str = "MyNewSchema"
+    schema: Type[Schema],
+    include_documentation: bool,
+    add_subschemas: bool,
+    class_name: str = "MyNewSchema",
 ) -> str:
     """Return the code for a given ``Schema`` as a string."""
     lines = f"class {class_name}(Schema):\n"
     if include_documentation:
         lines += '    """Add documentation here."""\n\n'
 
     for k, val in get_type_hints(schema).items():
@@ -48,29 +54,31 @@
             .replace("typing.", "")
         )
         if include_documentation:
             lines += f'    {k}: Annotated[{typehint}, ColumnMeta(comment="")]\n'
         else:
             lines += f"    {k}: {typehint}\n"
 
-    lines += _add_subschemas(schema, include_documentation)
+    if add_subschemas:
+        lines += _add_subschemas(schema, add_subschemas, include_documentation)
+
     return lines
 
 
-def _add_subschemas(schema: Type[Schema], include_documentation: bool) -> str:
+def _add_subschemas(schema: Type[Schema], add_subschemas: bool, include_documentation: bool) -> str:
     """Identifies whether any ``Column`` are of the ``StructType`` type and
     generates their schema recursively."""
     lines = ""
     for val in get_type_hints(schema).values():
         args = get_args(val)
         if not args:
             continue
 
         dtype = args[0]
         if get_origin(dtype) == StructType:
             lines += "\n\n"
             subschema: Type[Schema] = get_args(dtype)[0]
             lines += _build_schema_definition_string(
-                subschema, include_documentation, subschema.get_schema_name()
+                subschema, include_documentation, add_subschemas, subschema.get_schema_name()
             )
 
     return lines
```

### Comparing `typedspark-1.0.6/typedspark/_schema/get_schema_imports.py` & `typedspark-1.0.7/typedspark/_schema/get_schema_imports.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.6/typedspark/_schema/schema.py` & `typedspark-1.0.7/typedspark/_schema/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module containing classes and functions related to TypedSpark Schemas."""
 import inspect
 import re
-from typing import Any, Dict, List, Optional, Union, get_type_hints
+from typing import Any, Dict, List, Optional, Type, Union, get_args, get_type_hints
 
 from pyspark.sql import DataFrame
-from pyspark.sql.types import StructType
+from pyspark.sql.types import DataType, StructType
 
 from typedspark._core.column import Column
 from typedspark._schema.dlt_kwargs import DltKwargs
 from typedspark._schema.get_schema_definition import get_schema_definition_as_string
 from typedspark._schema.structfield import get_structfield
 
 
@@ -26,15 +26,15 @@
             b: Column[StringType]
 
         DataSet[A](df)
 
     The class methods of ``Schema`` are described here.
     """
 
-    _linked_dataframe: Optional[DataFrame] = None
+    _parent: Optional[Union[DataFrame, Column]] = None
     _current_id: Optional[int] = None
     _original_name: Optional[str] = None
 
     def __new__(cls, name: str, bases: Any, dct: Dict[str, Any]):
         cls._attributes = dir(cls)
 
         # initializes all uninitialied variables with a type annotation as None
@@ -46,20 +46,20 @@
 
         return type.__new__(cls, name, bases, dct)
 
     def __repr__(cls) -> str:
         return f"\n{str(cls)}"
 
     def __str__(cls) -> str:
-        return cls.get_schema_definition_as_string()
+        return cls.get_schema_definition_as_string(add_subschemas=False)
 
     def __getattribute__(cls, name: str) -> Any:
         """Python base function that gets attributes.
 
-        We listen here for anyone getting ``Column`` from the ``Schema``.
+        We listen here for anyone getting a ``Column`` from the ``Schema``.
         Even though they're not explicitely instantiated, we can instantiate
         them here whenever someone attempts to get them. This allows us to do the following:
 
         .. code-block:: python
 
             class A(Schema):
                 a: Column[IntegerType]
@@ -68,19 +68,37 @@
                 df.withColumn(A.a.str, lit(1))
                 .select(A.a)
             )
         """
         if name.startswith("__") or name == "_attributes" or name in cls._attributes:
             return object.__getattribute__(cls, name)
 
-        if name in get_type_hints(cls).keys():
-            return Column(name, cls._linked_dataframe, cls._current_id)
+        if name in get_type_hints(cls):
+            return Column(
+                name,
+                cls._get_dtype(name),  # type: ignore
+                cls._parent,
+                cls._current_id,
+            )
 
         raise TypeError(f"Schema {cls.get_schema_name()} does not have attribute {name}.")
 
+    def _get_dtype(cls, name: str) -> Type[DataType]:
+        """Returns the datatype of a column, e.g. Column[IntegerType] -> IntegerType."""
+        column = get_type_hints(cls)[name]
+        args = get_args(column)
+
+        if not args:
+            raise TypeError(
+                f"Column {cls.get_schema_name()}.{name} does not have an annotated type."
+            )
+
+        dtype = args[0]
+        return dtype
+
     def all_column_names(cls) -> List[str]:
         """Returns all column names for a given schema."""
         return list(get_type_hints(cls).keys())
 
     def all_column_names_except_for(cls, except_for: List[str]) -> List[str]:
         """Returns all column names for a given schema except for the columns
         specified in the ``except_for`` parameter."""
@@ -95,37 +113,41 @@
         return word.lower()
 
     def get_schema_definition_as_string(
         cls,
         schema_name: Optional[str] = None,
         include_documentation: bool = False,
         generate_imports: bool = True,
+        add_subschemas: bool = True,
     ) -> str:
         """Return the code for the ``Schema`` as a string."""
         if schema_name is None:
             schema_name = cls.get_schema_name()
         return get_schema_definition_as_string(
             cls,  # type: ignore
             include_documentation,
             generate_imports,
+            add_subschemas,
             schema_name,
         )
 
     def print_schema(
         cls,
         schema_name: Optional[str] = None,
         include_documentation: bool = False,
         generate_imports: bool = True,
+        add_subschemas: bool = False,
     ):  # pragma: no cover
         """Print the code for the ``Schema``."""
         print(
             cls.get_schema_definition_as_string(
                 schema_name=schema_name,
                 include_documentation=include_documentation,
                 generate_imports=generate_imports,
+                add_subschemas=add_subschemas,
             )
         )
 
     def get_docstring(cls) -> Union[str, None]:
         """Returns the docstring of the schema."""
         return inspect.getdoc(cls)
```

### Comparing `typedspark-1.0.6/typedspark/_schema/structfield.py` & `typedspark-1.0.7/typedspark/_schema/structfield.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.6/typedspark/_transforms/structtype_column.py` & `typedspark-1.0.7/typedspark/_transforms/structtype_column.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.6/typedspark/_transforms/transform_to_schema.py` & `typedspark-1.0.7/typedspark/_transforms/transform_to_schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.6/typedspark/_transforms/utils.py` & `typedspark-1.0.7/typedspark/_transforms/utils.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.6/typedspark/_utils/create_dataset.py` & `typedspark-1.0.7/typedspark/_utils/create_dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.6/typedspark/_utils/load_table.py` & `typedspark-1.0.7/typedspark/_utils/load_table.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.6/typedspark/_utils/register_schema_to_dataset.py` & `typedspark-1.0.7/typedspark/_utils/register_schema_to_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,12 +57,12 @@
 
     class LinkedSchema(schema):  # type: ignore
         """TypedSpark LinkedSchema.
 
         Contains the DataFrame that this Schema is linked to.
         """
 
-        _linked_dataframe = dataframe
+        _parent = dataframe
         _current_id = _counter()
         _original_name = schema.get_schema_name()
 
     return LinkedSchema  # type: ignore
```

### Comparing `typedspark-1.0.6/typedspark.egg-info/PKG-INFO` & `typedspark-1.0.7/typedspark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.0.6
+Version: 1.0.7
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
```

### Comparing `typedspark-1.0.6/typedspark.egg-info/SOURCES.txt` & `typedspark-1.0.7/typedspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

