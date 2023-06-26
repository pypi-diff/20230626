# Comparing `tmp/betterproto-2.0.0b5.tar.gz` & `tmp/betterproto-2.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterproto-2.0.0b5.tar", max compression
+gzip compressed data, was "betterproto-2.0.0b6.tar", max compression
```

## Comparing `betterproto-2.0.0b5.tar` & `betterproto-2.0.0b6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    15448 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/README.md
--rw-r--r--   0        0        0     3369 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/pyproject.toml
--rw-r--r--   0        0        0    54599 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/src/betterproto/__init__.py
--rw-r--r--   0        0        0      295 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/src/betterproto/_types.py
--rw-r--r--   0        0        0       99 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/src/betterproto/_version.py
--rw-r--r--   0        0        0     3543 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/src/betterproto/casing.py
--rw-r--r--   0        0        0        0 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/src/betterproto/compile/__init__.py
--rw-r--r--   0        0        0     6337 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/src/betterproto/compile/importing.py
--rw-r--r--   0        0        0      286 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/src/betterproto/compile/naming.py
--rw-r--r--   0        0        0        0 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/src/betterproto/grpc/__init__.py
--rw-r--r--   0        0        0     5295 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/src/betterproto/grpc/grpclib_client.py
--rw-r--r--   0        0        0      883 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/src/betterproto/grpc/grpclib_server.py
--rw-r--r--   0        0        0        0 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/src/betterproto/grpc/util/__init__.py
--rw-r--r--   0        0        0     6793 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/src/betterproto/grpc/util/async_channel.py
--rw-r--r--   0        0        0        0 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/src/betterproto/lib/__init__.py
--rw-r--r--   0        0        0        0 2022-08-01 23:28:49.275258 betterproto-2.0.0b5/src/betterproto/lib/google/__init__.py
--rw-r--r--   0        0        0    67675 2022-08-01 23:28:49.279258 betterproto-2.0.0b5/src/betterproto/lib/google/protobuf/__init__.py
--rw-r--r--   0        0        0     7028 2022-08-01 23:28:49.279258 betterproto-2.0.0b5/src/betterproto/lib/google/protobuf/compiler/__init__.py
--rw-r--r--   0        0        0       23 2022-08-01 23:28:49.279258 betterproto-2.0.0b5/src/betterproto/plugin/__init__.py
--rw-r--r--   0        0        0       32 2022-08-01 23:28:49.279258 betterproto-2.0.0b5/src/betterproto/plugin/__main__.py
--rw-r--r--   0        0        0     1321 2022-08-01 23:28:49.279258 betterproto-2.0.0b5/src/betterproto/plugin/compiler.py
--rwxr-xr-x   0        0        0     1471 2022-08-01 23:28:49.279258 betterproto-2.0.0b5/src/betterproto/plugin/main.py
--rw-r--r--   0        0        0    26871 2022-08-01 23:28:49.279258 betterproto-2.0.0b5/src/betterproto/plugin/models.py
--rw-r--r--   0        0        0     7017 2022-08-01 23:28:49.279258 betterproto-2.0.0b5/src/betterproto/plugin/parser.py
--rw-r--r--   0        0        0       48 2022-08-01 23:28:49.279258 betterproto-2.0.0b5/src/betterproto/plugin/plugin.bat
--rw-r--r--   0        0        0        0 2022-08-01 23:28:49.279258 betterproto-2.0.0b5/src/betterproto/py.typed
--rw-r--r--   0        0        0     7767 2022-08-01 23:28:49.279258 betterproto-2.0.0b5/src/betterproto/templates/template.py.j2
--rw-r--r--   0        0        0    17394 2022-08-01 23:28:57.488843 betterproto-2.0.0b5/setup.py
--rw-r--r--   0        0        0    16538 2022-08-01 23:28:57.490369 betterproto-2.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-26 19:43:35.990087 betterproto-2.0.0b6/LICENSE.md
+-rw-r--r--   0        0        0    16210 2023-06-26 19:43:35.990087 betterproto-2.0.0b6/README.md
+-rw-r--r--   0        0        0     3379 2023-06-26 19:43:35.990087 betterproto-2.0.0b6/pyproject.toml
+-rw-r--r--   0        0        0    56923 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/__init__.py
+-rw-r--r--   0        0        0      295 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/_types.py
+-rw-r--r--   0        0        0      184 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/_version.py
+-rw-r--r--   0        0        0     3543 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/casing.py
+-rw-r--r--   0        0        0        0 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/compile/__init__.py
+-rw-r--r--   0        0        0     6337 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/compile/importing.py
+-rw-r--r--   0        0        0      286 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/compile/naming.py
+-rw-r--r--   0        0        0        0 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/grpc/__init__.py
+-rw-r--r--   0        0        0     5295 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/grpc/grpclib_client.py
+-rw-r--r--   0        0        0      883 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/grpc/grpclib_server.py
+-rw-r--r--   0        0        0        0 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/grpc/util/__init__.py
+-rw-r--r--   0        0        0     6793 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/grpc/util/async_channel.py
+-rw-r--r--   0        0        0        0 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/lib/google/__init__.py
+-rw-r--r--   0        0        0    70836 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/lib/google/protobuf/__init__.py
+-rw-r--r--   0        0        0     7057 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/lib/google/protobuf/compiler/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/plugin/__init__.py
+-rw-r--r--   0        0        0       32 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/plugin/__main__.py
+-rw-r--r--   0        0        0     1321 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/plugin/compiler.py
+-rwxr-xr-x   0        0        0     1471 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/plugin/main.py
+-rw-r--r--   0        0        0    28031 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/plugin/models.py
+-rw-r--r--   0        0        0     7650 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/plugin/parser.py
+-rw-r--r--   0        0        0       48 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/plugin/plugin.bat
+-rw-r--r--   0        0        0        0 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/py.typed
+-rw-r--r--   0        0        0     8733 2023-06-26 19:43:35.994087 betterproto-2.0.0b6/src/betterproto/templates/template.py.j2
+-rw-r--r--   0        0        0    17329 1970-01-01 00:00:00.000000 betterproto-2.0.0b6/PKG-INFO
```

### Comparing `betterproto-2.0.0b5/README.md` & `betterproto-2.0.0b6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 ![](https://github.com/danielgtaylor/python-betterproto/workflows/CI/badge.svg)
 > :octocat: If you're reading this on github, please be aware that it might mention unreleased features! See the latest released README on [pypi](https://pypi.org/project/betterproto/).
 
 This project aims to provide an improved experience when using Protobuf / gRPC in a modern Python environment by making use of modern language features and generating readable, understandable, idiomatic Python code. It will not support legacy features or environments (e.g. Protobuf 2). The following are supported:
 
 - Protobuf 3 & gRPC code generation
   - Both binary & JSON serialization is built-in
-- Python 3.6+ making use of:
+- Python 3.7+ making use of:
   - Enums
   - Dataclasses
   - `async`/`await`
   - Timezone-aware `datetime` and `timedelta` objects
   - Relative imports
   - Mypy type checking
+- [Pydantic Models](https://docs.pydantic.dev/) generation (see #generating-pydantic-models)
 
 This project is heavily inspired by, and borrows functionality from:
 
 - https://github.com/protocolbuffers/protobuf/tree/master/python
 - https://github.com/eigenein/protobuf/
 - https://github.com/vmagamedov/grpclib
 
@@ -360,22 +361,41 @@
 '2019-01-01T12:00:00+00:00'
 
 >>> t.maybe = None
 >>> t.to_dict()
 {'ts': '2019-01-01T12:00:00Z', 'duration': '1.200s'}
 ```
 
+## Generating Pydantic Models
+
+You can use python-betterproto to generate pydantic based models, using
+pydantic dataclasses. This means the results of the protobuf unmarshalling will
+be typed checked. The usage is the same, but you need to add a custom option
+when calling the protobuf compiler:
+
+
+```
+protoc -I . --python_betterproto_opt=pydantic_dataclasses --python_betterproto_out=lib example.proto
+```
+
+With the important change being `--python_betterproto_opt=pydantic_dataclasses`. This will
+swap the dataclass implementation from the builtin python dataclass to the
+pydantic dataclass. You must have pydantic as a dependency in your project for
+this to work.
+
+
+
 ## Development
 
 - _Join us on [Slack](https://join.slack.com/t/betterproto/shared_invite/zt-f0n0uolx-iN8gBNrkPxtKHTLpG3o1OQ)!_
 - _See how you can help &rarr; [Contributing](.github/CONTRIBUTING.md)_
 
 ### Requirements
 
-- Python (3.6 or higher)
+- Python (3.7 or higher)
 
 - [poetry](https://python-poetry.org/docs/#installation)
   *Needed to install dependencies in a virtual environment*
 
 - [poethepoet](https://github.com/nat-n/poethepoet) for running development tasks as defined in pyproject.toml
   - Can be installed to your host environment via `pip install poethepoet` then executed as simple `poe`
   - or run from the poetry venv as `poetry run poe`
@@ -443,15 +463,15 @@
 ```
 
 ### (Re)compiling Google Well-known Types
 
 Betterproto includes compiled versions for Google's well-known types at [src/betterproto/lib/google](src/betterproto/lib/google).
 Be sure to regenerate these files when modifying the plugin output format, and validate by running the tests.
 
-Normally, the plugin does not compile any references to `google.protobuf`, since they are pre-compiled. To force compilation of `google.protobuf`, use the option `--custom_opt=INCLUDE_GOOGLE`. 
+Normally, the plugin does not compile any references to `google.protobuf`, since they are pre-compiled. To force compilation of `google.protobuf`, use the option `--custom_opt=INCLUDE_GOOGLE`.
 
 Assuming your `google.protobuf` source files (included with all releases of `protoc`) are located in `/usr/local/include`, you can regenerate them as follows:
 
 ```sh
 protoc \
     --plugin=protoc-gen-custom=src/betterproto/plugin/main.py \
     --custom_opt=INCLUDE_GOOGLE \
```

### Comparing `betterproto-2.0.0b5/pyproject.toml` & `betterproto-2.0.0b6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 [tool.poetry]
 name = "betterproto"
-version = "2.0.0b5"
+version = "2.0.0b6"
 description = "A better Protobuf / gRPC generator & library"
 authors = ["Daniel G. Taylor <danielgtaylor@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/danielgtaylor/python-betterproto"
 keywords = ["protobuf", "gRPC"]
 license = "MIT"
 packages = [
     { include = "betterproto", from = "src" }
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.6.2,<4.0"
+python = "^3.7"
 black = { version = ">=19.3b0", optional = true }
-dataclasses = { version = "^0.7", python = ">=3.6, <3.7" }
 grpclib = "^0.4.1"
+importlib-metadata = { version = ">=1.6.0", python = "<3.8" }
 jinja2 = { version = ">=3.0.3", optional = true }
 python-dateutil = "^2.8"
-isort = {version = "^5.10.1", optional = true}
+isort = {version = "^5.11.5", optional = true}
 
 [tool.poetry.dev-dependencies]
 asv = "^0.4.2"
 bpython = "^0.19"
-grpcio-tools = "^1.40.0"
+grpcio-tools = "^1.54.2"
 jinja2 = ">=3.0.3"
 mypy = "^0.930"
 poethepoet = ">=0.9.0"
-protobuf = "^3.12.2"
+protobuf = "^4.21.6"
 pytest = "^6.2.5"
 pytest-asyncio = "^0.12.0"
 pytest-cov = "^2.9.0"
 pytest-mock = "^3.1.1"
 sphinx = "3.1.2"
 sphinx-rtd-theme = "0.5.0"
 tomlkit = "^0.7.0"
 tox = "^3.15.1"
 pre-commit = "^2.17.0"
+pydantic = ">=1.8.0"
 
 
 [tool.poetry.scripts]
 protoc-gen-python_betterproto = "betterproto.plugin:main"
 
 [tool.poetry.extras]
 compiler = ["black", "isort", "jinja2"]
@@ -108,15 +109,15 @@
 combine_as_imports = true
 lines_after_imports = 2
 include_trailing_comma = true
 force_grid_wrap = 2
 src_paths = ["src", "tests"]
 
 [tool.black]
-target-version = ['py36']
+target-version = ['py37']
 
 [tool.doc8]
 paths = ["docs"]
 max_line_length = 88
 
 [tool.doc8.ignore_path_errors]
 "docs/migrating.rst" = [
@@ -126,15 +127,15 @@
 [tool.coverage.run]
 omit = ["betterproto/tests/*"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = true
-envlist = py36, py37, py38, py310
+envlist = py37, py38, py310
 
 [testenv]
 whitelist_externals = poetry
 commands =
     poetry install -v --extras compiler
     poetry run pytest --cov betterproto
 """
```

### Comparing `betterproto-2.0.0b5/src/betterproto/__init__.py` & `betterproto-2.0.0b6/src/betterproto/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Generator,
     Iterable,
     List,
+    Mapping,
     Optional,
     Set,
     Tuple,
     Type,
     Union,
     get_type_hints,
 )
@@ -624,15 +625,14 @@
     def __post_init__(self) -> None:
         # Keep track of whether every field was default
         all_sentinel = True
 
         # Set current field of each group after `__init__` has already been run.
         group_current: Dict[str, Optional[str]] = {}
         for field_name, meta in self._betterproto.meta_by_field_name.items():
-
             if meta.group:
                 group_current.setdefault(meta.group)
 
             value = self.__raw_get(field_name)
             if value != PLACEHOLDER and not (meta.optional and value is None):
                 # Found a non-sentinel value
                 all_sentinel = False
@@ -700,14 +700,21 @@
                 return value
 
             value = self._get_field_default(name)
             super().__setattr__(name, value)
             return value
 
     def __setattr__(self, attr: str, value: Any) -> None:
+        if (
+            isinstance(value, Message)
+            and hasattr(value, "_betterproto")
+            and not value._betterproto.meta_by_field_name
+        ):
+            value._serialized_on_wire = True
+
         if attr != "_serialized_on_wire":
             # Track when a field has been set.
             self.__dict__["_serialized_on_wire"] = True
 
         if hasattr(self, "_group_current"):  # __post_init__ had already run
             if attr in self._betterproto.oneof_group_by_field:
                 group = self._betterproto.oneof_group_by_field[attr]
@@ -802,14 +809,15 @@
                     for item in value:
                         output += (
                             _serialize_single(
                                 meta.number,
                                 meta.proto_type,
                                 item,
                                 wraps=meta.wraps or "",
+                                serialize_empty=True,
                             )
                             # if it's an empty message it still needs to be represented
                             # as an item in the repeated list
                             or b"\n\x00"
                         )
 
             elif isinstance(value, dict):
@@ -882,18 +890,18 @@
             return self._betterproto.default_gen[field_name]()
 
     @classmethod
     def _get_field_default_gen(cls, field: dataclasses.Field) -> Any:
         t = cls._type_hint(field.name)
 
         if hasattr(t, "__origin__"):
-            if t.__origin__ in (dict, Dict):
+            if t.__origin__ is dict:
                 # This is some kind of map (dict in Python).
                 return dict
-            elif t.__origin__ in (list, List):
+            elif t.__origin__ is list:
                 # This is some kind of list (repeated) field.
                 return list
             elif t.__origin__ is Union and t.__args__[1] is type(None):
                 # This is an optional field (either wrapped, or using proto3
                 # field presence). For setting the default we really don't care
                 # what kind of field it is.
                 return type(None)
@@ -1173,15 +1181,15 @@
                         output[cased_name] = [_dump_float(n) for n in value]
                     else:
                         output[cased_name] = _dump_float(value)
                 else:
                     output[cased_name] = value
         return output
 
-    def from_dict(self: T, value: Dict[str, Any]) -> T:
+    def from_dict(self: T, value: Mapping[str, Any]) -> T:
         """
         Parse the key/value pairs into the current message instance. This returns the
         instance itself and is therefore assignable and chainable.
 
         Parameters
         -----------
         value: Dict[:class:`str`, Any]
@@ -1256,33 +1264,50 @@
                         else:
                             v = _parse_float(value[key])
 
                 if v is not None:
                     setattr(self, field_name, v)
         return self
 
-    def to_json(self, indent: Union[None, int, str] = None) -> str:
+    def to_json(
+        self,
+        indent: Union[None, int, str] = None,
+        include_default_values: bool = False,
+        casing: Casing = Casing.CAMEL,
+    ) -> str:
         """A helper function to parse the message instance into its JSON
         representation.
 
         This is equivalent to::
 
             json.dumps(message.to_dict(), indent=indent)
 
         Parameters
         -----------
         indent: Optional[Union[:class:`int`, :class:`str`]]
             The indent to pass to :func:`json.dumps`.
 
+        include_default_values: :class:`bool`
+            If ``True`` will include the default values of fields. Default is ``False``.
+            E.g. an ``int32`` field will be included with a value of ``0`` if this is
+            set to ``True``, otherwise this would be ignored.
+
+        casing: :class:`Casing`
+            The casing to use for key values. Default is :attr:`Casing.CAMEL` for
+            compatibility purposes.
+
         Returns
         --------
         :class:`str`
             The JSON representation of the message.
         """
-        return json.dumps(self.to_dict(), indent=indent)
+        return json.dumps(
+            self.to_dict(include_default_values=include_default_values, casing=casing),
+            indent=indent,
+        )
 
     def from_json(self: T, value: Union[str, bytes]) -> T:
         """A helper function to return the message instance from its JSON
         representation. This returns the instance itself and is therefore assignable
         and chainable.
 
         This is equivalent to::
@@ -1351,14 +1376,17 @@
                     if value is not None or include_default_values:
                         output[cased_name] = value
                 elif field_is_repeated:
                     # Convert each item.
                     value = [i.to_pydict(casing, include_default_values) for i in value]
                     if value or include_default_values:
                         output[cased_name] = value
+                elif value is None:
+                    if include_default_values:
+                        output[cased_name] = None
                 elif (
                     value._serialized_on_wire
                     or include_default_values
                     or self._include_default_value_for_oneof(
                         field_name=field_name, meta=meta
                     )
                 ):
@@ -1376,15 +1404,15 @@
                 or self._include_default_value_for_oneof(
                     field_name=field_name, meta=meta
                 )
             ):
                 output[cased_name] = value
         return output
 
-    def from_pydict(self: T, value: Dict[str, Any]) -> T:
+    def from_pydict(self: T, value: Mapping[str, Any]) -> T:
         """
         Parse the key/value pairs into the current message instance. This returns the
         instance itself and is therefore assignable and chainable.
 
         Parameters
         -----------
         value: Dict[:class:`str`, Any]
@@ -1448,14 +1476,44 @@
         default = (
             PLACEHOLDER
             if not self._betterproto.meta_by_field_name[name].optional
             else None
         )
         return self.__raw_get(name) is not default
 
+    @classmethod
+    def _validate_field_groups(cls, values):
+        group_to_one_ofs = cls._betterproto_meta.oneof_field_by_group  # type: ignore
+        field_name_to_meta = cls._betterproto_meta.meta_by_field_name  # type: ignore
+
+        for group, field_set in group_to_one_ofs.items():
+
+            if len(field_set) == 1:
+                (field,) = field_set
+                field_name = field.name
+                meta = field_name_to_meta[field_name]
+
+                # This is a synthetic oneof; we should ignore it's presence and not consider it as a oneof.
+                if meta.optional:
+                    continue
+
+            set_fields = [
+                field.name for field in field_set if values[field.name] is not None
+            ]
+
+            if not set_fields:
+                raise ValueError(f"Group {group} has no value; all fields are None")
+            elif len(set_fields) > 1:
+                set_fields_str = ", ".join(set_fields)
+                raise ValueError(
+                    f"Group {group} has more than one value; fields {set_fields_str} are not None"
+                )
+
+        return values
+
 
 def serialized_on_wire(message: Message) -> bool:
     """
     If this message was or should be serialized on the wire. This can be used to detect
     presence (e.g. optional wrapper message) and is used internally during
     parsing/serialization.
 
@@ -1531,14 +1589,17 @@
     def to_datetime(self) -> datetime:
         ts = self.seconds + (self.nanos / 1e9)
         return datetime.fromtimestamp(ts, tz=timezone.utc)
 
     @staticmethod
     def timestamp_to_json(dt: datetime) -> str:
         nanos = dt.microsecond * 1e3
+        if dt.tzinfo is not None:
+            # change timezone aware datetime objects to utc
+            dt = dt.astimezone(timezone.utc)
         copy = dt.replace(microsecond=0, tzinfo=None)
         result = copy.isoformat()
         if (nanos % 1e9) == 0:
             # If there are 0 fractional digits, the fractional
             # point '.' should be omitted when serializing.
             return f"{result}Z"
         if (nanos % 1e6) == 0:
```

### Comparing `betterproto-2.0.0b5/src/betterproto/casing.py` & `betterproto-2.0.0b6/src/betterproto/casing.py`

 * *Files identical despite different names*

### Comparing `betterproto-2.0.0b5/src/betterproto/compile/importing.py` & `betterproto-2.0.0b6/src/betterproto/compile/importing.py`

 * *Files identical despite different names*

### Comparing `betterproto-2.0.0b5/src/betterproto/grpc/grpclib_client.py` & `betterproto-2.0.0b6/src/betterproto/grpc/grpclib_client.py`

 * *Files identical despite different names*

### Comparing `betterproto-2.0.0b5/src/betterproto/grpc/grpclib_server.py` & `betterproto-2.0.0b6/src/betterproto/grpc/grpclib_server.py`

 * *Files identical despite different names*

### Comparing `betterproto-2.0.0b5/src/betterproto/grpc/util/async_channel.py` & `betterproto-2.0.0b6/src/betterproto/grpc/util/async_channel.py`

 * *Files identical despite different names*

### Comparing `betterproto-2.0.0b5/src/betterproto/lib/google/protobuf/__init__.py` & `betterproto-2.0.0b6/src/betterproto/lib/google/protobuf/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,119 +1,207 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: google/protobuf/any.proto, google/protobuf/api.proto, google/protobuf/descriptor.proto, google/protobuf/duration.proto, google/protobuf/empty.proto, google/protobuf/field_mask.proto, google/protobuf/source_context.proto, google/protobuf/struct.proto, google/protobuf/timestamp.proto, google/protobuf/type.proto, google/protobuf/wrappers.proto
 # plugin: python-betterproto
+# This file has been @generated
 import warnings
 from dataclasses import dataclass
 from typing import (
     Dict,
     List,
 )
 
 import betterproto
-from betterproto.grpc.grpclib_server import ServiceBase
 
 
 class Syntax(betterproto.Enum):
     """The syntax in which a protocol buffer element is defined."""
 
-    # Syntax `proto2`.
     SYNTAX_PROTO2 = 0
-    # Syntax `proto3`.
+    """Syntax `proto2`."""
+
     SYNTAX_PROTO3 = 1
+    """Syntax `proto3`."""
 
 
 class FieldKind(betterproto.Enum):
+    """Basic field types."""
+
     TYPE_UNKNOWN = 0
+    """Field type unknown."""
+
     TYPE_DOUBLE = 1
+    """Field type double."""
+
     TYPE_FLOAT = 2
+    """Field type float."""
+
     TYPE_INT64 = 3
+    """Field type int64."""
+
     TYPE_UINT64 = 4
+    """Field type uint64."""
+
     TYPE_INT32 = 5
+    """Field type int32."""
+
     TYPE_FIXED64 = 6
+    """Field type fixed64."""
+
     TYPE_FIXED32 = 7
+    """Field type fixed32."""
+
     TYPE_BOOL = 8
+    """Field type bool."""
+
     TYPE_STRING = 9
+    """Field type string."""
+
     TYPE_GROUP = 10
+    """Field type group. Proto2 syntax only, and deprecated."""
+
     TYPE_MESSAGE = 11
+    """Field type message."""
+
     TYPE_BYTES = 12
+    """Field type bytes."""
+
     TYPE_UINT32 = 13
+    """Field type uint32."""
+
     TYPE_ENUM = 14
+    """Field type enum."""
+
     TYPE_SFIXED32 = 15
+    """Field type sfixed32."""
+
     TYPE_SFIXED64 = 16
+    """Field type sfixed64."""
+
     TYPE_SINT32 = 17
+    """Field type sint32."""
+
     TYPE_SINT64 = 18
+    """Field type sint64."""
 
 
 class FieldCardinality(betterproto.Enum):
+    """Whether a field is optional, required, or repeated."""
+
     CARDINALITY_UNKNOWN = 0
+    """For fields with unknown cardinality."""
+
     CARDINALITY_OPTIONAL = 1
+    """For optional fields."""
+
     CARDINALITY_REQUIRED = 2
+    """For required fields. Proto2 syntax only."""
+
     CARDINALITY_REPEATED = 3
+    """For repeated fields."""
 
 
 class FieldDescriptorProtoType(betterproto.Enum):
     TYPE_DOUBLE = 1
+    """0 is reserved for errors. Order is weird for historical reasons."""
+
     TYPE_FLOAT = 2
     TYPE_INT64 = 3
+    """
+    Not ZigZag encoded.  Negative numbers take 10 bytes.  Use TYPE_SINT64 if
+    negative values are likely.
+    """
+
     TYPE_UINT64 = 4
     TYPE_INT32 = 5
+    """
+    Not ZigZag encoded.  Negative numbers take 10 bytes.  Use TYPE_SINT32 if
+    negative values are likely.
+    """
+
     TYPE_FIXED64 = 6
     TYPE_FIXED32 = 7
     TYPE_BOOL = 8
     TYPE_STRING = 9
     TYPE_GROUP = 10
+    """
+    Tag-delimited aggregate. Group type is deprecated and not supported in
+    proto3. However, Proto3 implementations should still be able to parse the
+    group wire format and treat group fields as unknown fields.
+    """
+
     TYPE_MESSAGE = 11
     TYPE_BYTES = 12
+    """New in version 2."""
+
     TYPE_UINT32 = 13
     TYPE_ENUM = 14
     TYPE_SFIXED32 = 15
     TYPE_SFIXED64 = 16
     TYPE_SINT32 = 17
     TYPE_SINT64 = 18
 
 
 class FieldDescriptorProtoLabel(betterproto.Enum):
     LABEL_OPTIONAL = 1
+    """0 is reserved for errors"""
+
     LABEL_REQUIRED = 2
     LABEL_REPEATED = 3
 
 
 class FileOptionsOptimizeMode(betterproto.Enum):
+    """Generated classes can be optimized for speed or code size."""
+
     SPEED = 1
     CODE_SIZE = 2
+    """etc."""
+
     LITE_RUNTIME = 3
 
 
 class FieldOptionsCType(betterproto.Enum):
     STRING = 0
+    """Default mode."""
+
     CORD = 1
     STRING_PIECE = 2
 
 
 class FieldOptionsJsType(betterproto.Enum):
     JS_NORMAL = 0
+    """Use the default type."""
+
     JS_STRING = 1
+    """Use JavaScript strings."""
+
     JS_NUMBER = 2
+    """Use JavaScript numbers."""
 
 
 class MethodOptionsIdempotencyLevel(betterproto.Enum):
+    """
+    Is this method side-effect-free (or safe in HTTP parlance), or idempotent,
+    or neither? HTTP based RPC implementation may choose GET verb for safe
+    methods, and PUT verb for idempotent methods instead of the default POST.
+    """
+
     IDEMPOTENCY_UNKNOWN = 0
     NO_SIDE_EFFECTS = 1
     IDEMPOTENT = 2
 
 
 class NullValue(betterproto.Enum):
     """
     `NullValue` is a singleton enumeration to represent the null value for the
     `Value` type union.  The JSON representation for `NullValue` is JSON
     `null`.
     """
 
-    # Null value.
     NULL_VALUE = 0
+    """Null value."""
 
 
 @dataclass(eq=False, repr=False)
 class Any(betterproto.Message):
     """
     `Any` contains an arbitrary serialized protocol buffer message along with a
     URL that describes the type of the serialized message. Protobuf library
@@ -121,165 +209,203 @@
     or additional generated methods of the Any type. Example 1: Pack and unpack
     a message in C++.     Foo foo = ...;     Any any;     any.PackFrom(foo);
     ...     if (any.UnpackTo(&foo)) {       ...     } Example 2: Pack and
     unpack a message in Java.     Foo foo = ...;     Any any = Any.pack(foo);
     ...     if (any.is(Foo.class)) {       foo = any.unpack(Foo.class);     }
     Example 3: Pack and unpack a message in Python.     foo = Foo(...)     any
     = Any()     any.Pack(foo)     ...     if any.Is(Foo.DESCRIPTOR):
-    any.Unpack(foo)       ...  Example 4: Pack and unpack a message in Go
+    any.Unpack(foo)       ... Example 4: Pack and unpack a message in Go
     foo := &pb.Foo{...}      any, err := anypb.New(foo)      if err != nil {
     ...      }      ...      foo := &pb.Foo{}      if err :=
     any.UnmarshalTo(foo); err != nil {        ...      } The pack methods
     provided by protobuf library will by default use
     'type.googleapis.com/full.type.name' as the type URL and the unpack methods
     only use the fully qualified type name after the last '/' in the type URL,
-    for example "foo.bar.com/x/y.z" will yield type name "y.z". JSON ==== The
-    JSON representation of an `Any` value uses the regular representation of
-    the deserialized, embedded message, with an additional field `@type` which
+    for example "foo.bar.com/x/y.z" will yield type name "y.z". JSON The JSON
+    representation of an `Any` value uses the regular representation of the
+    deserialized, embedded message, with an additional field `@type` which
     contains the type URL. Example:     package google.profile;     message
     Person {       string first_name = 1;       string last_name = 2;     }
     {       "@type": "type.googleapis.com/google.profile.Person",
     "firstName": <string>,       "lastName": <string>     } If the embedded
     message type is well-known and has a custom JSON representation, that
     representation will be embedded adding a field `value` which holds the
     custom JSON in addition to the `@type` field. Example (for message
     [google.protobuf.Duration][]):     {       "@type":
     "type.googleapis.com/google.protobuf.Duration",       "value": "1.212s"
     }
     """
 
-    # A URL/resource name that uniquely identifies the type of the serialized
-    # protocol buffer message. This string must contain at least one "/"
-    # character. The last segment of the URL's path must represent the fully
-    # qualified name of the type (as in `path/google.protobuf.Duration`). The
-    # name should be in a canonical form (e.g., leading "." is not accepted). In
-    # practice, teams usually precompile into the binary all types that they
-    # expect it to use in the context of Any. However, for URLs which use the
-    # scheme `http`, `https`, or no scheme, one can optionally set up a type
-    # server that maps type URLs to message definitions as follows: * If no
-    # scheme is provided, `https` is assumed. * An HTTP GET on the URL must yield
-    # a [google.protobuf.Type][]   value in binary format, or produce an error. *
-    # Applications are allowed to cache lookup results based on the   URL, or
-    # have them precompiled into a binary to avoid any   lookup. Therefore,
-    # binary compatibility needs to be preserved   on changes to types. (Use
-    # versioned type names to manage   breaking changes.) Note: this
-    # functionality is not currently available in the official protobuf release,
-    # and it is not used for type URLs beginning with type.googleapis.com.
-    # Schemes other than `http`, `https` (or the empty scheme) might be used with
-    # implementation specific semantics.
     type_url: str = betterproto.string_field(1)
-    # Must be a valid serialized protocol buffer of the above specified type.
+    """
+    A URL/resource name that uniquely identifies the type of the serialized
+    protocol buffer message. This string must contain at least one "/"
+    character. The last segment of the URL's path must represent the fully
+    qualified name of the type (as in `path/google.protobuf.Duration`). The
+    name should be in a canonical form (e.g., leading "." is not accepted). In
+    practice, teams usually precompile into the binary all types that they
+    expect it to use in the context of Any. However, for URLs which use the
+    scheme `http`, `https`, or no scheme, one can optionally set up a type
+    server that maps type URLs to message definitions as follows: * If no
+    scheme is provided, `https` is assumed. * An HTTP GET on the URL must yield
+    a [google.protobuf.Type][]   value in binary format, or produce an error. *
+    Applications are allowed to cache lookup results based on the   URL, or
+    have them precompiled into a binary to avoid any   lookup. Therefore,
+    binary compatibility needs to be preserved   on changes to types. (Use
+    versioned type names to manage   breaking changes.) Note: this
+    functionality is not currently available in the official protobuf release,
+    and it is not used for type URLs beginning with type.googleapis.com.
+    Schemes other than `http`, `https` (or the empty scheme) might be used with
+    implementation specific semantics.
+    """
+
     value: bytes = betterproto.bytes_field(2)
+    """
+    Must be a valid serialized protocol buffer of the above specified type.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class SourceContext(betterproto.Message):
     """
     `SourceContext` represents information about the source of a protobuf
     element, like the file in which it is defined.
     """
 
-    # The path-qualified name of the .proto file that contained the associated
-    # protobuf element.  For example: `"google/protobuf/source_context.proto"`.
     file_name: str = betterproto.string_field(1)
+    """
+    The path-qualified name of the .proto file that contained the associated
+    protobuf element.  For example: `"google/protobuf/source_context.proto"`.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class Type(betterproto.Message):
     """A protocol buffer message type."""
 
-    # The fully qualified message name.
     name: str = betterproto.string_field(1)
-    # The list of fields.
+    """The fully qualified message name."""
+
     fields: List["Field"] = betterproto.message_field(2)
-    # The list of types appearing in `oneof` definitions in this type.
+    """The list of fields."""
+
     oneofs: List[str] = betterproto.string_field(3)
-    # The protocol buffer options.
+    """The list of types appearing in `oneof` definitions in this type."""
+
     options: List["Option"] = betterproto.message_field(4)
-    # The source context.
+    """The protocol buffer options."""
+
     source_context: "SourceContext" = betterproto.message_field(5)
-    # The source syntax.
+    """The source context."""
+
     syntax: "Syntax" = betterproto.enum_field(6)
+    """The source syntax."""
 
 
 @dataclass(eq=False, repr=False)
 class Field(betterproto.Message):
     """A single field of a message type."""
 
-    # The field type.
     kind: "FieldKind" = betterproto.enum_field(1)
-    # The field cardinality.
+    """The field type."""
+
     cardinality: "FieldCardinality" = betterproto.enum_field(2)
-    # The field number.
+    """The field cardinality."""
+
     number: int = betterproto.int32_field(3)
-    # The field name.
+    """The field number."""
+
     name: str = betterproto.string_field(4)
-    # The field type URL, without the scheme, for message or enumeration types.
-    # Example: `"type.googleapis.com/google.protobuf.Timestamp"`.
+    """The field name."""
+
     type_url: str = betterproto.string_field(6)
-    # The index of the field type in `Type.oneofs`, for message or enumeration
-    # types. The first type has index 1; zero means the type is not in the list.
+    """
+    The field type URL, without the scheme, for message or enumeration types.
+    Example: `"type.googleapis.com/google.protobuf.Timestamp"`.
+    """
+
     oneof_index: int = betterproto.int32_field(7)
-    # Whether to use alternative packed wire representation.
+    """
+    The index of the field type in `Type.oneofs`, for message or enumeration
+    types. The first type has index 1; zero means the type is not in the list.
+    """
+
     packed: bool = betterproto.bool_field(8)
-    # The protocol buffer options.
+    """Whether to use alternative packed wire representation."""
+
     options: List["Option"] = betterproto.message_field(9)
-    # The field JSON name.
+    """The protocol buffer options."""
+
     json_name: str = betterproto.string_field(10)
-    # The string value of the default value of this field. Proto2 syntax only.
+    """The field JSON name."""
+
     default_value: str = betterproto.string_field(11)
+    """
+    The string value of the default value of this field. Proto2 syntax only.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class Enum(betterproto.Message):
     """Enum type definition."""
 
-    # Enum type name.
     name: str = betterproto.string_field(1)
-    # Enum value definitions.
+    """Enum type name."""
+
     enumvalue: List["EnumValue"] = betterproto.message_field(
         2, wraps=betterproto.TYPE_ENUM
     )
-    # Protocol buffer options.
+    """Enum value definitions."""
+
     options: List["Option"] = betterproto.message_field(3)
-    # The source context.
+    """Protocol buffer options."""
+
     source_context: "SourceContext" = betterproto.message_field(4)
-    # The source syntax.
+    """The source context."""
+
     syntax: "Syntax" = betterproto.enum_field(5)
+    """The source syntax."""
 
 
 @dataclass(eq=False, repr=False)
 class EnumValue(betterproto.Message):
     """Enum value definition."""
 
-    # Enum value name.
     name: str = betterproto.string_field(1)
-    # Enum value number.
+    """Enum value name."""
+
     number: int = betterproto.int32_field(2)
-    # Protocol buffer options.
+    """Enum value number."""
+
     options: List["Option"] = betterproto.message_field(3)
+    """Protocol buffer options."""
 
 
 @dataclass(eq=False, repr=False)
 class Option(betterproto.Message):
     """
     A protocol buffer option, which can be attached to a message, field,
     enumeration, etc.
     """
 
-    # The option's name. For protobuf built-in options (options defined in
-    # descriptor.proto), this is the short name. For example, `"map_entry"`. For
-    # custom options, it should be the fully-qualified name. For example,
-    # `"google.api.http"`.
     name: str = betterproto.string_field(1)
-    # The option's value packed in an Any message. If the value is a primitive,
-    # the corresponding wrapper type defined in google/protobuf/wrappers.proto
-    # should be used. If the value is an enum, it should be stored as an int32
-    # value using the google.protobuf.Int32Value type.
+    """
+    The option's name. For protobuf built-in options (options defined in
+    descriptor.proto), this is the short name. For example, `"map_entry"`. For
+    custom options, it should be the fully-qualified name. For example,
+    `"google.api.http"`.
+    """
+
     value: "Any" = betterproto.message_field(2)
+    """
+    The option's value packed in an Any message. If the value is a primitive,
+    the corresponding wrapper type defined in google/protobuf/wrappers.proto
+    should be used. If the value is an enum, it should be stored as an int32
+    value using the google.protobuf.Int32Value type.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class Api(betterproto.Message):
     """
     Api is a light-weight descriptor for an API Interface. Interfaces are also
     described as "protocol buffer services" in some contexts, such as by the
@@ -287,62 +413,80 @@
     Services, which represent a concrete implementation of an interface as
     opposed to simply a description of methods and bindings. They are also
     sometimes simply referred to as "APIs" in other contexts, such as the name
     of this message itself. See https://cloud.google.com/apis/design/glossary
     for detailed terminology.
     """
 
-    # The fully qualified name of this interface, including package name followed
-    # by the interface's simple name.
     name: str = betterproto.string_field(1)
-    # The methods of this interface, in unspecified order.
+    """
+    The fully qualified name of this interface, including package name followed
+    by the interface's simple name.
+    """
+
     methods: List["Method"] = betterproto.message_field(2)
-    # Any metadata attached to the interface.
+    """The methods of this interface, in unspecified order."""
+
     options: List["Option"] = betterproto.message_field(3)
-    # A version string for this interface. If specified, must have the form
-    # `major-version.minor-version`, as in `1.10`. If the minor version is
-    # omitted, it defaults to zero. If the entire version field is empty, the
-    # major version is derived from the package name, as outlined below. If the
-    # field is not empty, the version in the package name will be verified to be
-    # consistent with what is provided here. The versioning schema uses [semantic
-    # versioning](http://semver.org) where the major version number indicates a
-    # breaking change and the minor version an additive, non-breaking change.
-    # Both version numbers are signals to users what to expect from different
-    # versions, and should be carefully chosen based on the product plan. The
-    # major version is also reflected in the package name of the interface, which
-    # must end in `v<major-version>`, as in `google.feature.v1`. For major
-    # versions 0 and 1, the suffix can be omitted. Zero major versions must only
-    # be used for experimental, non-GA interfaces.
+    """Any metadata attached to the interface."""
+
     version: str = betterproto.string_field(4)
-    # Source context for the protocol buffer service represented by this message.
+    """
+    A version string for this interface. If specified, must have the form
+    `major-version.minor-version`, as in `1.10`. If the minor version is
+    omitted, it defaults to zero. If the entire version field is empty, the
+    major version is derived from the package name, as outlined below. If the
+    field is not empty, the version in the package name will be verified to be
+    consistent with what is provided here. The versioning schema uses [semantic
+    versioning](http://semver.org) where the major version number indicates a
+    breaking change and the minor version an additive, non-breaking change.
+    Both version numbers are signals to users what to expect from different
+    versions, and should be carefully chosen based on the product plan. The
+    major version is also reflected in the package name of the interface, which
+    must end in `v<major-version>`, as in `google.feature.v1`. For major
+    versions 0 and 1, the suffix can be omitted. Zero major versions must only
+    be used for experimental, non-GA interfaces.
+    """
+
     source_context: "SourceContext" = betterproto.message_field(5)
-    # Included interfaces. See [Mixin][].
+    """
+    Source context for the protocol buffer service represented by this message.
+    """
+
     mixins: List["Mixin"] = betterproto.message_field(6)
-    # The source syntax of the service.
+    """Included interfaces. See [Mixin][]."""
+
     syntax: "Syntax" = betterproto.enum_field(7)
+    """The source syntax of the service."""
 
 
 @dataclass(eq=False, repr=False)
 class Method(betterproto.Message):
     """Method represents a method of an API interface."""
 
-    # The simple name of this method.
     name: str = betterproto.string_field(1)
-    # A URL of the input message type.
+    """The simple name of this method."""
+
     request_type_url: str = betterproto.string_field(2)
-    # If true, the request is streamed.
+    """A URL of the input message type."""
+
     request_streaming: bool = betterproto.bool_field(3)
-    # The URL of the output message type.
+    """If true, the request is streamed."""
+
     response_type_url: str = betterproto.string_field(4)
-    # If true, the response is streamed.
+    """The URL of the output message type."""
+
     response_streaming: bool = betterproto.bool_field(5)
-    # Any metadata attached to the method.
+    """If true, the response is streamed."""
+
     options: List["Option"] = betterproto.message_field(6)
-    # The source syntax of this method.
+    """Any metadata attached to the method."""
+
     syntax: "Syntax" = betterproto.enum_field(7)
+    """The source syntax of this method."""
 
 
 @dataclass(eq=False, repr=False)
 class Mixin(betterproto.Message):
     """
     Declares an API Interface to be included in this interface. The including
     interface must redeclare all the methods from the included interface, but
@@ -376,18 +520,21 @@
     google.acl.v1.AccessControl         root: acls This implies the following
     inherited HTTP annotation:     service Storage {       // Get the
     underlying ACL object.       rpc GetAcl(GetAclRequest) returns (Acl) {
     option (google.api.http).get = "/v2/acls/{resource=**}:getAcl";       }
     ...     }
     """
 
-    # The fully qualified name of the interface which is included.
     name: str = betterproto.string_field(1)
-    # If non-empty specifies a path under which inherited HTTP paths are rooted.
+    """The fully qualified name of the interface which is included."""
+
     root: str = betterproto.string_field(2)
+    """
+    If non-empty specifies a path under which inherited HTTP paths are rooted.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class FileDescriptorSet(betterproto.Message):
     """
     The protocol compiler can output a FileDescriptorSet containing the .proto
     files it parses.
@@ -398,35 +545,46 @@
 
 @dataclass(eq=False, repr=False)
 class FileDescriptorProto(betterproto.Message):
     """Describes a complete .proto file."""
 
     name: str = betterproto.string_field(1)
     package: str = betterproto.string_field(2)
-    # Names of files imported by this file.
     dependency: List[str] = betterproto.string_field(3)
-    # Indexes of the public imported files in the dependency list above.
+    """Names of files imported by this file."""
+
     public_dependency: List[int] = betterproto.int32_field(10)
-    # Indexes of the weak imported files in the dependency list. For Google-
-    # internal migration only. Do not use.
+    """Indexes of the public imported files in the dependency list above."""
+
     weak_dependency: List[int] = betterproto.int32_field(11)
-    # All top-level definitions in this file.
+    """
+    Indexes of the weak imported files in the dependency list. For Google-
+    internal migration only. Do not use.
+    """
+
     message_type: List["DescriptorProto"] = betterproto.message_field(4)
+    """All top-level definitions in this file."""
+
     enum_type: List["EnumDescriptorProto"] = betterproto.message_field(5)
     service: List["ServiceDescriptorProto"] = betterproto.message_field(6)
     extension: List["FieldDescriptorProto"] = betterproto.message_field(7)
     options: "FileOptions" = betterproto.message_field(8)
-    # This field contains optional information about the original source code.
-    # You may safely remove this entire field without harming runtime
-    # functionality of the descriptors -- the information is needed only by
-    # development tools.
     source_code_info: "SourceCodeInfo" = betterproto.message_field(9)
-    # The syntax of the proto file. The supported values are "proto2" and
-    # "proto3".
+    """
+    This field contains optional information about the original source code.
+    You may safely remove this entire field without harming runtime
+    functionality of the descriptors -- the information is needed only by
+    development tools.
+    """
+
     syntax: str = betterproto.string_field(12)
+    """
+    The syntax of the proto file. The supported values are "proto2" and
+    "proto3".
+    """
 
 
 @dataclass(eq=False, repr=False)
 class DescriptorProto(betterproto.Message):
     """Describes a message type."""
 
     name: str = betterproto.string_field(1)
@@ -436,17 +594,19 @@
     enum_type: List["EnumDescriptorProto"] = betterproto.message_field(4)
     extension_range: List["DescriptorProtoExtensionRange"] = betterproto.message_field(
         5
     )
     oneof_decl: List["OneofDescriptorProto"] = betterproto.message_field(8)
     options: "MessageOptions" = betterproto.message_field(7)
     reserved_range: List["DescriptorProtoReservedRange"] = betterproto.message_field(9)
-    # Reserved field names, which may not be used by fields in the same message.
-    # A given name may only be reserved once.
     reserved_name: List[str] = betterproto.string_field(10)
+    """
+    Reserved field names, which may not be used by fields in the same message.
+    A given name may only be reserved once.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class DescriptorProtoExtensionRange(betterproto.Message):
     start: int = betterproto.int32_field(1)
     end: int = betterproto.int32_field(2)
     options: "ExtensionRangeOptions" = betterproto.message_field(3)
@@ -462,67 +622,87 @@
 
     start: int = betterproto.int32_field(1)
     end: int = betterproto.int32_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class ExtensionRangeOptions(betterproto.Message):
-    # The parser stores options it doesn't recognize here. See above.
     uninterpreted_option: List["UninterpretedOption"] = betterproto.message_field(999)
+    """The parser stores options it doesn't recognize here. See above."""
 
 
 @dataclass(eq=False, repr=False)
 class FieldDescriptorProto(betterproto.Message):
     """Describes a field within a message."""
 
     name: str = betterproto.string_field(1)
     number: int = betterproto.int32_field(3)
     label: "FieldDescriptorProtoLabel" = betterproto.enum_field(4)
-    # If type_name is set, this need not be set.  If both this and type_name are
-    # set, this must be one of TYPE_ENUM, TYPE_MESSAGE or TYPE_GROUP.
     type: "FieldDescriptorProtoType" = betterproto.enum_field(5)
-    # For message and enum types, this is the name of the type.  If the name
-    # starts with a '.', it is fully-qualified.  Otherwise, C++-like scoping
-    # rules are used to find the type (i.e. first the nested types within this
-    # message are searched, then within the parent, on up to the root namespace).
+    """
+    If type_name is set, this need not be set.  If both this and type_name are
+    set, this must be one of TYPE_ENUM, TYPE_MESSAGE or TYPE_GROUP.
+    """
+
     type_name: str = betterproto.string_field(6)
-    # For extensions, this is the name of the type being extended.  It is
-    # resolved in the same manner as type_name.
+    """
+    For message and enum types, this is the name of the type.  If the name
+    starts with a '.', it is fully-qualified.  Otherwise, C++-like scoping
+    rules are used to find the type (i.e. first the nested types within this
+    message are searched, then within the parent, on up to the root namespace).
+    """
+
     extendee: str = betterproto.string_field(2)
-    # For numeric types, contains the original text representation of the value.
-    # For booleans, "true" or "false". For strings, contains the default text
-    # contents (not escaped in any way). For bytes, contains the C escaped value.
-    # All bytes >= 128 are escaped. TODO(kenton):  Base-64 encode?
+    """
+    For extensions, this is the name of the type being extended.  It is
+    resolved in the same manner as type_name.
+    """
+
     default_value: str = betterproto.string_field(7)
-    # If set, gives the index of a oneof in the containing type's oneof_decl
-    # list.  This field is a member of that oneof.
+    """
+    For numeric types, contains the original text representation of the value.
+    For booleans, "true" or "false". For strings, contains the default text
+    contents (not escaped in any way). For bytes, contains the C escaped value.
+    All bytes >= 128 are escaped.
+    """
+
     oneof_index: int = betterproto.int32_field(9)
-    # JSON name of this field. The value is set by protocol compiler. If the user
-    # has set a "json_name" option on this field, that option's value will be
-    # used. Otherwise, it's deduced from the field's name by converting it to
-    # camelCase.
+    """
+    If set, gives the index of a oneof in the containing type's oneof_decl
+    list.  This field is a member of that oneof.
+    """
+
     json_name: str = betterproto.string_field(10)
+    """
+    JSON name of this field. The value is set by protocol compiler. If the user
+    has set a "json_name" option on this field, that option's value will be
+    used. Otherwise, it's deduced from the field's name by converting it to
+    camelCase.
+    """
+
     options: "FieldOptions" = betterproto.message_field(8)
-    # If true, this is a proto3 "optional". When a proto3 field is optional, it
-    # tracks presence regardless of field type. When proto3_optional is true,
-    # this field must be belong to a oneof to signal to old proto3 clients that
-    # presence is tracked for this field. This oneof is known as a "synthetic"
-    # oneof, and this field must be its sole member (each proto3 optional field
-    # gets its own synthetic oneof). Synthetic oneofs exist in the descriptor
-    # only, and do not generate any API. Synthetic oneofs must be ordered after
-    # all "real" oneofs. For message fields, proto3_optional doesn't create any
-    # semantic change, since non-repeated message fields always track presence.
-    # However it still indicates the semantic detail of whether the user wrote
-    # "optional" or not. This can be useful for round-tripping the .proto file.
-    # For consistency we give message fields a synthetic oneof also, even though
-    # it is not required to track presence. This is especially important because
-    # the parser can't tell if a field is a message or an enum, so it must always
-    # create a synthetic oneof. Proto2 optional fields do not set this flag,
-    # because they already indicate optional with `LABEL_OPTIONAL`.
     proto3_optional: bool = betterproto.bool_field(17)
+    """
+    If true, this is a proto3 "optional". When a proto3 field is optional, it
+    tracks presence regardless of field type. When proto3_optional is true,
+    this field must be belong to a oneof to signal to old proto3 clients that
+    presence is tracked for this field. This oneof is known as a "synthetic"
+    oneof, and this field must be its sole member (each proto3 optional field
+    gets its own synthetic oneof). Synthetic oneofs exist in the descriptor
+    only, and do not generate any API. Synthetic oneofs must be ordered after
+    all "real" oneofs. For message fields, proto3_optional doesn't create any
+    semantic change, since non-repeated message fields always track presence.
+    However it still indicates the semantic detail of whether the user wrote
+    "optional" or not. This can be useful for round-tripping the .proto file.
+    For consistency we give message fields a synthetic oneof also, even though
+    it is not required to track presence. This is especially important because
+    the parser can't tell if a field is a message or an enum, so it must always
+    create a synthetic oneof. Proto2 optional fields do not set this flag,
+    because they already indicate optional with `LABEL_OPTIONAL`.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class OneofDescriptorProto(betterproto.Message):
     """Describes a oneof."""
 
     name: str = betterproto.string_field(1)
@@ -532,23 +712,28 @@
 @dataclass(eq=False, repr=False)
 class EnumDescriptorProto(betterproto.Message):
     """Describes an enum type."""
 
     name: str = betterproto.string_field(1)
     value: List["EnumValueDescriptorProto"] = betterproto.message_field(2)
     options: "EnumOptions" = betterproto.message_field(3)
-    # Range of reserved numeric values. Reserved numeric values may not be used
-    # by enum values in the same enum declaration. Reserved ranges may not
-    # overlap.
     reserved_range: List[
         "EnumDescriptorProtoEnumReservedRange"
     ] = betterproto.message_field(4)
-    # Reserved enum value names, which may not be reused. A given name may only
-    # be reserved once.
+    """
+    Range of reserved numeric values. Reserved numeric values may not be used
+    by enum values in the same enum declaration. Reserved ranges may not
+    overlap.
+    """
+
     reserved_name: List[str] = betterproto.string_field(5)
+    """
+    Reserved enum value names, which may not be reused. A given name may only
+    be reserved once.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class EnumDescriptorProtoEnumReservedRange(betterproto.Message):
     """
     Range of reserved numeric values. Reserved values may not be used by
     entries in the same enum. Reserved ranges may not overlap. Note that this
@@ -579,277 +764,383 @@
 
 
 @dataclass(eq=False, repr=False)
 class MethodDescriptorProto(betterproto.Message):
     """Describes a method of a service."""
 
     name: str = betterproto.string_field(1)
-    # Input and output type names.  These are resolved in the same way as
-    # FieldDescriptorProto.type_name, but must refer to a message type.
     input_type: str = betterproto.string_field(2)
+    """
+    Input and output type names.  These are resolved in the same way as
+    FieldDescriptorProto.type_name, but must refer to a message type.
+    """
+
     output_type: str = betterproto.string_field(3)
     options: "MethodOptions" = betterproto.message_field(4)
-    # Identifies if client streams multiple client messages
     client_streaming: bool = betterproto.bool_field(5)
-    # Identifies if server streams multiple server messages
+    """Identifies if client streams multiple client messages"""
+
     server_streaming: bool = betterproto.bool_field(6)
+    """Identifies if server streams multiple server messages"""
 
 
 @dataclass(eq=False, repr=False)
 class FileOptions(betterproto.Message):
-    # Sets the Java package where classes generated from this .proto will be
-    # placed.  By default, the proto package is used, but this is often
-    # inappropriate because proto packages do not normally start with backwards
-    # domain names.
     java_package: str = betterproto.string_field(1)
-    # Controls the name of the wrapper Java class generated for the .proto file.
-    # That class will always contain the .proto file's getDescriptor() method as
-    # well as any top-level extensions defined in the .proto file. If
-    # java_multiple_files is disabled, then all the other classes from the .proto
-    # file will be nested inside the single wrapper outer class.
+    """
+    Sets the Java package where classes generated from this .proto will be
+    placed.  By default, the proto package is used, but this is often
+    inappropriate because proto packages do not normally start with backwards
+    domain names.
+    """
+
     java_outer_classname: str = betterproto.string_field(8)
-    # If enabled, then the Java code generator will generate a separate .java
-    # file for each top-level message, enum, and service defined in the .proto
-    # file.  Thus, these types will *not* be nested inside the wrapper class
-    # named by java_outer_classname.  However, the wrapper class will still be
-    # generated to contain the file's getDescriptor() method as well as any top-
-    # level extensions defined in the file.
+    """
+    Controls the name of the wrapper Java class generated for the .proto file.
+    That class will always contain the .proto file's getDescriptor() method as
+    well as any top-level extensions defined in the .proto file. If
+    java_multiple_files is disabled, then all the other classes from the .proto
+    file will be nested inside the single wrapper outer class.
+    """
+
     java_multiple_files: bool = betterproto.bool_field(10)
-    # This option does nothing.
+    """
+    If enabled, then the Java code generator will generate a separate .java
+    file for each top-level message, enum, and service defined in the .proto
+    file.  Thus, these types will *not* be nested inside the wrapper class
+    named by java_outer_classname.  However, the wrapper class will still be
+    generated to contain the file's getDescriptor() method as well as any top-
+    level extensions defined in the file.
+    """
+
     java_generate_equals_and_hash: bool = betterproto.bool_field(20)
-    # If set true, then the Java2 code generator will generate code that throws
-    # an exception whenever an attempt is made to assign a non-UTF-8 byte
-    # sequence to a string field. Message reflection will do the same. However,
-    # an extension field still accepts non-UTF-8 byte sequences. This option has
-    # no effect on when used with the lite runtime.
+    """This option does nothing."""
+
     java_string_check_utf8: bool = betterproto.bool_field(27)
+    """
+    If set true, then the Java2 code generator will generate code that throws
+    an exception whenever an attempt is made to assign a non-UTF-8 byte
+    sequence to a string field. Message reflection will do the same. However,
+    an extension field still accepts non-UTF-8 byte sequences. This option has
+    no effect on when used with the lite runtime.
+    """
+
     optimize_for: "FileOptionsOptimizeMode" = betterproto.enum_field(9)
-    # Sets the Go package where structs generated from this .proto will be
-    # placed. If omitted, the Go package will be derived from the following:   -
-    # The basename of the package import path, if provided.   - Otherwise, the
-    # package statement in the .proto file, if present.   - Otherwise, the
-    # basename of the .proto file, without extension.
     go_package: str = betterproto.string_field(11)
-    # Should generic services be generated in each language?  "Generic" services
-    # are not specific to any particular RPC system.  They are generated by the
-    # main code generators in each language (without additional plugins). Generic
-    # services were the only kind of service generation supported by early
-    # versions of google.protobuf. Generic services are now considered deprecated
-    # in favor of using plugins that generate code specific to your particular
-    # RPC system.  Therefore, these default to false.  Old code which depends on
-    # generic services should explicitly set them to true.
+    """
+    Sets the Go package where structs generated from this .proto will be
+    placed. If omitted, the Go package will be derived from the following:   -
+    The basename of the package import path, if provided.   - Otherwise, the
+    package statement in the .proto file, if present.   - Otherwise, the
+    basename of the .proto file, without extension.
+    """
+
     cc_generic_services: bool = betterproto.bool_field(16)
+    """
+    Should generic services be generated in each language?  "Generic" services
+    are not specific to any particular RPC system.  They are generated by the
+    main code generators in each language (without additional plugins). Generic
+    services were the only kind of service generation supported by early
+    versions of google.protobuf. Generic services are now considered deprecated
+    in favor of using plugins that generate code specific to your particular
+    RPC system.  Therefore, these default to false.  Old code which depends on
+    generic services should explicitly set them to true.
+    """
+
     java_generic_services: bool = betterproto.bool_field(17)
     py_generic_services: bool = betterproto.bool_field(18)
     php_generic_services: bool = betterproto.bool_field(42)
-    # Is this file deprecated? Depending on the target platform, this can emit
-    # Deprecated annotations for everything in the file, or it will be completely
-    # ignored; in the very least, this is a formalization for deprecating files.
     deprecated: bool = betterproto.bool_field(23)
-    # Enables the use of arenas for the proto messages in this file. This applies
-    # only to generated classes for C++.
+    """
+    Is this file deprecated? Depending on the target platform, this can emit
+    Deprecated annotations for everything in the file, or it will be completely
+    ignored; in the very least, this is a formalization for deprecating files.
+    """
+
     cc_enable_arenas: bool = betterproto.bool_field(31)
-    # Sets the objective c class prefix which is prepended to all objective c
-    # generated classes from this .proto. There is no default.
+    """
+    Enables the use of arenas for the proto messages in this file. This applies
+    only to generated classes for C++.
+    """
+
     objc_class_prefix: str = betterproto.string_field(36)
-    # Namespace for generated classes; defaults to the package.
+    """
+    Sets the objective c class prefix which is prepended to all objective c
+    generated classes from this .proto. There is no default.
+    """
+
     csharp_namespace: str = betterproto.string_field(37)
-    # By default Swift generators will take the proto package and CamelCase it
-    # replacing '.' with underscore and use that to prefix the types/symbols
-    # defined. When this options is provided, they will use this value instead to
-    # prefix the types/symbols defined.
+    """Namespace for generated classes; defaults to the package."""
+
     swift_prefix: str = betterproto.string_field(39)
-    # Sets the php class prefix which is prepended to all php generated classes
-    # from this .proto. Default is empty.
+    """
+    By default Swift generators will take the proto package and CamelCase it
+    replacing '.' with underscore and use that to prefix the types/symbols
+    defined. When this options is provided, they will use this value instead to
+    prefix the types/symbols defined.
+    """
+
     php_class_prefix: str = betterproto.string_field(40)
-    # Use this option to change the namespace of php generated classes. Default
-    # is empty. When this option is empty, the package name will be used for
-    # determining the namespace.
+    """
+    Sets the php class prefix which is prepended to all php generated classes
+    from this .proto. Default is empty.
+    """
+
     php_namespace: str = betterproto.string_field(41)
-    # Use this option to change the namespace of php generated metadata classes.
-    # Default is empty. When this option is empty, the proto file name will be
-    # used for determining the namespace.
+    """
+    Use this option to change the namespace of php generated classes. Default
+    is empty. When this option is empty, the package name will be used for
+    determining the namespace.
+    """
+
     php_metadata_namespace: str = betterproto.string_field(44)
-    # Use this option to change the package of ruby generated classes. Default is
-    # empty. When this option is not set, the package name will be used for
-    # determining the ruby package.
+    """
+    Use this option to change the namespace of php generated metadata classes.
+    Default is empty. When this option is empty, the proto file name will be
+    used for determining the namespace.
+    """
+
     ruby_package: str = betterproto.string_field(45)
-    # The parser stores options it doesn't recognize here. See the documentation
-    # for the "Options" section above.
+    """
+    Use this option to change the package of ruby generated classes. Default is
+    empty. When this option is not set, the package name will be used for
+    determining the ruby package.
+    """
+
     uninterpreted_option: List["UninterpretedOption"] = betterproto.message_field(999)
+    """
+    The parser stores options it doesn't recognize here. See the documentation
+    for the "Options" section above.
+    """
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        if self.java_generate_equals_and_hash:
+        if self.is_set("java_generate_equals_and_hash"):
             warnings.warn(
                 "FileOptions.java_generate_equals_and_hash is deprecated",
                 DeprecationWarning,
             )
 
 
 @dataclass(eq=False, repr=False)
 class MessageOptions(betterproto.Message):
-    # Set true to use the old proto1 MessageSet wire format for extensions. This
-    # is provided for backwards-compatibility with the MessageSet wire format.
-    # You should not use this for any other reason:  It's less efficient, has
-    # fewer features, and is more complicated. The message must be defined
-    # exactly as follows:   message Foo {     option message_set_wire_format =
-    # true;     extensions 4 to max;   } Note that the message cannot have any
-    # defined fields; MessageSets only have extensions. All extensions of your
-    # type must be singular messages; e.g. they cannot be int32s, enums, or
-    # repeated messages. Because this is an option, the above two restrictions
-    # are not enforced by the protocol compiler.
     message_set_wire_format: bool = betterproto.bool_field(1)
-    # Disables the generation of the standard "descriptor()" accessor, which can
-    # conflict with a field of the same name.  This is meant to make migration
-    # from proto1 easier; new code should avoid fields named "descriptor".
+    """
+    Set true to use the old proto1 MessageSet wire format for extensions. This
+    is provided for backwards-compatibility with the MessageSet wire format.
+    You should not use this for any other reason:  It's less efficient, has
+    fewer features, and is more complicated. The message must be defined
+    exactly as follows:   message Foo {     option message_set_wire_format =
+    true;     extensions 4 to max;   } Note that the message cannot have any
+    defined fields; MessageSets only have extensions. All extensions of your
+    type must be singular messages; e.g. they cannot be int32s, enums, or
+    repeated messages. Because this is an option, the above two restrictions
+    are not enforced by the protocol compiler.
+    """
+
     no_standard_descriptor_accessor: bool = betterproto.bool_field(2)
-    # Is this message deprecated? Depending on the target platform, this can emit
-    # Deprecated annotations for the message, or it will be completely ignored;
-    # in the very least, this is a formalization for deprecating messages.
+    """
+    Disables the generation of the standard "descriptor()" accessor, which can
+    conflict with a field of the same name.  This is meant to make migration
+    from proto1 easier; new code should avoid fields named "descriptor".
+    """
+
     deprecated: bool = betterproto.bool_field(3)
-    # Whether the message is an automatically generated map entry type for the
-    # maps field. For maps fields:     map<KeyType, ValueType> map_field = 1; The
-    # parsed descriptor looks like:     message MapFieldEntry {         option
-    # map_entry = true;         optional KeyType key = 1;         optional
-    # ValueType value = 2;     }     repeated MapFieldEntry map_field = 1;
-    # Implementations may choose not to generate the map_entry=true message, but
-    # use a native map in the target language to hold the keys and values. The
-    # reflection APIs in such implementations still need to work as if the field
-    # is a repeated message field. NOTE: Do not set the option in .proto files.
-    # Always use the maps syntax instead. The option should only be implicitly
-    # set by the proto compiler parser.
+    """
+    Is this message deprecated? Depending on the target platform, this can emit
+    Deprecated annotations for the message, or it will be completely ignored;
+    in the very least, this is a formalization for deprecating messages.
+    """
+
     map_entry: bool = betterproto.bool_field(7)
-    # The parser stores options it doesn't recognize here. See above.
+    """
+    Whether the message is an automatically generated map entry type for the
+    maps field. For maps fields:     map<KeyType, ValueType> map_field = 1; The
+    parsed descriptor looks like:     message MapFieldEntry {         option
+    map_entry = true;         optional KeyType key = 1;         optional
+    ValueType value = 2;     }     repeated MapFieldEntry map_field = 1;
+    Implementations may choose not to generate the map_entry=true message, but
+    use a native map in the target language to hold the keys and values. The
+    reflection APIs in such implementations still need to work as if the field
+    is a repeated message field. NOTE: Do not set the option in .proto files.
+    Always use the maps syntax instead. The option should only be implicitly
+    set by the proto compiler parser.
+    """
+
     uninterpreted_option: List["UninterpretedOption"] = betterproto.message_field(999)
+    """The parser stores options it doesn't recognize here. See above."""
 
 
 @dataclass(eq=False, repr=False)
 class FieldOptions(betterproto.Message):
-    # The ctype option instructs the C++ code generator to use a different
-    # representation of the field than it normally would.  See the specific
-    # options below.  This option is not yet implemented in the open source
-    # release -- sorry, we'll try to include it in a future version!
     ctype: "FieldOptionsCType" = betterproto.enum_field(1)
-    # The packed option can be enabled for repeated primitive fields to enable a
-    # more efficient representation on the wire. Rather than repeatedly writing
-    # the tag and type for each element, the entire array is encoded as a single
-    # length-delimited blob. In proto3, only explicit setting it to false will
-    # avoid using packed encoding.
+    """
+    The ctype option instructs the C++ code generator to use a different
+    representation of the field than it normally would.  See the specific
+    options below.  This option is not yet implemented in the open source
+    release -- sorry, we'll try to include it in a future version!
+    """
+
     packed: bool = betterproto.bool_field(2)
-    # The jstype option determines the JavaScript type used for values of the
-    # field.  The option is permitted only for 64 bit integral and fixed types
-    # (int64, uint64, sint64, fixed64, sfixed64).  A field with jstype JS_STRING
-    # is represented as JavaScript string, which avoids loss of precision that
-    # can happen when a large value is converted to a floating point JavaScript.
-    # Specifying JS_NUMBER for the jstype causes the generated JavaScript code to
-    # use the JavaScript "number" type.  The behavior of the default option
-    # JS_NORMAL is implementation dependent. This option is an enum to permit
-    # additional types to be added, e.g. goog.math.Integer.
+    """
+    The packed option can be enabled for repeated primitive fields to enable a
+    more efficient representation on the wire. Rather than repeatedly writing
+    the tag and type for each element, the entire array is encoded as a single
+    length-delimited blob. In proto3, only explicit setting it to false will
+    avoid using packed encoding.
+    """
+
     jstype: "FieldOptionsJsType" = betterproto.enum_field(6)
-    # Should this field be parsed lazily?  Lazy applies only to message-type
-    # fields.  It means that when the outer message is initially parsed, the
-    # inner message's contents will not be parsed but instead stored in encoded
-    # form.  The inner message will actually be parsed when it is first accessed.
-    # This is only a hint.  Implementations are free to choose whether to use
-    # eager or lazy parsing regardless of the value of this option.  However,
-    # setting this option true suggests that the protocol author believes that
-    # using lazy parsing on this field is worth the additional bookkeeping
-    # overhead typically needed to implement it. This option does not affect the
-    # public interface of any generated code; all method signatures remain the
-    # same.  Furthermore, thread-safety of the interface is not affected by this
-    # option; const methods remain safe to call from multiple threads
-    # concurrently, while non-const methods continue to require exclusive access.
-    # Note that implementations may choose not to check required fields within a
-    # lazy sub-message.  That is, calling IsInitialized() on the outer message
-    # may return true even if the inner message has missing required fields. This
-    # is necessary because otherwise the inner message would have to be parsed in
-    # order to perform the check, defeating the purpose of lazy parsing.  An
-    # implementation which chooses not to check required fields must be
-    # consistent about it.  That is, for any particular sub-message, the
-    # implementation must either *always* check its required fields, or *never*
-    # check its required fields, regardless of whether or not the message has
-    # been parsed.
+    """
+    The jstype option determines the JavaScript type used for values of the
+    field.  The option is permitted only for 64 bit integral and fixed types
+    (int64, uint64, sint64, fixed64, sfixed64).  A field with jstype JS_STRING
+    is represented as JavaScript string, which avoids loss of precision that
+    can happen when a large value is converted to a floating point JavaScript.
+    Specifying JS_NUMBER for the jstype causes the generated JavaScript code to
+    use the JavaScript "number" type.  The behavior of the default option
+    JS_NORMAL is implementation dependent. This option is an enum to permit
+    additional types to be added, e.g. goog.math.Integer.
+    """
+
     lazy: bool = betterproto.bool_field(5)
-    # Is this field deprecated? Depending on the target platform, this can emit
-    # Deprecated annotations for accessors, or it will be completely ignored; in
-    # the very least, this is a formalization for deprecating fields.
+    """
+    Should this field be parsed lazily?  Lazy applies only to message-type
+    fields.  It means that when the outer message is initially parsed, the
+    inner message's contents will not be parsed but instead stored in encoded
+    form.  The inner message will actually be parsed when it is first accessed.
+    This is only a hint.  Implementations are free to choose whether to use
+    eager or lazy parsing regardless of the value of this option.  However,
+    setting this option true suggests that the protocol author believes that
+    using lazy parsing on this field is worth the additional bookkeeping
+    overhead typically needed to implement it. This option does not affect the
+    public interface of any generated code; all method signatures remain the
+    same.  Furthermore, thread-safety of the interface is not affected by this
+    option; const methods remain safe to call from multiple threads
+    concurrently, while non-const methods continue to require exclusive access.
+    Note that implementations may choose not to check required fields within a
+    lazy sub-message.  That is, calling IsInitialized() on the outer message
+    may return true even if the inner message has missing required fields. This
+    is necessary because otherwise the inner message would have to be parsed in
+    order to perform the check, defeating the purpose of lazy parsing.  An
+    implementation which chooses not to check required fields must be
+    consistent about it.  That is, for any particular sub-message, the
+    implementation must either *always* check its required fields, or *never*
+    check its required fields, regardless of whether or not the message has
+    been parsed. As of 2021, lazy does no correctness checks on the byte stream
+    during parsing.  This may lead to crashes if and when an invalid byte
+    stream is finally parsed upon access. TODO(b/211906113):  Enable validation
+    on lazy fields.
+    """
+
+    unverified_lazy: bool = betterproto.bool_field(15)
+    """
+    unverified_lazy does no correctness checks on the byte stream. This should
+    only be used where lazy with verification is prohibitive for performance
+    reasons.
+    """
+
     deprecated: bool = betterproto.bool_field(3)
-    # For Google-internal migration only. Do not use.
+    """
+    Is this field deprecated? Depending on the target platform, this can emit
+    Deprecated annotations for accessors, or it will be completely ignored; in
+    the very least, this is a formalization for deprecating fields.
+    """
+
     weak: bool = betterproto.bool_field(10)
-    # The parser stores options it doesn't recognize here. See above.
+    """For Google-internal migration only. Do not use."""
+
     uninterpreted_option: List["UninterpretedOption"] = betterproto.message_field(999)
+    """The parser stores options it doesn't recognize here. See above."""
 
 
 @dataclass(eq=False, repr=False)
 class OneofOptions(betterproto.Message):
-    # The parser stores options it doesn't recognize here. See above.
     uninterpreted_option: List["UninterpretedOption"] = betterproto.message_field(999)
+    """The parser stores options it doesn't recognize here. See above."""
 
 
 @dataclass(eq=False, repr=False)
 class EnumOptions(betterproto.Message):
-    # Set this option to true to allow mapping different tag names to the same
-    # value.
     allow_alias: bool = betterproto.bool_field(2)
-    # Is this enum deprecated? Depending on the target platform, this can emit
-    # Deprecated annotations for the enum, or it will be completely ignored; in
-    # the very least, this is a formalization for deprecating enums.
+    """
+    Set this option to true to allow mapping different tag names to the same
+    value.
+    """
+
     deprecated: bool = betterproto.bool_field(3)
-    # The parser stores options it doesn't recognize here. See above.
+    """
+    Is this enum deprecated? Depending on the target platform, this can emit
+    Deprecated annotations for the enum, or it will be completely ignored; in
+    the very least, this is a formalization for deprecating enums.
+    """
+
     uninterpreted_option: List["UninterpretedOption"] = betterproto.message_field(999)
+    """The parser stores options it doesn't recognize here. See above."""
 
 
 @dataclass(eq=False, repr=False)
 class EnumValueOptions(betterproto.Message):
-    # Is this enum value deprecated? Depending on the target platform, this can
-    # emit Deprecated annotations for the enum value, or it will be completely
-    # ignored; in the very least, this is a formalization for deprecating enum
-    # values.
     deprecated: bool = betterproto.bool_field(1)
-    # The parser stores options it doesn't recognize here. See above.
+    """
+    Is this enum value deprecated? Depending on the target platform, this can
+    emit Deprecated annotations for the enum value, or it will be completely
+    ignored; in the very least, this is a formalization for deprecating enum
+    values.
+    """
+
     uninterpreted_option: List["UninterpretedOption"] = betterproto.message_field(999)
+    """The parser stores options it doesn't recognize here. See above."""
 
 
 @dataclass(eq=False, repr=False)
 class ServiceOptions(betterproto.Message):
-    # Is this service deprecated? Depending on the target platform, this can emit
-    # Deprecated annotations for the service, or it will be completely ignored;
-    # in the very least, this is a formalization for deprecating services.
     deprecated: bool = betterproto.bool_field(33)
-    # The parser stores options it doesn't recognize here. See above.
+    """
+    Is this service deprecated? Depending on the target platform, this can emit
+    Deprecated annotations for the service, or it will be completely ignored;
+    in the very least, this is a formalization for deprecating services.
+    """
+
     uninterpreted_option: List["UninterpretedOption"] = betterproto.message_field(999)
+    """The parser stores options it doesn't recognize here. See above."""
 
 
 @dataclass(eq=False, repr=False)
 class MethodOptions(betterproto.Message):
-    # Is this method deprecated? Depending on the target platform, this can emit
-    # Deprecated annotations for the method, or it will be completely ignored; in
-    # the very least, this is a formalization for deprecating methods.
     deprecated: bool = betterproto.bool_field(33)
+    """
+    Is this method deprecated? Depending on the target platform, this can emit
+    Deprecated annotations for the method, or it will be completely ignored; in
+    the very least, this is a formalization for deprecating methods.
+    """
+
     idempotency_level: "MethodOptionsIdempotencyLevel" = betterproto.enum_field(34)
-    # The parser stores options it doesn't recognize here. See above.
     uninterpreted_option: List["UninterpretedOption"] = betterproto.message_field(999)
+    """The parser stores options it doesn't recognize here. See above."""
 
 
 @dataclass(eq=False, repr=False)
 class UninterpretedOption(betterproto.Message):
     """
     A message representing a option the parser does not recognize. This only
     appears in options protos created by the compiler::Parser class.
     DescriptorPool resolves these when building Descriptor objects. Therefore,
     options protos in descriptor objects (e.g. returned by
     Descriptor::options(), or produced by Descriptor::CopyTo()) will never have
     UninterpretedOptions in them.
     """
 
     name: List["UninterpretedOptionNamePart"] = betterproto.message_field(2)
-    # The value of the uninterpreted option, in whatever type the tokenizer
-    # identified it as during parsing. Exactly one of these should be set.
     identifier_value: str = betterproto.string_field(3)
+    """
+    The value of the uninterpreted option, in whatever type the tokenizer
+    identified it as during parsing. Exactly one of these should be set.
+    """
+
     positive_int_value: int = betterproto.uint64_field(4)
     negative_int_value: int = betterproto.int64_field(5)
     double_value: float = betterproto.double_field(6)
     string_value: bytes = betterproto.bytes_field(7)
     aggregate_value: str = betterproto.string_field(8)
 
 
@@ -870,120 +1161,142 @@
 @dataclass(eq=False, repr=False)
 class SourceCodeInfo(betterproto.Message):
     """
     Encapsulates information about the original source file from which a
     FileDescriptorProto was generated.
     """
 
-    # A Location identifies a piece of source code in a .proto file which
-    # corresponds to a particular definition.  This information is intended to be
-    # useful to IDEs, code indexers, documentation generators, and similar tools.
-    # For example, say we have a file like:   message Foo {     optional string
-    # foo = 1;   } Let's look at just the field definition:   optional string foo
-    # = 1;   ^       ^^     ^^  ^  ^^^   a       bc     de  f  ghi We have the
-    # following locations:   span   path               represents   [a,i)  [ 4,
-    # 0, 2, 0 ]     The whole field definition.   [a,b)  [ 4, 0, 2, 0, 4 ]  The
-    # label (optional).   [c,d)  [ 4, 0, 2, 0, 5 ]  The type (string).   [e,f)  [
-    # 4, 0, 2, 0, 1 ]  The name (foo).   [g,h)  [ 4, 0, 2, 0, 3 ]  The number
-    # (1). Notes: - A location may refer to a repeated field itself (i.e. not to
-    # any   particular index within it).  This is used whenever a set of elements
-    # are   logically enclosed in a single code segment.  For example, an entire
-    # extend block (possibly containing multiple extension definitions) will
-    # have an outer location whose path refers to the "extensions" repeated
-    # field without an index. - Multiple locations may have the same path.  This
-    # happens when a single   logical declaration is spread out across multiple
-    # places.  The most   obvious example is the "extend" block again -- there
-    # may be multiple   extend blocks in the same scope, each of which will have
-    # the same path. - A location's span is not always a subset of its parent's
-    # span.  For   example, the "extendee" of an extension declaration appears at
-    # the   beginning of the "extend" block and is shared by all extensions
-    # within   the block. - Just because a location's span is a subset of some
-    # other location's span   does not mean that it is a descendant.  For
-    # example, a "group" defines   both a type and a field in a single
-    # declaration.  Thus, the locations   corresponding to the type and field and
-    # their components will overlap. - Code which tries to interpret locations
-    # should probably be designed to   ignore those that it doesn't understand,
-    # as more types of locations could   be recorded in the future.
     location: List["SourceCodeInfoLocation"] = betterproto.message_field(1)
+    """
+    A Location identifies a piece of source code in a .proto file which
+    corresponds to a particular definition.  This information is intended to be
+    useful to IDEs, code indexers, documentation generators, and similar tools.
+    For example, say we have a file like:   message Foo {     optional string
+    foo = 1;   } Let's look at just the field definition:   optional string foo
+    = 1;   ^       ^^     ^^  ^  ^^^   a       bc     de  f  ghi We have the
+    following locations:   span   path               represents   [a,i)  [ 4,
+    0, 2, 0 ]     The whole field definition.   [a,b)  [ 4, 0, 2, 0, 4 ]  The
+    label (optional).   [c,d)  [ 4, 0, 2, 0, 5 ]  The type (string).   [e,f)  [
+    4, 0, 2, 0, 1 ]  The name (foo).   [g,h)  [ 4, 0, 2, 0, 3 ]  The number
+    (1). Notes: - A location may refer to a repeated field itself (i.e. not to
+    any   particular index within it).  This is used whenever a set of elements
+    are   logically enclosed in a single code segment.  For example, an entire
+    extend block (possibly containing multiple extension definitions) will
+    have an outer location whose path refers to the "extensions" repeated
+    field without an index. - Multiple locations may have the same path.  This
+    happens when a single   logical declaration is spread out across multiple
+    places.  The most   obvious example is the "extend" block again -- there
+    may be multiple   extend blocks in the same scope, each of which will have
+    the same path. - A location's span is not always a subset of its parent's
+    span.  For   example, the "extendee" of an extension declaration appears at
+    the   beginning of the "extend" block and is shared by all extensions
+    within   the block. - Just because a location's span is a subset of some
+    other location's span   does not mean that it is a descendant.  For
+    example, a "group" defines   both a type and a field in a single
+    declaration.  Thus, the locations   corresponding to the type and field and
+    their components will overlap. - Code which tries to interpret locations
+    should probably be designed to   ignore those that it doesn't understand,
+    as more types of locations could   be recorded in the future.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class SourceCodeInfoLocation(betterproto.Message):
-    # Identifies which part of the FileDescriptorProto was defined at this
-    # location. Each element is a field number or an index.  They form a path
-    # from the root FileDescriptorProto to the place where the definition.  For
-    # example, this path:   [ 4, 3, 2, 7, 1 ] refers to:   file.message_type(3)
-    # // 4, 3       .field(7)         // 2, 7       .name()           // 1 This
-    # is because FileDescriptorProto.message_type has field number 4:   repeated
-    # DescriptorProto message_type = 4; and DescriptorProto.field has field
-    # number 2:   repeated FieldDescriptorProto field = 2; and
-    # FieldDescriptorProto.name has field number 1:   optional string name = 1;
-    # Thus, the above path gives the location of a field name.  If we removed the
-    # last element:   [ 4, 3, 2, 7 ] this path refers to the whole field
-    # declaration (from the beginning of the label to the terminating semicolon).
     path: List[int] = betterproto.int32_field(1)
-    # Always has exactly three or four elements: start line, start column, end
-    # line (optional, otherwise assumed same as start line), end column. These
-    # are packed into a single field for efficiency.  Note that line and column
-    # numbers are zero-based -- typically you will want to add 1 to each before
-    # displaying to a user.
+    """
+    Identifies which part of the FileDescriptorProto was defined at this
+    location. Each element is a field number or an index.  They form a path
+    from the root FileDescriptorProto to the place where the definition occurs.
+    For example, this path:   [ 4, 3, 2, 7, 1 ] refers to:
+    file.message_type(3)  // 4, 3       .field(7)         // 2, 7       .name()
+    // 1 This is because FileDescriptorProto.message_type has field number 4:
+    repeated DescriptorProto message_type = 4; and DescriptorProto.field has
+    field number 2:   repeated FieldDescriptorProto field = 2; and
+    FieldDescriptorProto.name has field number 1:   optional string name = 1;
+    Thus, the above path gives the location of a field name.  If we removed the
+    last element:   [ 4, 3, 2, 7 ] this path refers to the whole field
+    declaration (from the beginning of the label to the terminating semicolon).
+    """
+
     span: List[int] = betterproto.int32_field(2)
-    # If this SourceCodeInfo represents a complete declaration, these are any
-    # comments appearing before and after the declaration which appear to be
-    # attached to the declaration. A series of line comments appearing on
-    # consecutive lines, with no other tokens appearing on those lines, will be
-    # treated as a single comment. leading_detached_comments will keep paragraphs
-    # of comments that appear before (but not connected to) the current element.
-    # Each paragraph, separated by empty lines, will be one comment element in
-    # the repeated field. Only the comment content is provided; comment markers
-    # (e.g. //) are stripped out.  For block comments, leading whitespace and an
-    # asterisk will be stripped from the beginning of each line other than the
-    # first. Newlines are included in the output. Examples:   optional int32 foo
-    # = 1;  // Comment attached to foo.   // Comment attached to bar.   optional
-    # int32 bar = 2;   optional string baz = 3;   // Comment attached to baz.
-    # // Another line attached to baz.   // Comment attached to qux.   //   //
-    # Another line attached to qux.   optional double qux = 4;   // Detached
-    # comment for corge. This is not leading or trailing comments   // to qux or
-    # corge because there are blank lines separating it from   // both.   //
-    # Detached comment for corge paragraph 2.   optional string corge = 5;   /*
-    # Block comment attached    * to corge.  Leading asterisks    * will be
-    # removed. */   /* Block comment attached to    * grault. */   optional int32
-    # grault = 6;   // ignored detached comments.
+    """
+    Always has exactly three or four elements: start line, start column, end
+    line (optional, otherwise assumed same as start line), end column. These
+    are packed into a single field for efficiency.  Note that line and column
+    numbers are zero-based -- typically you will want to add 1 to each before
+    displaying to a user.
+    """
+
     leading_comments: str = betterproto.string_field(3)
+    """
+    If this SourceCodeInfo represents a complete declaration, these are any
+    comments appearing before and after the declaration which appear to be
+    attached to the declaration. A series of line comments appearing on
+    consecutive lines, with no other tokens appearing on those lines, will be
+    treated as a single comment. leading_detached_comments will keep paragraphs
+    of comments that appear before (but not connected to) the current element.
+    Each paragraph, separated by empty lines, will be one comment element in
+    the repeated field. Only the comment content is provided; comment markers
+    (e.g. //) are stripped out.  For block comments, leading whitespace and an
+    asterisk will be stripped from the beginning of each line other than the
+    first. Newlines are included in the output. Examples:   optional int32 foo
+    = 1;  // Comment attached to foo.   // Comment attached to bar.   optional
+    int32 bar = 2;   optional string baz = 3;   // Comment attached to baz.
+    // Another line attached to baz.   // Comment attached to qux.   //   //
+    Another line attached to qux.   optional double qux = 4;   // Detached
+    comment for corge. This is not leading or trailing comments   // to qux or
+    corge because there are blank lines separating it from   // both.   //
+    Detached comment for corge paragraph 2.   optional string corge = 5;   /*
+    Block comment attached    * to corge.  Leading asterisks    * will be
+    removed. */   /* Block comment attached to    * grault. */   optional int32
+    grault = 6;   // ignored detached comments.
+    """
+
     trailing_comments: str = betterproto.string_field(4)
     leading_detached_comments: List[str] = betterproto.string_field(6)
 
 
 @dataclass(eq=False, repr=False)
 class GeneratedCodeInfo(betterproto.Message):
     """
     Describes the relationship between generated code and its original source
     file. A GeneratedCodeInfo message is associated with only one generated
     source file, but may contain references to different source .proto files.
     """
 
-    # An Annotation connects some span of text in generated code to an element of
-    # its generating .proto file.
     annotation: List["GeneratedCodeInfoAnnotation"] = betterproto.message_field(1)
+    """
+    An Annotation connects some span of text in generated code to an element of
+    its generating .proto file.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class GeneratedCodeInfoAnnotation(betterproto.Message):
-    # Identifies the element in the original source .proto file. This field is
-    # formatted the same as SourceCodeInfo.Location.path.
     path: List[int] = betterproto.int32_field(1)
-    # Identifies the filesystem path to the original source .proto.
+    """
+    Identifies the element in the original source .proto file. This field is
+    formatted the same as SourceCodeInfo.Location.path.
+    """
+
     source_file: str = betterproto.string_field(2)
-    # Identifies the starting offset in bytes in the generated code that relates
-    # to the identified object.
+    """Identifies the filesystem path to the original source .proto."""
+
     begin: int = betterproto.int32_field(3)
-    # Identifies the ending offset in bytes in the generated code that relates to
-    # the identified offset. The end offset should be one past the last relevant
-    # byte (so the length of the text = end - begin).
+    """
+    Identifies the starting offset in bytes in the generated code that relates
+    to the identified object.
+    """
+
     end: int = betterproto.int32_field(4)
+    """
+    Identifies the ending offset in bytes in the generated code that relates to
+    the identified offset. The end offset should be one past the last relevant
+    byte (so the length of the text = end - begin).
+    """
 
 
 @dataclass(eq=False, repr=False)
 class Duration(betterproto.Message):
     """
     A Duration represents a signed, fixed-length span of time represented as a
     count of seconds and fractions of seconds at nanosecond resolution. It is
@@ -1011,24 +1324,29 @@
     with nanoseconds expressed as fractional seconds. For example, 3 seconds
     with 0 nanoseconds should be encoded in JSON format as "3s", while 3
     seconds and 1 nanosecond should be expressed in JSON format as
     "3.000000001s", and 3 seconds and 1 microsecond should be expressed in JSON
     format as "3.000001s".
     """
 
-    # Signed seconds of the span of time. Must be from -315,576,000,000 to
-    # +315,576,000,000 inclusive. Note: these bounds are computed from: 60
-    # sec/min * 60 min/hr * 24 hr/day * 365.25 days/year * 10000 years
     seconds: int = betterproto.int64_field(1)
-    # Signed fractions of a second at nanosecond resolution of the span of time.
-    # Durations less than one second are represented with a 0 `seconds` field and
-    # a positive or negative `nanos` field. For durations of one second or more,
-    # a non-zero value for the `nanos` field must be of the same sign as the
-    # `seconds` field. Must be from -999,999,999 to +999,999,999 inclusive.
+    """
+    Signed seconds of the span of time. Must be from -315,576,000,000 to
+    +315,576,000,000 inclusive. Note: these bounds are computed from: 60
+    sec/min * 60 min/hr * 24 hr/day * 365.25 days/year * 10000 years
+    """
+
     nanos: int = betterproto.int32_field(2)
+    """
+    Signed fractions of a second at nanosecond resolution of the span of time.
+    Durations less than one second are represented with a 0 `seconds` field and
+    a positive or negative `nanos` field. For durations of one second or more,
+    a non-zero value for the `nanos` field must be of the same sign as the
+    `seconds` field. Must be from -999,999,999 to +999,999,999 inclusive.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class Empty(betterproto.Message):
     """
     A generic empty message that you can re-use to avoid defining duplicated
     empty messages in your APIs. A typical example is to use it as the request
@@ -1116,68 +1434,73 @@
     paths: "sub_message"     } Note that oneof type names ("test_oneof" in this
     case) cannot be used in paths. ## Field Mask Verification The
     implementation of any API method which has a FieldMask type field in the
     request should verify the included field paths, and return an
     `INVALID_ARGUMENT` error if any path is unmappable.
     """
 
-    # The set of field mask paths.
     paths: List[str] = betterproto.string_field(1)
+    """The set of field mask paths."""
 
 
 @dataclass(eq=False, repr=False)
 class Struct(betterproto.Message):
     """
     `Struct` represents a structured data value, consisting of fields which map
     to dynamically typed values. In some languages, `Struct` might be supported
     by a native representation. For example, in scripting languages like JS a
     struct is represented as an object. The details of that representation are
     described together with the proto support for the language. The JSON
     representation for `Struct` is JSON object.
     """
 
-    # Unordered map of dynamically typed values.
     fields: Dict[str, "Value"] = betterproto.map_field(
         1, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
     )
+    """Unordered map of dynamically typed values."""
 
 
 @dataclass(eq=False, repr=False)
 class Value(betterproto.Message):
     """
     `Value` represents a dynamically typed value which can be either null, a
     number, a string, a boolean, a recursive struct value, or a list of values.
-    A producer of value is expected to set one of that variants, absence of any
-    variant indicates an error. The JSON representation for `Value` is JSON
+    A producer of value is expected to set one of these variants. Absence of
+    any variant indicates an error. The JSON representation for `Value` is JSON
     value.
     """
 
-    # Represents a null value.
     null_value: "NullValue" = betterproto.enum_field(1, group="kind")
-    # Represents a double value.
+    """Represents a null value."""
+
     number_value: float = betterproto.double_field(2, group="kind")
-    # Represents a string value.
+    """Represents a double value."""
+
     string_value: str = betterproto.string_field(3, group="kind")
-    # Represents a boolean value.
+    """Represents a string value."""
+
     bool_value: bool = betterproto.bool_field(4, group="kind")
-    # Represents a structured value.
+    """Represents a boolean value."""
+
     struct_value: "Struct" = betterproto.message_field(5, group="kind")
-    # Represents a repeated `Value`.
+    """Represents a structured value."""
+
     list_value: "ListValue" = betterproto.message_field(6, group="kind")
+    """Represents a repeated `Value`."""
 
 
 @dataclass(eq=False, repr=False)
 class ListValue(betterproto.Message):
     """
     `ListValue` is a wrapper around a repeated field of values. The JSON
     representation for `ListValue` is JSON array.
     """
 
-    # Repeated field of dynamically typed values.
     values: List["Value"] = betterproto.message_field(1)
+    """Repeated field of dynamically typed values."""
 
 
 @dataclass(eq=False, repr=False)
 class Timestamp(betterproto.Message):
     """
     A Timestamp represents a point in time independent of any time zone or
     local calendar, encoded as a count of seconds and fractions of seconds at
@@ -1230,113 +1553,118 @@
     with the time format spec '%Y-%m-%dT%H:%M:%S.%fZ'. Likewise, in Java, one
     can use the Joda Time's [`ISODateTimeFormat.dateTime()`](
     http://www.joda.org/joda-
     time/apidocs/org/joda/time/format/ISODateTimeFormat.html#dateTime%2D%2D )
     to obtain a formatter capable of generating timestamps in this format.
     """
 
-    # Represents seconds of UTC time since Unix epoch 1970-01-01T00:00:00Z. Must
-    # be from 0001-01-01T00:00:00Z to 9999-12-31T23:59:59Z inclusive.
     seconds: int = betterproto.int64_field(1)
-    # Non-negative fractions of a second at nanosecond resolution. Negative
-    # second values with fractions must still have non-negative nanos values that
-    # count forward in time. Must be from 0 to 999,999,999 inclusive.
+    """
+    Represents seconds of UTC time since Unix epoch 1970-01-01T00:00:00Z. Must
+    be from 0001-01-01T00:00:00Z to 9999-12-31T23:59:59Z inclusive.
+    """
+
     nanos: int = betterproto.int32_field(2)
+    """
+    Non-negative fractions of a second at nanosecond resolution. Negative
+    second values with fractions must still have non-negative nanos values that
+    count forward in time. Must be from 0 to 999,999,999 inclusive.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class DoubleValue(betterproto.Message):
     """
     Wrapper message for `double`. The JSON representation for `DoubleValue` is
     JSON number.
     """
 
-    # The double value.
     value: float = betterproto.double_field(1)
+    """The double value."""
 
 
 @dataclass(eq=False, repr=False)
 class FloatValue(betterproto.Message):
     """
     Wrapper message for `float`. The JSON representation for `FloatValue` is
     JSON number.
     """
 
-    # The float value.
     value: float = betterproto.float_field(1)
+    """The float value."""
 
 
 @dataclass(eq=False, repr=False)
 class Int64Value(betterproto.Message):
     """
     Wrapper message for `int64`. The JSON representation for `Int64Value` is
     JSON string.
     """
 
-    # The int64 value.
     value: int = betterproto.int64_field(1)
+    """The int64 value."""
 
 
 @dataclass(eq=False, repr=False)
 class UInt64Value(betterproto.Message):
     """
     Wrapper message for `uint64`. The JSON representation for `UInt64Value` is
     JSON string.
     """
 
-    # The uint64 value.
     value: int = betterproto.uint64_field(1)
+    """The uint64 value."""
 
 
 @dataclass(eq=False, repr=False)
 class Int32Value(betterproto.Message):
     """
     Wrapper message for `int32`. The JSON representation for `Int32Value` is
     JSON number.
     """
 
-    # The int32 value.
     value: int = betterproto.int32_field(1)
+    """The int32 value."""
 
 
 @dataclass(eq=False, repr=False)
 class UInt32Value(betterproto.Message):
     """
     Wrapper message for `uint32`. The JSON representation for `UInt32Value` is
     JSON number.
     """
 
-    # The uint32 value.
     value: int = betterproto.uint32_field(1)
+    """The uint32 value."""
 
 
 @dataclass(eq=False, repr=False)
 class BoolValue(betterproto.Message):
     """
     Wrapper message for `bool`. The JSON representation for `BoolValue` is JSON
     `true` and `false`.
     """
 
-    # The bool value.
     value: bool = betterproto.bool_field(1)
+    """The bool value."""
 
 
 @dataclass(eq=False, repr=False)
 class StringValue(betterproto.Message):
     """
     Wrapper message for `string`. The JSON representation for `StringValue` is
     JSON string.
     """
 
-    # The string value.
     value: str = betterproto.string_field(1)
+    """The string value."""
 
 
 @dataclass(eq=False, repr=False)
 class BytesValue(betterproto.Message):
     """
     Wrapper message for `bytes`. The JSON representation for `BytesValue` is
     JSON string.
     """
 
-    # The bytes value.
     value: bytes = betterproto.bytes_field(1)
+    """The bytes value."""
```

### Comparing `betterproto-2.0.0b5/src/betterproto/lib/google/protobuf/compiler/__init__.py` & `betterproto-2.0.0b6/src/betterproto/lib/google/protobuf/compiler/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,128 +1,152 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: google/protobuf/compiler/plugin.proto
 # plugin: python-betterproto
+# This file has been @generated
 from dataclasses import dataclass
 from typing import List
 
 import betterproto
-from betterproto.grpc.grpclib_server import ServiceBase
+import betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
 
 class CodeGeneratorResponseFeature(betterproto.Enum):
+    """Sync with code_generator.h."""
+
     FEATURE_NONE = 0
     FEATURE_PROTO3_OPTIONAL = 1
 
 
 @dataclass(eq=False, repr=False)
 class Version(betterproto.Message):
     """The version number of protocol compiler."""
 
     major: int = betterproto.int32_field(1)
     minor: int = betterproto.int32_field(2)
     patch: int = betterproto.int32_field(3)
-    # A suffix for alpha, beta or rc release, e.g., "alpha-1", "rc2". It should
-    # be empty for mainline stable releases.
     suffix: str = betterproto.string_field(4)
+    """
+    A suffix for alpha, beta or rc release, e.g., "alpha-1", "rc2". It should
+    be empty for mainline stable releases.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class CodeGeneratorRequest(betterproto.Message):
     """An encoded CodeGeneratorRequest is written to the plugin's stdin."""
 
-    # The .proto files that were explicitly listed on the command-line.  The code
-    # generator should generate code only for these files.  Each file's
-    # descriptor will be included in proto_file, below.
     file_to_generate: List[str] = betterproto.string_field(1)
-    # The generator parameter passed on the command-line.
+    """
+    The .proto files that were explicitly listed on the command-line.  The code
+    generator should generate code only for these files.  Each file's
+    descriptor will be included in proto_file, below.
+    """
+
     parameter: str = betterproto.string_field(2)
-    # FileDescriptorProtos for all files in files_to_generate and everything they
-    # import.  The files will appear in topological order, so each file appears
-    # before any file that imports it. protoc guarantees that all proto_files
-    # will be written after the fields above, even though this is not technically
-    # guaranteed by the protobuf wire format.  This theoretically could allow a
-    # plugin to stream in the FileDescriptorProtos and handle them one by one
-    # rather than read the entire set into memory at once.  However, as of this
-    # writing, this is not similarly optimized on protoc's end -- it will store
-    # all fields in memory at once before sending them to the plugin. Type names
-    # of fields and extensions in the FileDescriptorProto are always fully
-    # qualified.
+    """The generator parameter passed on the command-line."""
+
     proto_file: List[
         "betterproto_lib_google_protobuf.FileDescriptorProto"
     ] = betterproto.message_field(15)
-    # The version number of protocol compiler.
+    """
+    FileDescriptorProtos for all files in files_to_generate and everything they
+    import.  The files will appear in topological order, so each file appears
+    before any file that imports it. protoc guarantees that all proto_files
+    will be written after the fields above, even though this is not technically
+    guaranteed by the protobuf wire format.  This theoretically could allow a
+    plugin to stream in the FileDescriptorProtos and handle them one by one
+    rather than read the entire set into memory at once.  However, as of this
+    writing, this is not similarly optimized on protoc's end -- it will store
+    all fields in memory at once before sending them to the plugin. Type names
+    of fields and extensions in the FileDescriptorProto are always fully
+    qualified.
+    """
+
     compiler_version: "Version" = betterproto.message_field(3)
+    """The version number of protocol compiler."""
 
 
 @dataclass(eq=False, repr=False)
 class CodeGeneratorResponse(betterproto.Message):
     """The plugin writes an encoded CodeGeneratorResponse to stdout."""
 
-    # Error message.  If non-empty, code generation failed.  The plugin process
-    # should exit with status code zero even if it reports an error in this way.
-    # This should be used to indicate errors in .proto files which prevent the
-    # code generator from generating correct code.  Errors which indicate a
-    # problem in protoc itself -- such as the input CodeGeneratorRequest being
-    # unparseable -- should be reported by writing a message to stderr and
-    # exiting with a non-zero status code.
     error: str = betterproto.string_field(1)
-    # A bitmask of supported features that the code generator supports. This is a
-    # bitwise "or" of values from the Feature enum.
+    """
+    Error message.  If non-empty, code generation failed.  The plugin process
+    should exit with status code zero even if it reports an error in this way.
+    This should be used to indicate errors in .proto files which prevent the
+    code generator from generating correct code.  Errors which indicate a
+    problem in protoc itself -- such as the input CodeGeneratorRequest being
+    unparseable -- should be reported by writing a message to stderr and
+    exiting with a non-zero status code.
+    """
+
     supported_features: int = betterproto.uint64_field(2)
+    """
+    A bitmask of supported features that the code generator supports. This is a
+    bitwise "or" of values from the Feature enum.
+    """
+
     file: List["CodeGeneratorResponseFile"] = betterproto.message_field(15)
 
 
 @dataclass(eq=False, repr=False)
 class CodeGeneratorResponseFile(betterproto.Message):
     """Represents a single generated file."""
 
-    # The file name, relative to the output directory.  The name must not contain
-    # "." or ".." components and must be relative, not be absolute (so, the file
-    # cannot lie outside the output directory).  "/" must be used as the path
-    # separator, not "\". If the name is omitted, the content will be appended to
-    # the previous file.  This allows the generator to break large files into
-    # small chunks, and allows the generated text to be streamed back to protoc
-    # so that large files need not reside completely in memory at one time.  Note
-    # that as of this writing protoc does not optimize for this -- it will read
-    # the entire CodeGeneratorResponse before writing files to disk.
     name: str = betterproto.string_field(1)
-    # If non-empty, indicates that the named file should already exist, and the
-    # content here is to be inserted into that file at a defined insertion point.
-    # This feature allows a code generator to extend the output produced by
-    # another code generator.  The original generator may provide insertion
-    # points by placing special annotations in the file that look like:
-    # @@protoc_insertion_point(NAME) The annotation can have arbitrary text
-    # before and after it on the line, which allows it to be placed in a comment.
-    # NAME should be replaced with an identifier naming the point -- this is what
-    # other generators will use as the insertion_point.  Code inserted at this
-    # point will be placed immediately above the line containing the insertion
-    # point (thus multiple insertions to the same point will come out in the
-    # order they were added). The double-@ is intended to make it unlikely that
-    # the generated code could contain things that look like insertion points by
-    # accident. For example, the C++ code generator places the following line in
-    # the .pb.h files that it generates:   //
-    # @@protoc_insertion_point(namespace_scope) This line appears within the
-    # scope of the file's package namespace, but outside of any particular class.
-    # Another plugin can then specify the insertion_point "namespace_scope" to
-    # generate additional classes or other declarations that should be placed in
-    # this scope. Note that if the line containing the insertion point begins
-    # with whitespace, the same whitespace will be added to every line of the
-    # inserted text.  This is useful for languages like Python, where indentation
-    # matters.  In these languages, the insertion point comment should be
-    # indented the same amount as any inserted code will need to be in order to
-    # work correctly in that context. The code generator that generates the
-    # initial file and the one which inserts into it must both run as part of a
-    # single invocation of protoc. Code generators are executed in the order in
-    # which they appear on the command line. If |insertion_point| is present,
-    # |name| must also be present.
+    """
+    The file name, relative to the output directory.  The name must not contain
+    "." or ".." components and must be relative, not be absolute (so, the file
+    cannot lie outside the output directory).  "/" must be used as the path
+    separator, not "\". If the name is omitted, the content will be appended to
+    the previous file.  This allows the generator to break large files into
+    small chunks, and allows the generated text to be streamed back to protoc
+    so that large files need not reside completely in memory at one time.  Note
+    that as of this writing protoc does not optimize for this -- it will read
+    the entire CodeGeneratorResponse before writing files to disk.
+    """
+
     insertion_point: str = betterproto.string_field(2)
-    # The file contents.
+    """
+    If non-empty, indicates that the named file should already exist, and the
+    content here is to be inserted into that file at a defined insertion point.
+    This feature allows a code generator to extend the output produced by
+    another code generator.  The original generator may provide insertion
+    points by placing special annotations in the file that look like:
+    @@protoc_insertion_point(NAME) The annotation can have arbitrary text
+    before and after it on the line, which allows it to be placed in a comment.
+    NAME should be replaced with an identifier naming the point -- this is what
+    other generators will use as the insertion_point.  Code inserted at this
+    point will be placed immediately above the line containing the insertion
+    point (thus multiple insertions to the same point will come out in the
+    order they were added). The double-@ is intended to make it unlikely that
+    the generated code could contain things that look like insertion points by
+    accident. For example, the C++ code generator places the following line in
+    the .pb.h files that it generates:   //
+    @@protoc_insertion_point(namespace_scope) This line appears within the
+    scope of the file's package namespace, but outside of any particular class.
+    Another plugin can then specify the insertion_point "namespace_scope" to
+    generate additional classes or other declarations that should be placed in
+    this scope. Note that if the line containing the insertion point begins
+    with whitespace, the same whitespace will be added to every line of the
+    inserted text.  This is useful for languages like Python, where indentation
+    matters.  In these languages, the insertion point comment should be
+    indented the same amount as any inserted code will need to be in order to
+    work correctly in that context. The code generator that generates the
+    initial file and the one which inserts into it must both run as part of a
+    single invocation of protoc. Code generators are executed in the order in
+    which they appear on the command line. If |insertion_point| is present,
+    |name| must also be present.
+    """
+
     content: str = betterproto.string_field(15)
-    # Information describing the file content being inserted. If an insertion
-    # point is used, this information will be appropriately offset and inserted
-    # into the code generation metadata for the generated files.
+    """The file contents."""
+
     generated_code_info: "betterproto_lib_google_protobuf.GeneratedCodeInfo" = (
         betterproto.message_field(16)
     )
-
-
-import betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
+    """
+    Information describing the file content being inserted. If an insertion
+    point is used, this information will be appropriately offset and inserted
+    into the code generation metadata for the generated files.
+    """
```

### Comparing `betterproto-2.0.0b5/src/betterproto/plugin/compiler.py` & `betterproto-2.0.0b6/src/betterproto/plugin/compiler.py`

 * *Files identical despite different names*

### Comparing `betterproto-2.0.0b5/src/betterproto/plugin/main.py` & `betterproto-2.0.0b6/src/betterproto/plugin/main.py`

 * *Files identical despite different names*

### Comparing `betterproto-2.0.0b5/src/betterproto/plugin/models.py` & `betterproto-2.0.0b6/src/betterproto/plugin/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,14 @@
         return get_comment(
             proto_file=self.source_file, path=self.path, indent=self.comment_indent
         )
 
 
 @dataclass
 class PluginRequestCompiler:
-
     plugin_request_obj: CodeGeneratorRequest
     output_packages: Dict[str, "OutputTemplate"] = field(default_factory=dict)
 
     @property
     def all_messages(self) -> List["MessageCompiler"]:
         """All of the messages in this request.
 
@@ -243,19 +242,21 @@
 
     parent_request: PluginRequestCompiler
     package_proto_obj: FileDescriptorProto
     input_files: List[str] = field(default_factory=list)
     imports: Set[str] = field(default_factory=set)
     datetime_imports: Set[str] = field(default_factory=set)
     typing_imports: Set[str] = field(default_factory=set)
+    pydantic_imports: Set[str] = field(default_factory=set)
     builtins_import: bool = False
     messages: List["MessageCompiler"] = field(default_factory=list)
     enums: List["EnumDefinitionCompiler"] = field(default_factory=list)
     services: List["ServiceCompiler"] = field(default_factory=list)
     imports_type_checking_only: Set[str] = field(default_factory=set)
+    pydantic_dataclasses: bool = False
     output: bool = True
 
     @property
     def package(self) -> str:
         """Name of input package.
 
         Returns
@@ -330,14 +331,28 @@
             if f.deprecated:
                 yield f.py_name
 
     @property
     def has_deprecated_fields(self) -> bool:
         return any(self.deprecated_fields)
 
+    @property
+    def has_oneof_fields(self) -> bool:
+        return any(isinstance(field, OneOfFieldCompiler) for field in self.fields)
+
+    @property
+    def has_message_field(self) -> bool:
+        return any(
+            (
+                field.proto_obj.type in PROTO_MESSAGE_TYPES
+                for field in self.fields
+                if isinstance(field.proto_obj, FieldDescriptorProto)
+            )
+        )
+
 
 def is_map(
     proto_field_obj: FieldDescriptorProto, parent_message: DescriptorProto
 ) -> bool:
     """True if proto_field_obj is a map, otherwise False."""
     if proto_field_obj.type == FieldDescriptorProtoType.TYPE_MESSAGE:
         if not hasattr(parent_message, "nested_type"):
@@ -428,22 +443,27 @@
         if "List[" in annotation:
             imports.add("List")
         if "Dict[" in annotation:
             imports.add("Dict")
         return imports
 
     @property
+    def pydantic_imports(self) -> Set[str]:
+        return set()
+
+    @property
     def use_builtins(self) -> bool:
         return self.py_type in self.parent.builtins_types or (
             self.py_type == self.py_name and self.py_name in dir(builtins)
         )
 
     def add_imports_to(self, output_file: OutputTemplate) -> None:
         output_file.datetime_imports.update(self.datetime_imports)
         output_file.typing_imports.update(self.typing_imports)
+        output_file.pydantic_imports.update(self.pydantic_imports)
         output_file.builtins_import = output_file.builtins_import or self.use_builtins
 
     @property
     def field_wraps(self) -> Optional[str]:
         """Returns betterproto wrapped field type or None."""
         match_wrapper = re.match(
             r"\.google\.protobuf\.(.+)Value$", self.proto_obj.type_name
@@ -565,14 +585,28 @@
         args = super().betterproto_field_args
         group = self.parent.proto_obj.oneof_decl[self.proto_obj.oneof_index].name
         args.append(f'group="{group}"')
         return args
 
 
 @dataclass
+class PydanticOneOfFieldCompiler(OneOfFieldCompiler):
+    @property
+    def optional(self) -> bool:
+        # Force the optional to be True. This will allow the pydantic dataclass
+        # to validate the object correctly by allowing the field to be let empty.
+        # We add a pydantic validator later to ensure exactly one field is defined.
+        return True
+
+    @property
+    def pydantic_imports(self) -> Set[str]:
+        return {"root_validator"}
+
+
+@dataclass
 class MapEntryCompiler(FieldCompiler):
     py_k_type: Type = PLACEHOLDER
     py_v_type: Type = PLACEHOLDER
     proto_k_type: str = PLACEHOLDER
     proto_v_type: str = PLACEHOLDER
 
     def __post_init__(self) -> None:
@@ -675,15 +709,14 @@
     @property
     def py_name(self) -> str:
         return pythonize_class_name(self.proto_name)
 
 
 @dataclass
 class ServiceMethodCompiler(ProtoContentBase):
-
     parent: ServiceCompiler
     proto_obj: MethodDescriptorProto
     path: List[int] = PLACEHOLDER
     comment_indent: int = 8
 
     def __post_init__(self) -> None:
         # Add method to service
@@ -746,15 +779,15 @@
         package, name = parse_source_type_name(self.proto_obj.input_type)
 
         # Nested types are currently flattened without dots.
         # Todo: keep a fully quantified name in types, that is
         # comparable with method.input_type
         for msg in self.request.all_messages:
             if (
-                msg.py_name == name.replace(".", "")
+                msg.py_name == pythonize_class_name(name.replace(".", ""))
                 and msg.output_file.package == package
             ):
                 return msg
         return None
 
     @property
     def py_input_message_type(self) -> str:
```

### Comparing `betterproto-2.0.0b5/src/betterproto/plugin/parser.py` & `betterproto-2.0.0b6/src/betterproto/plugin/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     Tuple,
     Union,
 )
 
 from betterproto.lib.google.protobuf import (
     DescriptorProto,
     EnumDescriptorProto,
+    FieldDescriptorProto,
     FileDescriptorProto,
     ServiceDescriptorProto,
 )
 from betterproto.lib.google.protobuf.compiler import (
     CodeGeneratorRequest,
     CodeGeneratorResponse,
     CodeGeneratorResponseFeature,
@@ -26,14 +27,15 @@
     EnumDefinitionCompiler,
     FieldCompiler,
     MapEntryCompiler,
     MessageCompiler,
     OneOfFieldCompiler,
     OutputTemplate,
     PluginRequestCompiler,
+    PydanticOneOfFieldCompiler,
     ServiceCompiler,
     ServiceMethodCompiler,
     is_map,
     is_oneof,
 )
 
 
@@ -87,14 +89,19 @@
             proto_file.package == "google.protobuf"
             and "INCLUDE_GOOGLE" not in plugin_options
         ):
             # If not INCLUDE_GOOGLE,
             # skip outputting Google's well-known types
             request_data.output_packages[output_package_name].output = False
 
+        if "pydantic_dataclasses" in plugin_options:
+            request_data.output_packages[
+                output_package_name
+            ].pydantic_dataclasses = True
+
     # Read Messages and Enums
     # We need to read Messages before Services in so that we can
     # get the references to input/output messages for each service
     for output_package_name, output_package in request_data.output_packages.items():
         for proto_input_file in output_package.input_files:
             for item, path in traverse(proto_input_file):
                 read_protobuf_type(
@@ -141,14 +148,32 @@
 
     for output_package_name in sorted(output_paths.union(init_files)):
         print(f"Writing {output_package_name}", file=sys.stderr)
 
     return response
 
 
+def _make_one_of_field_compiler(
+    output_package: OutputTemplate,
+    source_file: "FileDescriptorProto",
+    parent: MessageCompiler,
+    proto_obj: "FieldDescriptorProto",
+    path: List[int],
+) -> FieldCompiler:
+
+    pydantic = output_package.pydantic_dataclasses
+    Cls = PydanticOneOfFieldCompiler if pydantic else OneOfFieldCompiler
+    return Cls(
+        source_file=source_file,
+        parent=parent,
+        proto_obj=proto_obj,
+        path=path,
+    )
+
+
 def read_protobuf_type(
     item: DescriptorProto,
     path: List[int],
     source_file: "FileDescriptorProto",
     output_package: OutputTemplate,
 ) -> None:
     if isinstance(item, DescriptorProto):
@@ -164,19 +189,16 @@
                 MapEntryCompiler(
                     source_file=source_file,
                     parent=message_data,
                     proto_obj=field,
                     path=path + [2, index],
                 )
             elif is_oneof(field):
-                OneOfFieldCompiler(
-                    source_file=source_file,
-                    parent=message_data,
-                    proto_obj=field,
-                    path=path + [2, index],
+                _make_one_of_field_compiler(
+                    output_package, source_file, message_data, field, path + [2, index]
                 )
             else:
                 FieldCompiler(
                     source_file=source_file,
                     parent=message_data,
                     proto_obj=field,
                     path=path + [2, index],
```

### Comparing `betterproto-2.0.0b5/src/betterproto/templates/template.py.j2` & `betterproto-2.0.0b6/src/betterproto/templates/template.py.j2`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,39 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: {{ ', '.join(output_file.input_filenames) }}
 # plugin: python-betterproto
+# This file has been @generated
 {% for i in output_file.python_module_imports|sort %}
 import {{ i }}
 {% endfor %}
+
+{% if output_file.pydantic_dataclasses %}
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from dataclasses import dataclass
+else:
+    from pydantic.dataclasses import dataclass
+{%- else -%}
 from dataclasses import dataclass
+{% endif %}
+
 {% if output_file.datetime_imports %}
 from datetime import {% for i in output_file.datetime_imports|sort %}{{ i }}{% if not loop.last %}, {% endif %}{% endfor %}
 
 {% endif%}
 {% if output_file.typing_imports %}
 from typing import {% for i in output_file.typing_imports|sort %}{{ i }}{% if not loop.last %}, {% endif %}{% endfor %}
 
 {% endif %}
 
+{% if output_file.pydantic_imports %}
+from pydantic import {% for i in output_file.pydantic_imports|sort %}{{ i }}{% if not loop.last %}, {% endif %}{% endfor %}
+
+{% endif %}
+
 import betterproto
 {% if output_file.services %}
 from betterproto.grpc.grpclib_server import ServiceBase
 import grpclib
 {% endif %}
 
 {% for i in output_file.imports|sort %}
@@ -75,14 +91,19 @@
         super().__post_init__()
         {% for field in message.deprecated_fields %}
         if self.is_set("{{ field }}"):
             warnings.warn("{{ message.py_name }}.{{ field }} is deprecated", DeprecationWarning)
         {% endfor %}
     {%  endif %}
 
+    {% if output_file.pydantic_dataclasses and message.has_oneof_fields %}
+    @root_validator()
+    def check_oneof(cls, values):
+        return cls._validate_field_groups(values)
+    {%  endif %}
 
 {% endfor %}
 {% for service in output_file.services %}
 class {{ service.py_name }}Stub(betterproto.ServiceStub):
     {% if service.comment %}
 {{ service.comment }}
 
@@ -174,14 +195,17 @@
         {%- endif -%}
             ) -> {% if method.server_streaming %}AsyncIterator["{{ method.py_output_message_type }}"]{% else %}"{{ method.py_output_message_type }}"{% endif %}:
         {% if method.comment %}
 {{ method.comment }}
 
         {% endif %}
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+        {% if method.server_streaming %}
+        yield {{ method.py_output_message_type }}()
+        {% endif %}
 
     {% endfor %}
 
     {% for method in service.methods %}
     async def __rpc_{{ method.py_name }}(self, stream: "grpclib.server.Stream[{{ method.py_input_message_type }}, {{ method.py_output_message_type }}]") -> None:
         {% if not method.client_streaming %}
         request = await stream.recv_message()
@@ -218,7 +242,15 @@
             {{ method.py_input_message_type }},
             {{ method.py_output_message_type }},
         ),
         {% endfor %}
         }
 
 {% endfor %}
+
+{% if output_file.pydantic_dataclasses %}
+{% for message in output_file.messages %}
+{% if message.has_message_field %}
+{{ message.py_name }}.__pydantic_model__.update_forward_refs()  # type: ignore
+{% endif %}
+{% endfor %}
+{% endif %}
```

### Comparing `betterproto-2.0.0b5/setup.py` & `betterproto-2.0.0b6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,559 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: betterproto
+Version: 2.0.0b6
+Summary: A better Protobuf / gRPC generator & library
+Home-page: https://github.com/danielgtaylor/python-betterproto
+License: MIT
+Keywords: protobuf,gRPC
+Author: Daniel G. Taylor
+Author-email: danielgtaylor@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: compiler
+Requires-Dist: black (>=19.3b0) ; extra == "compiler"
+Requires-Dist: grpclib (>=0.4.1,<0.5.0)
+Requires-Dist: importlib-metadata (>=1.6.0) ; python_version < "3.8"
+Requires-Dist: isort (>=5.11.5,<6.0.0) ; extra == "compiler"
+Requires-Dist: jinja2 (>=3.0.3) ; extra == "compiler"
+Requires-Dist: python-dateutil (>=2.8,<3.0)
+Project-URL: Repository, https://github.com/danielgtaylor/python-betterproto
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Better Protobuf / gRPC Support for Python
 
-packages = \
-['betterproto',
- 'betterproto.compile',
- 'betterproto.grpc',
- 'betterproto.grpc.util',
- 'betterproto.lib',
- 'betterproto.lib.google',
- 'betterproto.lib.google.protobuf',
- 'betterproto.lib.google.protobuf.compiler',
- 'betterproto.plugin']
-
-package_data = \
-{'': ['*'], 'betterproto': ['templates/*']}
-
-install_requires = \
-['grpclib>=0.4.1,<0.5.0', 'python-dateutil>=2.8,<3.0']
-
-extras_require = \
-{':python_version >= "3.6" and python_version < "3.7"': ['dataclasses>=0.7,<0.8'],
- 'compiler': ['black>=19.3b0', 'jinja2>=3.0.3', 'isort>=5.10.1,<6.0.0']}
-
-entry_points = \
-{'console_scripts': ['protoc-gen-python_betterproto = betterproto.plugin:main']}
-
-setup_kwargs = {
-    'name': 'betterproto',
-    'version': '2.0.0b5',
-    'description': 'A better Protobuf / gRPC generator & library',
-    'long_description': '# Better Protobuf / gRPC Support for Python\n\n![](https://github.com/danielgtaylor/python-betterproto/workflows/CI/badge.svg)\n> :octocat: If you\'re reading this on github, please be aware that it might mention unreleased features! See the latest released README on [pypi](https://pypi.org/project/betterproto/).\n\nThis project aims to provide an improved experience when using Protobuf / gRPC in a modern Python environment by making use of modern language features and generating readable, understandable, idiomatic Python code. It will not support legacy features or environments (e.g. Protobuf 2). The following are supported:\n\n- Protobuf 3 & gRPC code generation\n  - Both binary & JSON serialization is built-in\n- Python 3.6+ making use of:\n  - Enums\n  - Dataclasses\n  - `async`/`await`\n  - Timezone-aware `datetime` and `timedelta` objects\n  - Relative imports\n  - Mypy type checking\n\nThis project is heavily inspired by, and borrows functionality from:\n\n- https://github.com/protocolbuffers/protobuf/tree/master/python\n- https://github.com/eigenein/protobuf/\n- https://github.com/vmagamedov/grpclib\n\n## Motivation\n\nThis project exists because I am unhappy with the state of the official Google protoc plugin for Python.\n\n- No `async` support (requires additional `grpclib` plugin)\n- No typing support or code completion/intelligence (requires additional `mypy` plugin)\n- No `__init__.py` module files get generated\n- Output is not importable\n  - Import paths break in Python 3 unless you mess with `sys.path`\n- Bugs when names clash (e.g. `codecs` package)\n- Generated code is not idiomatic\n  - Completely unreadable runtime code-generation\n  - Much code looks like C++ or Java ported 1:1 to Python\n  - Capitalized function names like `HasField()` and `SerializeToString()`\n  - Uses `SerializeToString()` rather than the built-in `__bytes__()`\n  - Special wrapped types don\'t use Python\'s `None`\n  - Timestamp/duration types don\'t use Python\'s built-in `datetime` module\n\n\nThis project is a reimplementation from the ground up focused on idiomatic modern Python to help fix some of the above. While it may not be a 1:1 drop-in replacement due to changed method names and call patterns, the wire format is identical.\n\n## Installation\n\nFirst, install the package. Note that the `[compiler]` feature flag tells it to install extra dependencies only needed by the `protoc` plugin:\n\n```sh\n# Install both the library and compiler\npip install "betterproto[compiler]"\n\n# Install just the library (to use the generated code output)\npip install betterproto\n```\n\n*Betterproto* is under active development. To install the latest beta version, use `pip install --pre betterproto`.\n\n## Getting Started\n\n### Compiling proto files\n\nGiven you installed the compiler and have a proto file, e.g `example.proto`:\n\n```protobuf\nsyntax = "proto3";\n\npackage hello;\n\n// Greeting represents a message you can tell a user.\nmessage Greeting {\n  string message = 1;\n}\n```\n\nYou can run the following to invoke protoc directly:\n\n```sh\nmkdir lib\nprotoc -I . --python_betterproto_out=lib example.proto\n```\n\nor run the following to invoke protoc via grpcio-tools:\n\n```sh\npip install grpcio-tools\npython -m grpc_tools.protoc -I . --python_betterproto_out=lib example.proto\n```\n\nThis will generate `lib/hello/__init__.py` which looks like:\n\n```python\n# Generated by the protocol buffer compiler.  DO NOT EDIT!\n# sources: example.proto\n# plugin: python-betterproto\nfrom dataclasses import dataclass\n\nimport betterproto\n\n\n@dataclass\nclass Greeting(betterproto.Message):\n    """Greeting represents a message you can tell a user."""\n\n    message: str = betterproto.string_field(1)\n```\n\nNow you can use it!\n\n```python\n>>> from lib.hello import Greeting\n>>> test = Greeting()\n>>> test\nGreeting(message=\'\')\n\n>>> test.message = "Hey!"\n>>> test\nGreeting(message="Hey!")\n\n>>> serialized = bytes(test)\n>>> serialized\nb\'\\n\\x04Hey!\'\n\n>>> another = Greeting().parse(serialized)\n>>> another\nGreeting(message="Hey!")\n\n>>> another.to_dict()\n{"message": "Hey!"}\n>>> another.to_json(indent=2)\n\'{\\n  "message": "Hey!"\\n}\'\n```\n\n### Async gRPC Support\n\nThe generated Protobuf `Message` classes are compatible with [grpclib](https://github.com/vmagamedov/grpclib) so you are free to use it if you like. That said, this project also includes support for async gRPC stub generation with better static type checking and code completion support. It is enabled by default.\n\nGiven an example service definition:\n\n```protobuf\nsyntax = "proto3";\n\npackage echo;\n\nmessage EchoRequest {\n  string value = 1;\n  // Number of extra times to echo\n  uint32 extra_times = 2;\n}\n\nmessage EchoResponse {\n  repeated string values = 1;\n}\n\nmessage EchoStreamResponse  {\n  string value = 1;\n}\n\nservice Echo {\n  rpc Echo(EchoRequest) returns (EchoResponse);\n  rpc EchoStream(EchoRequest) returns (stream EchoStreamResponse);\n}\n```\n\nGenerate echo proto file:\n\n```\npython -m grpc_tools.protoc -I . --python_betterproto_out=. echo.proto\n```\n\nA client can be implemented as follows:\n```python\nimport asyncio\nimport echo\n\nfrom grpclib.client import Channel\n\n\nasync def main():\n    channel = Channel(host="127.0.0.1", port=50051)\n    service = echo.EchoStub(channel)\n    response = await service.echo(echo.EchoRequest(value="hello", extra_times=1))\n    print(response)\n\n    async for response in service.echo_stream(echo.EchoRequest(value="hello", extra_times=1)):\n        print(response)\n\n    # don\'t forget to close the channel when done!\n    channel.close()\n\n\nif __name__ == "__main__":\n    loop = asyncio.get_event_loop()\n    loop.run_until_complete(main())\n\n```\n\nwhich would output\n```python\nEchoResponse(values=[\'hello\', \'hello\'])\nEchoStreamResponse(value=\'hello\')\nEchoStreamResponse(value=\'hello\')\n```\n\nThis project also produces server-facing stubs that can be used to implement a Python\ngRPC server.\nTo use them, simply subclass the base class in the generated files and override the\nservice methods:\n\n```python\nimport asyncio\nfrom echo import EchoBase, EchoRequest, EchoResponse, EchoStreamResponse\nfrom grpclib.server import Server\nfrom typing import AsyncIterator\n\n\nclass EchoService(EchoBase):\n    async def echo(self, echo_request: "EchoRequest") -> "EchoResponse":\n        return EchoResponse([echo_request.value for _ in range(echo_request.extra_times)])\n\n    async def echo_stream(self, echo_request: "EchoRequest") -> AsyncIterator["EchoStreamResponse"]:\n        for _ in range(echo_request.extra_times):\n            yield EchoStreamResponse(echo_request.value)\n\n\nasync def main():\n    server = Server([EchoService()])\n    await server.start("127.0.0.1", 50051)\n    await server.wait_closed()\n\nif __name__ == \'__main__\':\n    loop = asyncio.get_event_loop()\n    loop.run_until_complete(main())\n```\n\n### JSON\n\nBoth serializing and parsing are supported to/from JSON and Python dictionaries using the following methods:\n\n- Dicts: `Message().to_dict()`, `Message().from_dict(...)`\n- JSON: `Message().to_json()`, `Message().from_json(...)`\n\nFor compatibility the default is to convert field names to `camelCase`. You can control this behavior by passing a casing value, e.g:\n\n```python\nMyMessage().to_dict(casing=betterproto.Casing.SNAKE)\n```\n\n### Determining if a message was sent\n\nSometimes it is useful to be able to determine whether a message has been sent on the wire. This is how the Google wrapper types work to let you know whether a value is unset, set as the default (zero value), or set as something else, for example.\n\nUse `betterproto.serialized_on_wire(message)` to determine if it was sent. This is a little bit different from the official Google generated Python code, and it lives outside the generated `Message` class to prevent name clashes. Note that it **only** supports Proto 3 and thus can **only** be used to check if `Message` fields are set. You cannot check if a scalar was sent on the wire.\n\n```py\n# Old way (official Google Protobuf package)\n>>> mymessage.HasField(\'myfield\')\n\n# New way (this project)\n>>> betterproto.serialized_on_wire(mymessage.myfield)\n```\n\n### One-of Support\n\nProtobuf supports grouping fields in a `oneof` clause. Only one of the fields in the group may be set at a given time. For example, given the proto:\n\n```protobuf\nsyntax = "proto3";\n\nmessage Test {\n  oneof foo {\n    bool on = 1;\n    int32 count = 2;\n    string name = 3;\n  }\n}\n```\n\nYou can use `betterproto.which_one_of(message, group_name)` to determine which of the fields was set. It returns a tuple of the field name and value, or a blank string and `None` if unset.\n\n```py\n>>> test = Test()\n>>> betterproto.which_one_of(test, "foo")\n["", None]\n\n>>> test.on = True\n>>> betterproto.which_one_of(test, "foo")\n["on", True]\n\n# Setting one member of the group resets the others.\n>>> test.count = 57\n>>> betterproto.which_one_of(test, "foo")\n["count", 57]\n>>> test.on\nFalse\n\n# Default (zero) values also work.\n>>> test.name = ""\n>>> betterproto.which_one_of(test, "foo")\n["name", ""]\n>>> test.count\n0\n>>> test.on\nFalse\n```\n\nAgain this is a little different than the official Google code generator:\n\n```py\n# Old way (official Google protobuf package)\n>>> message.WhichOneof("group")\n"foo"\n\n# New way (this project)\n>>> betterproto.which_one_of(message, "group")\n["foo", "foo\'s value"]\n```\n\n### Well-Known Google Types\n\nGoogle provides several well-known message types like a timestamp, duration, and several wrappers used to provide optional zero value support. Each of these has a special JSON representation and is handled a little differently from normal messages. The Python mapping for these is as follows:\n\n| Google Message              | Python Type                              | Default                |\n| --------------------------- | ---------------------------------------- | ---------------------- |\n| `google.protobuf.duration`  | [`datetime.timedelta`][td]               | `0`                    |\n| `google.protobuf.timestamp` | Timezone-aware [`datetime.datetime`][dt] | `1970-01-01T00:00:00Z` |\n| `google.protobuf.*Value`    | `Optional[...]`                          | `None`                 |\n| `google.protobuf.*`         | `betterproto.lib.google.protobuf.*`      | `None`                 |\n\n[td]: https://docs.python.org/3/library/datetime.html#timedelta-objects\n[dt]: https://docs.python.org/3/library/datetime.html#datetime.datetime\n\nFor the wrapper types, the Python type corresponds to the wrapped type, e.g. `google.protobuf.BoolValue` becomes `Optional[bool]` while `google.protobuf.Int32Value` becomes `Optional[int]`. All of the optional values default to `None`, so don\'t forget to check for that possible state. Given:\n\n```protobuf\nsyntax = "proto3";\n\nimport "google/protobuf/duration.proto";\nimport "google/protobuf/timestamp.proto";\nimport "google/protobuf/wrappers.proto";\n\nmessage Test {\n  google.protobuf.BoolValue maybe = 1;\n  google.protobuf.Timestamp ts = 2;\n  google.protobuf.Duration duration = 3;\n}\n```\n\nYou can do stuff like:\n\n```py\n>>> t = Test().from_dict({"maybe": True, "ts": "2019-01-01T12:00:00Z", "duration": "1.200s"})\n>>> t\nTest(maybe=True, ts=datetime.datetime(2019, 1, 1, 12, 0, tzinfo=datetime.timezone.utc), duration=datetime.timedelta(seconds=1, microseconds=200000))\n\n>>> t.ts - t.duration\ndatetime.datetime(2019, 1, 1, 11, 59, 58, 800000, tzinfo=datetime.timezone.utc)\n\n>>> t.ts.isoformat()\n\'2019-01-01T12:00:00+00:00\'\n\n>>> t.maybe = None\n>>> t.to_dict()\n{\'ts\': \'2019-01-01T12:00:00Z\', \'duration\': \'1.200s\'}\n```\n\n## Development\n\n- _Join us on [Slack](https://join.slack.com/t/betterproto/shared_invite/zt-f0n0uolx-iN8gBNrkPxtKHTLpG3o1OQ)!_\n- _See how you can help &rarr; [Contributing](.github/CONTRIBUTING.md)_\n\n### Requirements\n\n- Python (3.6 or higher)\n\n- [poetry](https://python-poetry.org/docs/#installation)\n  *Needed to install dependencies in a virtual environment*\n\n- [poethepoet](https://github.com/nat-n/poethepoet) for running development tasks as defined in pyproject.toml\n  - Can be installed to your host environment via `pip install poethepoet` then executed as simple `poe`\n  - or run from the poetry venv as `poetry run poe`\n\n### Setup\n\n```sh\n# Get set up with the virtual env & dependencies\npoetry install -E compiler\n\n# Activate the poetry environment\npoetry shell\n```\n\n### Code style\n\nThis project enforces [black](https://github.com/psf/black) python code formatting.\n\nBefore committing changes run:\n\n```sh\npoe format\n```\n\nTo avoid merge conflicts later, non-black formatted python code will fail in CI.\n\n### Tests\n\nThere are two types of tests:\n\n1. Standard tests\n2. Custom tests\n\n#### Standard tests\n\nAdding a standard test case is easy.\n\n- Create a new directory `betterproto/tests/inputs/<name>`\n  - add `<name>.proto`  with a message called `Test`\n  - add `<name>.json` with some test data (optional)\n\nIt will be picked up automatically when you run the tests.\n\n- See also: [Standard Tests Development Guide](tests/README.md)\n\n#### Custom tests\n\nCustom tests are found in `tests/test_*.py` and are run with pytest.\n\n#### Running\n\nHere\'s how to run the tests.\n\n```sh\n# Generate assets from sample .proto files required by the tests\npoe generate\n# Run the tests\npoe test\n```\n\nTo run tests as they are run in CI (with tox) run:\n\n```sh\npoe full-test\n```\n\n### (Re)compiling Google Well-known Types\n\nBetterproto includes compiled versions for Google\'s well-known types at [src/betterproto/lib/google](src/betterproto/lib/google).\nBe sure to regenerate these files when modifying the plugin output format, and validate by running the tests.\n\nNormally, the plugin does not compile any references to `google.protobuf`, since they are pre-compiled. To force compilation of `google.protobuf`, use the option `--custom_opt=INCLUDE_GOOGLE`. \n\nAssuming your `google.protobuf` source files (included with all releases of `protoc`) are located in `/usr/local/include`, you can regenerate them as follows:\n\n```sh\nprotoc \\\n    --plugin=protoc-gen-custom=src/betterproto/plugin/main.py \\\n    --custom_opt=INCLUDE_GOOGLE \\\n    --custom_out=src/betterproto/lib \\\n    -I /usr/local/include/ \\\n    /usr/local/include/google/protobuf/*.proto\n```\n\n### TODO\n\n- [x] Fixed length fields\n  - [x] Packed fixed-length\n- [x] Zig-zag signed fields (sint32, sint64)\n- [x] Don\'t encode zero values for nested types\n- [x] Enums\n- [x] Repeated message fields\n- [x] Maps\n  - [x] Maps of message fields\n- [x] Support passthrough of unknown fields\n- [x] Refs to nested types\n- [x] Imports in proto files\n- [x] Well-known Google types\n  - [ ] Support as request input\n  - [ ] Support as response output\n    - [ ] Automatically wrap/unwrap responses\n- [x] OneOf support\n  - [x] Basic support on the wire\n  - [x] Check which was set from the group\n  - [x] Setting one unsets the others\n- [ ] JSON that isn\'t completely naive.\n  - [x] 64-bit ints as strings\n  - [x] Maps\n  - [x] Lists\n  - [x] Bytes as base64\n  - [ ] Any support\n  - [x] Enum strings\n  - [x] Well known types support (timestamp, duration, wrappers)\n  - [x] Support different casing (orig vs. camel vs. others?)\n- [x] Async service stubs\n  - [x] Unary-unary\n  - [x] Server streaming response\n  - [x] Client streaming request\n- [x] Renaming messages and fields to conform to Python name standards\n- [x] Renaming clashes with language keywords\n- [x] Python package\n- [x] Automate running tests\n- [ ] Cleanup!\n\n## Community\n\nJoin us on [Slack](https://join.slack.com/t/betterproto/shared_invite/zt-f0n0uolx-iN8gBNrkPxtKHTLpG3o1OQ)!\n\n## License\n\nCopyright © 2019 Daniel G. Taylor\n\nhttp://dgt.mit-license.org/\n',
-    'author': 'Daniel G. Taylor',
-    'author_email': 'danielgtaylor@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/danielgtaylor/python-betterproto',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6.2,<4.0',
+![](https://github.com/danielgtaylor/python-betterproto/workflows/CI/badge.svg)
+> :octocat: If you're reading this on github, please be aware that it might mention unreleased features! See the latest released README on [pypi](https://pypi.org/project/betterproto/).
+
+This project aims to provide an improved experience when using Protobuf / gRPC in a modern Python environment by making use of modern language features and generating readable, understandable, idiomatic Python code. It will not support legacy features or environments (e.g. Protobuf 2). The following are supported:
+
+- Protobuf 3 & gRPC code generation
+  - Both binary & JSON serialization is built-in
+- Python 3.7+ making use of:
+  - Enums
+  - Dataclasses
+  - `async`/`await`
+  - Timezone-aware `datetime` and `timedelta` objects
+  - Relative imports
+  - Mypy type checking
+- [Pydantic Models](https://docs.pydantic.dev/) generation (see #generating-pydantic-models)
+
+This project is heavily inspired by, and borrows functionality from:
+
+- https://github.com/protocolbuffers/protobuf/tree/master/python
+- https://github.com/eigenein/protobuf/
+- https://github.com/vmagamedov/grpclib
+
+## Motivation
+
+This project exists because I am unhappy with the state of the official Google protoc plugin for Python.
+
+- No `async` support (requires additional `grpclib` plugin)
+- No typing support or code completion/intelligence (requires additional `mypy` plugin)
+- No `__init__.py` module files get generated
+- Output is not importable
+  - Import paths break in Python 3 unless you mess with `sys.path`
+- Bugs when names clash (e.g. `codecs` package)
+- Generated code is not idiomatic
+  - Completely unreadable runtime code-generation
+  - Much code looks like C++ or Java ported 1:1 to Python
+  - Capitalized function names like `HasField()` and `SerializeToString()`
+  - Uses `SerializeToString()` rather than the built-in `__bytes__()`
+  - Special wrapped types don't use Python's `None`
+  - Timestamp/duration types don't use Python's built-in `datetime` module
+
+
+This project is a reimplementation from the ground up focused on idiomatic modern Python to help fix some of the above. While it may not be a 1:1 drop-in replacement due to changed method names and call patterns, the wire format is identical.
+
+## Installation
+
+First, install the package. Note that the `[compiler]` feature flag tells it to install extra dependencies only needed by the `protoc` plugin:
+
+```sh
+# Install both the library and compiler
+pip install "betterproto[compiler]"
+
+# Install just the library (to use the generated code output)
+pip install betterproto
+```
+
+*Betterproto* is under active development. To install the latest beta version, use `pip install --pre betterproto`.
+
+## Getting Started
+
+### Compiling proto files
+
+Given you installed the compiler and have a proto file, e.g `example.proto`:
+
+```protobuf
+syntax = "proto3";
+
+package hello;
+
+// Greeting represents a message you can tell a user.
+message Greeting {
+  string message = 1;
 }
+```
+
+You can run the following to invoke protoc directly:
+
+```sh
+mkdir lib
+protoc -I . --python_betterproto_out=lib example.proto
+```
+
+or run the following to invoke protoc via grpcio-tools:
+
+```sh
+pip install grpcio-tools
+python -m grpc_tools.protoc -I . --python_betterproto_out=lib example.proto
+```
+
+This will generate `lib/hello/__init__.py` which looks like:
+
+```python
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# sources: example.proto
+# plugin: python-betterproto
+from dataclasses import dataclass
+
+import betterproto
+
+
+@dataclass
+class Greeting(betterproto.Message):
+    """Greeting represents a message you can tell a user."""
+
+    message: str = betterproto.string_field(1)
+```
+
+Now you can use it!
+
+```python
+>>> from lib.hello import Greeting
+>>> test = Greeting()
+>>> test
+Greeting(message='')
+
+>>> test.message = "Hey!"
+>>> test
+Greeting(message="Hey!")
+
+>>> serialized = bytes(test)
+>>> serialized
+b'\n\x04Hey!'
+
+>>> another = Greeting().parse(serialized)
+>>> another
+Greeting(message="Hey!")
+
+>>> another.to_dict()
+{"message": "Hey!"}
+>>> another.to_json(indent=2)
+'{\n  "message": "Hey!"\n}'
+```
+
+### Async gRPC Support
+
+The generated Protobuf `Message` classes are compatible with [grpclib](https://github.com/vmagamedov/grpclib) so you are free to use it if you like. That said, this project also includes support for async gRPC stub generation with better static type checking and code completion support. It is enabled by default.
+
+Given an example service definition:
+
+```protobuf
+syntax = "proto3";
+
+package echo;
+
+message EchoRequest {
+  string value = 1;
+  // Number of extra times to echo
+  uint32 extra_times = 2;
+}
+
+message EchoResponse {
+  repeated string values = 1;
+}
+
+message EchoStreamResponse  {
+  string value = 1;
+}
+
+service Echo {
+  rpc Echo(EchoRequest) returns (EchoResponse);
+  rpc EchoStream(EchoRequest) returns (stream EchoStreamResponse);
+}
+```
+
+Generate echo proto file:
+
+```
+python -m grpc_tools.protoc -I . --python_betterproto_out=. echo.proto
+```
+
+A client can be implemented as follows:
+```python
+import asyncio
+import echo
+
+from grpclib.client import Channel
+
+
+async def main():
+    channel = Channel(host="127.0.0.1", port=50051)
+    service = echo.EchoStub(channel)
+    response = await service.echo(echo.EchoRequest(value="hello", extra_times=1))
+    print(response)
+
+    async for response in service.echo_stream(echo.EchoRequest(value="hello", extra_times=1)):
+        print(response)
+
+    # don't forget to close the channel when done!
+    channel.close()
+
+
+if __name__ == "__main__":
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(main())
+
+```
+
+which would output
+```python
+EchoResponse(values=['hello', 'hello'])
+EchoStreamResponse(value='hello')
+EchoStreamResponse(value='hello')
+```
+
+This project also produces server-facing stubs that can be used to implement a Python
+gRPC server.
+To use them, simply subclass the base class in the generated files and override the
+service methods:
+
+```python
+import asyncio
+from echo import EchoBase, EchoRequest, EchoResponse, EchoStreamResponse
+from grpclib.server import Server
+from typing import AsyncIterator
+
+
+class EchoService(EchoBase):
+    async def echo(self, echo_request: "EchoRequest") -> "EchoResponse":
+        return EchoResponse([echo_request.value for _ in range(echo_request.extra_times)])
+
+    async def echo_stream(self, echo_request: "EchoRequest") -> AsyncIterator["EchoStreamResponse"]:
+        for _ in range(echo_request.extra_times):
+            yield EchoStreamResponse(echo_request.value)
+
+
+async def main():
+    server = Server([EchoService()])
+    await server.start("127.0.0.1", 50051)
+    await server.wait_closed()
+
+if __name__ == '__main__':
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(main())
+```
+
+### JSON
+
+Both serializing and parsing are supported to/from JSON and Python dictionaries using the following methods:
+
+- Dicts: `Message().to_dict()`, `Message().from_dict(...)`
+- JSON: `Message().to_json()`, `Message().from_json(...)`
+
+For compatibility the default is to convert field names to `camelCase`. You can control this behavior by passing a casing value, e.g:
+
+```python
+MyMessage().to_dict(casing=betterproto.Casing.SNAKE)
+```
+
+### Determining if a message was sent
+
+Sometimes it is useful to be able to determine whether a message has been sent on the wire. This is how the Google wrapper types work to let you know whether a value is unset, set as the default (zero value), or set as something else, for example.
+
+Use `betterproto.serialized_on_wire(message)` to determine if it was sent. This is a little bit different from the official Google generated Python code, and it lives outside the generated `Message` class to prevent name clashes. Note that it **only** supports Proto 3 and thus can **only** be used to check if `Message` fields are set. You cannot check if a scalar was sent on the wire.
+
+```py
+# Old way (official Google Protobuf package)
+>>> mymessage.HasField('myfield')
+
+# New way (this project)
+>>> betterproto.serialized_on_wire(mymessage.myfield)
+```
+
+### One-of Support
+
+Protobuf supports grouping fields in a `oneof` clause. Only one of the fields in the group may be set at a given time. For example, given the proto:
+
+```protobuf
+syntax = "proto3";
+
+message Test {
+  oneof foo {
+    bool on = 1;
+    int32 count = 2;
+    string name = 3;
+  }
+}
+```
+
+You can use `betterproto.which_one_of(message, group_name)` to determine which of the fields was set. It returns a tuple of the field name and value, or a blank string and `None` if unset.
+
+```py
+>>> test = Test()
+>>> betterproto.which_one_of(test, "foo")
+["", None]
+
+>>> test.on = True
+>>> betterproto.which_one_of(test, "foo")
+["on", True]
+
+# Setting one member of the group resets the others.
+>>> test.count = 57
+>>> betterproto.which_one_of(test, "foo")
+["count", 57]
+>>> test.on
+False
+
+# Default (zero) values also work.
+>>> test.name = ""
+>>> betterproto.which_one_of(test, "foo")
+["name", ""]
+>>> test.count
+0
+>>> test.on
+False
+```
+
+Again this is a little different than the official Google code generator:
+
+```py
+# Old way (official Google protobuf package)
+>>> message.WhichOneof("group")
+"foo"
+
+# New way (this project)
+>>> betterproto.which_one_of(message, "group")
+["foo", "foo's value"]
+```
+
+### Well-Known Google Types
+
+Google provides several well-known message types like a timestamp, duration, and several wrappers used to provide optional zero value support. Each of these has a special JSON representation and is handled a little differently from normal messages. The Python mapping for these is as follows:
+
+| Google Message              | Python Type                              | Default                |
+| --------------------------- | ---------------------------------------- | ---------------------- |
+| `google.protobuf.duration`  | [`datetime.timedelta`][td]               | `0`                    |
+| `google.protobuf.timestamp` | Timezone-aware [`datetime.datetime`][dt] | `1970-01-01T00:00:00Z` |
+| `google.protobuf.*Value`    | `Optional[...]`                          | `None`                 |
+| `google.protobuf.*`         | `betterproto.lib.google.protobuf.*`      | `None`                 |
+
+[td]: https://docs.python.org/3/library/datetime.html#timedelta-objects
+[dt]: https://docs.python.org/3/library/datetime.html#datetime.datetime
+
+For the wrapper types, the Python type corresponds to the wrapped type, e.g. `google.protobuf.BoolValue` becomes `Optional[bool]` while `google.protobuf.Int32Value` becomes `Optional[int]`. All of the optional values default to `None`, so don't forget to check for that possible state. Given:
+
+```protobuf
+syntax = "proto3";
+
+import "google/protobuf/duration.proto";
+import "google/protobuf/timestamp.proto";
+import "google/protobuf/wrappers.proto";
+
+message Test {
+  google.protobuf.BoolValue maybe = 1;
+  google.protobuf.Timestamp ts = 2;
+  google.protobuf.Duration duration = 3;
+}
+```
+
+You can do stuff like:
+
+```py
+>>> t = Test().from_dict({"maybe": True, "ts": "2019-01-01T12:00:00Z", "duration": "1.200s"})
+>>> t
+Test(maybe=True, ts=datetime.datetime(2019, 1, 1, 12, 0, tzinfo=datetime.timezone.utc), duration=datetime.timedelta(seconds=1, microseconds=200000))
+
+>>> t.ts - t.duration
+datetime.datetime(2019, 1, 1, 11, 59, 58, 800000, tzinfo=datetime.timezone.utc)
+
+>>> t.ts.isoformat()
+'2019-01-01T12:00:00+00:00'
+
+>>> t.maybe = None
+>>> t.to_dict()
+{'ts': '2019-01-01T12:00:00Z', 'duration': '1.200s'}
+```
+
+## Generating Pydantic Models
+
+You can use python-betterproto to generate pydantic based models, using
+pydantic dataclasses. This means the results of the protobuf unmarshalling will
+be typed checked. The usage is the same, but you need to add a custom option
+when calling the protobuf compiler:
+
+
+```
+protoc -I . --python_betterproto_opt=pydantic_dataclasses --python_betterproto_out=lib example.proto
+```
+
+With the important change being `--python_betterproto_opt=pydantic_dataclasses`. This will
+swap the dataclass implementation from the builtin python dataclass to the
+pydantic dataclass. You must have pydantic as a dependency in your project for
+this to work.
+
+
+
+## Development
+
+- _Join us on [Slack](https://join.slack.com/t/betterproto/shared_invite/zt-f0n0uolx-iN8gBNrkPxtKHTLpG3o1OQ)!_
+- _See how you can help &rarr; [Contributing](.github/CONTRIBUTING.md)_
+
+### Requirements
+
+- Python (3.7 or higher)
+
+- [poetry](https://python-poetry.org/docs/#installation)
+  *Needed to install dependencies in a virtual environment*
+
+- [poethepoet](https://github.com/nat-n/poethepoet) for running development tasks as defined in pyproject.toml
+  - Can be installed to your host environment via `pip install poethepoet` then executed as simple `poe`
+  - or run from the poetry venv as `poetry run poe`
+
+### Setup
+
+```sh
+# Get set up with the virtual env & dependencies
+poetry install -E compiler
+
+# Activate the poetry environment
+poetry shell
+```
+
+### Code style
+
+This project enforces [black](https://github.com/psf/black) python code formatting.
+
+Before committing changes run:
+
+```sh
+poe format
+```
+
+To avoid merge conflicts later, non-black formatted python code will fail in CI.
+
+### Tests
+
+There are two types of tests:
+
+1. Standard tests
+2. Custom tests
+
+#### Standard tests
+
+Adding a standard test case is easy.
+
+- Create a new directory `betterproto/tests/inputs/<name>`
+  - add `<name>.proto`  with a message called `Test`
+  - add `<name>.json` with some test data (optional)
+
+It will be picked up automatically when you run the tests.
+
+- See also: [Standard Tests Development Guide](tests/README.md)
+
+#### Custom tests
+
+Custom tests are found in `tests/test_*.py` and are run with pytest.
+
+#### Running
+
+Here's how to run the tests.
+
+```sh
+# Generate assets from sample .proto files required by the tests
+poe generate
+# Run the tests
+poe test
+```
+
+To run tests as they are run in CI (with tox) run:
+
+```sh
+poe full-test
+```
+
+### (Re)compiling Google Well-known Types
+
+Betterproto includes compiled versions for Google's well-known types at [src/betterproto/lib/google](src/betterproto/lib/google).
+Be sure to regenerate these files when modifying the plugin output format, and validate by running the tests.
+
+Normally, the plugin does not compile any references to `google.protobuf`, since they are pre-compiled. To force compilation of `google.protobuf`, use the option `--custom_opt=INCLUDE_GOOGLE`.
+
+Assuming your `google.protobuf` source files (included with all releases of `protoc`) are located in `/usr/local/include`, you can regenerate them as follows:
+
+```sh
+protoc \
+    --plugin=protoc-gen-custom=src/betterproto/plugin/main.py \
+    --custom_opt=INCLUDE_GOOGLE \
+    --custom_out=src/betterproto/lib \
+    -I /usr/local/include/ \
+    /usr/local/include/google/protobuf/*.proto
+```
+
+### TODO
+
+- [x] Fixed length fields
+  - [x] Packed fixed-length
+- [x] Zig-zag signed fields (sint32, sint64)
+- [x] Don't encode zero values for nested types
+- [x] Enums
+- [x] Repeated message fields
+- [x] Maps
+  - [x] Maps of message fields
+- [x] Support passthrough of unknown fields
+- [x] Refs to nested types
+- [x] Imports in proto files
+- [x] Well-known Google types
+  - [ ] Support as request input
+  - [ ] Support as response output
+    - [ ] Automatically wrap/unwrap responses
+- [x] OneOf support
+  - [x] Basic support on the wire
+  - [x] Check which was set from the group
+  - [x] Setting one unsets the others
+- [ ] JSON that isn't completely naive.
+  - [x] 64-bit ints as strings
+  - [x] Maps
+  - [x] Lists
+  - [x] Bytes as base64
+  - [ ] Any support
+  - [x] Enum strings
+  - [x] Well known types support (timestamp, duration, wrappers)
+  - [x] Support different casing (orig vs. camel vs. others?)
+- [x] Async service stubs
+  - [x] Unary-unary
+  - [x] Server streaming response
+  - [x] Client streaming request
+- [x] Renaming messages and fields to conform to Python name standards
+- [x] Renaming clashes with language keywords
+- [x] Python package
+- [x] Automate running tests
+- [ ] Cleanup!
+
+## Community
+
+Join us on [Slack](https://join.slack.com/t/betterproto/shared_invite/zt-f0n0uolx-iN8gBNrkPxtKHTLpG3o1OQ)!
+
+## License
+
+Copyright © 2019 Daniel G. Taylor
 
+http://dgt.mit-license.org/
 
-setup(**setup_kwargs)
```

