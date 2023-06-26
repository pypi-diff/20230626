# Comparing `tmp/qtgql-0.120.1.tar.gz` & `tmp/qtgql-0.120.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.120.1.tar", max compression
+gzip compressed data, was "qtgql-0.120.2.tar", max compression
```

## Comparing `qtgql-0.120.1.tar` & `qtgql-0.120.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1064 2023-06-25 13:18:59.814578 qtgql-0.120.1/LICENSE
--rw-r--r--   0        0        0     1805 2023-06-25 13:18:59.814578 qtgql-0.120.1/README.md
--rw-r--r--   0        0        0     4428 2023-06-25 13:19:17.118449 qtgql-0.120.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     1919 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1548 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3105 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1179 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3226 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     4207 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    13536 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0      749 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0        0 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4164 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0      445 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1527 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     3059 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     1187 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0     2182 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     3223 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     5130 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3482 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    16797 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1151 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 qtgql-0.120.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-26 09:33:31.439471 qtgql-0.120.2/LICENSE
+-rw-r--r--   0        0        0     1805 2023-06-26 09:33:31.439471 qtgql-0.120.2/README.md
+-rw-r--r--   0        0        0     4428 2023-06-26 09:33:57.552766 qtgql-0.120.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     1919 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1548 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3105 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1179 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3226 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     4207 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    13536 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0      749 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4164 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0      445 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1527 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     3059 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     1187 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0     2446 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     4741 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     5196 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3482 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    16797 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1151 2023-06-26 09:33:31.455472 qtgql-0.120.2/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 qtgql-0.120.2/PKG-INFO
```

### Comparing `qtgql-0.120.1/LICENSE` & `qtgql-0.120.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/README.md` & `qtgql-0.120.2/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/pyproject.toml` & `qtgql-0.120.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.120.1"
+version = "0.120.2"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.120.1/qtgqlcodegen/cli.py` & `qtgql-0.120.2/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/config.py` & `qtgql-0.120.2/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/core/cppref.py` & `qtgql-0.120.2/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.120.2/qtgqlcodegen/core/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/core/template.py` & `qtgql-0.120.2/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/generator.py` & `qtgql-0.120.2/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/operation/definitions.py` & `qtgql-0.120.2/qtgqlcodegen/operation/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.120.2/qtgqlcodegen/operation/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/operation/template.py` & `qtgql-0.120.2/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/schema/definitions.py` & `qtgql-0.120.2/qtgqlcodegen/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.120.2/qtgqlcodegen/schema/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/schema/template.py` & `qtgql-0.120.2/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.120.2/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.120.2/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.120.2/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.120.2/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+{%- from "macros/deserialize_concrete_field.jinja.hpp" import  deserialize_concrete_field -%}
 {% macro update_concrete_field(proxy_field,f_concrete, fset_name, private_name, operation_pointer="operation") -%}
 {% set current -%}
 {% if not proxy_field.is_root and proxy_field.variable_uses  -%}
 inst->👉private_name👈.at(👉proxy_field.build_variables_tuple_for_field_arguments👈)
 {% else -%}
 inst->👉private_name👈
 {% endif -%}
@@ -34,14 +35,17 @@
 if (👉current👈 && 👉current👈->get_id() == 👉f_concrete.name👈_data.value("id").toString()){
 👉proxy_field.type.updater_name👈(👉current👈, 👉f_concrete.name👈_data,  👉operation_pointer👈);
 }
 else{
 inst->👉fset_name👈(👉proxy_field.type.deserializer_name👈(data.value("👉f_concrete.name👈").toObject(), 👉operation_pointer👈) 👉 setter_end 👈);
 }
 {% endif %}
+{% elif proxy_field.type.is_model %}
+{% set setter %}inst->👉 proxy_field.concrete.setter_name 👈{% endset %}
+👉deserialize_concrete_field(proxy_field, setter)👈
 {% else %}
 throw qtgql::exceptions::NotImplementedError({"👉proxy_field.type.__class__.__name__👈 is not supporting updates ATM"});
 {% endif %}
 }
 {% if proxy_field.type.is_optional %}
 else {
 inst->👉fset_name👈({} 👉 setter_end 👈);
```

### Comparing `qtgql-0.120.1/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.120.2/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -38,24 +38,24 @@
 
 {# members #}
 {% if context.debug -%}
 public: // WARNING: members are public because you have debug=True in your config file.
 {% else %}
 protected:
 {% endif %}
-{% if t.concrete.is_root %}
+{% if t.concrete.is_root %} {# // root types are singletons, no need for shared ptr -#}
 👉context.schema_ns👈::👉 t.concrete.name 👈 * m_inst;
 {% else %}
 const std::shared_ptr<👉context.schema_ns👈::👉 t.concrete.name 👈> m_inst;
 {% endif %}
 {% for ref_field in t.references -%}
 const 👉ref_field.property_type👈 m_👉ref_field.name👈 = {};
 {% endfor %}
 {%- for model_field in t.models -%}
-👉 model_field.property_type 👈 m_👉model_field.name👈;
+👉 model_field.property_type 👈 👉model_field.private_name👈;
 {% endfor %}
 
 public:
 {% if t.concrete.is_root %}
 👉 t.name 👈(👉 context.operation.name 👈 * operation);
 {% else %}
 👉 t.name 👈(👉 context.operation.name 👈 * operation, const std::shared_ptr<👉 t.concrete.name 👈> &inst);
```

### Comparing `qtgql-0.120.1/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.120.2/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/types.py` & `qtgql-0.120.2/qtgqlcodegen/types.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/qtgqlcodegen/utils.py` & `qtgql-0.120.2/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.1/PKG-INFO` & `qtgql-0.120.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.120.1
+Version: 0.120.2
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

