# Comparing `tmp/mypy-zope-0.9.1.tar.gz` & `tmp/mypy-zope-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-zope-0.9.1.tar", last modified: Fri Mar 24 19:20:13 2023, max compression
+gzip compressed data, was "mypy-zope-1.0.0.tar", last modified: Mon Jun 26 18:29:07 2023, max compression
```

## Comparing `mypy-zope-0.9.1.tar` & `mypy-zope-1.0.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-24 19:20:13.418509 mypy-zope-0.9.1/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2831 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/CHANGELOG.md
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1068 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/LICENSE
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      113 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/MANIFEST.in
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     6061 2023-03-24 19:20:13.418509 mypy-zope-0.9.1/PKG-INFO
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     5163 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/README.md
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1214 2023-03-24 19:20:13.418509 mypy-zope-0.9.1/setup.cfg
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       37 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/setup.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-24 19:20:13.410508 mypy-zope-0.9.1/src/
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-24 19:20:13.414508 mypy-zope-0.9.1/src/mypy_zope/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       26 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/mypy_zope/__init__.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    27495 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/mypy_zope/plugin.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-24 19:20:13.414508 mypy-zope-0.9.1/src/mypy_zope.egg-info/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     6061 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/mypy_zope.egg-info/PKG-INFO
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     3075 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/mypy_zope.egg-info/SOURCES.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/mypy_zope.egg-info/dependency_links.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/mypy_zope.egg-info/not-zip-safe
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       82 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/mypy_zope.egg-info/requires.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       21 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/mypy_zope.egg-info/top_level.txt
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-24 19:20:13.414508 mypy-zope-0.9.1/src/zope-stubs/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       30 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/__init__.pyi
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-24 19:20:13.414508 mypy-zope-0.9.1/src/zope-stubs/interface/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1453 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/__init__.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      214 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/_compat.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      128 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/_flatten.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2240 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/_zope_interface_coptimizations.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2832 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/adapter.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      395 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/advice.pyi
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-24 19:20:13.414508 mypy-zope-0.9.1/src/zope-stubs/interface/common/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      126 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/common/__init__.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     3041 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/common/idatetime.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1695 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/common/interfaces.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1901 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/common/mapping.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1743 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/common/sequence.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     3270 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/declarations.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      275 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/document.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      663 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/exceptions.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     3458 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/interface.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     7223 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/interfaces.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     4439 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/registry.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      191 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/ro.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      311 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/interface/verify.pyi
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-24 19:20:13.414508 mypy-zope-0.9.1/src/zope-stubs/schema/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1558 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/schema/__init__.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     4082 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/schema/_bootstrapfields.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     3256 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/schema/_bootstrapinterfaces.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      342 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/schema/_compat.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     3388 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/schema/_field.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      127 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/schema/_messageid.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      467 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/schema/_schema.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      943 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/schema/accessors.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1210 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/schema/fieldproperty.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     5608 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/schema/interfaces.pyi
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2159 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/src/zope-stubs/schema/vocabulary.pyi
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-24 19:20:13.414508 mypy-zope-0.9.1/tests/
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-24 19:20:13.418509 mypy-zope-0.9.1/tests/samples/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1039 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/adaptation.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      454 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/classimplements.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1352 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/classimplements_broken_iface.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      660 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/classimplements_broken_impl.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      462 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/classimplements_wrong.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      361 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/contextmanager.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      672 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/forward_reference_to_implementer.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      550 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/forwardref.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      729 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/impl_inheritance.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      582 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/impl_property.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      884 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/incompatible_signature.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      141 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/innerclass.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1180 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/interface_annotated_attribute.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      540 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/interface_attribute.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      787 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/interface_fieldproperty.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      325 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/interface_getattr.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1217 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/interface_implications.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1122 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/interface_inheritance.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1088 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/interface_mapping.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      464 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/interface_meta.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      178 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/interface_metaclass.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      432 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/interface_self.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      627 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/interface_unknown.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      682 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/interface_unknown_direct.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1060 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/interface_unknown_inherit.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1076 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/multiple_implementer.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      810 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/multiple_inheritance.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      415 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/nested_definitions.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      592 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/no_arg_method.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      530 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/not_fully_implemented.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      191 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/open.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1438 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/overload.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      714 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/overload_readme.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      760 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/parameterized_types.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      541 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/schema_bool.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      608 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/schema_field_outside_inteface.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1309 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/schema_number.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1555 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/schema_text.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      559 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/schema_unknown_field.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      492 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/simple_valid.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      558 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/unknown_interface.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      367 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/samples/unknown_metaclass.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2209 2023-03-24 19:20:13.000000 mypy-zope-0.9.1/tests/test_samples.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-26 18:29:07.759754 mypy-zope-1.0.0/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2902 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/CHANGELOG.md
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1068 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/LICENSE
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      113 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/MANIFEST.in
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     6074 2023-06-26 18:29:07.759754 mypy-zope-1.0.0/PKG-INFO
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     5163 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/README.md
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1227 2023-06-26 18:29:07.759754 mypy-zope-1.0.0/setup.cfg
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       37 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/setup.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-26 18:29:07.751753 mypy-zope-1.0.0/src/
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-26 18:29:07.755753 mypy-zope-1.0.0/src/mypy_zope/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       26 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/mypy_zope/__init__.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    27495 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/mypy_zope/plugin.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-26 18:29:07.755753 mypy-zope-1.0.0/src/mypy_zope.egg-info/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     6074 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/mypy_zope.egg-info/PKG-INFO
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     3075 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/mypy_zope.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/mypy_zope.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/mypy_zope.egg-info/not-zip-safe
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       82 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/mypy_zope.egg-info/requires.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       21 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/mypy_zope.egg-info/top_level.txt
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-26 18:29:07.755753 mypy-zope-1.0.0/src/zope-stubs/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       30 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/__init__.pyi
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-26 18:29:07.755753 mypy-zope-1.0.0/src/zope-stubs/interface/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1453 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/__init__.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      214 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/_compat.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      128 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/_flatten.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2240 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/_zope_interface_coptimizations.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2832 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/adapter.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      395 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/advice.pyi
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-26 18:29:07.755753 mypy-zope-1.0.0/src/zope-stubs/interface/common/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      126 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/common/__init__.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     3041 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/common/idatetime.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1695 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/common/interfaces.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1901 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/common/mapping.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1743 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/common/sequence.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     3270 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/declarations.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      275 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/document.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      663 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/exceptions.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     3458 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/interface.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     7223 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/interfaces.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     4439 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/registry.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      191 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/ro.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      311 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/interface/verify.pyi
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-26 18:29:07.755753 mypy-zope-1.0.0/src/zope-stubs/schema/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1558 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/schema/__init__.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     4082 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/schema/_bootstrapfields.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     3256 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/schema/_bootstrapinterfaces.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      342 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/schema/_compat.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     3388 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/schema/_field.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      127 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/schema/_messageid.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      467 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/schema/_schema.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      943 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/schema/accessors.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1210 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/schema/fieldproperty.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     5608 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/schema/interfaces.pyi
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2159 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/src/zope-stubs/schema/vocabulary.pyi
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-26 18:29:07.755753 mypy-zope-1.0.0/tests/
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-26 18:29:07.759754 mypy-zope-1.0.0/tests/samples/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1039 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/adaptation.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      454 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/classimplements.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1352 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/classimplements_broken_iface.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      660 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/classimplements_broken_impl.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      462 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/classimplements_wrong.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      361 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/contextmanager.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      672 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/forward_reference_to_implementer.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      550 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/forwardref.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      729 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/impl_inheritance.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      582 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/impl_property.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      884 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/incompatible_signature.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      141 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/innerclass.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1180 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/interface_annotated_attribute.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      540 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/interface_attribute.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      787 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/interface_fieldproperty.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      325 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/interface_getattr.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1217 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/interface_implications.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1122 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/interface_inheritance.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1088 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/interface_mapping.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      464 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/interface_meta.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      178 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/interface_metaclass.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      432 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/interface_self.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      627 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/interface_unknown.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      682 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/interface_unknown_direct.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1060 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/interface_unknown_inherit.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1076 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/multiple_implementer.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      810 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/multiple_inheritance.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      415 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/nested_definitions.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      592 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/no_arg_method.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      530 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/not_fully_implemented.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      191 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/open.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1438 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/overload.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      714 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/overload_readme.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      760 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/parameterized_types.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      538 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/schema_bool.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      608 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/schema_field_outside_inteface.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1297 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/schema_number.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1549 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/schema_text.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      559 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/schema_unknown_field.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      492 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/simple_valid.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      558 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/unknown_interface.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      367 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/samples/unknown_metaclass.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2243 2023-06-26 18:29:07.000000 mypy-zope-1.0.0/tests/test_samples.py
```

### Comparing `mypy-zope-0.9.1/CHANGELOG.md` & `mypy-zope-1.0.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## 1.0.0 (2023-06-26)
+------------------
+
+- Support mypy up to 1.5.0
+
+
 0.9.1 (2023-03-24)
 ------------------
 
 - Follow semantic versioning in mypy version pins (#96)
 
 
 0.9.0 (2023-02-10)
```

### Comparing `mypy-zope-0.9.1/LICENSE` & `mypy-zope-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/PKG-INFO` & `mypy-zope-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mypy-zope
-Version: 0.9.1
+Version: 1.0.0
 Summary: Plugin for mypy to support zope interfaces
 Home-page: https://github.com/Shoobx/mypy-zope
 Author: Andrey Lebedev
 Author-email: andrey.lebedev@gmail.com
 Keywords: mypy,zope,interfaces,typing
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mypy-zope-0.9.1/README.md` & `mypy-zope-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/setup.cfg` & `mypy-zope-1.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [metadata]
 name = mypy-zope
-version = 0.9.1
+version = 1.0.0
 author = Andrey Lebedev
 author_email = andrey.lebedev@gmail.com
 url = https://github.com/Shoobx/mypy-zope
 long_description = file: README.md
 long_description_content_type = text/markdown
 description = Plugin for mypy to support zope interfaces
 keywords = mypy, zope, interfaces, typing
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
@@ -24,15 +24,15 @@
 
 [options]
 packages = 
 	mypy_zope
 	zope-stubs
 package_dir = =src
 install_requires = 
-	mypy>=1.0.0,<1.1.0
+	mypy>=1.0.0,<1.5.0
 	zope.interface
 	zope.schema
 include_package_data = True
 zip_safe = False
 
 [options.extras_require]
 test =
```

### Comparing `mypy-zope-0.9.1/src/mypy_zope/plugin.py` & `mypy-zope-1.0.0/src/mypy_zope/plugin.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/mypy_zope.egg-info/PKG-INFO` & `mypy-zope-1.0.0/src/mypy_zope.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mypy-zope
-Version: 0.9.1
+Version: 1.0.0
 Summary: Plugin for mypy to support zope interfaces
 Home-page: https://github.com/Shoobx/mypy-zope
 Author: Andrey Lebedev
 Author-email: andrey.lebedev@gmail.com
 Keywords: mypy,zope,interfaces,typing
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mypy-zope-0.9.1/src/mypy_zope.egg-info/SOURCES.txt` & `mypy-zope-1.0.0/src/mypy_zope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/interface/__init__.pyi` & `mypy-zope-1.0.0/src/zope-stubs/interface/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/interface/_zope_interface_coptimizations.pyi` & `mypy-zope-1.0.0/src/zope-stubs/interface/_zope_interface_coptimizations.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/interface/adapter.pyi` & `mypy-zope-1.0.0/src/zope-stubs/interface/adapter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/interface/common/idatetime.pyi` & `mypy-zope-1.0.0/src/zope-stubs/interface/common/idatetime.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/interface/common/interfaces.pyi` & `mypy-zope-1.0.0/src/zope-stubs/interface/common/interfaces.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/interface/common/mapping.pyi` & `mypy-zope-1.0.0/src/zope-stubs/interface/common/mapping.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/interface/common/sequence.pyi` & `mypy-zope-1.0.0/src/zope-stubs/interface/common/sequence.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/interface/declarations.pyi` & `mypy-zope-1.0.0/src/zope-stubs/interface/declarations.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/interface/exceptions.pyi` & `mypy-zope-1.0.0/src/zope-stubs/interface/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/interface/interface.pyi` & `mypy-zope-1.0.0/src/zope-stubs/interface/interface.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/interface/interfaces.pyi` & `mypy-zope-1.0.0/src/zope-stubs/interface/interfaces.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/interface/registry.pyi` & `mypy-zope-1.0.0/src/zope-stubs/interface/registry.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/schema/__init__.pyi` & `mypy-zope-1.0.0/src/zope-stubs/schema/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/schema/_bootstrapfields.pyi` & `mypy-zope-1.0.0/src/zope-stubs/schema/_bootstrapfields.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/schema/_bootstrapinterfaces.pyi` & `mypy-zope-1.0.0/src/zope-stubs/schema/_bootstrapinterfaces.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/schema/_field.pyi` & `mypy-zope-1.0.0/src/zope-stubs/schema/_field.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/schema/accessors.pyi` & `mypy-zope-1.0.0/src/zope-stubs/schema/accessors.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/schema/fieldproperty.pyi` & `mypy-zope-1.0.0/src/zope-stubs/schema/fieldproperty.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/schema/interfaces.pyi` & `mypy-zope-1.0.0/src/zope-stubs/schema/interfaces.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/src/zope-stubs/schema/vocabulary.pyi` & `mypy-zope-1.0.0/src/zope-stubs/schema/vocabulary.pyi`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/adaptation.py` & `mypy-zope-1.0.0/tests/samples/adaptation.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/classimplements_broken_iface.py` & `mypy-zope-1.0.0/tests/samples/classimplements_broken_iface.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/classimplements_broken_impl.py` & `mypy-zope-1.0.0/tests/samples/classimplements_broken_impl.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/forward_reference_to_implementer.py` & `mypy-zope-1.0.0/tests/samples/forward_reference_to_implementer.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/forwardref.py` & `mypy-zope-1.0.0/tests/samples/forwardref.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/impl_inheritance.py` & `mypy-zope-1.0.0/tests/samples/impl_inheritance.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/impl_property.py` & `mypy-zope-1.0.0/tests/samples/impl_property.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/incompatible_signature.py` & `mypy-zope-1.0.0/tests/samples/incompatible_signature.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/interface_annotated_attribute.py` & `mypy-zope-1.0.0/tests/samples/interface_annotated_attribute.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/interface_attribute.py` & `mypy-zope-1.0.0/tests/samples/interface_attribute.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/interface_fieldproperty.py` & `mypy-zope-1.0.0/tests/samples/interface_fieldproperty.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/interface_implications.py` & `mypy-zope-1.0.0/tests/samples/interface_implications.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/interface_inheritance.py` & `mypy-zope-1.0.0/tests/samples/interface_inheritance.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/interface_mapping.py` & `mypy-zope-1.0.0/tests/samples/interface_mapping.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/interface_unknown.py` & `mypy-zope-1.0.0/tests/samples/interface_unknown.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/interface_unknown_direct.py` & `mypy-zope-1.0.0/tests/samples/interface_unknown_direct.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/interface_unknown_inherit.py` & `mypy-zope-1.0.0/tests/samples/interface_unknown_inherit.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/multiple_implementer.py` & `mypy-zope-1.0.0/tests/samples/multiple_implementer.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/multiple_inheritance.py` & `mypy-zope-1.0.0/tests/samples/multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/no_arg_method.py` & `mypy-zope-1.0.0/tests/samples/no_arg_method.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/not_fully_implemented.py` & `mypy-zope-1.0.0/tests/samples/not_fully_implemented.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/overload.py` & `mypy-zope-1.0.0/tests/samples/overload.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/overload_readme.py` & `mypy-zope-1.0.0/tests/samples/overload_readme.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/parameterized_types.py` & `mypy-zope-1.0.0/tests/samples/parameterized_types.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 class Something(object):
     def hello(self, names: List[int]) -> None:  # Wrong kind of list
         print(f"Hello, {names}")
 
 
 """
 <output>
-parameterized_types.py:15: error: Argument 1 of "Something" is incompatible with "hello" of supertype "ISomething"; supertype defines the argument type as "List[str]"
+parameterized_types.py:15: error: Argument 1 of "Something" is incompatible with "hello" of supertype "ISomething"; supertype defines the argument type as "list[str]"
 parameterized_types.py:15: note: This violates the Liskov substitution principle
 parameterized_types.py:15: note: See https://mypy.readthedocs.io/en/stable/common_issues.html#incompatible-overrides
 </output>
 """
```

### Comparing `mypy-zope-0.9.1/tests/samples/schema_bool.py` & `mypy-zope-1.0.0/tests/samples/schema_bool.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,10 +16,10 @@
     bm.flag = True
 
 if __name__ == '__main__':
     main()
 
 """
 <output>
-schema_bool.py:14: error: Incompatible types in assignment (expression has type "int", variable has type "Optional[bool]")
+schema_bool.py:14: error: Incompatible types in assignment (expression has type "int", variable has type "bool | None")
 </output>
 """
```

### Comparing `mypy-zope-0.9.1/tests/samples/schema_field_outside_inteface.py` & `mypy-zope-1.0.0/tests/samples/schema_field_outside_inteface.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/schema_number.py` & `mypy-zope-1.0.0/tests/samples/schema_number.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,13 +30,13 @@
 
 
 if __name__ == '__main__':
     main()
 
 """
 <output>
-schema_number.py:20: error: Incompatible types in assignment (expression has type "str", variable has type "Optional[complex]")
-schema_number.py:24: error: Incompatible types in assignment (expression has type "complex", variable has type "Optional[float]")
-schema_number.py:27: error: Incompatible types in assignment (expression has type "complex", variable has type "Optional[int]")
-schema_number.py:28: error: Incompatible types in assignment (expression has type "float", variable has type "Optional[int]")
+schema_number.py:20: error: Incompatible types in assignment (expression has type "str", variable has type "complex | None")
+schema_number.py:24: error: Incompatible types in assignment (expression has type "complex", variable has type "float | None")
+schema_number.py:27: error: Incompatible types in assignment (expression has type "complex", variable has type "int | None")
+schema_number.py:28: error: Incompatible types in assignment (expression has type "float", variable has type "int | None")
 </output>
 """
```

### Comparing `mypy-zope-0.9.1/tests/samples/schema_text.py` & `mypy-zope-1.0.0/tests/samples/schema_text.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,13 +36,13 @@
     bm.asciiline = True  # Error, it is a string
 
 if __name__ == '__main__':
     main()
 
 """
 <output>
-schema_text.py:33: error: Incompatible types in assignment (expression has type "int", variable has type "Optional[str]")
+schema_text.py:33: error: Incompatible types in assignment (expression has type "int", variable has type "str | None")
 schema_text.py:34: error: Incompatible types in assignment (expression has type "None", variable has type "str")
 schema_text.py:35: error: Incompatible types in assignment (expression has type "None", variable has type "str")
-schema_text.py:36: error: Incompatible types in assignment (expression has type "bool", variable has type "Optional[str]")
+schema_text.py:36: error: Incompatible types in assignment (expression has type "bool", variable has type "str | None")
 </output>
 """
```

### Comparing `mypy-zope-0.9.1/tests/samples/schema_unknown_field.py` & `mypy-zope-1.0.0/tests/samples/schema_unknown_field.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/samples/unknown_interface.py` & `mypy-zope-1.0.0/tests/samples/unknown_interface.py`

 * *Files identical despite different names*

### Comparing `mypy-zope-0.9.1/tests/test_samples.py` & `mypy-zope-1.0.0/tests/test_samples.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 def test_samples(samplefile, mypy_cache_dir):
     opts = options.Options()
     opts.cache_dir = mypy_cache_dir
     opts.show_traceback = True
     opts.namespace_packages = True
     opts.hide_error_codes = True
     opts.plugins = ['mypy_zope:plugin']
+    opts.python_version = (3, 11)
     # Config file is needed to load plugins, it doesn't not exist and is not
     # supposed to.
     opts.config_file = '    not_existing_config.ini'
 
     try:
         base_dir = os.path.dirname(samplefile)
         source = BuildSource(samplefile,
```

