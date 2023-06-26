# Comparing `tmp/graphene_protector-0.9.0.tar.gz` & `tmp/graphene_protector-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_protector-0.9.0.tar", max compression
+gzip compressed data, was "graphene_protector-0.9.1.tar", max compression
```

## Comparing `graphene_protector-0.9.0.tar` & `graphene_protector-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1060 2021-01-06 13:08:15.384908 graphene_protector-0.9.0/LICENSE
--rw-r--r--   0        0        0     5201 2023-01-24 08:30:45.728808 graphene_protector-0.9.0/README.md
--rw-r--r--   0        0        0       80 2023-01-24 07:51:26.443477 graphene_protector-0.9.0/graphene_protector/__init__.py
--rw-r--r--   0        0        0    13331 2023-01-24 08:32:58.288308 graphene_protector-0.9.0/graphene_protector/base.py
--rw-r--r--   0        0        0      903 2022-03-04 07:09:36.789424 graphene_protector-0.9.0/graphene_protector/django/base.py
--rw-r--r--   0        0        0      108 2022-03-04 12:07:02.200842 graphene_protector-0.9.0/graphene_protector/django/graphene.py
--rw-r--r--   0        0        0      113 2022-03-04 14:04:04.413879 graphene_protector-0.9.0/graphene_protector/django/strawberry.py
--rw-r--r--   0        0        0      263 2021-12-15 21:10:53.121887 graphene_protector-0.9.0/graphene_protector/graphene.py
--rw-r--r--   0        0        0      989 2023-01-24 08:32:04.578518 graphene_protector-0.9.0/graphene_protector/misc.py
--rw-r--r--   0        0        0     1695 2022-03-04 22:22:27.316624 graphene_protector-0.9.0/graphene_protector/strawberry.py
--rw-r--r--   0        0        0     1406 2023-01-24 08:40:24.225195 graphene_protector-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     6346 1970-01-01 00:00:00.000000 graphene_protector-0.9.0/setup.py
--rw-r--r--   0        0        0     6474 1970-01-01 00:00:00.000000 graphene_protector-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2021-01-06 13:08:15.384908 graphene_protector-0.9.1/LICENSE
+-rw-r--r--   0        0        0     5201 2023-01-26 08:54:32.089561 graphene_protector-0.9.1/README.md
+-rw-r--r--   0        0        0       80 2023-01-24 07:51:26.443477 graphene_protector-0.9.1/graphene_protector/__init__.py
+-rw-r--r--   0        0        0    13667 2023-01-26 08:57:09.374627 graphene_protector-0.9.1/graphene_protector/base.py
+-rw-r--r--   0        0        0      903 2023-01-26 08:54:32.096228 graphene_protector-0.9.1/graphene_protector/django/base.py
+-rw-r--r--   0        0        0      108 2022-03-04 12:07:02.200842 graphene_protector-0.9.1/graphene_protector/django/graphene.py
+-rw-r--r--   0        0        0      113 2022-03-04 14:04:04.413879 graphene_protector-0.9.1/graphene_protector/django/strawberry.py
+-rw-r--r--   0        0        0      263 2023-01-26 08:54:32.096228 graphene_protector-0.9.1/graphene_protector/graphene.py
+-rw-r--r--   0        0        0      989 2023-01-26 08:54:32.096228 graphene_protector-0.9.1/graphene_protector/misc.py
+-rw-r--r--   0        0        0     1695 2023-01-26 08:54:32.096228 graphene_protector-0.9.1/graphene_protector/strawberry.py
+-rw-r--r--   0        0        0     1406 2023-01-26 08:59:20.146962 graphene_protector-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6346 1970-01-01 00:00:00.000000 graphene_protector-0.9.1/setup.py
+-rw-r--r--   0        0        0     6474 1970-01-01 00:00:00.000000 graphene_protector-0.9.1/PKG-INFO
```

### Comparing `graphene_protector-0.9.0/LICENSE` & `graphene_protector-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_protector-0.9.0/README.md` & `graphene_protector-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `graphene_protector-0.9.0/graphene_protector/base.py` & `graphene_protector-0.9.1/graphene_protector/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 from dataclasses import fields, replace
 from functools import wraps
 from typing import Callable, List, Tuple
+from graphql import GraphQLInterfaceType, GraphQLObjectType, GraphQLUnionType
 
 from graphql.error import GraphQLError
 from graphql.execution import ExecutionResult
 from graphql.language import (
     DefinitionNode,
     FragmentSpreadNode,
     InlineFragmentNode,
@@ -18,16 +19,16 @@
 
 from .misc import (
     DEFAULT_LIMITS,
     MISSING,
     MISSING_LIMITS,
     ComplexityLimitReached,
     DepthLimitReached,
-    Limits,
     SelectionsLimitReached,
+    Limits,
 )
 
 
 def follow_of_type(field: GraphQLType) -> GraphQLType:
     while hasattr(field, "of_type"):
         field = getattr(field, "of_type")
     return field
@@ -81,15 +82,15 @@
 
 
 def check_resource_usage(
     schema,
     node: Node,
     validation_context: ValidationContext,
     limits: Limits,
-    on_error: Callable[[str, Node], None],
+    on_error: Callable[[GraphQLError], None],
     auto_snakecase=False,
     get_limits_for_field=limits_for_field,
     level_depth=0,
     level_complexity=0,
     _seen_limits=None,
 ) -> Tuple[int, int, int]:
     if _seen_limits is None:
@@ -116,19 +117,20 @@
         if fieldname.startswith("__"):
             continue
         if auto_snakecase and not hasattr(schema, fieldname):
             fieldname = to_snake_case(fieldname)
         if isinstance(field, FragmentSpreadNode):
             field = validation_context.getFragment(field.name.value)
 
-        # union
-        if hasattr(field, "types"):
+        if isinstance(field, (GraphQLUnionType, GraphQLInterfaceType)):
             merged_limits = limits
             local_selections = 0
-            for field_type in field.types:
+            for field_type in validation_context.schema.get_possible_types(
+                field
+            ):
                 (
                     new_depth,
                     new_depth_complexity,
                     local2_selections,
                 ) = check_resource_usage(
                     follow_of_type(field_type),
                     field,
@@ -166,30 +168,35 @@
             # because we have depth for that
             selections += local_selections
         elif field.selection_set:
             try:
                 schema_field = getattr(schema, fieldname)
             except AttributeError:
                 schema_field = schema
-                if hasattr(schema_field, "fields"):
-                    schema_field = follow_of_type(
-                        schema_field.fields[field.name.value]
+
+                # handle Fragment Spread nodes
+                if isinstance(schema_field, FragmentSpreadNode):
+                    schema_field = validation_context.getFragment(
+                        schema_field.name.value
                     )
             merged_limits, sub_limits = get_limits_for_field(
                 schema_field,
                 limits,
                 parent=schema,
                 fieldname=fieldname,
             )
             allow_reset = True
             if id(sub_limits) in _seen_limits:
                 allow_reset = False
             else:
                 _seen_limits.add(id(sub_limits))
-            if hasattr(schema_field, "types"):
+            if isinstance(
+                schema_field,
+                (GraphQLUnionType, GraphQLInterfaceType, GraphQLObjectType),
+            ):
                 sub_field_type = schema_field
             else:
                 sub_field_type = follow_of_type(schema_field.type)
             (
                 new_depth,
                 new_depth_complexity,
                 local_selections,
```

### Comparing `graphene_protector-0.9.0/graphene_protector/django/base.py` & `graphene_protector-0.9.1/graphene_protector/django/base.py`

 * *Files identical despite different names*

### Comparing `graphene_protector-0.9.0/graphene_protector/misc.py` & `graphene_protector-0.9.1/graphene_protector/misc.py`

 * *Files identical despite different names*

### Comparing `graphene_protector-0.9.0/graphene_protector/strawberry.py` & `graphene_protector-0.9.1/graphene_protector/strawberry.py`

 * *Files identical despite different names*

### Comparing `graphene_protector-0.9.0/pyproject.toml` & `graphene_protector-0.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphene-protector"
-version = "0.9.0"
+version = "0.9.1"
 description = "Protects graphene, graphql or strawberry against malicious queries"
 authors = ["alex <devkral@web.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/devkral/graphene-protector"
 keywords=[
     "graphql",
```

### Comparing `graphene_protector-0.9.0/setup.py` & `graphene_protector-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {'optional': ['graphene>=3',
               'graphene-django>=3',
               'strawberry-graphql>=0.92',
               'strawberry-graphql-django']}
 
 setup_kwargs = {
     'name': 'graphene-protector',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Protects graphene, graphql or strawberry against malicious queries',
     'long_description': '# What does this project solve?\n\nIt provides protection against malicious grapqhl requests (resource exhaustion).\nDespite its name it can be used with graphql (pure), graphene, strawberry.\nIt is implemented via a custom ValidationRule,\nsupports error reporting and early bail out strategies as well as limits for single fields\n\n# Installation\n\n```sh\npip install graphene-protector\n```\n\n# Integration\n\n## Django\n\nThis adds to django the following setting:\n\n-   GRAPHENE_PROTECTOR_DEPTH_LIMIT: max depth\n-   GRAPHENE_PROTECTOR_SELECTIONS_LIMIT: max selections\n-   GRAPHENE_PROTECTOR_COMPLEXITY_LIMIT: max (depth \\* selections)\n\nIntegrate with:\n\ngraphene:\n\n```python 3\n# schema.py\n# replace normal Schema import with:\nfrom graphene_protector.django.graphene import Schema\nschema = Schema(query=Query, mutation=Mutation)\n```\n\nand add in django settings to GRAPHENE\n\n```python 3\n\nGRAPHENE = {\n    ...\n    "SCHEMA": "path.to.schema",\n}\n```\n\nor strawberry:\n\n```python 3\n# schema.py\n# replace normal Schema import with:\nfrom graphene_protector.django.strawberry import Schema\nschema = Schema(query=Query, mutation=Mutation)\n```\n\nmanual way (note: import from django for including defaults from settings)\n\n```python 3\nfrom graphene_protector.django.graphene import Schema\n# or\n# from graphene_protector.django.strawberry import Schema\nschema = Schema(query=Query)\nresult = schema.execute(query_string)\n```\n\nmanual way with custom default Limits\n\n```python 3\nfrom graphene_protector import Limits\nfrom graphene_protector.django.graphene import Schema\n# or\n# from graphene_protector.django.strawberry import Schema\nschema = graphene.Schema(query=Query, limits=Limits(complexity=None))\nresult = schema.execute(\n    query_string\n)\n\n```\n\n## Graphene & Strawberry\n\nlimits keyword with Limits object is supported.\n\n```python 3\nfrom graphene_protector import Limits\nfrom graphene_protector.graphene import Schema\n# or\n# from graphene_protector.strawberry import Schema\nschema = Schema(query=Query, limits=Limits(depth=20, selections=None, complexity=100))\nresult = schema.execute(query_string)\n```\n\n## pure graphql\n\n```python 3\n\nfrom graphene_protector import LimitsValidationRule\nfrom graphql.type.schema import Schema\nschema = Schema(\n    query=Query,\n)\nquery_ast = parse("{ hello }")\nself.assertFalse(validate(schema, query_ast, [LimitsValidationRule]))\n\n```\n\nor with custom defaults\n\n```python 3\n\nfrom graphene_protector import Limits, LimitsValidationRule\nfrom graphql.type.schema import Schema\n\nclass CustomLimitsValidationRule(LimitsValidationRule):\n    default_limits = Limits(depth=20, selections=None, complexity=100)\n\nschema = Schema(\n    query=Query,\n)\nquery_ast = parse("{ hello }")\nself.assertFalse(validate(schema, query_ast, [LimitsValidationRule]))\n\n```\n\nstrawberry extension variant\n\n```python 3\nfrom graphene_protector import Limits\nfrom graphene_protector.strawberry import CustomGrapheneProtector\nfrom strawberry import Schema\nschema = Schema(query=Query, extensions=[CustomGrapheneProtector(Limits(depth=20, selections=None, complexity=100))])\nresult = schema.execute(query_string)\n```\n\nor with custom defaults via Mixin\n\n```python 3\n\nfrom graphene_protector import Limits, SchemaMixin, LimitsValidationRule\nfrom graphql.type.schema import Schema\n\nclass CustomSchema(SchemaMixin, Schema):\n    default_limits = Limits(depth=20, selections=None, complexity=100)\n\nschema = CustomSchema(\n    query=Query,\n)\nquery_ast = parse("{ hello }")\nself.assertFalse(validate(schema, query_ast, [LimitsValidationRule]))\n\n```\n\nstrawberry extension variant with mixin\n\n```python 3\nfrom graphene_protector import Limits, SchemaMixin\nfrom graphene_protector.strawberry import CustomGrapheneProtector\nfrom strawberry import Schema\n\nclass CustomSchema(SchemaMixin, Schema):\n    default_limits = Limits(depth=20, selections=None, complexity=100)\n\nschema = Schema(query=Query, extensions=[CustomGrapheneProtector()])\nresult = schema.execute(query_string)\n```\n\n## Limits\n\nA Limits object has following attributes:\n\n-   depth: max depth (default: 20, None disables feature)\n-   selections: max selections (default: None, None disables feature)\n-   complexity: max (depth subtree \\* selections subtree) (default: 100, None disables feature)\n\nthey overwrite django settings if specified.\n\n## decorating single fields\n\nSometimes single fields should have different limits:\n\n```python\n    person1 = Limits(depth=10)(graphene.Field(Person))\n```\n\nLimits are inherited for unspecified parameters\n\n## one-time disable limit checks\n\nto disable checks for one operation use check_limits=False (works for:\nexecute, execute_async (if available), subscribe (if available)):\n\n```python 3\nfrom graphene_protector import Limits\nfrom graphene_protector.graphene import Schema\nschema = Schema(query=Query, limits=Limits(depth=20, selections=None, complexity=100))\nresult = schema.execute(query_string, check_limits=False)\n```\n\n# Development\n\nI am open for new ideas.\nIf you want some new or better algorithms integrated just make a PR\n\n# related projects:\n\n-   secure-graphene: lacks django integration, some features and has a not so easy findable name.\n    But I accept: it is the "not invented here"-syndrome\n\n# TODO\n\n-   test mutations\n',
     'author': 'alex',
     'author_email': 'devkral@web.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/devkral/graphene-protector',
```

### Comparing `graphene_protector-0.9.0/PKG-INFO` & `graphene_protector-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-protector
-Version: 0.9.0
+Version: 0.9.1
 Summary: Protects graphene, graphql or strawberry against malicious queries
 Home-page: https://github.com/devkral/graphene-protector
 License: MIT
 Keywords: graphql,strawberry,extension
 Author: alex
 Author-email: devkral@web.de
 Requires-Python: >=3.8,<4
```

