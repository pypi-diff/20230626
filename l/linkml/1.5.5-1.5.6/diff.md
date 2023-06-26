# Comparing `tmp/linkml-1.5.5.tar.gz` & `tmp/linkml-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml-1.5.5.tar", max compression
+gzip compressed data, was "linkml-1.5.6.tar", max compression
```

## Comparing `linkml-1.5.5.tar` & `linkml-1.5.6.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     6555 2023-05-27 01:45:11.889278 linkml-1.5.5/LICENSE
--rw-r--r--   0        0        0     1369 2023-05-27 01:45:11.889278 linkml-1.5.5/README.md
--rw-r--r--   0        0        0     3227 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/__init__.py
--rw-r--r--   0        0        0      326 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/_version.py
--rw-r--r--   0        0        0    51005 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/PythonGenNotes.md
--rw-r--r--   0        0        0     4158 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/README.md
--rw-r--r--   0        0        0      616 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/common/__init__.py
--rw-r--r--   0        0        0     2040 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/common/type_designators.py
--rw-r--r--   0        0        0     3118 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/csvgen.py
--rw-r--r--   0        0        0     2873 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/class.md.jinja2
--rw-r--r--   0        0        0     2682 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/class_diagram.md.jinja2
--rw-r--r--   0        0        0     1321 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/common_metadata.md.jinja2
--rw-r--r--   0        0        0     1018 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/enum.md.jinja2
--rw-r--r--   0        0        0     1466 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/index.md.jinja2
--rw-r--r--   0        0        0      501 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/index.tex.jinja2
--rw-r--r--   0        0        0       70 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/schema.md.jinja2
--rw-r--r--   0        0        0     2557 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen/slot.md.jinja2
--rw-r--r--   0        0        0     1704 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/docgen/subset.md.jinja2
--rw-r--r--   0        0        0      635 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/docgen/type.md.jinja2
--rw-r--r--   0        0        0    32994 2023-05-27 01:45:11.909278 linkml-1.5.5/linkml/generators/docgen.py
--rw-r--r--   0        0        0     5112 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/dotgen.py
--rw-r--r--   0        0        0    10913 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/erdiagramgen.py
--rw-r--r--   0        0        0     6894 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/excelgen.py
--rw-r--r--   0        0        0     6393 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/golanggen.py
--rw-r--r--   0        0        0     3575 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/golrgen.py
--rw-r--r--   0        0        0     2347 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/graphqlgen.py
--rw-r--r--   0        0        0      444 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/javagen/example_template.java.jinja2
--rw-r--r--   0        0        0     1737 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/javagen/java_record_template.jinja2
--rw-r--r--   0        0        0     5499 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/javagen.py
--rw-r--r--   0        0        0     8821 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/jsonldcontextgen.py
--rw-r--r--   0        0        0     7952 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/jsonldgen.py
--rw-r--r--   0        0        0    21688 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/jsonschemagen.py
--rw-r--r--   0        0        0     3555 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/linkmlgen.py
--rw-r--r--   0        0        0    34422 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/markdowngen.py
--rw-r--r--   0        0        0     6532 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/namespacegen.py
--rw-r--r--   0        0        0     7831 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/oocodegen.py
--rw-r--r--   0        0        0    29182 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/owlgen.py
--rw-r--r--   0        0        0     4911 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/prefixmapgen.py
--rw-r--r--   0        0        0     9811 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/projectgen.py
--rw-r--r--   0        0        0     2443 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/protogen.py
--rw-r--r--   0        0        0    22150 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/pydanticgen.py
--rw-r--r--   0        0        0    50389 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/pythongen.py
--rw-r--r--   0        0        0     2825 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/rdfgen.py
--rw-r--r--   0        0        0     5621 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/shaclgen.py
--rw-r--r--   0        0        0     9547 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/shexgen.py
--rw-r--r--   0        0        0     6632 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sparqlgen.py
--rw-r--r--   0        0        0      166 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2575 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
--rw-r--r--   0        0        0     1625 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
--rw-r--r--   0        0        0     9334 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sqlalchemygen.py
--rw-r--r--   0        0        0    18626 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sqlddlgen.py
--rw-r--r--   0        0        0    11387 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sqltablegen.py
--rw-r--r--   0        0        0     7177 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/sssomgen.py
--rw-r--r--   0        0        0     1788 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/string_template.md
--rw-r--r--   0        0        0     3020 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/summarygen.py
--rw-r--r--   0        0        0     4760 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/terminusdbgen.py
--rw-r--r--   0        0        0     6094 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/typescriptgen.py
--rw-r--r--   0        0        0     1746 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/yamlgen.py
--rw-r--r--   0        0        0    13311 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/generators/yumlgen.py
--rw-r--r--   0        0        0        0 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/__init__.py
--rw-r--r--   0        0        0     4323 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/cli.py
--rw-r--r--   0        0        0      292 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/config/datamodel/.linkmllint.yaml
--rw-r--r--   0        0        0        0 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/config/datamodel/__init__.py
--rw-r--r--   0        0        0    17711 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/config/datamodel/config.py
--rw-r--r--   0        0        0     6980 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/config/datamodel/config.yaml
--rw-r--r--   0        0        0      540 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/config/default.yaml
--rw-r--r--   0        0        0      198 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/config/recommended.yaml
--rw-r--r--   0        0        0      269 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/formatters/__init__.py
--rw-r--r--   0        0        0      518 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/formatters/formatter.py
--rw-r--r--   0        0        0      767 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/formatters/json_formatter.py
--rw-r--r--   0        0        0     2605 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/formatters/markdown_formatter.py
--rw-r--r--   0        0        0     2085 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/formatters/terminal_formatter.py
--rw-r--r--   0        0        0      871 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/formatters/tsv_formatter.py
--rw-r--r--   0        0        0     5004 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/linter.py
--rw-r--r--   0        0        0    11649 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/linter/rules.py
--rw-r--r--   0        0        0       55 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/reporting/__init__.py
--rw-r--r--   0        0        0     9189 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/reporting/model.py
--rw-r--r--   0        0        0        0 2023-05-27 01:45:11.913278 linkml-1.5.5/linkml/transformers/__init__.py
--rw-r--r--   0        0        0    18594 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/transformers/relmodel_transformer.py
--rw-r--r--   0        0        0     5455 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/transformers/schema_renamer.py
--rw-r--r--   0        0        0        0 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/__init__.py
--rw-r--r--   0        0        0     6463 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/converter.py
--rw-r--r--   0        0        0     4384 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/datautils.py
--rw-r--r--   0        0        0      490 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/datavalidator.py
--rw-r--r--   0        0        0     6999 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/execute_tutorial.py
--rw-r--r--   0        0        0    39737 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/generator.py
--rw-r--r--   0        0        0      445 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/helpers.py
--rw-r--r--   0        0        0     5773 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/ifabsent_functions.py
--rw-r--r--   0        0        0     9498 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/mergeutils.py
--rw-r--r--   0        0        0     4560 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/rawloader.py
--rw-r--r--   0        0        0     9065 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/schema_builder.py
--rw-r--r--   0        0        0    13464 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/schema_fixer.py
--rw-r--r--   0        0        0    48537 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/schemaloader.py
--rw-r--r--   0        0        0    19733 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/schemasynopsis.py
--rw-r--r--   0        0        0    16297 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/sqlutils.py
--rw-r--r--   0        0        0     2395 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/typereferences.py
--rw-r--r--   0        0        0     1514 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/utils/validation.py
--rw-r--r--   0        0        0      140 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/validators/__init__.py
--rw-r--r--   0        0        0     6255 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/validators/jsonschemavalidator.py
--rw-r--r--   0        0        0     4873 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/validators/sparqlvalidator.py
--rw-r--r--   0        0        0        0 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/workspaces/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/workspaces/datamodel/__init__.py
--rw-r--r--   0        0        0    15641 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/workspaces/datamodel/workspaces.py
--rw-r--r--   0        0        0     4233 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/workspaces/datamodel/workspaces.yaml
--rw-r--r--   0        0        0    11912 2023-05-27 01:45:11.917278 linkml-1.5.5/linkml/workspaces/example_runner.py
--rw-r--r--   0        0        0     4974 2023-05-27 01:45:45.953462 linkml-1.5.5/pyproject.toml
--rw-r--r--   0        0        0     6458 1970-01-01 00:00:00.000000 linkml-1.5.5/setup.py
--rw-r--r--   0        0        0     3529 1970-01-01 00:00:00.000000 linkml-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0     6555 2023-06-26 20:53:47.206194 linkml-1.5.6/LICENSE
+-rw-r--r--   0        0        0     1369 2023-06-26 20:53:47.206194 linkml-1.5.6/README.md
+-rw-r--r--   0        0        0     3227 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/__init__.py
+-rw-r--r--   0        0        0      326 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/_version.py
+-rw-r--r--   0        0        0    51006 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/PythonGenNotes.md
+-rw-r--r--   0        0        0     4158 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/README.md
+-rw-r--r--   0        0        0      616 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/common/__init__.py
+-rw-r--r--   0        0        0     2042 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/common/type_designators.py
+-rw-r--r--   0        0        0     3118 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/csvgen.py
+-rw-r--r--   0        0        0     2873 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/docgen/class.md.jinja2
+-rw-r--r--   0        0        0     2682 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/docgen/class_diagram.md.jinja2
+-rw-r--r--   0        0        0     1321 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/docgen/common_metadata.md.jinja2
+-rw-r--r--   0        0        0     1018 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/docgen/enum.md.jinja2
+-rw-r--r--   0        0        0     1466 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/docgen/index.md.jinja2
+-rw-r--r--   0        0        0      501 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/docgen/index.tex.jinja2
+-rw-r--r--   0        0        0       70 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/docgen/schema.md.jinja2
+-rw-r--r--   0        0        0     2557 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/docgen/slot.md.jinja2
+-rw-r--r--   0        0        0     1704 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/docgen/subset.md.jinja2
+-rw-r--r--   0        0        0      635 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/docgen/type.md.jinja2
+-rw-r--r--   0        0        0    32996 2023-06-26 20:53:47.226194 linkml-1.5.6/linkml/generators/docgen.py
+-rw-r--r--   0        0        0     5112 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/dotgen.py
+-rw-r--r--   0        0        0    10910 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/erdiagramgen.py
+-rw-r--r--   0        0        0     6894 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/excelgen.py
+-rw-r--r--   0        0        0     6393 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/golanggen.py
+-rw-r--r--   0        0        0     3575 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/golrgen.py
+-rw-r--r--   0        0        0     2347 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/graphqlgen.py
+-rw-r--r--   0        0        0      444 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/javagen/example_template.java.jinja2
+-rw-r--r--   0        0        0     1737 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/javagen/java_record_template.jinja2
+-rw-r--r--   0        0        0     5499 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/javagen.py
+-rw-r--r--   0        0        0     8821 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/jsonldcontextgen.py
+-rw-r--r--   0        0        0     7952 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/jsonldgen.py
+-rw-r--r--   0        0        0    21709 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/jsonschemagen.py
+-rw-r--r--   0        0        0     3556 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/linkmlgen.py
+-rw-r--r--   0        0        0    34422 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/markdowngen.py
+-rw-r--r--   0        0        0     6532 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/namespacegen.py
+-rw-r--r--   0        0        0     7831 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/oocodegen.py
+-rw-r--r--   0        0        0    29766 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/owlgen.py
+-rw-r--r--   0        0        0     4911 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/prefixmapgen.py
+-rw-r--r--   0        0        0     9811 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/projectgen.py
+-rw-r--r--   0        0        0     2443 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/protogen.py
+-rw-r--r--   0        0        0    22150 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/pydanticgen.py
+-rw-r--r--   0        0        0    50389 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/pythongen.py
+-rw-r--r--   0        0        0     2825 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/rdfgen.py
+-rw-r--r--   0        0        0     5621 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/shaclgen.py
+-rw-r--r--   0        0        0     9547 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/shexgen.py
+-rw-r--r--   0        0        0     6631 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/sparqlgen.py
+-rw-r--r--   0        0        0      166 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2575 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
+-rw-r--r--   0        0        0     1625 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
+-rw-r--r--   0        0        0     9334 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/sqlalchemygen.py
+-rw-r--r--   0        0        0    18626 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/sqlddlgen.py
+-rw-r--r--   0        0        0    11387 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/sqltablegen.py
+-rw-r--r--   0        0        0     7177 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/sssomgen.py
+-rw-r--r--   0        0        0     1788 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/string_template.md
+-rw-r--r--   0        0        0     3020 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/summarygen.py
+-rw-r--r--   0        0        0     4760 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/terminusdbgen.py
+-rw-r--r--   0        0        0     6094 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/typescriptgen.py
+-rw-r--r--   0        0        0     1746 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/yamlgen.py
+-rw-r--r--   0        0        0    13311 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/generators/yumlgen.py
+-rw-r--r--   0        0        0        0 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/__init__.py
+-rw-r--r--   0        0        0     4323 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/cli.py
+-rw-r--r--   0        0        0      292 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/config/datamodel/.linkmllint.yaml
+-rw-r--r--   0        0        0        0 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/config/datamodel/__init__.py
+-rw-r--r--   0        0        0    17711 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/config/datamodel/config.py
+-rw-r--r--   0        0        0     6980 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/config/datamodel/config.yaml
+-rw-r--r--   0        0        0      540 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/config/default.yaml
+-rw-r--r--   0        0        0      198 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/config/recommended.yaml
+-rw-r--r--   0        0        0      269 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/formatters/__init__.py
+-rw-r--r--   0        0        0      518 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/formatters/formatter.py
+-rw-r--r--   0        0        0      767 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/formatters/json_formatter.py
+-rw-r--r--   0        0        0     2605 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/formatters/markdown_formatter.py
+-rw-r--r--   0        0        0     2085 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/formatters/terminal_formatter.py
+-rw-r--r--   0        0        0      871 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/formatters/tsv_formatter.py
+-rw-r--r--   0        0        0     5004 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/linter.py
+-rw-r--r--   0        0        0    11649 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/linter/rules.py
+-rw-r--r--   0        0        0       55 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/reporting/__init__.py
+-rw-r--r--   0        0        0     9189 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/reporting/model.py
+-rw-r--r--   0        0        0        0 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/transformers/__init__.py
+-rw-r--r--   0        0        0    18594 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/transformers/relmodel_transformer.py
+-rw-r--r--   0        0        0     5455 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/transformers/schema_renamer.py
+-rw-r--r--   0        0        0        0 2023-06-26 20:53:47.230194 linkml-1.5.6/linkml/utils/__init__.py
+-rw-r--r--   0        0        0     6393 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/converter.py
+-rw-r--r--   0        0        0     3874 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/datautils.py
+-rw-r--r--   0        0        0      490 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/datavalidator.py
+-rw-r--r--   0        0        0     6999 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/execute_tutorial.py
+-rw-r--r--   0        0        0    39737 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/generator.py
+-rw-r--r--   0        0        0      445 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/helpers.py
+-rw-r--r--   0        0        0     5773 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/ifabsent_functions.py
+-rw-r--r--   0        0        0     9498 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/mergeutils.py
+-rw-r--r--   0        0        0     4560 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/rawloader.py
+-rw-r--r--   0        0        0     9065 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/schema_builder.py
+-rw-r--r--   0        0        0    13464 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/schema_fixer.py
+-rw-r--r--   0        0        0    48537 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/schemaloader.py
+-rw-r--r--   0        0        0    19732 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/schemasynopsis.py
+-rw-r--r--   0        0        0    16297 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/sqlutils.py
+-rw-r--r--   0        0        0     2395 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/typereferences.py
+-rw-r--r--   0        0        0     1514 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/utils/validation.py
+-rw-r--r--   0        0        0      140 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/validators/__init__.py
+-rw-r--r--   0        0        0     7393 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/validators/jsonschemavalidator.py
+-rw-r--r--   0        0        0     4873 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/validators/sparqlvalidator.py
+-rw-r--r--   0        0        0        0 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/workspaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/workspaces/datamodel/__init__.py
+-rw-r--r--   0        0        0    15641 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/workspaces/datamodel/workspaces.py
+-rw-r--r--   0        0        0     4233 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/workspaces/datamodel/workspaces.yaml
+-rw-r--r--   0        0        0    11913 2023-06-26 20:53:47.234194 linkml-1.5.6/linkml/workspaces/example_runner.py
+-rw-r--r--   0        0        0     5287 2023-06-26 20:54:16.718117 linkml-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0     6458 1970-01-01 00:00:00.000000 linkml-1.5.6/setup.py
+-rw-r--r--   0        0        0     3529 1970-01-01 00:00:00.000000 linkml-1.5.6/PKG-INFO
```

### Comparing `linkml-1.5.5/LICENSE` & `linkml-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/README.md` & `linkml-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/__init__.py` & `linkml-1.5.6/linkml/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/PythonGenNotes.md` & `linkml-1.5.6/linkml/generators/PythonGenNotes.md`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 The python first emits a class declaration for the base class -- in this case, the class `Integer` which derives from
 the builtin type `int`.  Four class variables are included in the generation:
 * `type_class_uri` - the URIRef for the type itself
 * `type_class_curie` - the string CURIE representation of the type
 * `type_name` - the non-mangled name assigned to the type in the original definition
 * `type_model_uri` - the URIRef of the type definition in the default LinkML namespace
 
-The python then emits a class definition for the `Integers` classe, where we have defined four slot type permutations:
+The python then emits a class definition for the `Integers` class, where we have defined four slot type permutations:
 
 1) `mand_integer` - a single valued required type:
 
     * The type, `int`, is from the `base` attribute. The python generator does make use of strictly positional parameters,
     so all type declarations will have an appropriate default, which is `None` in this case:
     
         `mand_integer: int = None`
@@ -185,15 +185,15 @@
     * `__post_init__` adds type coercion if necessary
     
 4) `opt_multi_integer`: list:
     * Accept one of `None`, `int`, list of `int`, or anything that can be coerced into `List[int]`:
     
         `opt_multi_integer: Optional[Union[int, List[int]]] = empty_list()`
         
-    * The absence of a list property is always represented as an emtpy list:
+    * The absence of a list property is always represented as an empty list:
         ```        
         if self.opt_multi_integer is None:
             self.opt_multi_integer = []
         ```
       
     * Coerce any other non-list into a list:
         ```        
@@ -1228,26 +1228,26 @@
 ```
 The first two tests are pretty close to what we saw earlier, with the exception that you can't pass an isolated
 dictionary.  You can construct a list of integers with a single value:
 
 ```python
     my_entries = ListOfIntegers(17)
 ```
-Which would, if the class `ListOfIntegers`'s first variable was a multivalued slot with a range of intgers, result in
+Which would, if the class `ListOfIntegers`'s first variable was a multivalued slot with a range of integers, result in
 `my_entries.v == [17]`.  When dealing with classes, however, the following:
 ```python
     my_entries = ListOfClasses(dict(name='element1', value=17))
 ```
 would fail, as it would try to convert this into a list with two `IdentifiedThreeElementClass` entries.
 
 The final line in the `__post_init__` section:
 ```python
     self._normalize_inlined_slot(slot_name="v1", slot_type=IdentifiedThreeElementClass, key_name="name", inlined_as_list=True, keyed=True)
 ```
-passes the remainder of the post initilization normalization to a function defined in `YAMLRoot`.  
+passes the remainder of the post initialization normalization to a function defined in `YAMLRoot`.  
 
 
 The final case, Case 2.4 (Inlined as dictionary) is essentially the same, with the exception that the target type is
 a dictionary rather than a list.  
   
 ```yaml
 OptionalMultivaluedInlinedIdentifiedThreeElementRangeList:
```

### Comparing `linkml-1.5.5/linkml/generators/README.md` & `linkml-1.5.6/linkml/generators/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/__init__.py` & `linkml-1.5.6/linkml/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/common/type_designators.py` & `linkml-1.5.6/linkml/generators/common/type_designators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from linkml_runtime.linkml_model.meta import SlotDefinition, ClassDefinition
 from linkml_runtime.utils.schemaview import SchemaView
 from linkml_runtime.utils.formatutils import camelcase
 from typing import List, Tuple
 
 def get_type_designator_value(sv: SchemaView, type_designator_slot: SlotDefinition, class_def: ClassDefinition) -> str:
     """
-        retuns the correct value for a type designator field for a given class, depending on its range
+        returns the correct value for a type designator field for a given class, depending on its range
         this implements the logic described in https://github.com/linkml/linkml/issues/945:
     """
     slot_types = set(sv.type_ancestors(type_designator_slot.range))
     if 'uri' in slot_types:
         return sv.get_uri(class_def,expand=True,native=False)
     elif 'uriorcurie' in slot_types:
         return sv.get_uri(class_def,expand=False, native=False)
@@ -17,15 +17,15 @@
         return class_def.name
     else:
         return sv.get_uri(class_def,expand=False, native=False)
 
 
 def get_accepted_type_designator_values(sv: SchemaView, type_designator_slot: SlotDefinition, class_def: ClassDefinition) -> List[str]:
     """
-        retuns the accepted values for a type designator field for a given class, depending on its range
+        returns the accepted values for a type designator field for a given class, depending on its range
         this implements the logic described in https://github.com/linkml/linkml/issues/945:
     """
     accepted_uri_values = [
             sv.get_uri(class_def, expand=True, native=True),
             sv.get_uri(class_def, expand=True, native=False),
             sv.get_uri(class_def, expand=False, native=True),
             sv.get_uri(class_def, expand=False, native=False),
```

### Comparing `linkml-1.5.5/linkml/generators/csvgen.py` & `linkml-1.5.6/linkml/generators/csvgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/docgen/class.md.jinja2` & `linkml-1.5.6/linkml/generators/docgen/class.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/docgen/class_diagram.md.jinja2` & `linkml-1.5.6/linkml/generators/docgen/class_diagram.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/docgen/common_metadata.md.jinja2` & `linkml-1.5.6/linkml/generators/docgen/common_metadata.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/docgen/enum.md.jinja2` & `linkml-1.5.6/linkml/generators/docgen/enum.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/docgen/index.md.jinja2` & `linkml-1.5.6/linkml/generators/docgen/index.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/docgen/slot.md.jinja2` & `linkml-1.5.6/linkml/generators/docgen/slot.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/docgen/subset.md.jinja2` & `linkml-1.5.6/linkml/generators/docgen/subset.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/docgen/type.md.jinja2` & `linkml-1.5.6/linkml/generators/docgen/type.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/docgen.py` & `linkml-1.5.6/linkml/generators/docgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
             return self.format
 
     def _get_template(self, element_type: str) -> Template:
         """
         Create a jinja2 template object for a given schema element type
 
         The default location for templates is in the linkml/docgen folder,
-        but this can be overriden
+        but this can be overridden
         :param element_type: e.g. class, enum, index, subset, ...
         :return:
         """
         if self.template_mappings and element_type in self.template_mappings:
             path = self.template_mappings[element_type]
             # TODO: relative paths
             # loader = FileSystemLoader()
@@ -429,15 +429,15 @@
 
         return f"[{n}]({rel_path}.md)"
 
     def inheritance_tree(
         self, element: Definition, children: bool = True, **kwargs
     ) -> str:
         """
-        Show an element in the context of its is-a hierachy
+        Show an element in the context of its is-a hierarchy
 
         Limitations: currently only implemented for markdown (uses nested bullets)
 
         :param element: slot or class to be shown
         :param children: if true, show direct children
         :param mixins: if true, show mixins alongside each element
         :param kwargs:
```

### Comparing `linkml-1.5.5/linkml/generators/dotgen.py` & `linkml-1.5.6/linkml/generators/dotgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/erdiagramgen.py` & `linkml-1.5.6/linkml/generators/erdiagramgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,19 +199,19 @@
     def serialize_diagram(self, diagram: ERDiagram) -> str:
         """
         Serialize an ER Diagram, from the native pydantic schema.
 
         :param diagram: ER Diagram
         :return:
         """
-        ser = str(diagram)
+        er = str(diagram)
         if self.format == 'markdown':
-            return f'```mermaid\n{ser}\n```\n'
+            return f'```mermaid\n{er}\n```\n'
         else:
-            return ser
+            return er
 
     def add_class(self, class_name: ClassDefinitionName, diagram: ERDiagram) -> None:
         """
         Add a class to the ER Diagram.
 
         :param class_name: ClassDefinitionName
         :param diagram: ER Diagram
```

### Comparing `linkml-1.5.5/linkml/generators/excelgen.py` & `linkml-1.5.6/linkml/generators/excelgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/golanggen.py` & `linkml-1.5.6/linkml/generators/golanggen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/golrgen.py` & `linkml-1.5.6/linkml/generators/golrgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/graphqlgen.py` & `linkml-1.5.6/linkml/generators/graphqlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/javagen/java_record_template.jinja2` & `linkml-1.5.6/linkml/generators/javagen/java_record_template.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/javagen.py` & `linkml-1.5.6/linkml/generators/javagen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/jsonldcontextgen.py` & `linkml-1.5.6/linkml/generators/jsonldcontextgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/jsonldgen.py` & `linkml-1.5.6/linkml/generators/jsonldgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/jsonschemagen.py` & `linkml-1.5.6/linkml/generators/jsonschemagen.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,36 +302,36 @@
         enum_schema = JsonSchema({
             "type": "string",
             "enum": permissible_values_texts,
             "description": be(enum.description),
         })
         self.top_level_schema.add_def(enum.name, enum_schema)
 
-    def get_type_info_for_slot_subschema(self, slot: AnonymousSlotExpression, parent_slot_is_inlined: bool) -> Tuple[str, str, Union[str, List[str]]]:
+    def get_type_info_for_slot_subschema(self, slot: AnonymousSlotExpression) -> Tuple[str, str, Union[str, List[str]]]:
         typ = None  # JSON Schema type (https://json-schema.org/understanding-json-schema/reference/type.html)
         reference = None  # Reference to a JSON schema entity (https://json-schema.org/understanding-json-schema/structuring.html#ref)
         fmt = None  # JSON Schema format (https://json-schema.org/understanding-json-schema/reference/string.html#format)
 
         slot_is_inlined = self.schemaview.is_inlined(slot)
         if slot.range in self.schemaview.all_types().keys():
             schema_type = self.schemaview.induced_type(slot.range)
             (typ, fmt) = json_schema_types.get(schema_type.base.lower(), ("string", None))
         elif slot.range in self.schemaview.all_enums().keys():
             reference = slot.range
         elif slot.range in self.schemaview.all_classes().keys():
-            if slot_is_inlined or parent_slot_is_inlined:
+            if slot_is_inlined:
                 descendants = [desc for desc in self.schemaview.class_descendants(slot.range) 
                     if not self.schemaview.get_class(desc).abstract]
                 if descendants and self.include_range_class_descendants:
                     reference = descendants
                 else:
                     reference = slot.range
             else:
                 id_slot = self.schemaview.get_identifier_slot(slot.range)
-                typ = id_slot.range or "string"
+                return self.get_type_info_for_slot_subschema(id_slot)
 
         return (typ, fmt, reference)
     
     def get_value_constraints_for_slot(self, slot: Union[AnonymousSlotExpression, None]) -> JsonSchema:
         if slot is None:
             return JsonSchema()
         
@@ -344,15 +344,15 @@
         return constraints
 
     def get_subschema_for_slot(self, slot: SlotDefinition, omit_type: bool = False) -> JsonSchema:
         prop = JsonSchema()
         slot_is_multivalued = 'multivalued' in slot and slot.multivalued
         slot_is_inlined = self.schemaview.is_inlined(slot)
         if not omit_type:
-            typ, fmt, reference = self.get_type_info_for_slot_subschema(slot, slot_is_inlined)
+            typ, fmt, reference = self.get_type_info_for_slot_subschema(slot)
             if slot_is_inlined:
                 # If inline we have to include redefined slots
                 if slot_is_multivalued:
                     range_id_slot, range_simple_dict_value_slot, range_required_slots = self._get_range_associated_slots(slot)
                     # if the range class has an ID and the slot is not inlined as a list, then we need to consider
                     # various inlined as dict formats
                     if range_id_slot is not None and not slot.inlined_as_list:
@@ -448,23 +448,26 @@
         class_id_slot = self.schemaview.get_identifier_slot(cls.name, use_key=True)
         slot_is_required = slot.required or slot == class_id_slot
 
         aliased_slot_name = self.aliased_slot_name(slot)
         prop = self.get_subschema_for_slot(slot)
         subschema.add_property(aliased_slot_name, prop, slot_is_required)
 
-    def serialize(self, **kwargs) -> str:
+    def generate(self) -> dict:
         self.start_schema()
         for enum_definition in self.schemaview.all_enums().values():
             self.handle_enum(enum_definition)
 
         for class_definition in self.schemaview.all_classes().values():
             self.handle_class(class_definition)
 
-        return self.top_level_schema.to_json(sort_keys=True, indent=self.indent if self.indent > 0 else None)
+        return self.top_level_schema
+        
+    def serialize(self, **kwargs) -> str:
+        return self.generate().to_json(sort_keys=True, indent=self.indent if self.indent > 0 else None)
     
     def _get_range_associated_slots(self, slot: SlotDefinition) -> Tuple[Union[SlotDefinition, None], Union[SlotDefinition, None], Union[List[SlotDefinition], None]]:
         range_class = self.schemaview.get_class(slot.range)
         if range_class is None:
             return None, None, None
         
         range_class_id_slot = self.schemaview.get_identifier_slot(range_class.name, use_key=True)
```

### Comparing `linkml-1.5.5/linkml/generators/linkmlgen.py` & `linkml-1.5.6/linkml/generators/linkmlgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     def __post_init__(self):
         # TODO: consider moving up a level
         super().__post_init__()
         self.schemaview = SchemaView(self.schema, merge_imports=self.mergeimports)
 
     def materialize_classes(self) -> None:
-        """Materialize class slots from schema as attribues, in place"""
+        """Materialize class slots from schema as attributes, in place"""
         all_classes = self.schemaview.all_classes()
 
         for c_name, c_def in all_classes.items():
             attrs = self.schemaview.class_induced_slots(c_name)
             for attr in attrs:
                 c_def.attributes[attr.name] = attr
```

### Comparing `linkml-1.5.5/linkml/generators/markdowngen.py` & `linkml-1.5.6/linkml/generators/markdowngen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/namespacegen.py` & `linkml-1.5.6/linkml/generators/namespacegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/oocodegen.py` & `linkml-1.5.6/linkml/generators/oocodegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/owlgen.py` & `linkml-1.5.6/linkml/generators/owlgen.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     metadata_profile: MetadataProfile = None
     ontology_uri_suffix: str = None
     metaclasses: bool = field(default_factory=lambda: True)
     add_ols_annotations: bool = field(default_factory=lambda: True)
     graph: Optional[Graph] = None
     top_value_uri: Optional[URIRef] = None
     type_objects: bool = field(default_factory=lambda: True)
+    assert_equivalent_classes: bool = False
 
     def visit_schema(self, output: Optional[str] = None, **_):
         owl_id = self.schema.id
         if self.ontology_uri_suffix:
             owl_id = f"{owl_id}{self.ontology_uri_suffix}"
         base = URIRef(owl_id)
         self.graph = Graph(identifier=base)
@@ -262,14 +263,21 @@
                     self.graph.add(
                         (
                             self.graph.identifier,
                             URIRef("http://purl.obolibrary.org/obo/IAO_0000700"),
                             cls_uri,
                         )
                     )
+
+        if cls.class_uri and self.assert_equivalent_classes:
+            eq_class_uri = self.namespaces.uri_for(cls.class_uri)
+            if str(eq_class_uri) != cls.definition_uri:
+                self.graph.add((cls_uri, OWL.equivalentClass, eq_class_uri))
+                self.graph.remove((cls_uri, SKOS.exactMatch, eq_class_uri))
+
         # If defining slots, we generate an equivalentClass entry
         # equ_node = BNode()
         # self.graph.add((cls_uri, OWL.equivalentClass, equ_node))
         # self.graph.add((equ_node, RDF.type, OWL.Class))
         #
         # elts = []
         # if cls.is_a:
@@ -675,14 +683,20 @@
 )
 @click.option(
     "--ontology-uri-suffix",
     default=".owl.ttl",
     show_default=True,
     help="Suffix to append to schema id to generate OWL Ontology IRI",
 )
+@click.option(
+    "--assert-equivalent-classes/--no-assert-equivalent-classes",
+    default=False,
+    show_default=True,
+    help="If true, add owl:equivalentClass between a class and a class_uri",
+)
 @click.version_option(__version__, "-V", "--version")
 def cli(yamlfile, metadata_profile: str, **kwargs):
     """Generate an OWL representation of a LinkML model
 
     Examples:
 
         Generate OWL using default parameters:
```

### Comparing `linkml-1.5.5/linkml/generators/prefixmapgen.py` & `linkml-1.5.6/linkml/generators/prefixmapgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     slot_class_maps: Dict = field(default_factory=lambda: dict())
     base: str = None
 
     def __post_init__(self):
         super().__post_init__()
         if self.namespaces is None:
             raise TypeError(
-                "Schema text must be supplied to context generater.  Preparsed schema will not work"
+                "Schema text must be supplied to context generator.  Preparsed schema will not work"
             )
 
     def visit_schema(
         self, base: Optional[str] = None, output: Optional[str] = None, **_
     ):
         # Add any explicitly declared prefixes
         for prefix in self.schema.prefixes.values():
```

### Comparing `linkml-1.5.5/linkml/generators/projectgen.py` & `linkml-1.5.6/linkml/generators/projectgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/protogen.py` & `linkml-1.5.6/linkml/generators/protogen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/pydanticgen.py` & `linkml-1.5.6/linkml/generators/pydanticgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/pythongen.py` & `linkml-1.5.6/linkml/generators/pythongen.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,15 +329,15 @@
                 if pkeys:
                     for pk in pkeys:
                         classname = camelcase(cls.name) + camelcase(
                             self.aliased_slot_name(pk)
                         )
                         # If we've got a parent slot and the range of the parent is the range of the child, the
                         # child slot is a subclass of the parent.  Otherwise, the child range has been overridden,
-                        # so the inheritence chain has been broken
+                        # so the inheritance chain has been broken
                         parent_pk = (
                             self.class_identifier(cls.is_a) if cls.is_a else None
                         )
                         parent_pk_slot = (
                             self.schema.slots[parent_pk] if parent_pk else None
                         )
                         pk_slot = self.schema.slots[pk]
@@ -513,15 +513,15 @@
         ]
         return "\n\t".join(type_meta)
 
     def gen_class_variables(self, cls: ClassDefinition) -> str:
         """
         Generate the variable declarations for a dataclass.
 
-        :param cls: class containing variables to be rendered in inheritence hierarchy
+        :param cls: class containing variables to be rendered in inheritance hierarchy
         :return: variable declarations for target class and its ancestors
         """
         initializers = []
 
         is_root = not cls.is_a
         domain_slots = self.domain_slots(cls)
 
@@ -819,15 +819,15 @@
                     f"if not isinstance(self.{aliased_slot_name}, {base_type_name}):"
                 )
             else:
                 rlines.append(
                     f"if self.{aliased_slot_name} is not None and "
                     f"not isinstance(self.{aliased_slot_name}, {base_type_name}):"
                 )
-            # A really wierd case -- a class that has no properties
+            # A really weird case -- a class that has no properties
             if (
                 slot.range in self.schema.classes
                 and not self.schema.classes[slot.range].slots
             ):
                 rlines.append(f"\tself.{aliased_slot_name} = {base_type_name}()")
             else:
                 if (
```

### Comparing `linkml-1.5.5/linkml/generators/rdfgen.py` & `linkml-1.5.6/linkml/generators/rdfgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/shaclgen.py` & `linkml-1.5.6/linkml/generators/shaclgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/shexgen.py` & `linkml-1.5.6/linkml/generators/shexgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/sparqlgen.py` & `linkml-1.5.6/linkml/generators/sparqlgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 @shared_arguments(SparqlGenerator)
 @click.command()
 @click.option("--dir", "-d", help="Directory in which queries will be deposited")
 @click.version_option(__version__, "-V", "--version")
 def cli(yamlfile, dir, **kwargs):
     """Generate SPARQL queries for validation
 
-    This will generate a directory of queries that cann be used for QC over a triplestore that
+    This will generate a directory of queries that can be used for QC over a triplestore that
     is conformant to the same LinkML schema.
 
     Each query in the directory will be of the form
 
         CHECK_<ConstraintType>_<SchemaElement>.rq
 
     Example:
```

### Comparing `linkml-1.5.5/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py` & `linkml-1.5.6/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py` & `linkml-1.5.6/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/sqlalchemygen.py` & `linkml-1.5.6/linkml/generators/sqlalchemygen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/sqlddlgen.py` & `linkml-1.5.6/linkml/generators/sqlddlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/sqltablegen.py` & `linkml-1.5.6/linkml/generators/sqltablegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/sssomgen.py` & `linkml-1.5.6/linkml/generators/sssomgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/string_template.md` & `linkml-1.5.6/linkml/generators/string_template.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/summarygen.py` & `linkml-1.5.6/linkml/generators/summarygen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/terminusdbgen.py` & `linkml-1.5.6/linkml/generators/terminusdbgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/typescriptgen.py` & `linkml-1.5.6/linkml/generators/typescriptgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/yamlgen.py` & `linkml-1.5.6/linkml/generators/yamlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/generators/yumlgen.py` & `linkml-1.5.6/linkml/generators/yumlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/linter/cli.py` & `linkml-1.5.6/linkml/linter/cli.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/linter/config/datamodel/config.py` & `linkml-1.5.6/linkml/linter/config/datamodel/config.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/linter/config/datamodel/config.yaml` & `linkml-1.5.6/linkml/linter/config/datamodel/config.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/linter/config/default.yaml` & `linkml-1.5.6/linkml/linter/config/default.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/linter/formatters/formatter.py` & `linkml-1.5.6/linkml/linter/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/linter/formatters/json_formatter.py` & `linkml-1.5.6/linkml/linter/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/linter/formatters/markdown_formatter.py` & `linkml-1.5.6/linkml/linter/formatters/markdown_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/linter/formatters/terminal_formatter.py` & `linkml-1.5.6/linkml/linter/formatters/terminal_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/linter/formatters/tsv_formatter.py` & `linkml-1.5.6/linkml/linter/formatters/tsv_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/linter/linter.py` & `linkml-1.5.6/linkml/linter/linter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/linter/rules.py` & `linkml-1.5.6/linkml/linter/rules.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/reporting/model.py` & `linkml-1.5.6/linkml/reporting/model.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/transformers/relmodel_transformer.py` & `linkml-1.5.6/linkml/transformers/relmodel_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/transformers/schema_renamer.py` & `linkml-1.5.6/linkml/transformers/schema_renamer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/utils/converter.py` & `linkml-1.5.6/linkml/utils/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,16 +155,14 @@
     if output_format == "json-ld":
         if len(context) == 0:
             if schema is not None:
                 context = [_get_context(schema)]
             else:
                 raise Exception("Must pass in context OR schema for RDF output")
         outargs["contexts"] = list(context)
-        outargs["fmt"] = "json-ld"
-        outargs["schemaview"] = sv
     if output_format == "rdf" or output_format == "ttl":
         if sv is None:
             raise Exception(f"Must pass schema arg")
         outargs["schemaview"] = sv
     if _is_xsv(output_format):
         if index_slot is None:
             index_slot = infer_index_slot(sv, target_class)
```

### Comparing `linkml-1.5.5/linkml/utils/datautils.py` & `linkml-1.5.6/linkml/utils/datautils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import os
 from collections import defaultdict
 from typing import Optional, Union
 
-from linkml_runtime.dumpers.csv_dumper import CSVDumper
-from linkml_runtime.dumpers.json_dumper import JSONDumper
-from linkml_runtime.dumpers.rdf_dumper import RDFDumper
-from linkml_runtime.dumpers.rdflib_dumper import RDFLibDumper
-from linkml_runtime.dumpers.yaml_dumper import YAMLDumper
-from linkml_runtime.linkml_model.meta import (ClassDefinitionName,
-                                              SchemaDefinition,
-                                              SlotDefinitionName)
-from linkml_runtime.loaders.csv_loader import CSVLoader
-from linkml_runtime.loaders.json_loader import JSONLoader
+from linkml_runtime.dumpers import (
+    CSVDumper,
+    JSONDumper,
+    RDFLibDumper,
+    TSVDumper,
+    YAMLDumper,
+)
+from linkml_runtime.linkml_model.meta import ClassDefinitionName, SlotDefinitionName
+from linkml_runtime.loaders import (
+    CSVLoader,
+    JSONLoader,
+    RDFLibLoader,
+    TSVLoader,
+    YAMLLoader,
+)
 from linkml_runtime.loaders.loader_root import Loader
-from linkml_runtime.loaders.rdf_loader import RDFLoader
-from linkml_runtime.loaders.rdflib_loader import RDFLibLoader
-from linkml_runtime.loaders.yaml_loader import YAMLLoader
 from linkml_runtime.utils.schemaview import SchemaView
-from linkml_runtime.utils.yamlutils import YAMLRoot
 
 from linkml.generators.jsonldcontextgen import ContextGenerator
 
 dumpers_loaders = {
     "yml": (YAMLDumper, YAMLLoader),
     "yaml": (YAMLDumper, YAMLLoader),
     "json": (JSONDumper, JSONLoader),
     "rdf": (RDFLibDumper, RDFLibLoader),
     "ttl": (RDFLibDumper, RDFLibLoader),
-    "json-ld": (RDFLibDumper, RDFLibLoader),
+    "json-ld": (JSONDumper, JSONLoader),
     "csv": (CSVDumper, CSVLoader),
-    "tsv": (CSVDumper, CSVLoader),
+    "tsv": (TSVDumper, TSVLoader),
 }
 
 aliases = {
     "rdf": "ttl",
     "jsonld": "json-ld",
 }
```

### Comparing `linkml-1.5.5/linkml/utils/execute_tutorial.py` & `linkml-1.5.6/linkml/utils/execute_tutorial.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             if ">" in cmd:
                 # redirects not support in subprocess.run
                 pos = cmd.index(">")
                 outpath = cmd[pos + 1 :]
                 cmd = cmd[0:pos]
                 if len(outpath) > 1:
                     raise Exception(
-                        f"Maximim 1 token after > in {block.content}. Got: {outpath}"
+                        f"Maximum 1 token after > in {block.content}. Got: {outpath}"
                     )
                 outpath = str(Path(directory, *outpath))
                 logging.info(f"OUTPATH = {outpath}")
             else:
                 outpath = None
             logging.info(f"Executing: {cmd}")
             r = subprocess.run(cmd, cwd=directory, capture_output=True)
```

### Comparing `linkml-1.5.5/linkml/utils/generator.py` & `linkml-1.5.6/linkml/utils/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
             for prefix in self.schema.prefixes.values():
                 self.namespaces[prefix.prefix_prefix] = prefix.prefix_reference
 
     def serialize(self, **kwargs) -> str:
         """
         Generate output in the required format
 
-        :param kwargs: Generater specific parameters
+        :param kwargs: Generator specific parameters
         :return: Generated output
         """
         output = StringIO()
         # Note: we currently redirect stdout, this means that print statements within
         # each generator will be redirected to the StringIO object.
         # See https://github.com/linkml/linkml/issues/923 for discussion on simplifying this
         with redirect_stdout(output):
```

### Comparing `linkml-1.5.5/linkml/utils/ifabsent_functions.py` & `linkml-1.5.6/linkml/utils/ifabsent_functions.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/utils/mergeutils.py` & `linkml-1.5.6/linkml/utils/mergeutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/utils/rawloader.py` & `linkml-1.5.6/linkml/utils/rawloader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/utils/schema_builder.py` & `linkml-1.5.6/linkml/utils/schema_builder.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/utils/schema_fixer.py` & `linkml-1.5.6/linkml/utils/schema_fixer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/utils/schemaloader.py` & `linkml-1.5.6/linkml/utils/schemaloader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/utils/schemasynopsis.py` & `linkml-1.5.6/linkml/utils/schemasynopsis.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
 
     def summarize_element(self, typ: RefType, k: ElementName, v: Element) -> None:
         """
          Summarize element level items
 
         :param typ: element type
         :param k: element name
-        :param v: element deffinition
+        :param v: element definition
         :return:
         """
         if k != v.name:
             raise ValueError(
                 "{typ} name mismatch: {k} != {v.name}"
             )  # should never happen
         for subset in v.in_subset:
```

### Comparing `linkml-1.5.5/linkml/utils/sqlutils.py` & `linkml-1.5.6/linkml/utils/sqlutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/utils/typereferences.py` & `linkml-1.5.6/linkml/utils/typereferences.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/utils/validation.py` & `linkml-1.5.6/linkml/utils/validation.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/validators/jsonschemavalidator.py` & `linkml-1.5.6/linkml/validators/jsonschemavalidator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,69 @@
-import json
 import logging
 import sys
-from dataclasses import dataclass
-from typing import TextIO, Type, Union, Dict, Optional
+from dataclasses import asdict, dataclass, field
+from functools import lru_cache
+from typing import Any, Iterable, List, Type, Union
 
 import click
 import jsonschema
-from linkml_runtime.dumpers import json_dumper
-from linkml_runtime.linkml_model import SchemaDefinition, ClassDefinitionName
+from jsonschema.exceptions import best_match
+from linkml_runtime.linkml_model import ClassDefinitionName, SchemaDefinition
 from linkml_runtime.utils.compile_python import compile_python
 from linkml_runtime.utils.dictutils import as_simple_dict
 from linkml_runtime.utils.schemaview import SchemaView
 from linkml_runtime.utils.yamlutils import YAMLRoot
 
 from linkml._version import __version__
 from linkml.generators.jsonschemagen import JsonSchemaGenerator
 from linkml.generators.pythongen import PythonGenerator
 from linkml.utils import datautils
 from linkml.utils.datavalidator import DataValidator
 
 
+class HashableSchemaDefinition(SchemaDefinition):
+
+    def __hash__(self) -> int:
+        return hash(self.id)
+
+
+@lru_cache(maxsize=None)
+def _generate_jsonschema(schema, top_class, closed):
+    logging.debug(f"Generating JSON Schema")
+    not_closed = not closed
+    return JsonSchemaGenerator(
+        schema=schema,
+        mergeimports=True,
+        top_class=top_class,
+        not_closed=not_closed,
+    ).generate()
+
+
+class JsonSchemaDataValidatorError(Exception):
+    def __init__(self, validation_messages: List[str]) -> None:
+        super().__init__("\n".join(validation_messages))
+        self.validation_messages = validation_messages
+
+
 @dataclass
 class JsonSchemaDataValidator(DataValidator):
     """
     Implementation of DataValidator that wraps jsonschema validation
     """
 
-    jsonschema_objs: Optional[Dict[str, Dict]] = None
-    """Cached outputs of jsonschema generation"""
+    _hashable_schema: Union[str, HashableSchemaDefinition] = field(init=False, repr=False)
+
+    def __setattr__(self, __name: str, __value: Any) -> None:
+        if (__name == 'schema'):
+            if isinstance(__value, SchemaDefinition):
+                self._hashable_schema = HashableSchemaDefinition(**asdict(__value))
+            else:
+                self._hashable_schema = __value
+        return super().__setattr__(__name, __value)
+        
 
     def validate_file(self, input: str, format: str = "json", **kwargs):
         return self.validate_object(obj)
 
     def validate_object(
         self, data: YAMLRoot, target_class: Type[YAMLRoot] = None, closed: bool = True
     ) -> None:
@@ -42,67 +74,54 @@
         :param target_class: class in schema to validate against
         :param closed:
         :return:
         """
         if target_class is None:
             target_class = type(data)
         inst_dict = as_simple_dict(data)
-        not_closed = not closed
-        if self.schema is None:
-            raise ValueError(f"schema object must be set")
-        if self.jsonschema_objs is None:
-            self.jsonschema_objs = {}
-        schema_id = self.schema.id if isinstance(self.schema, SchemaDefinition) else self.schema
-        cache_params = frozenset([schema_id, target_class.class_name])
-        if cache_params not in self.jsonschema_objs:
-            jsonschemastr = JsonSchemaGenerator(
-                self.schema,
-                mergeimports=True,
-                top_class=target_class.class_name,
-                not_closed=not_closed,
-            ).serialize(not_closed=not_closed)
-            jsonschema_obj = json.loads(jsonschemastr)
-            self.jsonschema_objs[cache_params] = jsonschema_obj
-        else:
-            logging.info(f"Using cached jsonschema for {schema_id}")
-            jsonschema_obj = self.jsonschema_objs[cache_params]
-        return jsonschema.validate(inst_dict, schema=jsonschema_obj, format_checker=jsonschema.Draft7Validator.FORMAT_CHECKER)
+        self.validate_dict(inst_dict, target_class.class_name, closed)
 
     def validate_dict(
         self, data: dict, target_class: ClassDefinitionName = None, closed: bool = True
     ) -> None:
         """
         validates instance data against a schema
 
         :param data: dictionary object
         :param target_class: class in schema to validate against
         :param closed:
         :return:
         """
-        not_closed = not closed
+        results = list(self.iter_validate_dict(data, target_class, closed))
+        if results:
+            raise JsonSchemaDataValidatorError(results)
+
+    def iter_validate_dict(
+        self, data: dict, target_class_name: ClassDefinitionName = None, closed: bool = True
+    ) -> Iterable[str]:
         if self.schema is None:
             raise ValueError(f"schema object must be set")
-        if target_class is None:
+        if target_class_name is None:
             roots = [c.name for c in self.schema.classes.values() if c.tree_root]
             if len(roots) != 1:
                 raise ValueError(f"Cannot determine tree root: {roots}")
-            target_class = roots[0]
-        jsonschemastr = JsonSchemaGenerator(
-            self.schema,
-            mergeimports=True,
-            top_class=target_class,
-            not_closed=not_closed,
-        ).serialize(not_closed=not_closed)
-        jsonschema_obj = json.loads(jsonschemastr)
-        return jsonschema.validate(data, schema=jsonschema_obj, format_checker=jsonschema.Draft7Validator.FORMAT_CHECKER)
+            target_class_name = roots[0]
+        jsonschema_obj = _generate_jsonschema(self._hashable_schema, target_class_name, closed)
+        validator = jsonschema.Draft7Validator(
+            jsonschema_obj, format_checker=jsonschema.Draft7Validator.FORMAT_CHECKER
+        )
+        for error in validator.iter_errors(data):
+            best_error = best_match([error])
+            # TODO: This should return some kind of standard validation result
+            # object, but until that is defined just yield string messages
+            yield f"{best_error.message} in {best_error.json_path}"
 
 
 @click.command()
 @click.option("--module", "-m", help="Path to python datamodel module")
-@click.option("--output", "-o", help="Path to output file")
 @click.option(
     "--input-format",
     "-f",
     type=click.Choice(list(datautils.dumpers_loaders.keys())),
     help="Input format. Inferred from input suffix if not specified",
 )
 @click.option(
@@ -110,24 +129,29 @@
     "-C",
     help="name of class in datamodel that the root node instantiates",
 )
 @click.option(
     "--index-slot", "-S", help="top level slot. Required for CSV dumping/loading"
 )
 @click.option("--schema", "-s", help="Path to schema specified as LinkML yaml")
+@click.option(
+    "--exit-on-first-failure/--no-exit-on-first-failure", 
+    default=False,
+    help="Exit after the first validation failure is found. If not specified all validation failures are reported."
+)
 @click.argument("input")
 @click.version_option(__version__, "-V", "--version")
 def cli(
     input,
     module,
     target_class,
-    output=None,
     input_format=None,
     schema=None,
     index_slot=None,
+    exit_on_first_failure=False,
 ) -> None:
     """
     Validates instance data
     """
     if module is None:
         if schema is None:
             raise Exception("must pass one of module OR schema")
@@ -153,20 +177,37 @@
             if index_slot is None:
                 raise Exception("--index-slot is required for CSV input")
         inargs["index_slot"] = index_slot
         inargs["schema"] = schema
     if datautils._is_rdf_format(input_format):
         inargs["schemaview"] = sv
         inargs["fmt"] = input_format
-    obj = loader.load(source=input, target_class=py_target_class, **inargs)
+
+    try:
+        data_as_dict = loader.load_as_dict(source=input, **inargs)
+    except NotImplementedError:
+        obj = loader.load(source=input, target_class=py_target_class, **inargs)
+        data_as_dict = as_simple_dict(obj)
+
     # Validation
     if schema is None:
         raise Exception(
             "--schema must be passed in order to validate. Suppress with --no-validate"
         )
+
     validator = JsonSchemaDataValidator(schema)
-    results = validator.validate_object(obj, target_class=py_target_class)
-    print(results)
+    error_count = 0
+    for error in validator.iter_validate_dict(
+        data_as_dict, target_class_name=py_target_class.class_name
+    ):
+        error_count += 1
+        click.echo(click.style("\u2717 ", fg="red") + error)
+        if exit_on_first_failure:
+            sys.exit(1)
+
+    if not error_count:
+        click.echo(click.style("\u2713 ", fg="green") + "No problems found")
 
+    sys.exit(0 if error_count == 0 else 1)
 
 if __name__ == "__main__":
     cli(sys.argv[1:])
```

### Comparing `linkml-1.5.5/linkml/validators/sparqlvalidator.py` & `linkml-1.5.6/linkml/validators/sparqlvalidator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/workspaces/datamodel/workspaces.py` & `linkml-1.5.6/linkml/workspaces/datamodel/workspaces.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/workspaces/datamodel/workspaces.yaml` & `linkml-1.5.6/linkml/workspaces/datamodel/workspaces.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.5/linkml/workspaces/example_runner.py` & `linkml-1.5.6/linkml/workspaces/example_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
                 try:
                     validator.validate_dict(input_dict, tc, closed=True)
                     # json validation is incomplete: also try object instantiation
                     self._load_from_dict(input_dict, target_class=tc)
                 except Exception as e:
                     success = False
                     if not counter_examples:
-                        raise ValueError(f"Example {input_example} failed validation: {e}")
+                        raise ValueError(f"Example {input_example} failed validation:\n{e}")
                 if counter_examples:
                     if success:
                         raise ValueError(f"Counter example {input_example} succeeded validation")
                     continue
                 obj = self._load_from_dict(input_dict, target_class=tc)
                 for fmt in self.output_formats:
                     output_file = f"{base}.{fmt}"
```

### Comparing `linkml-1.5.5/pyproject.toml` & `linkml-1.5.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml"
-version = "1.5.5"
+version = "1.5.6"
 description = "Linked Open Data Modeling Language"
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harold Solbrig <solbrig@jhu.edu>",
     "Sujay Patil <spatil@lbl.gov>",
     "Harshad Hegde <hhegde@lbl.gov>",
     "Sierra Moxon <smoxon@lbl.gov>",
@@ -102,15 +102,15 @@
 graphviz = ">=0.10.1"
 hbreader = "*"
 isodate = ">=0.6.0"
 jinja2 = ">= 3.1.0"
 jsonasobj2 = "==1.*,>=1.0.0,>=1.0.3"
 jsonschema = {extras = ["format"], version = ">=4.0.0"}
 linkml-dataops = "*"
-linkml-runtime = ">=1.5.3"
+linkml-runtime = ">=1.5.4"
 openpyxl = "*"
 parse = "*"
 prefixcommons = ">=0.1.7"
 prefixmaps = ">=0.1.3"
 pydantic = "*"
 pyjsg = ">=0.11.6"
 pyshex = ">=0.7.20"
@@ -140,7 +140,16 @@
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinxcontrib-mermaid", "furo"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
+
+[tool.codespell]
+# TODO: bring in tests in too
+skip = '.git,*.pdf,*.svg,tests,pyproject.toml,*.dill'
+# Ignore table where words could be split across rows
+# Ignore shortcut specifications like [Ff]alse
+ignore-regex = '(\|.*\|.*\|.*\||\[[A-Z][a-z]\][a-z][a-z])'
+#
+ignore-words-list = 'mater,connexion,infarction'
```

### Comparing `linkml-1.5.5/setup.py` & `linkml-1.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'graphviz>=0.10.1',
  'hbreader',
  'isodate>=0.6.0',
  'jinja2>=3.1.0',
  'jsonasobj2>=1.0.3,<2.0.0',
  'jsonschema[format]>=4.0.0',
  'linkml-dataops',
- 'linkml-runtime>=1.5.3',
+ 'linkml-runtime>=1.5.4',
  'openpyxl',
  'parse',
  'prefixcommons>=0.1.7',
  'prefixmaps>=0.1.3',
  'pydantic',
  'pyjsg>=0.11.6',
  'pyshex>=0.7.20',
@@ -101,15 +101,15 @@
                      'linkml-sqldb = linkml.utils.sqlutils:main',
                      'linkml-validate = '
                      'linkml.validators.jsonschemavalidator:cli',
                      'run-tutorial = linkml.utils.execute_tutorial:cli']}
 
 setup_kwargs = {
     'name': 'linkml',
-    'version': '1.5.5',
+    'version': '1.5.6',
     'description': 'Linked Open Data Modeling Language',
     'long_description': '[![Pyversions](https://img.shields.io/pypi/pyversions/linkml.svg)](https://pypi.python.org/pypi/linkml)\n![](https://github.com/linkml/linkml/workflows/Build/badge.svg)\n[![PyPi](https://img.shields.io/pypi/v/linkml.svg)](https://pypi.python.org/pypi/linkml)\n[![badge](https://img.shields.io/badge/launch-binder-579ACA.svg)](https://mybinder.org/v2/gh/linkml/linkml/main?filepath=notebooks)\n[![DOI](https://zenodo.org/badge/13996/linkml/linkml.svg)](https://zenodo.org/badge/latestdoi/13996/linkml/linkml)\n[![PyPIDownloadsTotal](https://pepy.tech/badge/linkml)](https://pepy.tech/project/linkml)\n[![PyPIDownloadsMonth](https://img.shields.io/pypi/dm/linkml?logo=PyPI&color=blue)](https://pypi.org/project/linkml)\n[![codecov](https://codecov.io/gh/linkml/linkml/branch/main/graph/badge.svg?token=WNQNG986UN)](https://codecov.io/gh/linkml/linkml)\n\n\n# LinkML - Linked Data Modeling Language\n\nLinkML is a linked data modeling language following object-oriented and ontological principles. LinkML models are typically authored in YAML, and can be converted to other schema representation formats such as JSON or RDF.\n\nThis repo holds the tools for generating and working with LinkML. For the LinkML schema (metamodel), please see https://github.com/linkml/linkml-model\n\nThe complete documentation for LinkML can be found here:\n\n - [linkml.io/linkml](https://linkml.io/linkml)\n',
     'author': 'Chris Mungall',
     'author_email': 'cjmungall@lbl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://linkml.io/linkml/',
```

### Comparing `linkml-1.5.5/PKG-INFO` & `linkml-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml
-Version: 1.5.5
+Version: 1.5.6
 Summary: Linked Open Data Modeling Language
 Home-page: https://linkml.io/linkml/
 Keywords: schema,linked data,data modeling,rdf,owl,biolink
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.7.6,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,15 +29,15 @@
 Requires-Dist: graphviz (>=0.10.1)
 Requires-Dist: hbreader
 Requires-Dist: isodate (>=0.6.0)
 Requires-Dist: jinja2 (>=3.1.0)
 Requires-Dist: jsonasobj2 (>=1.0.3,<2.0.0)
 Requires-Dist: jsonschema[format] (>=4.0.0)
 Requires-Dist: linkml-dataops
-Requires-Dist: linkml-runtime (>=1.5.3)
+Requires-Dist: linkml-runtime (>=1.5.4)
 Requires-Dist: openpyxl
 Requires-Dist: parse
 Requires-Dist: prefixcommons (>=0.1.7)
 Requires-Dist: prefixmaps (>=0.1.3)
 Requires-Dist: pydantic
 Requires-Dist: pyjsg (>=0.11.6)
 Requires-Dist: pyshex (>=0.7.20)
```

