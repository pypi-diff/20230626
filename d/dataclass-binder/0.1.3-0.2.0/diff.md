# Comparing `tmp/dataclass_binder-0.1.3.tar.gz` & `tmp/dataclass_binder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_binder-0.1.3.tar", max compression
+gzip compressed data, was "dataclass_binder-0.2.0.tar", max compression
```

## Comparing `dataclass_binder-0.1.3.tar` & `dataclass_binder-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-03-05 09:05:41.825690 dataclass_binder-0.1.3/LICENSE
--rw-r--r--   0        0        0    13629 2023-03-05 09:05:41.825690 dataclass_binder-0.1.3/README.md
--rw-r--r--   0        0        0     1855 2023-03-05 09:06:03.397879 dataclass_binder-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      172 2023-03-05 09:05:41.825690 dataclass_binder-0.1.3/src/dataclass_binder/__init__.py
--rw-r--r--   0        0        0    27404 2023-03-05 09:05:41.825690 dataclass_binder-0.1.3/src/dataclass_binder/_impl.py
--rw-r--r--   0        0        0        0 2023-03-05 09:05:41.825690 dataclass_binder-0.1.3/src/dataclass_binder/py.typed
--rw-r--r--   0        0        0    14896 1970-01-01 00:00:00.000000 dataclass_binder-0.1.3/setup.py
--rw-r--r--   0        0        0    14545 1970-01-01 00:00:00.000000 dataclass_binder-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-26 06:28:05.950435 dataclass_binder-0.2.0/LICENSE
+-rw-r--r--   0        0        0    15881 2023-06-26 06:28:05.950435 dataclass_binder-0.2.0/README.md
+-rw-r--r--   0        0        0     2512 2023-06-26 06:28:27.198699 dataclass_binder-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-06-26 06:28:05.950435 dataclass_binder-0.2.0/src/dataclass_binder/__init__.py
+-rw-r--r--   0        0        0    28033 2023-06-26 06:28:05.950435 dataclass_binder-0.2.0/src/dataclass_binder/_impl.py
+-rw-r--r--   0        0        0        0 2023-06-26 06:28:05.950435 dataclass_binder-0.2.0/src/dataclass_binder/py.typed
+-rw-r--r--   0        0        0    17237 1970-01-01 00:00:00.000000 dataclass_binder-0.2.0/setup.py
+-rw-r--r--   0        0        0    16797 1970-01-01 00:00:00.000000 dataclass_binder-0.2.0/PKG-INFO
```

### Comparing `dataclass_binder-0.1.3/LICENSE` & `dataclass_binder-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclass_binder-0.1.3/README.md` & `dataclass_binder-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 
 ## Usage
 
 The `dataclass_binder` module contains the `Binder` class which makes it easy to bind TOML data, such as a configuration file, to Python [dataclasses](https://docs.python.org/3/library/dataclasses.html).
 
 The binding is a two-step process:
-- specialize the `Binder` class by using your top-level dataclass as a type argument
+- instantiate the `Binder` class by passing your top-level dataclass as an argument
 - call the `parse_toml()` method, providing the path of the configuration file as its argument
 
 Put together, the code looks like this:
 
 ```py
 import logging
 import sys
@@ -115,73 +115,83 @@
 
 
 logger = logging.getLogger(__name__)
 
 if __name__ == "__main__":
     config_file = Path("config.toml")
     try:
-        config = Binder[Config].parse_toml(config_file)
+        config = Binder(Config).parse_toml(config_file)
     except Exception as ex:
         logger.critical("Error reading configuration file '%s': %s", config_file, ex)
         sys.exit(1)
 ```
 
 ### Binding a Pre-parsed Dictionary
 
 If you don't want to bind the contents of a full file, there is also the option to bind a pre-parsed dictionary instead.
-For this, you can use the `bind()` method on the specialized `Binder` class.
+For this, you can use the `bind()` method on the `Binder` object.
 
-For example, the following service uses a hybrid configuration format where a single file configures both the service itself and logging system:
+For example, the following service is configured by one table within a larger TOML configuration file:
 
 ```py
-import logging.config
-
 import tomllib  # or 'tomli' on Python <3.11
 from dataclass_binder import Binder
 
 
 with open("config.toml", "rb") as f:
     config = tomllib.load(f)
-service_config = Binder[ServiceConfig].bind(config["service"])
-logging.config.dictConfig(config["logging"])
+service_config = Binder(ServiceConfig).bind(config["service"])
 ```
 
 To keep these examples short, from now on `import` statements will only be included the first time a particular imported name is used.
 
 ### Basic Types
 
 Dataclass fields correspond to TOML keys. In the dataclass, underscores are used as word separators, while dashes are used in the TOML file. Let's configure a service that listens on a TCP port for requests and stores its data in a database, using the following TOML fragment:
 
 ```toml
 database-url = 'postgresql://user:password@host/db'
-port = 5432
+port = 8080
 ```
 
 This configuration can be bound to the following dataclass:
 
 ```py
 from dataclasses import dataclass
 
 @dataclass
 class Config:
     database_url: str
     port: int
+    verbose: bool
 ```
 
+The `float` type can be used to bind floating point numbers.
+Support for `Decimal` is not there at the moment but would be relatively easy to add, as `tomllib`/`tomli` has an option for that.
+
+### Defaults
+
 Fields can be made optional by assigning a default value. Using `None` as a default value is allowed too:
 
 ```py
 @dataclass
 class Config:
     verbose: bool = False
     webhook_url: str | None = None
 ```
 
-The `float` type can be used to bind floating point numbers.
-Support for `Decimal` is not there at the moment but would be relatively easy to add, as `tomllib`/`tomli` has an option for that.
+If you want to mix fields with and without defaults in any order, mark the fields as keyword-only:
+
+```py
+@dataclass(kw_only=True)
+class Config:
+    database_url: str
+    verbose: bool = False
+    port: int
+```
 
 ### Dates and Times
 
 TOML handles dates and timestamps as first-class values.
 Date, time and date+time TOML values are bound to `datetime.date`, `datetime.time` and `datetime.datetime` Python objects respectively.
 
 There is also support for time intervals using `datetime.timedelta`:
@@ -266,15 +276,67 @@
 token = "12345"
 
 [[webhooks]]
 url = "https://host2/hook"
 token = "frperg"
 ```
 
-Always define additional dataclasses at the module level in your Python code: if the class is for example defined inside a function, the `Binder` specialization will not be able to find it.
+Always define additional dataclasses at the module level in your Python code: if the class is for example defined inside a function, the `Binder` constructor will not be able to find it.
+
+### Untyped Data
+
+Sometimes the full structure of the data you want to bind is either too complex or too much in flux to be worth fully annotating.
+In such a situation, you can use `typing.Any` as the annotation to simply capture the output of Python's TOML parser without type-checking it.
+
+In the following example, a service uses the Python standard library logging implementation, configured using the [configuration dictionary schema](https://docs.python.org/3/library/logging.config.html#logging-config-dictschema):
+
+```py
+import logging.config
+from dataclasses import dataclass
+from typing import Any
+
+from dataclass_binder import Binder
+
+
+@dataclass
+class Config:
+    database_url: str
+    logging: Any
+
+
+def run(url: str) -> None:
+    logging.info("Service starting")
+
+
+if __name__ == "__main__":
+    config = Binder[Config].parse_toml("service.toml")
+    logging.config.dictConfig(config.logging)
+    run(config.database_url)
+```
+
+The `service.toml` configuration file for this service could look like this:
+
+```toml
+database-url = 'postgresql://user:password@host/db'
+
+[logging]
+version = 1
+
+[logging.root]
+level = 'INFO'
+handlers = ['file']
+
+[logging.handlers.file]
+class = 'logging.handlers.RotatingFileHandler'
+filename = 'service.log'
+formatter = 'simple'
+
+[logging.formatters.simple]
+format = '%(asctime)s %(name)s %(levelname)s %(message)s'
+```
 
 ### Plugins
 
 To select plugins to activate, you can bind Python classes or modules using `type[BaseClass]` and `types.ModuleType` annotations respectively:
 
 ```py
 from dataclasses import dataclass, field
@@ -373,15 +435,15 @@
 # Default:
 # port = 12345
 port = 8080
 ```
 
 ### Troubleshooting
 
-Finally, a troubleshooting tip: instead of the full `Binder[Config].parse_toml()`, first try to execute only `Binder[Config]`.
+Finally, a troubleshooting tip: instead of the full `Binder(Config).parse_toml()`, first try to execute only `Binder(Config)`.
 If that fails, the problem is in the dataclass definitions.
 If that succeeds, but the `parse_toml()` call fails, the problem is that the TOML file does not match the format defined in the dataclasses.
 
 
 ## Development Environment
 
 [Poetry](https://python-poetry.org/) is used to set up a virtual environment with all the dependencies and development tools that you need:
@@ -403,14 +465,20 @@
 ## Release Procedure
 
 - Verify that CI passes on the branch that you want to release (typically `main`)
 - Create a release on the GitHub web interface; name the tag `v<major>.<minor>.<patchlevel>`
 - After publishing the release on GitHub, the package will be built and published on PyPI automatically via Actions
 
 
+## Deprecations
+
+### Binder Specialization
+
+Prior to version 0.2.0, the `Binder` class was specialized using a type argument (`Binder[Config]`) rather than instantiation (`Binder(config)`). The old syntax is still supported for now, but the backwards compatibility might be removed in a minor release prior to 1.0 if it becomes a maintenance burden, so please update your code.
+
 ## Changelog
 
 ### 0.1.0 - 2023-02-21:
 
 - First open source release; thanks to my employer [Protix](https://protix.eu/) for making this possible
 
 ### 0.1.1 - 2023-02-22:
@@ -420,7 +488,13 @@
 ### 0.1.2 - 2023-03-03:
 
 - Fix `get()` and `[]` on object bound to read-only mapping ([#6](https://github.com/ProtixIT/dataclass-binder/issues/6))
 
 ### 0.1.3 - 2023-03-05:
 
 - Ignore dataclass fields with `init=False` ([#2](https://github.com/ProtixIT/dataclass-binder/issues/2))
+
+### 0.2.0 - 2023-06-26:
+
+- Instantiate `Binder` instead of specializing it ([#14](https://github.com/ProtixIT/dataclass-binder/pull/14))
+- Support `typing.Any` as a field annotation ([#10](https://github.com/ProtixIT/dataclass-binder/issues/10))
+- Fix crash in `format_template()` on optional fields with non-string annotations ([#16](https://github.com/ProtixIT/dataclass-binder/pull/16))
```

### Comparing `dataclass_binder-0.1.3/src/dataclass_binder/_impl.py` & `dataclass_binder-0.2.0/src/dataclass_binder/_impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,43 +11,48 @@
 from datetime import date, datetime, time, timedelta
 from functools import reduce
 from importlib import import_module
 from inspect import cleandoc, get_annotations, getmodule, getsource, isabstract
 from pathlib import Path
 from textwrap import dedent
 from types import MappingProxyType, ModuleType, NoneType, UnionType
-from typing import Any, BinaryIO, ClassVar, Generic, TypeVar, Union, cast, get_args, get_origin
+from typing import TYPE_CHECKING, Any, BinaryIO, Generic, TypeVar, Union, cast, get_args, get_origin
 from weakref import WeakKeyDictionary
 
 if sys.version_info < (3, 11):
     import tomli as tomllib  # pragma: no cover
 else:
     import tomllib  # pragma: no cover
 
 
-def _collect_type(field_type: type, context: str) -> type:
+def _collect_type(field_type: type, context: str) -> type | Binder[Any]:
     """
     Verify and streamline a type annotation.
 
     Streamlining means that when there are multiple ways to express the same typing,
     we pick one and convert the alternative forms to that.
 
     Raises TypeError if the annotation is not supported.
     """
     origin = get_origin(field_type)
     if origin is None:
-        if not isinstance(field_type, type):
+        if field_type is Any:
+            return object
+        elif not isinstance(field_type, type):
             raise TypeError(f"Annotation for field '{context}' is not a type")
-        elif issubclass(field_type, (str, int, float, date, time, timedelta, ModuleType)):
+        elif issubclass(field_type, str | int | float | date | time | timedelta | ModuleType):
             return field_type
         elif field_type is type:
-            # https://github.com/python/mypy/issues/12392
+            # https://github.com/python/mypy/issues/13026
             return cast(type, type[Any])  # type: ignore[index]
         elif hasattr(field_type, "__class_getitem__"):
             raise TypeError(f"Field '{context}' needs type argument(s)")
+        else:
+            # Any type that we don't explicitly support is treated as a nested data class.
+            return Binder(field_type)
     elif origin in (UnionType, Union):
         collected_types = [
             # Note that 'arg' cannot be a union itself, as Python automatically flattens nested union types.
             _collect_type(arg, context)
             for arg in get_args(field_type)
             # Optional fields are allowed, but None can only be the default, not the parsed value.
             if arg is not NoneType
@@ -59,15 +64,15 @@
         else:
             return reduce(operator.__or__, collected_types)
     elif issubclass(origin, Mapping):
         type_args = get_args(field_type)
         try:
             key_type, value_type = type_args
         except ValueError:
-            raise TypeError(f"Mapping '{context}' must have two type arguments")
+            raise TypeError(f"Mapping '{context}' must have two type arguments") from None
         if key_type is not str:
             raise TypeError(f"Mapping '{context}' has key type '{key_type.__name__}', expected 'str'")
         return origin[(key_type, _collect_type(value_type, f"{context}[]"))]  # type: ignore[no-any-return]
     elif issubclass(origin, Iterable):
         args = get_args(field_type)
         arg_context = f"{context}[]"
         if issubclass(origin, tuple):
@@ -92,17 +97,14 @@
             if not isinstance(base, type):
                 raise TypeError(f"type[...] annotation for '{context}' must have a type as its argument")
             collected_types.append(type[base])  # type: ignore[index]
         return reduce(operator.__or__, collected_types)
     else:
         raise TypeError(f"Field '{context}' has unsupported generic type '{origin.__name__}'")
 
-    # Any type that we don't explicitly support is treated as a nested data class.
-    return Binder.__class_getitem__(field_type)
-
 
 def _find_object_by_name(name: str, context: str) -> object:
     """
     Look up a Python object by its fully-qualified name.
 
     Raises ValueError if the name could not be resolved.
     """
@@ -142,15 +144,15 @@
     Raises KeyError if no such field exists.
     """
     if full_name in field_names:
         return full_name, None
     try:
         name, suffix = full_name.rsplit("_", 1)
     except ValueError:
-        raise KeyError(full_name)
+        raise KeyError(full_name) from None
     if name in field_names:
         return name, suffix
     else:
         raise KeyError(full_name)
 
 
 def _get_fields(cls: type) -> Iterator[tuple[str, type]]:
@@ -169,68 +171,73 @@
     for field_container in reversed(cls.__mro__):
         for name, annotation in get_annotations(field_container).items():
             field = fields_by_name[name]
             if not field.init:
                 continue
             if isinstance(annotation, str):
                 try:
-                    annotation = eval(annotation, cls_globals, cls_locals)
+                    annotation = eval(annotation, cls_globals, cls_locals)  # noqa: PGH001
                 except NameError as ex:
                     raise TypeError(f"Failed to parse annotation of field '{cls.__name__}.{name}': {ex}") from None
             yield name, annotation
 
 
 _TIMEDELTA_SUFFIXES = {"days", "seconds", "microseconds", "milliseconds", "minutes", "hours", "weeks"}
 
 T = TypeVar("T")
 
-_binder_cache: MutableMapping[type, type] = WeakKeyDictionary()
 
-
-class Binder(Generic[T]):
+class _BinderCache(type, Generic[T]):
     """
-    Binds TOML data to a specific dataclass.
+    Cache that returns a dedicated `Binder` instance for each dataclass.
     """
 
-    __slots__ = ()
-    _field_types: ClassVar[Mapping[str, type]]
-
-    @classmethod
-    def _get_config_class(cls) -> type[T]:
-        config_class: type[T]
-        (config_class,) = cls.__orig_bases__[0].__args__  # type: ignore[attr-defined]
-        if isinstance(config_class, TypeVar):
-            raise TypeError("Binder must be specialized before use, for example Binder[MyDataClass]")
-        return config_class
+    _cache: MutableMapping[T, Binder[T]] = WeakKeyDictionary()
 
-    def __class_getitem__(cls, config_class: type[T]) -> type[Binder[T]]:
+    def __call__(cls, dataclass: T) -> Binder[T]:
         try:
-            return _binder_cache[config_class]
+            return cls._cache[dataclass]
         except KeyError:
             pass
 
-        field_types = {
-            field_name: _collect_type(field_type, f"{config_class.__name__}.{field_name}")
-            for field_name, field_type in _get_fields(config_class)
-        }
+        instance: Binder[T] = super().__call__(dataclass)
+        cls._cache[dataclass] = instance
+        return instance
+
 
-        class SpecializedBinder(super().__class_getitem__(config_class)):  # type: ignore[misc]
-            _config_class = config_class
-            _field_types = field_types
+class Binder(Generic[T], metaclass=_BinderCache):
+    """
+    Binds TOML data to a specific dataclass.
+    """
 
-        _binder_cache[config_class] = SpecializedBinder
-        return SpecializedBinder
+    __slots__ = ("_dataclass", "_field_types")
+    _dataclass: type[T]
+    _field_types: Mapping[str, type | Binder[Any]]
+
+    def __class_getitem__(cls: type[Binder[T]], dataclass: type[T]) -> Binder[T]:
+        """Deprecated: use `Binder(MyDataClass)` instead."""
+        return cls(dataclass)
+
+    def __init__(self, dataclass: type[T]) -> None:
+        self._dataclass = dataclass
+        self._field_types = {
+            field_name: _collect_type(field_type, f"{dataclass.__name__}.{field_name}")
+            for field_name, field_type in _get_fields(dataclass)
+        }
 
-    @classmethod
-    def _bind_to_single_type(cls, value: object, field_type: type, context: str) -> object:
+    def _bind_to_single_type(self, value: object, field_type: type | Binder[Any], context: str) -> object:
         """
         Convert a TOML value to a singular (non-union) field type.
 
         Raises TypeError if the TOML value's type doesn't match the field type.
         """
+        if isinstance(field_type, Binder):
+            if not isinstance(value, dict):
+                raise TypeError(f"Value for '{context}' has type '{type(value).__name__}', expected table")
+            return field_type._bind_to_class(value, context)  # noqa: SLF001
         origin = get_origin(field_type)
         if origin is None:
             if field_type is ModuleType:
                 if not isinstance(value, str):
                     raise TypeError(
                         f"Expected TOML string for Python reference '{context}', got '{type(value).__name__}'"
                     )
@@ -243,48 +250,46 @@
                     return value
                 elif isinstance(value, time):
                     return timedelta(
                         hours=value.hour, minutes=value.minute, seconds=value.second, microseconds=value.microsecond
                     )
                 else:
                     raise TypeError(f"Value for '{context}' has type '{type(value).__name__}', expected time")
-            elif issubclass(field_type, Binder):
-                if not isinstance(value, dict):
-                    raise TypeError(f"Value for '{context}' has type '{type(value).__name__}', expected table")
-                return field_type._bind_to_class(value, context)
-            elif isinstance(value, field_type) and (type(value) is not bool or field_type is bool):
+            elif isinstance(value, field_type) and (
+                type(value) is not bool or field_type is bool or field_type is object
+            ):
                 return value
         elif issubclass(origin, Mapping):
             if not isinstance(value, dict):
                 raise TypeError(f"Value for '{context}' has type '{type(value).__name__}', expected table")
             key_type, elem_type = get_args(field_type)
-            mapping = {key: cls._bind_to_field(elem, elem_type, f'{context}["{key}"]') for key, elem in value.items()}
+            mapping = {key: self._bind_to_field(elem, elem_type, f'{context}["{key}"]') for key, elem in value.items()}
             return (
                 (mapping if isinstance(origin, MutableMapping) else MappingProxyType(mapping))
                 if isabstract(origin)
                 else field_type(mapping)
             )
         elif issubclass(origin, Iterable):
             if not isinstance(value, list):
                 raise TypeError(f"Value for '{context}' has type '{type(value).__name__}', expected array")
             type_args = get_args(field_type)
             if issubclass(origin, tuple):
                 if len(type_args) == len(value):
                     return tuple(
-                        cls._bind_to_field(elem, elem_type, f"{context}[{index}]")
-                        for index, (elem, elem_type) in enumerate(zip(value, type_args))
+                        self._bind_to_field(elem, elem_type, f"{context}[{index}]")
+                        for index, (elem, elem_type) in enumerate(zip(value, type_args, strict=True))
                     )
                 else:
                     raise TypeError(f"Expected {len(type_args)} elements for '{context}', got {len(value)}")
             (elem_type,) = type_args
             container_class = (
                 (list if isinstance(origin, MutableSequence) else tuple) if isabstract(origin) else field_type
             )
             return container_class(
-                cls._bind_to_field(elem, elem_type, f"{context}[{index}]") for index, elem in enumerate(value)
+                self._bind_to_field(elem, elem_type, f"{context}[{index}]") for index, elem in enumerate(value)
             )
         elif origin is type:
             if not isinstance(value, str):
                 raise TypeError(f"Expected TOML string for Python reference '{context}', got '{type(value).__name__}'")
             obj = _find_object_by_name(value, context)
             if not isinstance(obj, type):
                 raise TypeError(f"Value for '{context}' has type '{type(obj).__name__}', expected class")
@@ -294,85 +299,97 @@
                 return obj
             else:
                 raise TypeError(
                     f"Resolved '{context}' to class '{obj.__name__}', expected subclass of '{expected_type.__name__}'"
                 )
         else:
             # This is currently unreachable because we reject unsupported generic types in _collect_type().
-            assert False
+            raise AssertionError(origin)
 
         raise TypeError(f"Value for '{context}' has type '{type(value).__name__}', expected '{field_type.__name__}'")
 
-    @classmethod
-    def _bind_to_field(cls, value: object, field_type: type, context: str) -> object:
+    def _bind_to_field(self, value: object, field_type: type | Binder[Any], context: str) -> object:
         """
         Convert a TOML value to a field type which is possibly a union type.
 
         Raises TypeError if the TOML value's type doesn't match the field type.
         """
         if get_origin(field_type) is UnionType:
             for arg in get_args(field_type):
                 try:
-                    return cls._bind_to_single_type(value, arg, context)
+                    return self._bind_to_single_type(value, arg, context)
                 except TypeError:
                     # TODO: This is inefficient: we format and then discard the error string.
                     #       Union types are not used a lot though, so it's fine for now.
                     # TODO: When the union contains multiple custom classes, we pick the first that succeeds.
                     #       It would be cleaner to limit custom classes to one at collection time.
                     pass
             raise TypeError(f"Value for '{context}' has type '{type(value).__name__}', expected '{field_type}'")
         else:
-            return cls._bind_to_single_type(value, field_type, context)
+            return self._bind_to_single_type(value, field_type, context)
 
-    @classmethod
-    def _bind_to_class(cls: type[Binder[T]], toml_dict: Mapping[str, Any], context: str) -> T:
-        field_types = cls._field_types
+    def _bind_to_class(self, toml_dict: Mapping[str, Any], context: str) -> T:
+        field_types = self._field_types
         parsed = {}
         for key, value in toml_dict.items():
             if "_" in key:
                 raise ValueError(f"Underscore found in TOML key '{key}'")
             field_name = key.replace("-", "_")
             try:
                 field_name, suffix = _find_field(field_name, field_types)
             except KeyError:
                 raise ValueError(f"Field '{context}.{field_name}' does not exist") from None
 
             field_type = field_types[field_name]
             if suffix is not None:
                 if field_type is timedelta and suffix in _TIMEDELTA_SUFFIXES:
-                    if isinstance(value, (int, float)) and not isinstance(value, bool):
+                    if isinstance(value, int | float) and not isinstance(value, bool):
                         value = timedelta(**{suffix: value})
                     else:
                         raise TypeError(
                             f"Value for '{context}.{field_name}' with suffix '{suffix}' "
                             f"has type '{type(value).__name__}', expected number"
                         )
                 else:
+                    type_name = (
+                        field_type._dataclass if isinstance(field_type, Binder) else field_type  # noqa: SLF001
+                    ).__name__
                     raise ValueError(
-                        f"Field '{context}.{field_name}' has type '{field_type.__name__}', "
+                        f"Field '{context}.{field_name}' has type '{type_name}', "
                         f"which does not support suffix '{suffix}'"
                     )
 
-            parsed[field_name] = cls._bind_to_field(value, field_type, f"{context}.{field_name}")
+            parsed[field_name] = self._bind_to_field(value, field_type, f"{context}.{field_name}")
+
+        return self._dataclass(**parsed)
 
-        return cls._get_config_class()(**parsed)
+    if TYPE_CHECKING:
+        # These definitions exist to support the deprecated `Binder[DC]` syntax in mypy.
 
-    @classmethod
-    def bind(cls, data: Mapping[str, Any]) -> T:
-        return cls._bind_to_class(data, cls._get_config_class().__name__)
-
-    @classmethod
-    def parse_toml(cls, file: BinaryIO | str | Path) -> T:
-        match file:
-            case Path() | str():
-                with open(file, "rb") as stream:
-                    data = tomllib.load(stream)
-            case _:
-                data = tomllib.load(file)
-        return cls.bind(data)
+        @classmethod
+        def bind(cls, data: Mapping[str, Any]) -> T:
+            ...
+
+        @classmethod
+        def parse_toml(cls, file: BinaryIO | str | Path) -> T:
+            ...
+
+    else:
+
+        def bind(self, data: Mapping[str, Any]) -> T:
+            return self._bind_to_class(data, self._dataclass.__name__)
+
+        def parse_toml(self, file: BinaryIO | str | Path) -> T:
+            match file:
+                case Path() | str():
+                    with open(file, "rb") as stream:
+                        data = tomllib.load(stream)
+                case _:
+                    data = tomllib.load(file)
+            return self.bind(data)
 
 
 def format_toml_pair(key: str, value: object) -> str:
     """Format a key/value pair as TOML text."""
     suffix, data = _to_toml_pair(value)
     if suffix is not None:
         key += suffix
@@ -518,24 +535,24 @@
                     yield ", "
                 yield from _iter_format_value(elem)
             yield "]"
         case _:
             raise TypeError(type(value).__name__)
 
 
-def get_field_docstrings(config_class: type[Any]) -> Mapping[str, str]:
+def get_field_docstrings(dataclass: type[Any]) -> Mapping[str, str]:
     """
     Return a mapping of field name to the docstring for that field.
 
     Attribute docstrings are not supported by the Python runtime, therefore we must read them from the source code.
     If the source code cannot be found, an empty mapping is returned.
     """
 
     try:
-        source = getsource(config_class)
+        source = getsource(dataclass)
     except (OSError, TypeError):
         # According to the documentation only OSError can be raised, but Python 3.10 raises TypeError for
         # sourceless dataclasses.
         #   https://github.com/python/cpython/issues/98239
         return {}
 
     module_def = ast.parse(dedent(source), "<string>")
@@ -555,31 +572,31 @@
                 else:
                     docstrings[scope] = cleandoc(docstring)
     return docstrings
 
 
 def format_template(class_or_instance: Any) -> Iterator[str]:
     """
-    Yield lines of TOML text as a template for configuring the given data class or instance.
+    Yield lines of TOML text as a template for populating the given data class or instance.
 
     If an instance is provided, values from that instance will be used to populate the template.
     If a class is provided, values will be derived from the field types.
     """
 
     if isinstance(class_or_instance, type):
-        config_class = class_or_instance
+        dataclass = class_or_instance
         instance = None
     else:
-        config_class = class_or_instance.__class__
+        dataclass = class_or_instance.__class__
         instance = class_or_instance
 
-    docstrings = get_field_docstrings(config_class)
+    docstrings = get_field_docstrings(dataclass)
 
     first = True
-    for field in fields(config_class):
+    for field in fields(dataclass):
         if not field.init:
             continue
 
         if first:
             first = False
         else:
             yield ""
@@ -602,47 +619,45 @@
             if default is None:
                 yield "# Optional."
             else:
                 yield "# Mandatory."
             if value is None:
                 comment = "# " if default is None else ""
                 key_fmt = "".join(_iter_format_key(key))
-                value_fmt = _format_value_for_field(config_class, field)
+                value_fmt = _format_value_for_field(dataclass, field)
                 yield f"{comment}{key_fmt} = {value_fmt}"
         else:
             yield "# Default:"
             yield f"# {format_toml_pair(key, default)}"
         if value is not None:
             yield f"{format_toml_pair(key, value)}"
 
 
-def _format_value_for_field(config_class: type[Any], field: Field) -> str:
+def _format_value_for_field(dataclass: type[Any], field: Field) -> str:
     """Format an example value or placeholder for a value depending on the given field's type."""
 
-    field_type: type[Any] | str | None = field.type
-    if isinstance(field_type, str):
+    annotated_type: type[Any] | str | None = field.type
+    if isinstance(annotated_type, str):
         module_locals = {}
-        module = getmodule(config_class)
+        module = getmodule(dataclass)
         if module is not None:
             for name in dir(module):
                 module_locals[name] = getattr(module, name)
         try:
-            evaluated_type = eval(field_type, globals(), module_locals)
+            evaluated_type = eval(annotated_type, globals(), module_locals)  # noqa: PGH001
         except Exception:
-            field_type = None
-        else:
-            field_type = _collect_type(evaluated_type, f"{config_class.__name__}.{field.name}")
-
-    if field_type is None:
-        return "???"
+            return "???"
     else:
-        return _format_value_for_type(field_type)
+        evaluated_type = annotated_type
+
+    field_type = _collect_type(evaluated_type, f"{dataclass.__name__}.{field.name}")
+    return _format_value_for_type(field_type)
 
 
-def _format_value_for_type(field_type: type[Any]) -> str:
+def _format_value_for_type(field_type: type[Any] | Binder[Any]) -> str:
     origin = get_origin(field_type)
     if origin is None:
         if field_type is str:
             return "'???'"
         elif field_type is bool:
             return "true | false"
         elif field_type is int:
@@ -653,37 +668,37 @@
             return "'fully.qualified.module.name'"
         elif field_type is datetime:
             return "2020-01-01 00:00:00+01:00"
         elif field_type is date:
             return "2020-01-01"
         elif field_type is time or field_type is timedelta:
             return "00:00:00"
-        elif is_dataclass(field_type):
-            return "".join(_format_fields_inline(field_type))
+        elif isinstance(field_type, Binder):
+            return "".join(_format_fields_inline(field_type._dataclass))  # noqa: SLF001
         else:
             # We have handled all the non-generic types supported by _collect_type().
-            assert False
+            raise AssertionError(field_type)
     elif origin in (UnionType, Union):
         return " | ".join(_format_value_for_type(arg) for arg in get_args(field_type))
     elif issubclass(origin, Mapping):
         return "{}"
     elif issubclass(origin, Iterable):
         return "[]"
     elif origin is type:
         return "'fully.qualified.class.name'"
     else:
         # This is currently unreachable because we reject unsupported generic types in _collect_type().
-        assert False
+        raise AssertionError(origin)
 
 
-def _format_fields_inline(config_class: type[Any]) -> Iterable[str]:
+def _format_fields_inline(dataclass: type[Any]) -> Iterable[str]:
     yield "{"
     first = True
-    for field in fields(config_class):
+    for field in fields(dataclass):
         if first:
             first = False
         else:
             yield ", "
         yield from _iter_format_key(field.name.replace("_", "-"))
         yield " = "
-        yield _format_value_for_field(config_class, field)
+        yield _format_value_for_field(dataclass, field)
     yield "}"
```

### Comparing `dataclass_binder-0.1.3/setup.py` & `dataclass_binder-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'dataclass-binder',
-    'version': '0.1.3',
+    'version': '0.2.0',
     'description': 'Library to bind TOML data to Python dataclasses in a type-safe way.',
-    'long_description': '# Dataclass Binder\n\nLibrary to bind TOML data to Python dataclasses in a type-safe way.\n\n\n## Features\n\nCurrently it has the following properties that might set it apart from other data binding libraries:\n\n- requires Python 3.10+\n- relies only on dataclasses from the Python standard library\n- detailed error messages which mention location, expected data and actual data\n- strict parsing which considers unknown keys to be errors\n- support for durations (`timedelta`)\n- support for immutable (frozen) dataclasses\n- can bind data from files, I/O streams or pre-parsed dictionaries\n- can generate configuration templates from dataclass definitions\n\nThis library was originally designed for parsing configuration files.\nAs TOML\'s data model is very similar to JSON\'s, adding support for JSON in the future would be an option and would make the library useful for binding HTTP API requests.\n\n\n## Maturity\n\nThis library is fully type-checked, has unit tests which provide 100% branch coverage and is used in production, so it should be reliable.\n\nThe API might still change in incompatible ways until the 1.0 release.\nIn particular the following aspects are subject to change:\n\n- use of key suffixes for `timedelta`: this mechanism doesn\'t work for arrays\n- the handling of separators in keys: currently `-` in TOML is mapped to `_` in Python and `_` is forbidden in TOML; most applications seem to accept both `-` and `_` in TOML instead\n\n\n## Why Dataclasses?\n\nA typical TOML, JSON or YAML parser returns the parse results as a nested dictionary.\nYou might wonder why you would want to use a data binding library rather than just getting the values directly from that dictionary.\n\nLet\'s take the following example code for a service that connects to a database using a connection URL configured in a TOML file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\n\n\ndef read_config() -> dict:\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n    return config\n\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    print("connect to database:", url)\n\nconfig = read_config()\n...\nhandle_request(config)\n```\n\nIf the configuration is missing a `database-url` key or its value is not a string, this service would start up without complaints and then fail when the first requests comes in.\nIt would be better to instead check the configuration on startup, so let\'s add code for that:\n\n```py\ndef read_config():\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n\n    url = config["database-url"]\n    if not isinstance(url, str):\n        raise TypeError(\n            f"Value for \'database-url\' has type \'{type(url).__name__}\', expected \'str\'"\n        )\n\n    return config\n```\n\nImagine you have 20 different configurable options: you\'d need this code 20 times.\n\nNow let\'s assume that you use a type checker like `mypy`.\nInside `read_config()`, the type checker will know that `url` is a `str`, but if you fetch the same value elsewhere in the code, that information is lost:\n\n```py\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    reveal_type(url)\n    print("connect to database:", url)\n```\n\nWhen you run `mypy` on this code, it will output \'Revealed type is "Any"\'.\nFalling back to `Any` means type checking will not be able to find type mismatches and autocomplete in an IDE will not work well either.\n\nDeclaring the desired type in a dataclass solves both these issues:\n- the type can be verified at runtime before instantiating the dataclass\n- tooling knows the type when you read the value from the dataclass\n\nHaving the dataclass as a central and formal place for defining the configuration format is also an advantage.\nFor example, it enables automatic generation of a documented configuration file template.\n\n\n## Usage\n\nThe `dataclass_binder` module contains the `Binder` class which makes it easy to bind TOML data, such as a configuration file, to Python [dataclasses](https://docs.python.org/3/library/dataclasses.html).\n\nThe binding is a two-step process:\n- specialize the `Binder` class by using your top-level dataclass as a type argument\n- call the `parse_toml()` method, providing the path of the configuration file as its argument\n\nPut together, the code looks like this:\n\n```py\nimport logging\nimport sys\nfrom pathlib import Path\n\nfrom dataclass_binder import Binder\n\n\nlogger = logging.getLogger(__name__)\n\nif __name__ == "__main__":\n    config_file = Path("config.toml")\n    try:\n        config = Binder[Config].parse_toml(config_file)\n    except Exception as ex:\n        logger.critical("Error reading configuration file \'%s\': %s", config_file, ex)\n        sys.exit(1)\n```\n\n### Binding a Pre-parsed Dictionary\n\nIf you don\'t want to bind the contents of a full file, there is also the option to bind a pre-parsed dictionary instead.\nFor this, you can use the `bind()` method on the specialized `Binder` class.\n\nFor example, the following service uses a hybrid configuration format where a single file configures both the service itself and logging system:\n\n```py\nimport logging.config\n\nimport tomllib  # or \'tomli\' on Python <3.11\nfrom dataclass_binder import Binder\n\n\nwith open("config.toml", "rb") as f:\n    config = tomllib.load(f)\nservice_config = Binder[ServiceConfig].bind(config["service"])\nlogging.config.dictConfig(config["logging"])\n```\n\nTo keep these examples short, from now on `import` statements will only be included the first time a particular imported name is used.\n\n### Basic Types\n\nDataclass fields correspond to TOML keys. In the dataclass, underscores are used as word separators, while dashes are used in the TOML file. Let\'s configure a service that listens on a TCP port for requests and stores its data in a database, using the following TOML fragment:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\nport = 5432\n```\n\nThis configuration can be bound to the following dataclass:\n\n```py\nfrom dataclasses import dataclass\n\n@dataclass\nclass Config:\n    database_url: str\n    port: int\n```\n\nFields can be made optional by assigning a default value. Using `None` as a default value is allowed too:\n\n```py\n@dataclass\nclass Config:\n    verbose: bool = False\n    webhook_url: str | None = None\n```\n\nThe `float` type can be used to bind floating point numbers.\nSupport for `Decimal` is not there at the moment but would be relatively easy to add, as `tomllib`/`tomli` has an option for that.\n\n### Dates and Times\n\nTOML handles dates and timestamps as first-class values.\nDate, time and date+time TOML values are bound to `datetime.date`, `datetime.time` and `datetime.datetime` Python objects respectively.\n\nThere is also support for time intervals using `datetime.timedelta`:\n\n```py\nfrom datetime import timedelta\n\n@dataclass\nclass Config:\n    retry_after: timedelta\n    delete_after: timedelta\n```\n\nIntervals shorter than a day can be specified using a TOML time value.\nLonger intervals are supported by adding an `-hours`, `-days`, or `-weeks` suffix.\nOther supported suffixes are `-minutes`, `-seconds`, `-milliseconds` and `-microseconds`, but these are there for completeness sake and less likely to be useful.\nHere is an example TOML fragment corresponding to the dataclass above:\n\n```toml\nretry-after = 00:02:30\ndelete-after-days = 30\n```\n\n### Collections\n\nLists and dictionaries can be used to bind TOML arrays and tables.\nIf you want to make a `list` or `dict` optional, you need to provide a default value via the `default_factory` mechanism as usual, see the [dataclasses documentation](https://docs.python.org/3/library/dataclasses.html#mutable-default-values) for details.\n\n```py\nfrom dataclasses import dataclass, field\n\n@dataclass\nclass Config:\n    tags: list[str] = field(default_factory=list)\n    limits: dict[str, int]\n```\n\nThe dataclass above can be used to bind the following TOML fragment:\n\n```toml\ntags = ["production", "development"]\nlimits = {ram-gb = 1, disk-gb = 100}\n```\n\nAn alternative to `default_factory` is to use a homogeneous (single element type) tuple:\n\n```py\n@dataclass\nclass Config:\n    tags: tuple[str, ...] = ()\n    limits: dict[str, int]\n```\n\nHeterogeneous tuples are supported too: for example `tuple[str, bool]` binds a TOML array that must always have a string as its first element and a Boolean as its second and last element.\nIt is generally clearer though to define a separate dataclass when you need more than one value to configure something:\n\n```py\n@dataclass\nclass Webhook:\n    url: str\n    token: str\n\n@dataclass\nclass Config:\n    webhooks: tuple[Webhook, ...] = ()\n```\n\nThe extra keys (`url` and `token` in this example) provide the clarity:\n\n```toml\nwebhooks = [\n    {url = "https://host1/notify", token = "12345"},\n    {url = "https://host2/hook", token = "frperg"}\n]\n```\n\nTOML\'s array-of-tables syntax can make this configuration a bit easier on the eyes:\n\n```toml\n[[webhooks]]\nurl = "https://host1/notify"\ntoken = "12345"\n\n[[webhooks]]\nurl = "https://host2/hook"\ntoken = "frperg"\n```\n\nAlways define additional dataclasses at the module level in your Python code: if the class is for example defined inside a function, the `Binder` specialization will not be able to find it.\n\n### Plugins\n\nTo select plugins to activate, you can bind Python classes or modules using `type[BaseClass]` and `types.ModuleType` annotations respectively:\n\n```py\nfrom dataclasses import dataclass, field\nfrom types import ModuleType\n\nfrom supertool.plugins import PostProcessor\n\n\n@dataclass\nclass PluginConfig:\n    postprocessors = tuple[type[PostProcessor], ...] = ()\n    modules: dict[str, ModuleType] = field(default_factory=dict)\n```\n\nIn the TOML, you specify Python classes or modules using their fully qualified names:\n\n```toml\npostprocessors = ["supertool_addons.reporters.JSONReport"]\nmodules = {lint = "supertool_addons.linter"}\n```\n\nThere is no mechanism yet to add configuration to be used by the plugins.\n\n### Immutable\n\nIf you prefer immutable configuration objects, you can achieve that using the `frozen` argument of the `dataclass` decorator and using abstract collection types in the annotations. For example, the following dataclass will be instantiated with a `tuple` object for `tags` and an immutable dictionary view for `limits`:\n\n```py\nfrom collections.abc import Mapping, Sequence\n\n\n@dataclass(frozen=True)\nclass Config:\n    tags: Sequence[str] = ()\n    limits: Mapping[str, int]\n```\n\n### Generating a Configuration Template\n\nTo provide users with a starting point for configuring your application/service, you can automatically generate a configuration template from the information in the dataclass.\n\nFor example, when the following dataclass defines your configuration:\n\n```py\n@dataclass\nclass Config:\n    database_url: str\n    """The URL of the database to connect to."""\n\n    port: int = 12345\n    """TCP port on which to accept connections."""\n```\n\nYou can generate a template configuration file using:\n\n```py\nfrom dataclass_binder import format_template\n\n\nfor line in format_template(Config):\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'???\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\n```\n\nIt is also possible to provide placeholder values by passing a dataclass instance rather than the dataclass itself to `format_template()`:\n\n```py\nTEMPLATE = Config(\n    database_url="postgresql://<username>:<password>@<hostname>/<database name>",\n    port=8080,\n)\n\nfor line in format_template(TEMPLATE):\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'postgresql://<username>:<password>@<hostname>/<database name>\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\nport = 8080\n```\n\n### Troubleshooting\n\nFinally, a troubleshooting tip: instead of the full `Binder[Config].parse_toml()`, first try to execute only `Binder[Config]`.\nIf that fails, the problem is in the dataclass definitions.\nIf that succeeds, but the `parse_toml()` call fails, the problem is that the TOML file does not match the format defined in the dataclasses.\n\n\n## Development Environment\n\n[Poetry](https://python-poetry.org/) is used to set up a virtual environment with all the dependencies and development tools that you need:\n\n    $ cd dataclass-binder\n    $ poetry install\n\nYou can activate a shell which contains the development tools in its search path:\n\n    $ poetry shell\n\nWe recommend setting up pre-commit hooks for Git in the `dataclass-binder` work area.\nThese hooks automatically run a few simple checks and cleanups when you create a new commit.\nAfter you first set up your virtual environment with Poetry, run this command to install the pre-commit hooks:\n\n    $ pre-commit install\n\n\n## Release Procedure\n\n- Verify that CI passes on the branch that you want to release (typically `main`)\n- Create a release on the GitHub web interface; name the tag `v<major>.<minor>.<patchlevel>`\n- After publishing the release on GitHub, the package will be built and published on PyPI automatically via Actions\n\n\n## Changelog\n\n### 0.1.0 - 2023-02-21:\n\n- First open source release; thanks to my employer [Protix](https://protix.eu/) for making this possible\n\n### 0.1.1 - 2023-02-22:\n\n- Relax `Binder.bind()` argument type to `Mapping` ([#3](https://github.com/ProtixIT/dataclass-binder/issues/3))\n\n### 0.1.2 - 2023-03-03:\n\n- Fix `get()` and `[]` on object bound to read-only mapping ([#6](https://github.com/ProtixIT/dataclass-binder/issues/6))\n\n### 0.1.3 - 2023-03-05:\n\n- Ignore dataclass fields with `init=False` ([#2](https://github.com/ProtixIT/dataclass-binder/issues/2))\n',
+    'long_description': '# Dataclass Binder\n\nLibrary to bind TOML data to Python dataclasses in a type-safe way.\n\n\n## Features\n\nCurrently it has the following properties that might set it apart from other data binding libraries:\n\n- requires Python 3.10+\n- relies only on dataclasses from the Python standard library\n- detailed error messages which mention location, expected data and actual data\n- strict parsing which considers unknown keys to be errors\n- support for durations (`timedelta`)\n- support for immutable (frozen) dataclasses\n- can bind data from files, I/O streams or pre-parsed dictionaries\n- can generate configuration templates from dataclass definitions\n\nThis library was originally designed for parsing configuration files.\nAs TOML\'s data model is very similar to JSON\'s, adding support for JSON in the future would be an option and would make the library useful for binding HTTP API requests.\n\n\n## Maturity\n\nThis library is fully type-checked, has unit tests which provide 100% branch coverage and is used in production, so it should be reliable.\n\nThe API might still change in incompatible ways until the 1.0 release.\nIn particular the following aspects are subject to change:\n\n- use of key suffixes for `timedelta`: this mechanism doesn\'t work for arrays\n- the handling of separators in keys: currently `-` in TOML is mapped to `_` in Python and `_` is forbidden in TOML; most applications seem to accept both `-` and `_` in TOML instead\n\n\n## Why Dataclasses?\n\nA typical TOML, JSON or YAML parser returns the parse results as a nested dictionary.\nYou might wonder why you would want to use a data binding library rather than just getting the values directly from that dictionary.\n\nLet\'s take the following example code for a service that connects to a database using a connection URL configured in a TOML file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\n\n\ndef read_config() -> dict:\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n    return config\n\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    print("connect to database:", url)\n\nconfig = read_config()\n...\nhandle_request(config)\n```\n\nIf the configuration is missing a `database-url` key or its value is not a string, this service would start up without complaints and then fail when the first requests comes in.\nIt would be better to instead check the configuration on startup, so let\'s add code for that:\n\n```py\ndef read_config():\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n\n    url = config["database-url"]\n    if not isinstance(url, str):\n        raise TypeError(\n            f"Value for \'database-url\' has type \'{type(url).__name__}\', expected \'str\'"\n        )\n\n    return config\n```\n\nImagine you have 20 different configurable options: you\'d need this code 20 times.\n\nNow let\'s assume that you use a type checker like `mypy`.\nInside `read_config()`, the type checker will know that `url` is a `str`, but if you fetch the same value elsewhere in the code, that information is lost:\n\n```py\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    reveal_type(url)\n    print("connect to database:", url)\n```\n\nWhen you run `mypy` on this code, it will output \'Revealed type is "Any"\'.\nFalling back to `Any` means type checking will not be able to find type mismatches and autocomplete in an IDE will not work well either.\n\nDeclaring the desired type in a dataclass solves both these issues:\n- the type can be verified at runtime before instantiating the dataclass\n- tooling knows the type when you read the value from the dataclass\n\nHaving the dataclass as a central and formal place for defining the configuration format is also an advantage.\nFor example, it enables automatic generation of a documented configuration file template.\n\n\n## Usage\n\nThe `dataclass_binder` module contains the `Binder` class which makes it easy to bind TOML data, such as a configuration file, to Python [dataclasses](https://docs.python.org/3/library/dataclasses.html).\n\nThe binding is a two-step process:\n- instantiate the `Binder` class by passing your top-level dataclass as an argument\n- call the `parse_toml()` method, providing the path of the configuration file as its argument\n\nPut together, the code looks like this:\n\n```py\nimport logging\nimport sys\nfrom pathlib import Path\n\nfrom dataclass_binder import Binder\n\n\nlogger = logging.getLogger(__name__)\n\nif __name__ == "__main__":\n    config_file = Path("config.toml")\n    try:\n        config = Binder(Config).parse_toml(config_file)\n    except Exception as ex:\n        logger.critical("Error reading configuration file \'%s\': %s", config_file, ex)\n        sys.exit(1)\n```\n\n### Binding a Pre-parsed Dictionary\n\nIf you don\'t want to bind the contents of a full file, there is also the option to bind a pre-parsed dictionary instead.\nFor this, you can use the `bind()` method on the `Binder` object.\n\nFor example, the following service is configured by one table within a larger TOML configuration file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\nfrom dataclass_binder import Binder\n\n\nwith open("config.toml", "rb") as f:\n    config = tomllib.load(f)\nservice_config = Binder(ServiceConfig).bind(config["service"])\n```\n\nTo keep these examples short, from now on `import` statements will only be included the first time a particular imported name is used.\n\n### Basic Types\n\nDataclass fields correspond to TOML keys. In the dataclass, underscores are used as word separators, while dashes are used in the TOML file. Let\'s configure a service that listens on a TCP port for requests and stores its data in a database, using the following TOML fragment:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\nport = 8080\n```\n\nThis configuration can be bound to the following dataclass:\n\n```py\nfrom dataclasses import dataclass\n\n@dataclass\nclass Config:\n    database_url: str\n    port: int\n    verbose: bool\n```\n\nThe `float` type can be used to bind floating point numbers.\nSupport for `Decimal` is not there at the moment but would be relatively easy to add, as `tomllib`/`tomli` has an option for that.\n\n### Defaults\n\nFields can be made optional by assigning a default value. Using `None` as a default value is allowed too:\n\n```py\n@dataclass\nclass Config:\n    verbose: bool = False\n    webhook_url: str | None = None\n```\n\nIf you want to mix fields with and without defaults in any order, mark the fields as keyword-only:\n\n```py\n@dataclass(kw_only=True)\nclass Config:\n    database_url: str\n    verbose: bool = False\n    port: int\n```\n\n### Dates and Times\n\nTOML handles dates and timestamps as first-class values.\nDate, time and date+time TOML values are bound to `datetime.date`, `datetime.time` and `datetime.datetime` Python objects respectively.\n\nThere is also support for time intervals using `datetime.timedelta`:\n\n```py\nfrom datetime import timedelta\n\n@dataclass\nclass Config:\n    retry_after: timedelta\n    delete_after: timedelta\n```\n\nIntervals shorter than a day can be specified using a TOML time value.\nLonger intervals are supported by adding an `-hours`, `-days`, or `-weeks` suffix.\nOther supported suffixes are `-minutes`, `-seconds`, `-milliseconds` and `-microseconds`, but these are there for completeness sake and less likely to be useful.\nHere is an example TOML fragment corresponding to the dataclass above:\n\n```toml\nretry-after = 00:02:30\ndelete-after-days = 30\n```\n\n### Collections\n\nLists and dictionaries can be used to bind TOML arrays and tables.\nIf you want to make a `list` or `dict` optional, you need to provide a default value via the `default_factory` mechanism as usual, see the [dataclasses documentation](https://docs.python.org/3/library/dataclasses.html#mutable-default-values) for details.\n\n```py\nfrom dataclasses import dataclass, field\n\n@dataclass\nclass Config:\n    tags: list[str] = field(default_factory=list)\n    limits: dict[str, int]\n```\n\nThe dataclass above can be used to bind the following TOML fragment:\n\n```toml\ntags = ["production", "development"]\nlimits = {ram-gb = 1, disk-gb = 100}\n```\n\nAn alternative to `default_factory` is to use a homogeneous (single element type) tuple:\n\n```py\n@dataclass\nclass Config:\n    tags: tuple[str, ...] = ()\n    limits: dict[str, int]\n```\n\nHeterogeneous tuples are supported too: for example `tuple[str, bool]` binds a TOML array that must always have a string as its first element and a Boolean as its second and last element.\nIt is generally clearer though to define a separate dataclass when you need more than one value to configure something:\n\n```py\n@dataclass\nclass Webhook:\n    url: str\n    token: str\n\n@dataclass\nclass Config:\n    webhooks: tuple[Webhook, ...] = ()\n```\n\nThe extra keys (`url` and `token` in this example) provide the clarity:\n\n```toml\nwebhooks = [\n    {url = "https://host1/notify", token = "12345"},\n    {url = "https://host2/hook", token = "frperg"}\n]\n```\n\nTOML\'s array-of-tables syntax can make this configuration a bit easier on the eyes:\n\n```toml\n[[webhooks]]\nurl = "https://host1/notify"\ntoken = "12345"\n\n[[webhooks]]\nurl = "https://host2/hook"\ntoken = "frperg"\n```\n\nAlways define additional dataclasses at the module level in your Python code: if the class is for example defined inside a function, the `Binder` constructor will not be able to find it.\n\n### Untyped Data\n\nSometimes the full structure of the data you want to bind is either too complex or too much in flux to be worth fully annotating.\nIn such a situation, you can use `typing.Any` as the annotation to simply capture the output of Python\'s TOML parser without type-checking it.\n\nIn the following example, a service uses the Python standard library logging implementation, configured using the [configuration dictionary schema](https://docs.python.org/3/library/logging.config.html#logging-config-dictschema):\n\n```py\nimport logging.config\nfrom dataclasses import dataclass\nfrom typing import Any\n\nfrom dataclass_binder import Binder\n\n\n@dataclass\nclass Config:\n    database_url: str\n    logging: Any\n\n\ndef run(url: str) -> None:\n    logging.info("Service starting")\n\n\nif __name__ == "__main__":\n    config = Binder[Config].parse_toml("service.toml")\n    logging.config.dictConfig(config.logging)\n    run(config.database_url)\n```\n\nThe `service.toml` configuration file for this service could look like this:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\n\n[logging]\nversion = 1\n\n[logging.root]\nlevel = \'INFO\'\nhandlers = [\'file\']\n\n[logging.handlers.file]\nclass = \'logging.handlers.RotatingFileHandler\'\nfilename = \'service.log\'\nformatter = \'simple\'\n\n[logging.formatters.simple]\nformat = \'%(asctime)s %(name)s %(levelname)s %(message)s\'\n```\n\n### Plugins\n\nTo select plugins to activate, you can bind Python classes or modules using `type[BaseClass]` and `types.ModuleType` annotations respectively:\n\n```py\nfrom dataclasses import dataclass, field\nfrom types import ModuleType\n\nfrom supertool.plugins import PostProcessor\n\n\n@dataclass\nclass PluginConfig:\n    postprocessors = tuple[type[PostProcessor], ...] = ()\n    modules: dict[str, ModuleType] = field(default_factory=dict)\n```\n\nIn the TOML, you specify Python classes or modules using their fully qualified names:\n\n```toml\npostprocessors = ["supertool_addons.reporters.JSONReport"]\nmodules = {lint = "supertool_addons.linter"}\n```\n\nThere is no mechanism yet to add configuration to be used by the plugins.\n\n### Immutable\n\nIf you prefer immutable configuration objects, you can achieve that using the `frozen` argument of the `dataclass` decorator and using abstract collection types in the annotations. For example, the following dataclass will be instantiated with a `tuple` object for `tags` and an immutable dictionary view for `limits`:\n\n```py\nfrom collections.abc import Mapping, Sequence\n\n\n@dataclass(frozen=True)\nclass Config:\n    tags: Sequence[str] = ()\n    limits: Mapping[str, int]\n```\n\n### Generating a Configuration Template\n\nTo provide users with a starting point for configuring your application/service, you can automatically generate a configuration template from the information in the dataclass.\n\nFor example, when the following dataclass defines your configuration:\n\n```py\n@dataclass\nclass Config:\n    database_url: str\n    """The URL of the database to connect to."""\n\n    port: int = 12345\n    """TCP port on which to accept connections."""\n```\n\nYou can generate a template configuration file using:\n\n```py\nfrom dataclass_binder import format_template\n\n\nfor line in format_template(Config):\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'???\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\n```\n\nIt is also possible to provide placeholder values by passing a dataclass instance rather than the dataclass itself to `format_template()`:\n\n```py\nTEMPLATE = Config(\n    database_url="postgresql://<username>:<password>@<hostname>/<database name>",\n    port=8080,\n)\n\nfor line in format_template(TEMPLATE):\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'postgresql://<username>:<password>@<hostname>/<database name>\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\nport = 8080\n```\n\n### Troubleshooting\n\nFinally, a troubleshooting tip: instead of the full `Binder(Config).parse_toml()`, first try to execute only `Binder(Config)`.\nIf that fails, the problem is in the dataclass definitions.\nIf that succeeds, but the `parse_toml()` call fails, the problem is that the TOML file does not match the format defined in the dataclasses.\n\n\n## Development Environment\n\n[Poetry](https://python-poetry.org/) is used to set up a virtual environment with all the dependencies and development tools that you need:\n\n    $ cd dataclass-binder\n    $ poetry install\n\nYou can activate a shell which contains the development tools in its search path:\n\n    $ poetry shell\n\nWe recommend setting up pre-commit hooks for Git in the `dataclass-binder` work area.\nThese hooks automatically run a few simple checks and cleanups when you create a new commit.\nAfter you first set up your virtual environment with Poetry, run this command to install the pre-commit hooks:\n\n    $ pre-commit install\n\n\n## Release Procedure\n\n- Verify that CI passes on the branch that you want to release (typically `main`)\n- Create a release on the GitHub web interface; name the tag `v<major>.<minor>.<patchlevel>`\n- After publishing the release on GitHub, the package will be built and published on PyPI automatically via Actions\n\n\n## Deprecations\n\n### Binder Specialization\n\nPrior to version 0.2.0, the `Binder` class was specialized using a type argument (`Binder[Config]`) rather than instantiation (`Binder(config)`). The old syntax is still supported for now, but the backwards compatibility might be removed in a minor release prior to 1.0 if it becomes a maintenance burden, so please update your code.\n\n## Changelog\n\n### 0.1.0 - 2023-02-21:\n\n- First open source release; thanks to my employer [Protix](https://protix.eu/) for making this possible\n\n### 0.1.1 - 2023-02-22:\n\n- Relax `Binder.bind()` argument type to `Mapping` ([#3](https://github.com/ProtixIT/dataclass-binder/issues/3))\n\n### 0.1.2 - 2023-03-03:\n\n- Fix `get()` and `[]` on object bound to read-only mapping ([#6](https://github.com/ProtixIT/dataclass-binder/issues/6))\n\n### 0.1.3 - 2023-03-05:\n\n- Ignore dataclass fields with `init=False` ([#2](https://github.com/ProtixIT/dataclass-binder/issues/2))\n\n### 0.2.0 - 2023-06-26:\n\n- Instantiate `Binder` instead of specializing it ([#14](https://github.com/ProtixIT/dataclass-binder/pull/14))\n- Support `typing.Any` as a field annotation ([#10](https://github.com/ProtixIT/dataclass-binder/issues/10))\n- Fix crash in `format_template()` on optional fields with non-string annotations ([#16](https://github.com/ProtixIT/dataclass-binder/pull/16))\n',
     'author': 'Maarten ter Huurne',
     'author_email': 'maarten.terhuurne@protix.eu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ProtixIT/dataclass-binder',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `dataclass_binder-0.1.3/PKG-INFO` & `dataclass_binder-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-binder
-Version: 0.1.3
+Version: 0.2.0
 Summary: Library to bind TOML data to Python dataclasses in a type-safe way.
 Home-page: https://github.com/ProtixIT/dataclass-binder
 License: MIT
 Keywords: dataclass,toml,bind,binding
 Author: Maarten ter Huurne
 Author-email: maarten.terhuurne@protix.eu
 Requires-Python: >=3.10,<4.0
@@ -118,15 +118,15 @@
 
 
 ## Usage
 
 The `dataclass_binder` module contains the `Binder` class which makes it easy to bind TOML data, such as a configuration file, to Python [dataclasses](https://docs.python.org/3/library/dataclasses.html).
 
 The binding is a two-step process:
-- specialize the `Binder` class by using your top-level dataclass as a type argument
+- instantiate the `Binder` class by passing your top-level dataclass as an argument
 - call the `parse_toml()` method, providing the path of the configuration file as its argument
 
 Put together, the code looks like this:
 
 ```py
 import logging
 import sys
@@ -136,73 +136,83 @@
 
 
 logger = logging.getLogger(__name__)
 
 if __name__ == "__main__":
     config_file = Path("config.toml")
     try:
-        config = Binder[Config].parse_toml(config_file)
+        config = Binder(Config).parse_toml(config_file)
     except Exception as ex:
         logger.critical("Error reading configuration file '%s': %s", config_file, ex)
         sys.exit(1)
 ```
 
 ### Binding a Pre-parsed Dictionary
 
 If you don't want to bind the contents of a full file, there is also the option to bind a pre-parsed dictionary instead.
-For this, you can use the `bind()` method on the specialized `Binder` class.
+For this, you can use the `bind()` method on the `Binder` object.
 
-For example, the following service uses a hybrid configuration format where a single file configures both the service itself and logging system:
+For example, the following service is configured by one table within a larger TOML configuration file:
 
 ```py
-import logging.config
-
 import tomllib  # or 'tomli' on Python <3.11
 from dataclass_binder import Binder
 
 
 with open("config.toml", "rb") as f:
     config = tomllib.load(f)
-service_config = Binder[ServiceConfig].bind(config["service"])
-logging.config.dictConfig(config["logging"])
+service_config = Binder(ServiceConfig).bind(config["service"])
 ```
 
 To keep these examples short, from now on `import` statements will only be included the first time a particular imported name is used.
 
 ### Basic Types
 
 Dataclass fields correspond to TOML keys. In the dataclass, underscores are used as word separators, while dashes are used in the TOML file. Let's configure a service that listens on a TCP port for requests and stores its data in a database, using the following TOML fragment:
 
 ```toml
 database-url = 'postgresql://user:password@host/db'
-port = 5432
+port = 8080
 ```
 
 This configuration can be bound to the following dataclass:
 
 ```py
 from dataclasses import dataclass
 
 @dataclass
 class Config:
     database_url: str
     port: int
+    verbose: bool
 ```
 
+The `float` type can be used to bind floating point numbers.
+Support for `Decimal` is not there at the moment but would be relatively easy to add, as `tomllib`/`tomli` has an option for that.
+
+### Defaults
+
 Fields can be made optional by assigning a default value. Using `None` as a default value is allowed too:
 
 ```py
 @dataclass
 class Config:
     verbose: bool = False
     webhook_url: str | None = None
 ```
 
-The `float` type can be used to bind floating point numbers.
-Support for `Decimal` is not there at the moment but would be relatively easy to add, as `tomllib`/`tomli` has an option for that.
+If you want to mix fields with and without defaults in any order, mark the fields as keyword-only:
+
+```py
+@dataclass(kw_only=True)
+class Config:
+    database_url: str
+    verbose: bool = False
+    port: int
+```
 
 ### Dates and Times
 
 TOML handles dates and timestamps as first-class values.
 Date, time and date+time TOML values are bound to `datetime.date`, `datetime.time` and `datetime.datetime` Python objects respectively.
 
 There is also support for time intervals using `datetime.timedelta`:
@@ -287,15 +297,67 @@
 token = "12345"
 
 [[webhooks]]
 url = "https://host2/hook"
 token = "frperg"
 ```
 
-Always define additional dataclasses at the module level in your Python code: if the class is for example defined inside a function, the `Binder` specialization will not be able to find it.
+Always define additional dataclasses at the module level in your Python code: if the class is for example defined inside a function, the `Binder` constructor will not be able to find it.
+
+### Untyped Data
+
+Sometimes the full structure of the data you want to bind is either too complex or too much in flux to be worth fully annotating.
+In such a situation, you can use `typing.Any` as the annotation to simply capture the output of Python's TOML parser without type-checking it.
+
+In the following example, a service uses the Python standard library logging implementation, configured using the [configuration dictionary schema](https://docs.python.org/3/library/logging.config.html#logging-config-dictschema):
+
+```py
+import logging.config
+from dataclasses import dataclass
+from typing import Any
+
+from dataclass_binder import Binder
+
+
+@dataclass
+class Config:
+    database_url: str
+    logging: Any
+
+
+def run(url: str) -> None:
+    logging.info("Service starting")
+
+
+if __name__ == "__main__":
+    config = Binder[Config].parse_toml("service.toml")
+    logging.config.dictConfig(config.logging)
+    run(config.database_url)
+```
+
+The `service.toml` configuration file for this service could look like this:
+
+```toml
+database-url = 'postgresql://user:password@host/db'
+
+[logging]
+version = 1
+
+[logging.root]
+level = 'INFO'
+handlers = ['file']
+
+[logging.handlers.file]
+class = 'logging.handlers.RotatingFileHandler'
+filename = 'service.log'
+formatter = 'simple'
+
+[logging.formatters.simple]
+format = '%(asctime)s %(name)s %(levelname)s %(message)s'
+```
 
 ### Plugins
 
 To select plugins to activate, you can bind Python classes or modules using `type[BaseClass]` and `types.ModuleType` annotations respectively:
 
 ```py
 from dataclasses import dataclass, field
@@ -394,15 +456,15 @@
 # Default:
 # port = 12345
 port = 8080
 ```
 
 ### Troubleshooting
 
-Finally, a troubleshooting tip: instead of the full `Binder[Config].parse_toml()`, first try to execute only `Binder[Config]`.
+Finally, a troubleshooting tip: instead of the full `Binder(Config).parse_toml()`, first try to execute only `Binder(Config)`.
 If that fails, the problem is in the dataclass definitions.
 If that succeeds, but the `parse_toml()` call fails, the problem is that the TOML file does not match the format defined in the dataclasses.
 
 
 ## Development Environment
 
 [Poetry](https://python-poetry.org/) is used to set up a virtual environment with all the dependencies and development tools that you need:
@@ -424,14 +486,20 @@
 ## Release Procedure
 
 - Verify that CI passes on the branch that you want to release (typically `main`)
 - Create a release on the GitHub web interface; name the tag `v<major>.<minor>.<patchlevel>`
 - After publishing the release on GitHub, the package will be built and published on PyPI automatically via Actions
 
 
+## Deprecations
+
+### Binder Specialization
+
+Prior to version 0.2.0, the `Binder` class was specialized using a type argument (`Binder[Config]`) rather than instantiation (`Binder(config)`). The old syntax is still supported for now, but the backwards compatibility might be removed in a minor release prior to 1.0 if it becomes a maintenance burden, so please update your code.
+
 ## Changelog
 
 ### 0.1.0 - 2023-02-21:
 
 - First open source release; thanks to my employer [Protix](https://protix.eu/) for making this possible
 
 ### 0.1.1 - 2023-02-22:
@@ -442,7 +510,13 @@
 
 - Fix `get()` and `[]` on object bound to read-only mapping ([#6](https://github.com/ProtixIT/dataclass-binder/issues/6))
 
 ### 0.1.3 - 2023-03-05:
 
 - Ignore dataclass fields with `init=False` ([#2](https://github.com/ProtixIT/dataclass-binder/issues/2))
 
+### 0.2.0 - 2023-06-26:
+
+- Instantiate `Binder` instead of specializing it ([#14](https://github.com/ProtixIT/dataclass-binder/pull/14))
+- Support `typing.Any` as a field annotation ([#10](https://github.com/ProtixIT/dataclass-binder/issues/10))
+- Fix crash in `format_template()` on optional fields with non-string annotations ([#16](https://github.com/ProtixIT/dataclass-binder/pull/16))
+
```

