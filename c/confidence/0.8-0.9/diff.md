# Comparing `tmp/confidence-0.8-py3-none-any.whl.zip` & `tmp/confidence-0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 17603 bytes, number of entries: 10
+Zip file size: 18348 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx      533 b- defN 20-Jul-02 14:08 confidence/__init__.py
--rw-rw-r--  2.0 unx      781 b- defN 20-Jul-02 14:08 confidence/exceptions.py
--rw-rw-r--  2.0 unx    11862 b- defN 20-Dec-14 11:47 confidence/io.py
--rw-rw-r--  2.0 unx    12584 b- defN 20-Dec-14 11:47 confidence/models.py
--rw-rw-r--  2.0 unx     3456 b- defN 20-Dec-14 11:47 confidence/utils.py
--rw-rw-r--  2.0 unx    11357 b- defN 20-Dec-14 11:55 confidence-0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6749 b- defN 20-Dec-14 11:55 confidence-0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 20-Dec-14 11:55 confidence-0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 20-Dec-14 11:55 confidence-0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      778 b- defN 20-Dec-14 11:55 confidence-0.8.dist-info/RECORD
-10 files, 48203 bytes uncompressed, 16291 bytes compressed:  66.2%
+-rw-rw-r--  2.0 unx      848 b- defN 21-Feb-01 14:49 confidence/exceptions.py
+-rw-rw-r--  2.0 unx    12503 b- defN 21-Feb-01 14:49 confidence/io.py
+-rw-rw-r--  2.0 unx    14243 b- defN 21-Feb-01 14:49 confidence/models.py
+-rw-rw-r--  2.0 unx     3845 b- defN 21-Feb-01 14:49 confidence/utils.py
+-rw-rw-r--  2.0 unx    11357 b- defN 21-Feb-01 14:52 confidence-0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6816 b- defN 21-Feb-01 14:52 confidence-0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 21-Feb-01 14:52 confidence-0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 21-Feb-01 14:52 confidence-0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      778 b- defN 21-Feb-01 14:52 confidence-0.9.dist-info/RECORD
+10 files, 51026 bytes uncompressed, 17036 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: confidence/models.py
 Comment: 
 
 Filename: confidence/utils.py
 Comment: 
 
-Filename: confidence-0.8.dist-info/LICENSE
+Filename: confidence-0.9.dist-info/LICENSE
 Comment: 
 
-Filename: confidence-0.8.dist-info/METADATA
+Filename: confidence-0.9.dist-info/METADATA
 Comment: 
 
-Filename: confidence-0.8.dist-info/WHEEL
+Filename: confidence-0.9.dist-info/WHEEL
 Comment: 
 
-Filename: confidence-0.8.dist-info/top_level.txt
+Filename: confidence-0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: confidence-0.8.dist-info/RECORD
+Filename: confidence-0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## confidence/exceptions.py

```diff
@@ -1,30 +1,33 @@
+import typing
+
+
 class ConfigurationError(KeyError):
     pass
 
 
 class MergeConflictError(ConfigurationError):
     """
     Error raised during loading configuration sources that conflict internally.
     """
-    def __init__(self, *args, key):
+    def __init__(self, *args: typing.Any, key: str):
         super().__init__(*args)
         self.conflict = key
 
 
 class NotConfiguredError(ConfigurationError):
     """
     Error raised when a requested configuration key is unavailable and no
     default / fallback value is provided.
     """
-    def __init__(self, *args, key):
+    def __init__(self, *args: typing.Any, key: str):
         super().__init__(*args)
         self.key = key
 
 
 class ConfiguredReferenceError(ConfigurationError):
     """
     Error raised a referenced configuration key is unavailable.
     """
-    def __init__(self, *args, key):
+    def __init__(self, *args: typing.Any, key: str):
         super().__init__(*args)
         self.key = key
```

## confidence/io.py

```diff
@@ -1,44 +1,41 @@
 from enum import IntEnum
 from functools import partial
 from itertools import product
 from os import environ, path
 import re
+import typing
 
 import yaml
 
-from confidence.models import _NoDefault, Configuration, Missing, NotConfigured
+from confidence.models import Configuration, Missing, NoDefault, NotConfigured
 
 
-def read_xdg_config_dirs(name, extension):
+def read_xdg_config_dirs(name: str, extension: str) -> Configuration:
     """
     Read from files found in XDG-specified system-wide configuration paths,
     defaulting to ``/etc/xdg``. Depends on ``XDG_CONFIG_DIRS`` environment
     variable.
 
     :param name: application or configuration set name
     :param extension: file extension to look for
     :return: a `.Configuration` instance with values read from XDG-specified
         directories
     """
-    # find optional value of ${XDG_CONFIG_DIRS}
-    config_dirs = environ.get('XDG_CONFIG_DIRS')
-    if config_dirs:
-        # PATH-like env vars operate in decreasing precedence, reverse this path set to mimic the end result
-        config_dirs = reversed(config_dirs.split(path.pathsep))
-    else:
-        # XDG spec: "If $XDG_CONFIG_DIRS is either not set or empty, a value equal to /etc/xdg should be used."
-        config_dirs = ['/etc/xdg']
+    # XDG spec: "If $XDG_CONFIG_DIRS is either not set or empty, a value equal to /etc/xdg should be used."
+    config_dirs = environ.get('XDG_CONFIG_DIRS', '/etc/xdg')
+    # PATH-like env vars operate in decreasing precedence, reverse this path set to mimic the end result
+    config_dirs = reversed(config_dirs.split(path.pathsep))
 
     # load a file from all config dirs, default to NotConfigured
     return loadf(*(path.join(config_dir, f'{name}.{extension}') for config_dir in config_dirs),
                  default=NotConfigured)
 
 
-def read_xdg_config_home(name, extension):
+def read_xdg_config_home(name: str, extension: str) -> Configuration:
     """
     Read from file found in XDG-specified configuration home directory,
     expanding to ``${HOME}/.config/name.extension`` by default. Depends on
     ``XDG_CONFIG_HOME`` or ``HOME`` environment variables.
 
     :param name: application or configuration set name
     :param extension: file extension to look for
@@ -51,15 +48,15 @@
         # see https://specifications.freedesktop.org/basedir-spec/latest/ar01s03.html
         config_home = path.expanduser('~/.config')
 
     # expand to full path to configuration file in XDG config path
     return loadf(path.join(config_home, f'{name}.{extension}'), default=NotConfigured)
 
 
-def read_envvars(name, extension):
+def read_envvars(name: str, extension: typing.Optional[str] = None) -> Configuration:
     """
     Read environment variables starting with ``NAME_``, where subsequent
     underscores are interpreted as namespaces. Underscores can be retained as
     namespaces by doubling them up, e.g. ``NAME_SPA__CE_KEY`` would be
     accessible in the resulting `.Configuration` as
     ``c.spa_ce.key``, where ``c`` is the `.Configuration` instance.
 
@@ -81,24 +78,24 @@
               for var, value in environ.items()
               # TODO: document ignoring envvar_file
               if var.lower().startswith(prefix) and var.lower() != envvar_file}
     # TODO: envvar values can only be str, how do we configure non-str values?
     if not values:
         return NotConfigured
 
-    def dotted(name):
+    def dotted(name: str) -> str:
         # replace 'regular' underscores (those between alphanumeric characters) with dots first
         name = re.sub(r'([0-9A-Za-z])_([0-9A-Za-z])', r'\1.\2', name)
         # unescape double underscores back to a single one
         return re.sub(r'__', '_', name)
 
     return Configuration({dotted(name): value for name, value in values.items()})
 
 
-def read_envvar_file(name, extension):
+def read_envvar_file(name: str, extension: typing.Optional[str] = None) -> Configuration:
     """
     Read values from a file provided as a environment variable
     ``NAME_CONFIG_FILE``.
 
     :param name: environment variable prefix to look for (without the
         ``_CONFIG_FILE``)
     :param extension: *(unused)*
@@ -109,15 +106,15 @@
         # envvar set, load value as file
         return loadf(envvar_file)
     else:
         # envvar not set, return an empty source
         return NotConfigured
 
 
-def read_envvar_dir(envvar, name, extension):
+def read_envvar_dir(envvar: str, name: str, extension: str) -> Configuration:
     """
     Read values from a file located in a directory specified by a particular
     environment file. ``read_envvar_dir('HOME', 'example', 'yaml')`` would
     look for a file at ``/home/user/example.yaml``. When the environment
     variable isn't set or the file does not exist, `NotConfigured` will be
     returned.
 
@@ -144,15 +141,15 @@
 
     system = 0  #: system-wide configuration locations
     user = 1  #: user-local configuration locations
     application = 2  #: application-local configuration locations (dependent on the current working directory)
     environment = 3  #: configuration from environment variables
 
 
-_LOADERS = {
+_LOADERS: typing.Mapping[Locality, typing.Iterable[typing.Union[str, typing.Callable]]] = {
     Locality.system: (
         # system-wide locations
         read_xdg_config_dirs,
         '/etc/{name}.{extension}',
         '/Library/Preferences/{name}.{extension}',
         partial(read_envvar_dir, 'PROGRAMDATA'),
     ),
@@ -175,15 +172,15 @@
         # application-specific environment variables
         read_envvar_file,
         read_envvars,
     )
 }
 
 
-def loaders(*specifiers):
+def loaders(*specifiers: typing.Union[Locality, str]) -> typing.Iterable[typing.Union[str, typing.Callable]]:
     """
     Generates loaders in the specified order.
 
     Arguments can be `.Locality` instances, producing the loader(s) available
     for that locality, `str` instances (used as file path templates) or
     `callable`s. These can be mixed:
 
@@ -214,65 +211,70 @@
 
 DEFAULT_LOAD_ORDER = tuple(loaders(Locality.system,
                                    Locality.user,
                                    Locality.application,
                                    Locality.environment))
 
 
-def load(*fps, missing=Missing.silent):
+def load(*fps: typing.IO, missing: typing.Any = Missing.silent) -> Configuration:
     """
     Read a `.Configuration` instance from file-like objects.
 
     :param fps: file-like objects (supporting ``.read()``)
     :param missing: policy to be used when a configured key is missing, either
         as a `.Missing` instance or a default value
     :return: a `.Configuration` instance providing values from *fps*
     :rtype: `.Configuration`
     """
     return Configuration(*(yaml.safe_load(fp.read()) for fp in fps), missing=missing)
 
 
-def loadf(*fnames, default=_NoDefault, missing=Missing.silent):
+def loadf(*fnames: str,
+          default: typing.Any = NoDefault,
+          missing: typing.Any = Missing.silent) -> Configuration:
     """
     Read a `.Configuration` instance from named files.
 
     :param fnames: name of the files to ``open()``
     :param default: `dict` or `.Configuration` to use when a file does not
         exist (default is to raise a `FileNotFoundError`)
     :param missing: policy to be used when a configured key is missing, either
         as a `.Missing` instance or a default value
     :return: a `.Configuration` instance providing values from *fnames*
     :rtype: `.Configuration`
     """
-    def readf(fname):
-        if default is _NoDefault or path.exists(fname):
+    def readf(fname: str) -> typing.Mapping[str, typing.Any]:
+        if default is NoDefault or path.exists(fname):
             # (attempt to) open fname if it exists OR if we're expected to raise an error on a missing file
             with open(fname, 'r') as fp:
                 # default to empty dict, yaml.safe_load will return None for an empty document
                 return yaml.safe_load(fp.read()) or {}
         else:
             return default
 
     return Configuration(*(readf(path.expanduser(fname)) for fname in fnames), missing=missing)
 
 
-def loads(*strings, missing=Missing.silent):
+def loads(*strings: str, missing: typing.Any = Missing.silent) -> Configuration:
     """
     Read a `.Configuration` instance from strings.
 
     :param strings: configuration contents
     :param missing: policy to be used when a configured key is missing, either
         as a `.Missing` instance or a default value
     :return: a `.Configuration` instance providing values from *strings*
     :rtype: `.Configuration`
     """
     return Configuration(*(yaml.safe_load(string) for string in strings), missing=missing)
 
 
-def load_name(*names, load_order=DEFAULT_LOAD_ORDER, extension='yaml', missing=Missing.silent):
+def load_name(*names: str,
+              load_order: typing.Iterable[typing.Union[str, typing.Callable]] = DEFAULT_LOAD_ORDER,
+              extension: str = 'yaml',
+              missing: typing.Any = Missing.silent) -> Configuration:
     """
     Read a `.Configuration` instance by name, trying to read from files in
     increasing significance. The default load order is `.system`, `.user`,
     `.application`, `.environment`.
 
     Multiple names are combined with multiple loaders using names as the 'inner
     loop / selector', loading ``/etc/name1.yaml`` and ``/etc/name2.yaml``
@@ -284,15 +286,15 @@
         increasing order of significance
     :param extension: file extension to be used
     :param missing: policy to be used when a configured key is missing, either
         as a `.Missing` instance or a default value
     :return: a `.Configuration` instances providing values loaded from *names*
         in *load_order* ordering
     """
-    def generate_sources():
+    def generate_sources() -> typing.Iterable[typing.Mapping[str, typing.Any]]:
         # argument order for product matters, for names "foo" and "bar":
         # /etc/foo.yaml before /etc/bar.yaml, but both of them before ~/.foo.yaml and ~/.bar.yaml
         for source, name in product(load_order, names):
             if callable(source):
                 yield source(name, extension)
             else:
                 # expand user to turn ~/.name.yaml into /home/user/.name.yaml
```

## confidence/models.py

```diff
@@ -1,42 +1,44 @@
 from collections.abc import Mapping, Sequence
 from enum import Enum
 from itertools import chain
 import re
+import typing
 
 from confidence.exceptions import ConfiguredReferenceError, NotConfiguredError
 from confidence.utils import _Conflict, _merge, _split_keys
 
 
 class Missing(Enum):
     silent = 'silent'  #: return `.NotConfigured` for unconfigured keys, avoiding errors
     error = 'error'  #: raise an `AttributeError` for unconfigured keys
 
 
-class _NoDefault:
-    def __repr__(self):
-        return '(raise)'
-
-    __str__ = __repr__
-
-
-# overwrite _NoDefault as an instance of itself
-_NoDefault = _NoDefault()
+# define a sentinel value to indicate there is no default value specified (None would be a valid default value)
+# as this is used as an argument default to indicate that an error should be raised when a value is not found, make
+# sure that the repr-value of NoDefault shows up as '(raise)' in documentation
+NoDefault = type('NoDefault', (object,), {
+    '__repr__': lambda self: '(raise)',
+    '__str__': lambda self: '(raise)'
+})()  # create instance of that new type to assign to NoDefault
 
 
 class Configuration(Mapping):
     """
     A collection of configured values, retrievable as either `dict`-like items
     or attributes.
     """
 
     # match a reference as ${key.to.be.resolved}
     _reference_pattern = re.compile(r'\${(?P<path>[^${}]+?)}')
 
-    def __init__(self, *sources, separator='.', missing=Missing.silent):
+    def __init__(self,
+                 *sources: typing.Mapping[str, typing.Any],
+                 separator: str = '.',
+                 missing: typing.Any = Missing.silent):
         """
         Create a new `.Configuration`, based on one or multiple source mappings.
 
         :param sources: source mappings to base this `.Configuration` on,
             ordered from least to most significant
         :param separator: the character(s) to use as the separator between keys
         :param missing: policy to be used when a configured key is missing,
@@ -44,37 +46,37 @@
         """
         self._separator = separator
         self._missing = missing
         self._root = self
 
         if isinstance(self._missing, Missing):
             self._missing = {Missing.silent: NotConfigured,
-                             Missing.error: _NoDefault}[missing]
+                             Missing.error: NoDefault}[missing]
 
-        self._source = {}
+        self._source: typing.MutableMapping[str, typing.Any] = {}
         for source in sources:
             if source:
                 while isinstance(source, Configuration):
                     # _merge will walk source.items(), using source.get(), avoid resolving references now
                     source = source._source
 
                 # merge values from source into self._source, overwriting any corresponding keys
                 _merge(self._source,
                        _split_keys(source, separator=self._separator, colliding=_COLLIDING_KEYS),
                        conflict=_Conflict.overwrite)
 
-    def _wrap(self, value):
+    def _wrap(self, value: typing.MutableMapping[str, typing.Any]) -> 'Configuration':
         # create an instance of our current type, copying 'configured' properties / policies
         namespace = type(self)(separator=self._separator, missing=self._missing)
         namespace._source = value
         # carry the root object from namespace to namespace, references are always resolved from root
         namespace._root = self._root
         return namespace
 
-    def _resolve(self, value):
+    def _resolve(self, value: str) -> typing.Any:
         match = self._reference_pattern.search(value)
         references = set()
         try:
             while match:
                 path = match.group('path')
                 if path in references:
                     raise ConfiguredReferenceError(f'cannot resolve recursive reference {path}', key=path)
@@ -104,17 +106,22 @@
                 if isinstance(value, str):
                     match = self._reference_pattern.search(value)
                 else:
                     match = None
 
             return value
         except NotConfiguredError as e:
-            raise ConfiguredReferenceError(f'unable to resolve referenced key {match.group("path")}', key=e.key) from e
+            missing_key = match.group('path')  # type: ignore
+            raise ConfiguredReferenceError(f'unable to resolve referenced key {missing_key}', key=e.key) from e
 
-    def get(self, path, default=_NoDefault, as_type=None, resolve_references=True):
+    def get(self,
+            path: str,
+            default: typing.Any = NoDefault,
+            as_type: typing.Optional[typing.Callable] = None,
+            resolve_references: bool = True) -> typing.Any:
         """
         Gets a value for the specified path.
 
         :param path: the configuration key to fetch a value for, steps
             separated by the separator supplied to the constructor (default
             ``.``)
         :param default: a value to return if no value is found for the
@@ -151,21 +158,21 @@
             else:
                 # a 'simple' value, nothing to do
                 return value
         except ConfiguredReferenceError:
             # also a KeyError, but this one should bubble to caller
             raise
         except KeyError as e:
-            if default is not _NoDefault:
+            if default is not NoDefault:
                 return default
             else:
                 missing_key = self._separator.join(steps_taken)
                 raise NotConfiguredError(f'no configuration for key {missing_key}', key=missing_key) from e
 
-    def __getattr__(self, attr):
+    def __getattr__(self, attr: str) -> typing.Any:
         """
         Gets a 'single step value', as either a configured value or a
         namespace-like object in the form of a `.Configuration` instance. An
         unconfigured value will return `.NotConfigured`, a 'silent' sentinel
         value.
 
         :param attr: the 'step' (key, attribute, …) to take
@@ -173,136 +180,136 @@
             instance (`.NotConfigured` in case of an unconfigured 'step')
         """
         try:
             return self.get(attr, default=self._missing)
         except NotConfiguredError as e:
             raise AttributeError(attr) from e
 
-    def __setattr__(self, name, value):
+    def __setattr__(self, name: str, value: typing.Any) -> None:
         """
         Attempts to set a named attribute to this `.Configuration` instance.
         Only protected / private style attribute names are accepted, anything
         not starting with an underscore will raise an `AttributeError`.
 
         :param name: name of the attribute to set
         :param value: value to be associated to *name*
         """
         if name.startswith('_'):
             super().__setattr__(name, value)
         else:
             raise AttributeError(f'assignment not supported ({name})')
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._source)
 
-    def __getitem__(self, item):
+    def __getitem__(self, item: str) -> typing.Any:
         return self.get(item)
 
-    def __iter__(self):
+    def __iter__(self) -> typing.Iterator[str]:
         return iter(self._source)
 
-    def __dir__(self):
+    def __dir__(self) -> typing.Iterable[str]:
         return sorted(set(chain(super().__dir__(), self.keys())))
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         # even though keys should always be str, no need to crash on repr() in edge cases
         keys = ', '.join(str(key) for key in self.keys())
         return f'<{self.__class__.__module__}.{self.__class__.__name__} keys={{{keys}}}>'
 
-    def __getstate__(self):
+    def __getstate__(self) -> typing.Dict[str, typing.Any]:
         state = self.__dict__.copy()
 
         # NB: both 'magic missing values' are required to be the same specific instances at runtime, encode them as
         #     their corresponding Missing instances for pickling (but leave them as-is otherwise)
         if state['_missing'] is NotConfigured:
             state['_missing'] = Missing.silent
-        elif state['_missing'] is _NoDefault:
+        elif state['_missing'] is NoDefault:
             state['_missing'] = Missing.error
 
         return state
 
-    def __setstate__(self, state):
+    def __setstate__(self, state: typing.Dict[str, typing.Any]) -> None:
         self.__dict__ = state
 
         if isinstance(self._missing, Missing):
             # reverse the Missing encoding done in __getstate__
             self._missing = {Missing.silent: NotConfigured,
-                             Missing.error: _NoDefault}[self._missing]
-
-
-class NotConfigured(Configuration):
-    """
-    Sentinel value to signal there is no value for a requested key.
-    """
-    def __bool__(self):
-        return False
-
-    def __repr__(self):
-        return '(not configured)'
-
-    __str__ = __repr__
+                             Missing.error: NoDefault}[self._missing]
 
 
-# overwrite NotConfigured as an instance of itself, a Configuration instance without any values
+# define NotConfigured as a class first (using type() to keep the type checker happy)
+NotConfigured = type('NotConfigured', (Configuration,), {
+    '__bool__': lambda self: False,
+    '__repr__': lambda self: '(not configured)',
+    '__str__': lambda self: '(not configured)',
+    '__doc__': 'Sentinel value to signal there is no value for a requested key.'
+})
+# overwrite the NotConfigured type as an instance of itself, serving as a sentinel value that some requested key was
+# not configured, while still acting like a Configuration object
 NotConfigured = NotConfigured()
-# NB: NotConfigured._missing refers to the NotConfigured *class* at this point, fix this after the name override
-NotConfigured._missing = NotConfigured
+# NotConfigured._missing refers to the NotConfigured *type* at this point, overwrite it with the sentinel value
+NotConfigured._missing = NotConfigured  # type: ignore
 
 
+# collect the names of all defined members of a Configuration instance to be used to warn for configured keys that
+# collide with defined members (making them unavailable through attribute access)
 _COLLIDING_KEYS = frozenset(dir(Configuration()))
 
 
 class ConfigurationSequence(Sequence):
     """
     A sequence of configured values, retrievable as if this were a `list`.
     """
 
-    def __init__(self, source, factory):
+    def __init__(self,
+                 source: typing.Sequence,
+                 factory: typing.Callable):
         """
         Create a new `._ConfigurationSequence`, based on a single source
         sequence, pointing back to 'root' `Configuration` through *factory*.
 
         :param source: a `Sequence` to wrap
         :param factory: a `callable` to wrap `Mapping` values with
         """
         self._source = source
         self._factory = factory
 
-    def __getitem__(self, item):
+    def __getitem__(self, item: typing.Union[int, slice]) -> typing.Any:
         # retrieve value of interest (NB: item can be a slice, but we'll let _source take care of that)
         value = self._source[item]
         if isinstance(value, Mapping):
             # invoke the factory function (provided by Configuration) for a Mapping value
             return self._factory(value)
         if isinstance(value, Sequence) and not isinstance(value, (str, bytes)):
             # wrap a sequence value with an 'instance of self'
             return type(self)(value, self._factory)
         else:
             # a 'simple' value, nothing to do
             return value
 
-    def __len__(self):
+    def __len__(self) -> int:
         # emulating a simple sequence, delegate length to _source
         return len(self._source)
 
-    def __add__(self, other):
+    def __add__(self, other: typing.Sequence[typing.Any]) -> 'ConfigurationSequence':
         if not isinstance(other, Sequence) or isinstance(other, (str, bytes)):
             # incompatible types, let Python resolve an action for this, like calling other.__radd__ or raising a
             # TypeError
             return NotImplemented
 
         # left-hand operand is self, expect return value to be the same as left-hand operand
         # create a new sequence with extended source, assuming self's type will retain the 'magic'
         return type(self)(list(self._source) + list(other), factory=self._factory)
 
-    def __radd__(self, other):
+    def __radd__(self, other: typing.Sequence) -> typing.Sequence:
         if not isinstance(other, Sequence) or isinstance(other, (str, bytes)):
             # incompatible types, let Python resolve an action for this
             return NotImplemented
 
         # left-hand operand is other, expect return value to be the same as left-hand operand
         # list(self) ensures all mapping type values in self._source are wrapped by factory, retaining the 'magic'
-        return type(other)(list(other) + list(self))
+        # NB: assumes other's type will have a single-argument __init__ accepting a list
+        return type(other)(list(other) + list(self))  # type: ignore
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         values = ', '.join(repr(value) for value in self)
         return f'<{self.__class__.__module__}.{self.__class__.__name__} [{values}]>'
```

## confidence/utils.py

```diff
@@ -1,20 +1,24 @@
 from collections.abc import Mapping
 from enum import IntEnum
+import typing
 import warnings
 
 from confidence.exceptions import MergeConflictError
 
 
 class _Conflict(IntEnum):
     overwrite = 0
     error = 1
 
 
-def _merge(left, right, path=None, conflict=_Conflict.error):
+def _merge(left: typing.MutableMapping[str, typing.Any],
+           right: typing.Mapping[str, typing.Any],
+           path: typing.Optional[typing.List[str]] = None,
+           conflict: _Conflict = _Conflict.error) -> typing.Mapping[str, typing.Any]:
     """
     Merges values in place from *right* into *left*.
 
     :param left: mapping to merge into
     :param right: mapping to merge from
     :param path: `list` of keys processed before (used for error reporting
         only, should only need to be provided by recursive calls)
@@ -42,30 +46,32 @@
         else:
             # key not yet in left or not considering conflicts, simple addition of right's mapping to left
             left[key] = right[key]
 
     return left
 
 
-def _split_keys(mapping, separator='.', colliding=None):
+def _split_keys(mapping: typing.Mapping[str, typing.Any],
+                separator: str = '.',
+                colliding: typing.Optional[typing.Container] = None) -> typing.Mapping[str, typing.Any]:
     """
     Recursively walks *mapping* to split keys that contain the separator into
     nested mappings.
 
     .. note::
 
         Keys not of type `str` are not supported and will raise errors.
 
     :param mapping: the mapping to process
     :param separator: the character (sequence) to use as the separator between
         keys
     :return: a mapping where keys containing *separator* are split into nested
         mappings
     """
-    result = {}
+    result: typing.MutableMapping[str, typing.Any] = {}
 
     for key, value in mapping.items():
         if isinstance(value, Mapping):
             # recursively split key(s) in value
             value = _split_keys(value, separator)
 
         # reject non-str keys, avoid complicating access patterns
```

## Comparing `confidence-0.8.dist-info/LICENSE` & `confidence-0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `confidence-0.8.dist-info/METADATA` & `confidence-0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confidence
-Version: 0.8
+Version: 0.9
 Summary: Simple module to load and use configuration in a clean, 'pythonic' way.
 Home-page: https://github.com/HolmesNL/confidence/
 Author: Netherlands Forensic Institute
 Author-email: holmesnl@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: configuration
 Platform: UNKNOWN
@@ -122,14 +122,19 @@
 ~~~~
 
 
 
 Changes
 =======
 
+0.9 (2021-02-01)
+----------------
+
+- Add type hints to confidence
+
 0.8 (2020-12-14)
 ----------------
 
 - Add human-readable `repr`s to `Configuration` and `ConfigurationSequence`
 - Make `ConfigurationSequence` more list-like by enabling addition operator (`configured_sequence + [1, 2, 3]` or `(1, 2, 3) + configured_sequence`)
 
 0.7 (2020-07-10)
```

## Comparing `confidence-0.8.dist-info/RECORD` & `confidence-0.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 confidence/__init__.py,sha256=kskxLSsW9HMNHemSp5uStfLtKl_skL37NLY4hUyr6FU,533
-confidence/exceptions.py,sha256=RmP1seYwVExmYH0QBYBqms9755q4unp_CG_60GBsW98,781
-confidence/io.py,sha256=33XJuQPsKGMEzTE6Hjvg006IWEwt1mjAGJkkSBGeDKk,11862
-confidence/models.py,sha256=kOIUgSByTno58fjB467gBHqeW3rT1Zea0IDhfnzRmJQ,12584
-confidence/utils.py,sha256=PgQJMovDHrbniCLatlw8PVH9l88QBjXizrvcwFhV81E,3456
-confidence-0.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-confidence-0.8.dist-info/METADATA,sha256=Mi-5a06i9yd61ajZ6dnEE4PKOTsUvNmDaNet12P1nC8,6749
-confidence-0.8.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
-confidence-0.8.dist-info/top_level.txt,sha256=PKVnVBfMkyaVb35_Q2VEY7iCL6-v-d5oopNbPbBRF7Q,11
-confidence-0.8.dist-info/RECORD,,
+confidence/exceptions.py,sha256=v4YBSG6B7TWUGs_E_7yvt092l-pQO20eqo9WdJm5Em0,848
+confidence/io.py,sha256=JjoAP4rWu714ojCx5rBhf6WiwGMQoANY7sTyeBIMuXE,12503
+confidence/models.py,sha256=80EYoEbVS2xtZNVE9Ynhy217LHkKg4KPiwotIjGscd0,14243
+confidence/utils.py,sha256=4zYBbvUiugGGVnKZxhz8KBc-bqZt9jMEDS5Ac7S4de8,3845
+confidence-0.9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+confidence-0.9.dist-info/METADATA,sha256=UeRj0BwI3i3yAXz1OmyiWBR-gdnsb6nPVY5-YNB2cK4,6816
+confidence-0.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+confidence-0.9.dist-info/top_level.txt,sha256=PKVnVBfMkyaVb35_Q2VEY7iCL6-v-d5oopNbPbBRF7Q,11
+confidence-0.9.dist-info/RECORD,,
```

