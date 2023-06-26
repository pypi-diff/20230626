# Comparing `tmp/metricflow-0.92.1.tar.gz` & `tmp/metricflow-0.93.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricflow-0.92.1.tar", max compression
+gzip compressed data, was "metricflow-0.93.0.tar", max compression
```

## Comparing `metricflow-0.92.1.tar` & `metricflow-0.93.0.tar`

### file list

```diff
@@ -1,655 +1,661 @@
--rw-r--r--   0        0        0    34523 2022-04-14 00:24:14.568413 metricflow-0.92.1/LICENSE
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/__init__.py
--rw-r--r--   0        0        0       28 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/cli/__init__.py
--rw-r--r--   0        0        0     5083 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/cli/cli_context.py
--rw-r--r--   0        0        0      137 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/cli/constants.py
--rw-r--r--   0        0        0    23046 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/cli/main.py
--rw-r--r--   0        0        0      595 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/cli/models.py
--rw-r--r--   0        0        0      351 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/cli/sample_models/countries.yaml
--rw-r--r--   0        0        0      529 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/cli/sample_models/customers.yaml
--rw-r--r--   0        0        0     4360 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/cli/sample_models/transactions.yaml
--rw-r--r--   0        0        0      268 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/cli/time_source.py
--rw-r--r--   0        0        0     7937 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/cli/tutorial.py
--rw-r--r--   0        0        0     7491 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/cli/utils.py
--rw-r--r--   0        0        0     1341 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/column_assoc.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/configuration/__init__.py
--rw-r--r--   0        0        0      699 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/configuration/config_builder.py
--rw-r--r--   0        0        0     1374 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/configuration/config_handler.py
--rw-r--r--   0        0        0      386 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/configuration/constants.py
--rw-r--r--   0        0        0     3597 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/configuration/env_var.py
--rw-r--r--   0        0        0     1639 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/configuration/yaml_handler.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/constraints/__init__.py
--rw-r--r--   0        0        0     4554 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/constraints/time_constraint.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dag/__init__.py
--rw-r--r--   0        0        0     4802 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dag/dag_to_text.py
--rw-r--r--   0        0        0     1864 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dag/dag_visualization.py
--rw-r--r--   0        0        0     3044 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dag/id_generation.py
--rw-r--r--   0        0        0     5389 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dag/mf_dag.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dataflow/__init__.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dataflow/builder/__init__.py
--rw-r--r--   0        0        0     6133 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dataflow/builder/costing.py
--rw-r--r--   0        0        0    32565 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dataflow/builder/dataflow_plan_builder.py
--rw-r--r--   0        0        0     4224 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dataflow/builder/node_data_set.py
--rw-r--r--   0        0        0    18866 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dataflow/builder/node_evaluator.py
--rw-r--r--   0        0        0     6319 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dataflow/builder/partitions.py
--rw-r--r--   0        0        0    29076 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dataflow/dataflow_plan.py
--rw-r--r--   0        0        0     1653 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dataflow/dataflow_plan_to_text.py
--rw-r--r--   0        0        0     1234 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dataflow/sql_table.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dataset/__init__.py
--rw-r--r--   0        0        0    21276 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dataset/convert_data_source.py
--rw-r--r--   0        0        0      917 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dataset/data_source_adapter.py
--rw-r--r--   0        0        0      600 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/dataset/dataset.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/engine/__init__.py
--rw-r--r--   0        0        0    21647 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/engine/metricflow_engine.py
--rw-r--r--   0        0        0      783 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/engine/utils.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.572413 metricflow-0.92.1/metricflow/errors/__init__.py
--rw-r--r--   0        0        0     2845 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/errors/errors.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/execution/__init__.py
--rw-r--r--   0        0        0     8172 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/execution/execution_plan.py
--rw-r--r--   0        0        0     1010 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/execution/execution_plan_to_text.py
--rw-r--r--   0        0        0     3009 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/execution/executor.py
--rw-r--r--   0        0        0     7956 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/instances.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/__init__.py
--rw-r--r--   0        0        0     2155 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/graph.py
--rw-r--r--   0        0        0     1513 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/model_transformer.py
--rw-r--r--   0        0        0     3638 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/model_validator.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/objects/__init__.py
--rw-r--r--   0        0        0     1836 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/objects/common.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/objects/constraints/__init__.py
--rw-r--r--   0        0        0     5174 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/objects/constraints/where.py
--rw-r--r--   0        0        0     4554 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/objects/data_source.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/objects/elements/__init__.py
--rw-r--r--   0        0        0     1445 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/objects/elements/dimension.py
--rw-r--r--   0        0        0     2207 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/objects/elements/identifier.py
--rw-r--r--   0        0        0     1917 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/objects/elements/measure.py
--rw-r--r--   0        0        0     1269 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/objects/materialization.py
--rw-r--r--   0        0        0     3975 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/objects/metric.py
--rw-r--r--   0        0        0      504 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/objects/user_configured_model.py
--rw-r--r--   0        0        0      994 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/objects/utils.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/parsing/__init__.py
--rw-r--r--   0        0        0    10245 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/parsing/dir_to_model.py
--rw-r--r--   0        0        0     9891 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/parsing/schemas.py
--rw-r--r--   0        0        0     3927 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/parsing/schemas_internal.py
--rw-r--r--   0        0        0     2522 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/parsing/validation.py
--rw-r--r--   0        0        0      124 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/parsing/yaml_file.py
--rw-r--r--   0        0        0     1468 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/parsing/yaml_loader.py
--rw-r--r--   0        0        0     1150 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/semantic_model.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/semantics/__init__.py
--rw-r--r--   0        0        0     1740 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/semantics/data_source_container.py
--rw-r--r--   0        0        0    27358 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/semantics/linkable_spec_resolver.py
--rw-r--r--   0        0        0     1613 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/semantics/links_new.py
--rw-r--r--   0        0        0    19194 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/semantics/semantic_containers.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/transformations/__init__.py
--rw-r--r--   0        0        0     1413 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/transformations/boolean_measure.py
--rw-r--r--   0        0        0     1364 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/transformations/identifiers.py
--rw-r--r--   0        0        0     1980 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/transformations/names.py
--rw-r--r--   0        0        0     2113 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/transformations/proxy_measure.py
--rw-r--r--   0        0        0      435 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/transformations/transform_rule.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/validations/__init__.py
--rw-r--r--   0        0        0     3410 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/validations/common_identifiers.py
--rw-r--r--   0        0        0     5661 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/validations/data_sources.py
--rw-r--r--   0        0        0    10225 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/validations/dim_names.py
--rw-r--r--   0        0        0     7055 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/validations/dimension_const.py
--rw-r--r--   0        0        0     5548 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/validations/element_const.py
--rw-r--r--   0        0        0     6083 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/validations/identifiers.py
--rw-r--r--   0        0        0     4526 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/validations/metrics.py
--rw-r--r--   0        0        0     2244 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/validations/non_empty.py
--rw-r--r--   0        0        0     6702 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/validations/unique_valid_name.py
--rw-r--r--   0        0        0     9787 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/model/validations/validator_helpers.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/naming/__init__.py
--rw-r--r--   0        0        0     2837 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/naming/linkable_spec_name.py
--rw-r--r--   0        0        0     6382 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/object_utils.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/plan_conversion/__init__.py
--rw-r--r--   0        0        0     4752 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/plan_conversion/column_resolver.py
--rw-r--r--   0        0        0     7103 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/plan_conversion/dataflow_to_execution.py
--rw-r--r--   0        0        0    61606 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/plan_conversion/dataflow_to_sql.py
--rw-r--r--   0        0        0    24459 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/plan_conversion/instance_converters.py
--rw-r--r--   0        0        0    10086 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/plan_conversion/node_processor.py
--rw-r--r--   0        0        0     2089 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/plan_conversion/select_column_gen.py
--rw-r--r--   0        0        0     7078 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/plan_conversion/spec_transforms.py
--rw-r--r--   0        0        0     5744 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/plan_conversion/sql_dataset.py
--rw-r--r--   0        0        0     3788 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/plan_conversion/time_spine.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/protocols/__init__.py
--rw-r--r--   0        0        0     6301 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/protocols/sql_client.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/py.typed
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/query/__init__.py
--rw-r--r--   0        0        0      137 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/query/query_exceptions.py
--rw-r--r--   0        0        0    36401 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/query/query_parser.py
--rw-r--r--   0        0        0      667 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/spec_set_transforms.py
--rw-r--r--   0        0        0    20040 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/specs.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/sql/__init__.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/sql/optimizer/__init__.py
--rw-r--r--   0        0        0    10064 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/sql/optimizer/column_pruner.py
--rw-r--r--   0        0        0     1761 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/sql/optimizer/optimization_levels.py
--rw-r--r--   0        0        0    29728 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/sql/optimizer/rewriting_sub_query_reducer.py
--rw-r--r--   0        0        0      377 2022-04-14 00:24:14.576413 metricflow-0.92.1/metricflow/sql/optimizer/sql_query_plan_optimizer.py
--rw-r--r--   0        0        0     8502 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql/optimizer/sub_query_reducer.py
--rw-r--r--   0        0        0     3356 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql/optimizer/table_alias_simplifier.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql/render/__init__.py
--rw-r--r--   0        0        0     2806 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql/render/big_query.py
--rw-r--r--   0        0        0    10341 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql/render/expr_renderer.py
--rw-r--r--   0        0        0      750 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql/render/redshift.py
--rw-r--r--   0        0        0    11294 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql/render/sql_plan_renderer.py
--rw-r--r--   0        0        0     2235 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql/render/sqlite.py
--rw-r--r--   0        0        0     1113 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql/sql_bind_parameters.py
--rw-r--r--   0        0        0    41788 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql/sql_exprs.py
--rw-r--r--   0        0        0     9902 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql/sql_plan.py
--rw-r--r--   0        0        0     1371 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql/sql_plan_to_text.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql_clients/__init__.py
--rw-r--r--   0        0        0     6603 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql_clients/base_sql_client_implementation.py
--rw-r--r--   0        0        0     3494 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql_clients/big_query.py
--rw-r--r--   0        0        0      693 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql_clients/common_client.py
--rw-r--r--   0        0        0     3104 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql_clients/redshift.py
--rw-r--r--   0        0        0     8839 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql_clients/snowflake.py
--rw-r--r--   0        0        0     4790 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql_clients/sql_utils.py
--rw-r--r--   0        0        0     4947 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql_clients/sqlalchemy_dialect.py
--rw-r--r--   0        0        0     4027 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/sql_clients/sqlite.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/telemetry/__init__.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/telemetry/handlers/__init__.py
--rw-r--r--   0        0        0     3624 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/telemetry/handlers/handlers.py
--rw-r--r--   0        0        0      725 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/telemetry/handlers/python_log.py
--rw-r--r--   0        0        0     2889 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/telemetry/models.py
--rw-r--r--   0        0        0     6141 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/telemetry/reporter.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/__init__.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/cli/__init__.py
--rw-r--r--   0        0        0     3033 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/cli/test_cli.py
--rw-r--r--   0        0        0     2177 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/compare_df.py
--rw-r--r--   0        0        0      579 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/conftest.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/constraints/__init__.py
--rw-r--r--   0        0        0      523 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/constraints/test_where.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/dataflow/__init__.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/dataflow/builder/__init__.py
--rw-r--r--   0        0        0     2264 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/dataflow/builder/test_costing.py
--rw-r--r--   0        0        0    19494 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/dataflow/builder/test_dataflow_plan_builder.py
--rw-r--r--   0        0        0     6996 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/dataflow/builder/test_node_data_set.py
--rw-r--r--   0        0        0    21186 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/dataflow/builder/test_node_evaluator.py
--rw-r--r--   0        0        0      933 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/dataflow/test_sql_table.py
--rw-r--r--   0        0        0     1247 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/dataflow_plan_to_svg.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/dataset/__init__.py
--rw-r--r--   0        0        0    10330 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/dataset/test_convert_data_source.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/execution/__init__.py
--rw-r--r--   0        0        0     1491 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/execution/noop_task.py
--rw-r--r--   0        0        0     2426 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/execution/test_sequential_executor.py
--rw-r--r--   0        0        0     2170 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/execution/test_tasks.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/__init__.py
--rw-r--r--   0        0        0     3307 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/cli_fixtures.py
--rw-r--r--   0        0        0     3263 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/dataflow_fixtures.py
--rw-r--r--   0        0        0     1654 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/id_fixtures.py
--rw-r--r--   0        0        0    11044 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_fixtures.py
--rw-r--r--   0        0        0      432 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/composite_identifier_model/materializations.yaml
--rw-r--r--   0        0        0      600 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/composite_identifier_model/messages_source.yaml
--rw-r--r--   0        0        0      444 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/composite_identifier_model/more_users_source.yaml
--rw-r--r--   0        0        0      704 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/composite_identifier_model/users_source.yaml
--rw-r--r--   0        0        0      568 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/extended_date_model/data_sources/bookings_from_sql_query_source.yaml
--rw-r--r--   0        0        0      468 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/extended_date_model/data_sources/bookings_monthly_source.yaml
--rw-r--r--   0        0        0      680 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/extended_date_model/data_sources/extended_bookings_source.yaml
--rw-r--r--   0        0        0      381 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/extended_date_model/data_sources/listings_extended_source.yaml
--rw-r--r--   0        0        0      488 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/join_types_model/bookings_source.yaml
--rw-r--r--   0        0        0      330 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/join_types_model/listings_source.yaml
--rw-r--r--   0        0        0      638 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/multi_hop_join_model/partitioned_data_sources/account_month_txns.yaml
--rw-r--r--   0        0        0      481 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/multi_hop_join_model/partitioned_data_sources/bridge_table.yaml
--rw-r--r--   0        0        0      507 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/multi_hop_join_model/partitioned_data_sources/customer_other_data.yaml
--rw-r--r--   0        0        0      505 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/multi_hop_join_model/partitioned_data_sources/customer_table.yaml
--rw-r--r--   0        0        0      451 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/multi_hop_join_model/partitioned_data_sources/third_hop_table.yaml
--rw-r--r--   0        0        0      494 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/multi_hop_join_model/unpartitioned_data_sources/account_month_txns.yaml
--rw-r--r--   0        0        0      337 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/multi_hop_join_model/unpartitioned_data_sources/bridge_table.yaml
--rw-r--r--   0        0        0      363 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/multi_hop_join_model/unpartitioned_data_sources/customer_other_data.yaml
--rw-r--r--   0        0        0      361 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/multi_hop_join_model/unpartitioned_data_sources/customer_table.yaml
--rw-r--r--   0        0        0      307 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/multi_hop_join_model/unpartitioned_data_sources/third_hop_table.yaml
--rw-r--r--   0        0        0      638 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/non_ds_model/bookings_source.yaml
--rw-r--r--   0        0        0      636 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/non_ds_model/listings_latest.yaml
--rw-r--r--   0        0        0     1359 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/data_sources/bookings_source.yaml
--rw-r--r--   0        0        0      421 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/data_sources/companies.yaml
--rw-r--r--   0        0        0      711 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/data_sources/id_verifications.yaml
--rw-r--r--   0        0        0      959 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/data_sources/listings_latest.yaml
--rw-r--r--   0        0        0      355 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/data_sources/lux_listing_mapping.yaml
--rw-r--r--   0        0        0      504 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/data_sources/revenue.yaml
--rw-r--r--   0        0        0      628 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/data_sources/user_ds_source.yaml
--rw-r--r--   0        0        0      424 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/data_sources/users_latest.yaml
--rw-r--r--   0        0        0      855 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/data_sources/views_source.yaml
--rw-r--r--   0        0        0     2607 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/materializations.yaml
--rw-r--r--   0        0        0     6205 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/metrics.yaml
--rw-r--r--   0        0        0     3192 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/setup_fixtures.py
--rw-r--r--   0        0        0     1546 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/sql_client_fixtures.py
--rw-r--r--   0        0        0      280 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/sql_fixtures.py
--rw-r--r--   0        0        0    19919 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/fixtures/table_fixtures.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/integration/__init__.py
--rw-r--r--   0        0        0     6212 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/integration/configured_test_case.py
--rw-r--r--   0        0        0     1729 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/integration/conftest.py
--rw-r--r--   0        0        0     5256 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/integration/test_cases/itest_composite_identifier.yaml
--rw-r--r--   0        0        0     3739 2022-04-14 00:24:14.580413 metricflow-0.92.1/metricflow/test/integration/test_cases/itest_constraints.yaml
--rw-r--r--   0        0        0     9546 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_cases/itest_cumulative_metric.yaml
--rw-r--r--   0        0        0     3909 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_cases/itest_dimensions.yaml
--rw-r--r--   0        0        0     1053 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_cases/itest_dundered_identifiers.yaml
--rw-r--r--   0        0        0    11208 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_cases/itest_granularity.yaml
--rw-r--r--   0        0        0     1241 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_cases/itest_joins.yaml
--rw-r--r--   0        0        0     1927 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_cases/itest_measure_aggregations.yaml
--rw-r--r--   0        0        0    11456 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_cases/itest_metrics.yaml
--rw-r--r--   0        0        0     5422 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_cases/itest_multi_hop_join.yaml
--rw-r--r--   0        0        0     1615 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_cases/itest_order_limit.yaml
--rw-r--r--   0        0        0     2901 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_cases/itest_partitions.yaml
--rw-r--r--   0        0        0     4098 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_cases/itest_simple.yaml
--rw-r--r--   0        0        0      693 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_cases/itest_simple_non_ds.yaml
--rw-r--r--   0        0        0     9100 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_configured_cases.py
--rw-r--r--   0        0        0     2601 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_rendered_query.py
--rw-r--r--   0        0        0     1445 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/integration/test_write_to_table.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/model/__init__.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/model/semantics/__init__.py
--rw-r--r--   0        0        0     2432 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/model/semantics/test_linkable_spec_resolver.py
--rw-r--r--   0        0        0     5934 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/model/test_data_source_container.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/model/validations/__init__.py
--rw-r--r--   0        0        0     1256 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/model/validations/test_common_identifiers.py
--rw-r--r--   0        0        0     1144 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/model/validations/test_data_sources.py
--rw-r--r--   0        0        0     1163 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/model/validations/test_dim_names.py
--rw-r--r--   0        0        0     7492 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/model/validations/test_dimension_const.py
--rw-r--r--   0        0        0     2445 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/model/validations/test_element_const.py
--rw-r--r--   0        0        0     9680 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/model/validations/test_identifiers.py
--rw-r--r--   0        0        0     1629 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/model/validations/test_measures.py
--rw-r--r--   0        0        0     8382 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/model/validations/test_metrics.py
--rw-r--r--   0        0        0    10625 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/model/validations/test_unique_valid_name.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/plan_conversion/__init__.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/plan_conversion/instance_converters/__init__.py
--rw-r--r--   0        0        0     6919 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/plan_conversion/instance_converters/test_create_select_columns_with_measures_aggregated.py
--rw-r--r--   0        0        0     7219 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/plan_conversion/test_dataflow_to_execution.py
--rw-r--r--   0        0        0    43436 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/plan_conversion/test_dataflow_to_sql_plan.py
--rw-r--r--   0        0        0     1373 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/plan_conversion/test_time_spine.py
--rw-r--r--   0        0        0    10672 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/plan_utils.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/prototype_utils.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/query/__init__.py
--rw-r--r--   0        0        0     7544 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/query/test_query_parser.py
--rw-r--r--   0        0        0     2842 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/query/test_query_parser_suggestions.py
--rw-r--r--   0        0        0      463 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_dont_prune_if_in_where__after_pruning.sql
--rw-r--r--   0        0        0      525 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_dont_prune_if_in_where__before_pruning.sql
--rw-r--r--   0        0        0      494 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_dont_prune_with_str_expr__after_pruning.sql
--rw-r--r--   0        0        0      494 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_dont_prune_with_str_expr__before_pruning.sql
--rw-r--r--   0        0        0      727 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_no_pruning__after_pruning.sql
--rw-r--r--   0        0        0      727 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_no_pruning__before_pruning.sql
--rw-r--r--   0        0        0      608 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_from_source__after_pruning.sql
--rw-r--r--   0        0        0      637 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_from_source__before_pruning.sql
--rw-r--r--   0        0        0      192 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_grandparents__after_pruning.sql
--rw-r--r--   0        0        0      210 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_grandparents__before_pruning.sql
--rw-r--r--   0        0        0      271 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_grandparents_in_join_query__after_pruning.sql
--rw-r--r--   0        0        0      289 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_grandparents_in_join_query__before_pruning.sql
--rw-r--r--   0        0        0      598 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_joined_source__after_pruning.sql
--rw-r--r--   0        0        0      629 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_joined_source__before_pruning.sql
--rw-r--r--   0        0        0      430 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_str_expr__after_pruning.sql
--rw-r--r--   0        0        0      498 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_str_expr__before_pruning.sql
--rw-r--r--   0        0        0      434 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_with_str_expr__after_pruning.sql
--rw-r--r--   0        0        0      494 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_with_str_expr__before_pruning.sql
--rw-r--r--   0        0        0      548 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/BigQuerySqlClient/test_convert_query_data_source__plan0.sql
--rw-r--r--   0        0        0     2071 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/BigQuerySqlClient/test_convert_table_data_source_with_measures__plan0.sql
--rw-r--r--   0        0        0      891 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/BigQuerySqlClient/test_convert_table_data_source_without_measures__plan0.sql
--rw-r--r--   0        0        0      550 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/RedshiftSqlClient/test_convert_query_data_source__plan0.sql
--rw-r--r--   0        0        0     2079 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/RedshiftSqlClient/test_convert_table_data_source_with_measures__plan0.sql
--rw-r--r--   0        0        0      895 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/RedshiftSqlClient/test_convert_table_data_source_without_measures__plan0.sql
--rw-r--r--   0        0        0      550 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SnowflakeSqlClient/test_convert_query_data_source__plan0.sql
--rw-r--r--   0        0        0     2079 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SnowflakeSqlClient/test_convert_table_data_source_with_measures__plan0.sql
--rw-r--r--   0        0        0      895 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SnowflakeSqlClient/test_convert_table_data_source_without_measures__plan0.sql
--rw-r--r--   0        0        0      474 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SqliteSqlClient/test_convert_query_data_source__plan0.sql
--rw-r--r--   0        0        0     1663 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SqliteSqlClient/test_convert_table_data_source_with_measures__plan0.sql
--rw-r--r--   0        0        0      767 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SqliteSqlClient/test_convert_table_data_source_without_measures__plan0.sql
--rw-r--r--   0        0        0     2209 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_cumulative_metric__dfp_0.xml
--rw-r--r--   0        0        0     7389 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_distinct_values_plan__dfp_0.xml
--rw-r--r--   0        0        0     6268 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_expr_metrics_plan__dfp_0.xml
--rw-r--r--   0        0        0     5960 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_joined_plan__dfp_0.xml
--rw-r--r--   0        0        0     2199 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_limit_rows_plan__dfp_0.xml
--rw-r--r--   0        0        0    14843 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_multi_data_source_ratio_metrics_plan__dfp_0.xml
--rw-r--r--   0        0        0    21417 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_multihop_join_plan__dfp_0.xml
--rw-r--r--   0        0        0     4585 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_multiple_metrics_plan__dfp_0.xml
--rw-r--r--   0        0        0     2918 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_order_by_plan__dfp_0.xml
--rw-r--r--   0        0        0     1789 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_simple_plan__dfp_0.xml
--rw-r--r--   0        0        0     6469 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_single_data_source_ratio_metrics_plan__dfp_0.xml
--rw-r--r--   0        0        0     8627 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_where_constrained_plan__dfp_0.xml
--rw-r--r--   0        0        0     4454 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_where_constrained_plan_time_dimension__dfp_0.xml
--rw-r--r--   0        0        0     7129 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_where_constrained_with_common_linkable_plan__dfp_0.xml
--rw-r--r--   0        0        0     9336 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_combined_metrics_plan__ep_0.xml
--rw-r--r--   0        0        0     3100 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_joined_plan__ep_0.xml
--rw-r--r--   0        0        0     3820 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_multihop_joined_plan__ep_0.xml
--rw-r--r--   0        0        0     4045 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_small_combined_metrics_plan__ep_0.xml
--rw-r--r--   0        0        0     9336 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_combined_metrics_plan__ep_0.xml
--rw-r--r--   0        0        0     3100 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_joined_plan__ep_0.xml
--rw-r--r--   0        0        0     3820 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_multihop_joined_plan__ep_0.xml
--rw-r--r--   0        0        0     4045 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_small_combined_metrics_plan__ep_0.xml
--rw-r--r--   0        0        0     9336 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_combined_metrics_plan__ep_0.xml
--rw-r--r--   0        0        0     3100 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_joined_plan__ep_0.xml
--rw-r--r--   0        0        0     3820 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_multihop_joined_plan__ep_0.xml
--rw-r--r--   0        0        0     4045 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_small_combined_metrics_plan__ep_0.xml
--rw-r--r--   0        0        0     9336 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_combined_metrics_plan__ep_0.xml
--rw-r--r--   0        0        0     3100 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_joined_plan__ep_0.xml
--rw-r--r--   0        0        0     3820 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_multihop_joined_plan__ep_0.xml
--rw-r--r--   0        0        0     4045 2022-04-14 00:24:14.584413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_small_combined_metrics_plan__ep_0.xml
--rw-r--r--   0        0        0     4377 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/DataflowPlan/test_compute_metrics_node_simple_expr__plan0.xml
--rw-r--r--   0        0        0     1876 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier__plan0.sql
--rw-r--r--   0        0        0      498 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier__plan0_optimized.sql
--rw-r--r--   0        0        0     6616 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_join__plan0.sql
--rw-r--r--   0        0        0      982 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_join__plan0_optimized.sql
--rw-r--r--   0        0        0     2171 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_order_by__plan0.sql
--rw-r--r--   0        0        0      584 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql
--rw-r--r--   0        0        0     6799 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node__plan0.sql
--rw-r--r--   0        0        0      726 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node__plan0_optimized.sql
--rw-r--r--   0        0        0    15499 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql
--rw-r--r--   0        0        0     2411 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql
--rw-r--r--   0        0        0     7002 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql
--rw-r--r--   0        0        0     1016 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql
--rw-r--r--   0        0        0     6850 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_simple_expr__plan0.sql
--rw-r--r--   0        0        0      747 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql
--rw-r--r--   0        0        0     3445 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_constrain_primary_time_dimension__plan0.sql
--rw-r--r--   0        0        0      415 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_constrain_primary_time_dimension__plan0_optimized.sql
--rw-r--r--   0        0        0     1639 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric__plan0.sql
--rw-r--r--   0        0        0      698 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric__plan0_optimized.sql
--rw-r--r--   0        0        0     1599 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_grain_to_date__plan0.sql
--rw-r--r--   0        0        0      658 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql
--rw-r--r--   0        0        0      942 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_ds__plan0.sql
--rw-r--r--   0        0        0      307 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_ds__plan0_optimized.sql
--rw-r--r--   0        0        0     1508 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window__plan0.sql
--rw-r--r--   0        0        0      552 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window__plan0_optimized.sql
--rw-r--r--   0        0        0     2557 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql
--rw-r--r--   0        0        0     1233 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql
--rw-r--r--   0        0        0     2696 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_with_time_constraint__plan0.sql
--rw-r--r--   0        0        0     1350 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql
--rw-r--r--   0        0        0     7886 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_distinct_values__plan0.sql
--rw-r--r--   0        0        0      697 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_distinct_values__plan0_optimized.sql
--rw-r--r--   0        0        0     3092 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_node__plan0.sql
--rw-r--r--   0        0        0      236 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_node__plan0_optimized.sql
--rw-r--r--   0        0        0     3320 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_with_where_constraint_node__plan0.sql
--rw-r--r--   0        0        0      365 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_with_where_constraint_node__plan0_optimized.sql
--rw-r--r--   0        0        0     8009 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql
--rw-r--r--   0        0        0     1057 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql
--rw-r--r--   0        0        0     3741 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_limit_rows__plan0.sql
--rw-r--r--   0        0        0      429 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_limit_rows__plan0_optimized.sql
--rw-r--r--   0        0        0     2989 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_local_dimension_using_local_identifier__plan0.sql
--rw-r--r--   0        0        0      446 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_local_dimension_using_local_identifier__plan0_optimized.sql
--rw-r--r--   0        0        0     3572 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_measure_aggregation_node__plan0.sql
--rw-r--r--   0        0        0      475 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_measure_aggregation_node__plan0_optimized.sql
--rw-r--r--   0        0        0     8764 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multi_join_node__plan0.sql
--rw-r--r--   0        0        0     1166 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multi_join_node__plan0_optimized.sql
--rw-r--r--   0        0        0     9999 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multihop_node__plan0.sql
--rw-r--r--   0        0        0     1255 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multihop_node__plan0_optimized.sql
--rw-r--r--   0        0        0     3922 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_order_by_node__plan0.sql
--rw-r--r--   0        0        0      517 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_order_by_node__plan0_optimized.sql
--rw-r--r--   0        0        0     6724 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_partitioned_join__plan0.sql
--rw-r--r--   0        0        0      863 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_partitioned_join__plan0_optimized.sql
--rw-r--r--   0        0        0     6046 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_single_join_node__plan0.sql
--rw-r--r--   0        0        0      617 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_single_join_node__plan0_optimized.sql
--rw-r--r--   0        0        0     2926 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_source_node__plan0.sql
--rw-r--r--   0        0        0     2042 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_source_node__plan0_optimized.sql
--rw-r--r--   0        0        0     1880 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier__plan0.sql
--rw-r--r--   0        0        0      498 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier__plan0_optimized.sql
--rw-r--r--   0        0        0     6628 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_join__plan0.sql
--rw-r--r--   0        0        0     1008 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_join__plan0_optimized.sql
--rw-r--r--   0        0        0     2175 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_order_by__plan0.sql
--rw-r--r--   0        0        0      584 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql
--rw-r--r--   0        0        0     6815 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node__plan0.sql
--rw-r--r--   0        0        0      743 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node__plan0_optimized.sql
--rw-r--r--   0        0        0    15549 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql
--rw-r--r--   0        0        0     2465 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql
--rw-r--r--   0        0        0     7036 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql
--rw-r--r--   0        0        0     1051 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql
--rw-r--r--   0        0        0     6866 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_simple_expr__plan0.sql
--rw-r--r--   0        0        0      786 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql
--rw-r--r--   0        0        0     3455 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_constrain_primary_time_dimension__plan0.sql
--rw-r--r--   0        0        0      417 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_constrain_primary_time_dimension__plan0_optimized.sql
--rw-r--r--   0        0        0     1619 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric__plan0.sql
--rw-r--r--   0        0        0      699 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric__plan0_optimized.sql
--rw-r--r--   0        0        0     1618 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_grain_to_date__plan0.sql
--rw-r--r--   0        0        0      698 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql
--rw-r--r--   0        0        0      944 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_ds__plan0.sql
--rw-r--r--   0        0        0      307 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_ds__plan0_optimized.sql
--rw-r--r--   0        0        0     1514 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window__plan0.sql
--rw-r--r--   0        0        0      577 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window__plan0_optimized.sql
--rw-r--r--   0        0        0     2569 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql
--rw-r--r--   0        0        0     1265 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql
--rw-r--r--   0        0        0     2682 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_with_time_constraint__plan0.sql
--rw-r--r--   0        0        0     1356 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql
--rw-r--r--   0        0        0     7902 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_distinct_values__plan0.sql
--rw-r--r--   0        0        0      707 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_distinct_values__plan0_optimized.sql
--rw-r--r--   0        0        0     3100 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_node__plan0.sql
--rw-r--r--   0        0        0      236 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_node__plan0_optimized.sql
--rw-r--r--   0        0        0     3328 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_with_where_constraint_node__plan0.sql
--rw-r--r--   0        0        0      365 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_with_where_constraint_node__plan0_optimized.sql
--rw-r--r--   0        0        0     8025 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql
--rw-r--r--   0        0        0     1057 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql
--rw-r--r--   0        0        0     3749 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_limit_rows__plan0.sql
--rw-r--r--   0        0        0      429 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_limit_rows__plan0_optimized.sql
--rw-r--r--   0        0        0     2997 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_local_dimension_using_local_identifier__plan0.sql
--rw-r--r--   0        0        0      446 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_local_dimension_using_local_identifier__plan0_optimized.sql
--rw-r--r--   0        0        0     3580 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_measure_aggregation_node__plan0.sql
--rw-r--r--   0        0        0      475 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_measure_aggregation_node__plan0_optimized.sql
--rw-r--r--   0        0        0     8788 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multi_join_node__plan0.sql
--rw-r--r--   0        0        0     1166 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multi_join_node__plan0_optimized.sql
--rw-r--r--   0        0        0    10015 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multihop_node__plan0.sql
--rw-r--r--   0        0        0     1251 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multihop_node__plan0_optimized.sql
--rw-r--r--   0        0        0     3930 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_order_by_node__plan0.sql
--rw-r--r--   0        0        0      517 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_order_by_node__plan0_optimized.sql
--rw-r--r--   0        0        0     6744 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_partitioned_join__plan0.sql
--rw-r--r--   0        0        0      883 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_partitioned_join__plan0_optimized.sql
--rw-r--r--   0        0        0     6062 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_single_join_node__plan0.sql
--rw-r--r--   0        0        0      617 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_single_join_node__plan0_optimized.sql
--rw-r--r--   0        0        0     2934 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_source_node__plan0.sql
--rw-r--r--   0        0        0     2050 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_source_node__plan0_optimized.sql
--rw-r--r--   0        0        0     1880 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier__plan0.sql
--rw-r--r--   0        0        0      498 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier__plan0_optimized.sql
--rw-r--r--   0        0        0     6628 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_join__plan0.sql
--rw-r--r--   0        0        0     1008 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_join__plan0_optimized.sql
--rw-r--r--   0        0        0     2175 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_order_by__plan0.sql
--rw-r--r--   0        0        0      584 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql
--rw-r--r--   0        0        0     6815 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node__plan0.sql
--rw-r--r--   0        0        0      743 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node__plan0_optimized.sql
--rw-r--r--   0        0        0    15529 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql
--rw-r--r--   0        0        0     2445 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql
--rw-r--r--   0        0        0     7016 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql
--rw-r--r--   0        0        0     1031 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql
--rw-r--r--   0        0        0     6866 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_simple_expr__plan0.sql
--rw-r--r--   0        0        0      786 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql
--rw-r--r--   0        0        0     3455 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_constrain_primary_time_dimension__plan0.sql
--rw-r--r--   0        0        0      417 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_constrain_primary_time_dimension__plan0_optimized.sql
--rw-r--r--   0        0        0     1619 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric__plan0.sql
--rw-r--r--   0        0        0      699 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric__plan0_optimized.sql
--rw-r--r--   0        0        0     1618 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_grain_to_date__plan0.sql
--rw-r--r--   0        0        0      698 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql
--rw-r--r--   0        0        0      944 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_ds__plan0.sql
--rw-r--r--   0        0        0      307 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_ds__plan0_optimized.sql
--rw-r--r--   0        0        0     1514 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window__plan0.sql
--rw-r--r--   0        0        0      577 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window__plan0_optimized.sql
--rw-r--r--   0        0        0     2569 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql
--rw-r--r--   0        0        0     1265 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql
--rw-r--r--   0        0        0     2682 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_with_time_constraint__plan0.sql
--rw-r--r--   0        0        0     1356 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql
--rw-r--r--   0        0        0     7902 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_distinct_values__plan0.sql
--rw-r--r--   0        0        0      707 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_distinct_values__plan0_optimized.sql
--rw-r--r--   0        0        0     3100 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_node__plan0.sql
--rw-r--r--   0        0        0      236 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_node__plan0_optimized.sql
--rw-r--r--   0        0        0     3328 2022-04-14 00:24:14.588413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_with_where_constraint_node__plan0.sql
--rw-r--r--   0        0        0      365 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_with_where_constraint_node__plan0_optimized.sql
--rw-r--r--   0        0        0     8025 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql
--rw-r--r--   0        0        0     1057 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql
--rw-r--r--   0        0        0     3749 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_limit_rows__plan0.sql
--rw-r--r--   0        0        0      429 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_limit_rows__plan0_optimized.sql
--rw-r--r--   0        0        0     2997 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_local_dimension_using_local_identifier__plan0.sql
--rw-r--r--   0        0        0      446 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_local_dimension_using_local_identifier__plan0_optimized.sql
--rw-r--r--   0        0        0     3580 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_measure_aggregation_node__plan0.sql
--rw-r--r--   0        0        0      475 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_measure_aggregation_node__plan0_optimized.sql
--rw-r--r--   0        0        0     8788 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multi_join_node__plan0.sql
--rw-r--r--   0        0        0     1166 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multi_join_node__plan0_optimized.sql
--rw-r--r--   0        0        0    10015 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multihop_node__plan0.sql
--rw-r--r--   0        0        0     1251 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multihop_node__plan0_optimized.sql
--rw-r--r--   0        0        0     3930 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_order_by_node__plan0.sql
--rw-r--r--   0        0        0      517 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_order_by_node__plan0_optimized.sql
--rw-r--r--   0        0        0     6744 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_partitioned_join__plan0.sql
--rw-r--r--   0        0        0      883 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_partitioned_join__plan0_optimized.sql
--rw-r--r--   0        0        0     6062 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_single_join_node__plan0.sql
--rw-r--r--   0        0        0      617 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_single_join_node__plan0_optimized.sql
--rw-r--r--   0        0        0     2934 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_source_node__plan0.sql
--rw-r--r--   0        0        0     2050 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_source_node__plan0_optimized.sql
--rw-r--r--   0        0        0     1728 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier__plan0.sql
--rw-r--r--   0        0        0      498 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier__plan0_optimized.sql
--rw-r--r--   0        0        0     6092 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_join__plan0.sql
--rw-r--r--   0        0        0     1008 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_join__plan0_optimized.sql
--rw-r--r--   0        0        0     2023 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_order_by__plan0.sql
--rw-r--r--   0        0        0      584 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql
--rw-r--r--   0        0        0     5983 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node__plan0.sql
--rw-r--r--   0        0        0      743 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node__plan0_optimized.sql
--rw-r--r--   0        0        0    13913 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql
--rw-r--r--   0        0        0     2445 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql
--rw-r--r--   0        0        0     6184 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql
--rw-r--r--   0        0        0     1031 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql
--rw-r--r--   0        0        0     6034 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_simple_expr__plan0.sql
--rw-r--r--   0        0        0      786 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql
--rw-r--r--   0        0        0     3045 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_constrain_primary_time_dimension__plan0.sql
--rw-r--r--   0        0        0      407 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_constrain_primary_time_dimension__plan0_optimized.sql
--rw-r--r--   0        0        0     1541 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric__plan0.sql
--rw-r--r--   0        0        0      673 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric__plan0_optimized.sql
--rw-r--r--   0        0        0     1534 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_grain_to_date__plan0.sql
--rw-r--r--   0        0        0      666 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql
--rw-r--r--   0        0        0      868 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_ds__plan0.sql
--rw-r--r--   0        0        0      307 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_ds__plan0_optimized.sql
--rw-r--r--   0        0        0     1438 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window__plan0.sql
--rw-r--r--   0        0        0      572 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window__plan0_optimized.sql
--rw-r--r--   0        0        0     2463 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql
--rw-r--r--   0        0        0     1248 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql
--rw-r--r--   0        0        0     2574 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_with_time_constraint__plan0.sql
--rw-r--r--   0        0        0     1337 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql
--rw-r--r--   0        0        0     7070 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_distinct_values__plan0.sql
--rw-r--r--   0        0        0      707 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_distinct_values__plan0_optimized.sql
--rw-r--r--   0        0        0     2700 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_node__plan0.sql
--rw-r--r--   0        0        0      236 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_node__plan0_optimized.sql
--rw-r--r--   0        0        0     2928 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_with_where_constraint_node__plan0.sql
--rw-r--r--   0        0        0      365 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_with_where_constraint_node__plan0_optimized.sql
--rw-r--r--   0        0        0     7193 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql
--rw-r--r--   0        0        0     1057 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql
--rw-r--r--   0        0        0     3349 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_limit_rows__plan0.sql
--rw-r--r--   0        0        0      429 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_limit_rows__plan0_optimized.sql
--rw-r--r--   0        0        0     2565 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_local_dimension_using_local_identifier__plan0.sql
--rw-r--r--   0        0        0      446 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_local_dimension_using_local_identifier__plan0_optimized.sql
--rw-r--r--   0        0        0     3180 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_measure_aggregation_node__plan0.sql
--rw-r--r--   0        0        0      475 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_measure_aggregation_node__plan0_optimized.sql
--rw-r--r--   0        0        0     7524 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multi_join_node__plan0.sql
--rw-r--r--   0        0        0     1166 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multi_join_node__plan0_optimized.sql
--rw-r--r--   0        0        0     9231 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multihop_node__plan0.sql
--rw-r--r--   0        0        0     1251 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multihop_node__plan0_optimized.sql
--rw-r--r--   0        0        0     3530 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_order_by_node__plan0.sql
--rw-r--r--   0        0        0      517 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_order_by_node__plan0_optimized.sql
--rw-r--r--   0        0        0     5712 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_partitioned_join__plan0.sql
--rw-r--r--   0        0        0      883 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_partitioned_join__plan0_optimized.sql
--rw-r--r--   0        0        0     5230 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_single_join_node__plan0.sql
--rw-r--r--   0        0        0      617 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_single_join_node__plan0_optimized.sql
--rw-r--r--   0        0        0     2534 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_source_node__plan0.sql
--rw-r--r--   0        0        0     2066 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_source_node__plan0_optimized.sql
--rw-r--r--   0        0        0    11288 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_composite_identifier__plan0.xml
--rw-r--r--   0        0        0    35872 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_composite_identifier_with_join__plan0.xml
--rw-r--r--   0        0        0    13595 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_composite_identifier_with_order_by__plan0.xml
--rw-r--r--   0        0        0    33841 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node__plan0.xml
--rw-r--r--   0        0        0    79506 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.xml
--rw-r--r--   0        0        0    34942 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node_ratio_from_single_data_source__plan0.xml
--rw-r--r--   0        0        0    33940 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node_simple_expr__plan0.xml
--rw-r--r--   0        0        0    15272 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_constrain_primary_time_dimension__plan0.xml
--rw-r--r--   0        0        0     9065 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric__plan0.xml
--rw-r--r--   0        0        0     9065 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_grain_to_date__plan0.xml
--rw-r--r--   0        0        0     4867 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_no_ds__plan0.xml
--rw-r--r--   0        0        0     9065 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_no_window__plan0.xml
--rw-r--r--   0        0        0    13917 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_no_window_with_time_constraint__plan0.xml
--rw-r--r--   0        0        0    13905 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_with_time_constraint__plan0.xml
--rw-r--r--   0        0        0    40126 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_distinct_values__plan0.xml
--rw-r--r--   0        0        0    13320 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_filter_node__plan0.xml
--rw-r--r--   0        0        0    15261 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_filter_with_where_constraint_node__plan0.xml
--rw-r--r--   0        0        0    42120 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_filter_with_where_constraint_on_join_dim__plan0.xml
--rw-r--r--   0        0        0    18678 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_limit_rows__plan0.xml
--rw-r--r--   0        0        0    14904 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_local_dimension_using_local_identifier__plan0.xml
--rw-r--r--   0        0        0    16720 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_measure_aggregation_node__plan0.xml
--rw-r--r--   0        0        0    40964 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_multi_join_node__plan0.xml
--rw-r--r--   0        0        0    49219 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_multihop_node__plan0.xml
--rw-r--r--   0        0        0    20916 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_order_by_node__plan0.xml
--rw-r--r--   0        0        0    32547 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_partitioned_join__plan0.xml
--rw-r--r--   0        0        0    28042 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_single_join_node__plan0.xml
--rw-r--r--   0        0        0    12099 2022-04-14 00:24:14.592413 metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_source_node__plan0.xml
--rw-r--r--   0        0        0      100 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_engine_specific_rendering.py/SqlQueryPlan/BigQuerySqlClient/test_cast_to_timestamp__plan0.sql
--rw-r--r--   0        0        0      101 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_engine_specific_rendering.py/SqlQueryPlan/RedshiftSqlClient/test_cast_to_timestamp__plan0.sql
--rw-r--r--   0        0        0      101 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_engine_specific_rendering.py/SqlQueryPlan/SnowflakeSqlClient/test_cast_to_timestamp__plan0.sql
--rw-r--r--   0        0        0       96 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_engine_specific_rendering.py/SqlQueryPlan/SqliteSqlClient/test_cast_to_timestamp__plan0.sql
--rw-r--r--   0        0        0      572 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/BigQuerySqlClient/test_render_query__query0.sql
--rw-r--r--   0        0        0      681 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/BigQuerySqlClient/test_render_write_to_table_query__query0.sql
--rw-r--r--   0        0        0      574 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/RedshiftSqlClient/test_render_query__query0.sql
--rw-r--r--   0        0        0      683 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/RedshiftSqlClient/test_render_write_to_table_query__query0.sql
--rw-r--r--   0        0        0      574 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SnowflakeSqlClient/test_render_query__query0.sql
--rw-r--r--   0        0        0      683 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SnowflakeSqlClient/test_render_write_to_table_query__query0.sql
--rw-r--r--   0        0        0      564 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SqliteSqlClient/test_render_query__query0.sql
--rw-r--r--   0        0        0      673 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SqliteSqlClient/test_render_write_to_table_query__query0.sql
--rw-r--r--   0        0        0      655 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_colliding_alias__after_reducing.sql
--rw-r--r--   0        0        0      655 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_colliding_alias__before_reducing.sql
--rw-r--r--   0        0        0      575 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_all_join_sources__after_reducing.sql
--rw-r--r--   0        0        0     1003 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_all_join_sources__before_reducing.sql
--rw-r--r--   0        0        0      504 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_join__after_reducing.sql
--rw-r--r--   0        0        0      641 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_join__before_reducing.sql
--rw-r--r--   0        0        0      205 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_sub_query__after_reducing.sql
--rw-r--r--   0        0        0      354 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_sub_query__before_reducing.sql
--rw-r--r--   0        0        0       62 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_component_rendering__plan0.sql
--rw-r--r--   0        0        0      127 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_component_rendering__plan1.sql
--rw-r--r--   0        0        0      189 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_component_rendering__plan2.sql
--rw-r--r--   0        0        0      254 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_component_rendering__plan3.sql
--rw-r--r--   0        0        0      275 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_component_rendering__plan4.sql
--rw-r--r--   0        0        0      289 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_component_rendering__plan5.sql
--rw-r--r--   0        0        0       62 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_render_limit__plan0.sql
--rw-r--r--   0        0        0      116 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_render_order_by__plan0.sql
--rw-r--r--   0        0        0       87 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_render_where__plan0.sql
--rw-r--r--   0        0        0       62 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_component_rendering__plan0.sql
--rw-r--r--   0        0        0      127 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_component_rendering__plan1.sql
--rw-r--r--   0        0        0      189 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_component_rendering__plan2.sql
--rw-r--r--   0        0        0      254 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_component_rendering__plan3.sql
--rw-r--r--   0        0        0      275 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_component_rendering__plan4.sql
--rw-r--r--   0        0        0      289 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_component_rendering__plan5.sql
--rw-r--r--   0        0        0       62 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_render_limit__plan0.sql
--rw-r--r--   0        0        0      116 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_render_order_by__plan0.sql
--rw-r--r--   0        0        0       87 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_render_where__plan0.sql
--rw-r--r--   0        0        0       62 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_component_rendering__plan0.sql
--rw-r--r--   0        0        0      127 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_component_rendering__plan1.sql
--rw-r--r--   0        0        0      189 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_component_rendering__plan2.sql
--rw-r--r--   0        0        0      254 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_component_rendering__plan3.sql
--rw-r--r--   0        0        0      275 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_component_rendering__plan4.sql
--rw-r--r--   0        0        0      289 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_component_rendering__plan5.sql
--rw-r--r--   0        0        0       62 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_render_limit__plan0.sql
--rw-r--r--   0        0        0      116 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_render_order_by__plan0.sql
--rw-r--r--   0        0        0       87 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_render_where__plan0.sql
--rw-r--r--   0        0        0       62 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_component_rendering__plan0.sql
--rw-r--r--   0        0        0      127 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_component_rendering__plan1.sql
--rw-r--r--   0        0        0      189 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_component_rendering__plan2.sql
--rw-r--r--   0        0        0      254 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_component_rendering__plan3.sql
--rw-r--r--   0        0        0      275 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_component_rendering__plan4.sql
--rw-r--r--   0        0        0      289 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_component_rendering__plan5.sql
--rw-r--r--   0        0        0       62 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_render_limit__plan0.sql
--rw-r--r--   0        0        0      116 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_render_order_by__plan0.sql
--rw-r--r--   0        0        0       87 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_render_where__plan0.sql
--rw-r--r--   0        0        0      117 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sub_query_reducer.py/SqlQueryPlan/test_reduce_sub_query__after_reducing.sql
--rw-r--r--   0        0        0      257 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sub_query_reducer.py/SqlQueryPlan/test_reduce_sub_query__before_reducing.sql
--rw-r--r--   0        0        0      167 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sub_query_reducer.py/SqlQueryPlan/test_rewrite_order_by_with_a_join_in_parent__after_reducing.sql
--rw-r--r--   0        0        0      232 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_sub_query_reducer.py/SqlQueryPlan/test_rewrite_order_by_with_a_join_in_parent__before_reducing.sql
--rw-r--r--   0        0        0      403 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_table_alias_simplifier.py/SqlQueryPlan/test_table_alias_simplification__after_alias_simplification.sql
--rw-r--r--   0        0        0      479 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/snapshots/test_table_alias_simplifier.py/SqlQueryPlan/test_table_alias_simplification__before_alias_simplification.sql
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/sql/__init__.py
--rw-r--r--   0        0        0     3390 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/sql/compare_sql_plan.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/sql/optimizer/__init__.py
--rw-r--r--   0        0        0    34136 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/sql/optimizer/test_column_pruner.py
--rw-r--r--   0        0        0    29034 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/sql/optimizer/test_rewriting_sub_query_reducer.py
--rw-r--r--   0        0        0     8944 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/sql/optimizer/test_sub_query_reducer.py
--rw-r--r--   0        0        0     6274 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/sql/optimizer/test_table_alias_simplifier.py
--rw-r--r--   0        0        0     1988 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/sql/test_engine_specific_rendering.py
--rw-r--r--   0        0        0     7909 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/sql/test_sql_expr_render.py
--rw-r--r--   0        0        0    11429 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/sql/test_sql_plan_render.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/sql_clients/__init__.py
--rw-r--r--   0        0        0     4380 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/sql_clients/test_sql_client.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/telemetry/__init__.py
--rw-r--r--   0        0        0     3415 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/telemetry/test_telemetry.py
--rw-r--r--   0        0        0     1427 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/test_object_utils.py
--rw-r--r--   0        0        0     7061 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/test_specs.py
--rw-r--r--   0        0        0     2901 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/test_utils.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/time/__init__.py
--rw-r--r--   0        0        0      589 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/time/configurable_time_source.py
--rw-r--r--   0        0        0     9898 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/test/time/test_time_granularity_solver.py
--rw-r--r--   0        0        0        0 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/time/__init__.py
--rw-r--r--   0        0        0      377 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/time/time_constants.py
--rw-r--r--   0        0        0     8065 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/time/time_granularity.py
--rw-r--r--   0        0        0    12945 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/time/time_granularity_solver.py
--rw-r--r--   0        0        0      361 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/time/time_source.py
--rw-r--r--   0        0        0      549 2022-04-14 00:24:14.596413 metricflow-0.92.1/metricflow/visitor.py
--rw-r--r--   0        0        0     1465 2022-04-14 00:24:14.596413 metricflow-0.92.1/pyproject.toml
--rw-r--r--   0        0        0     6504 2022-04-14 00:25:18.801188 metricflow-0.92.1/setup.py
--rw-r--r--   0        0        0     1586 2022-04-14 00:25:18.801752 metricflow-0.92.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-04-27 23:54:18.969907 metricflow-0.93.0/LICENSE
+-rw-r--r--   0        0        0       73 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/__init__.py
+-rw-r--r--   0        0        0    11086 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/api/metricflow_client.py
+-rw-r--r--   0        0        0       28 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/cli/__init__.py
+-rw-r--r--   0        0        0     4475 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/cli/cli_context.py
+-rw-r--r--   0        0        0      137 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/cli/constants.py
+-rw-r--r--   0        0        0    23046 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/cli/main.py
+-rw-r--r--   0        0        0      351 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/cli/sample_models/countries.yaml
+-rw-r--r--   0        0        0      529 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/cli/sample_models/customers.yaml
+-rw-r--r--   0        0        0     4360 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/cli/sample_models/transactions.yaml
+-rw-r--r--   0        0        0     7937 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/cli/tutorial.py
+-rw-r--r--   0        0        0     7325 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/cli/utils.py
+-rw-r--r--   0        0        0     1341 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/column_assoc.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/configuration/__init__.py
+-rw-r--r--   0        0        0      699 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/configuration/config_builder.py
+-rw-r--r--   0        0        0     1374 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/configuration/config_handler.py
+-rw-r--r--   0        0        0      409 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/configuration/constants.py
+-rw-r--r--   0        0        0     3597 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/configuration/env_var.py
+-rw-r--r--   0        0        0     1516 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/configuration/yaml_handler.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/constraints/__init__.py
+-rw-r--r--   0        0        0     4554 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/constraints/time_constraint.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/dag/__init__.py
+-rw-r--r--   0        0        0     4802 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/dag/dag_to_text.py
+-rw-r--r--   0        0        0     1864 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/dag/dag_visualization.py
+-rw-r--r--   0        0        0     3044 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/dag/id_generation.py
+-rw-r--r--   0        0        0     5389 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/dag/mf_dag.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/dataflow/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/dataflow/builder/__init__.py
+-rw-r--r--   0        0        0     6133 2022-04-27 23:54:18.973907 metricflow-0.93.0/metricflow/dataflow/builder/costing.py
+-rw-r--r--   0        0        0    32565 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/dataflow/builder/dataflow_plan_builder.py
+-rw-r--r--   0        0        0     4224 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/dataflow/builder/node_data_set.py
+-rw-r--r--   0        0        0    18866 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/dataflow/builder/node_evaluator.py
+-rw-r--r--   0        0        0     6319 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/dataflow/builder/partitions.py
+-rw-r--r--   0        0        0    29076 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/dataflow/dataflow_plan.py
+-rw-r--r--   0        0        0     1653 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/dataflow/dataflow_plan_to_text.py
+-rw-r--r--   0        0        0     1234 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/dataflow/sql_table.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/dataset/__init__.py
+-rw-r--r--   0        0        0    21276 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/dataset/convert_data_source.py
+-rw-r--r--   0        0        0      917 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/dataset/data_source_adapter.py
+-rw-r--r--   0        0        0      600 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/dataset/dataset.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/engine/__init__.py
+-rw-r--r--   0        0        0    23208 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/engine/metricflow_engine.py
+-rw-r--r--   0        0        0      595 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/engine/models.py
+-rw-r--r--   0        0        0      268 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/engine/time_source.py
+-rw-r--r--   0        0        0     1327 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/engine/utils.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/errors/__init__.py
+-rw-r--r--   0        0        0     2845 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/errors/errors.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/execution/__init__.py
+-rw-r--r--   0        0        0     8172 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/execution/execution_plan.py
+-rw-r--r--   0        0        0     1010 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/execution/execution_plan_to_text.py
+-rw-r--r--   0        0        0     3009 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/execution/executor.py
+-rw-r--r--   0        0        0     7956 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/instances.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/__init__.py
+-rw-r--r--   0        0        0     2155 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/graph.py
+-rw-r--r--   0        0        0     1513 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/model_transformer.py
+-rw-r--r--   0        0        0     3676 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/model_validator.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/objects/__init__.py
+-rw-r--r--   0        0        0     1836 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/objects/common.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/objects/constraints/__init__.py
+-rw-r--r--   0        0        0     5174 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/objects/constraints/where.py
+-rw-r--r--   0        0        0     4554 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/objects/data_source.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/objects/elements/__init__.py
+-rw-r--r--   0        0        0     1445 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/objects/elements/dimension.py
+-rw-r--r--   0        0        0     2207 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/objects/elements/identifier.py
+-rw-r--r--   0        0        0     1917 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/objects/elements/measure.py
+-rw-r--r--   0        0        0     1269 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/objects/materialization.py
+-rw-r--r--   0        0        0     3975 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/objects/metric.py
+-rw-r--r--   0        0        0      504 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/objects/user_configured_model.py
+-rw-r--r--   0        0        0      994 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/objects/utils.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/parsing/__init__.py
+-rw-r--r--   0        0        0    10245 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/parsing/dir_to_model.py
+-rw-r--r--   0        0        0     9891 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/parsing/schemas.py
+-rw-r--r--   0        0        0     3927 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/parsing/schemas_internal.py
+-rw-r--r--   0        0        0     2522 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/parsing/validation.py
+-rw-r--r--   0        0        0      124 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/parsing/yaml_file.py
+-rw-r--r--   0        0        0     1468 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/parsing/yaml_loader.py
+-rw-r--r--   0        0        0     1150 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/semantic_model.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/semantics/__init__.py
+-rw-r--r--   0        0        0     1740 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/semantics/data_source_container.py
+-rw-r--r--   0        0        0    27358 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/semantics/linkable_spec_resolver.py
+-rw-r--r--   0        0        0     1613 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/semantics/links_new.py
+-rw-r--r--   0        0        0    19194 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/semantics/semantic_containers.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/transformations/__init__.py
+-rw-r--r--   0        0        0     1413 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/transformations/boolean_measure.py
+-rw-r--r--   0        0        0     1364 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/transformations/identifiers.py
+-rw-r--r--   0        0        0     1980 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/transformations/names.py
+-rw-r--r--   0        0        0     2113 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/transformations/proxy_measure.py
+-rw-r--r--   0        0        0      435 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/transformations/transform_rule.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/validations/__init__.py
+-rw-r--r--   0        0        0     3410 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/validations/common_identifiers.py
+-rw-r--r--   0        0        0     5661 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/validations/data_sources.py
+-rw-r--r--   0        0        0    10208 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/validations/dim_names.py
+-rw-r--r--   0        0        0     7055 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/validations/dimension_const.py
+-rw-r--r--   0        0        0     5548 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/validations/element_const.py
+-rw-r--r--   0        0        0     6083 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/validations/identifiers.py
+-rw-r--r--   0        0        0     5137 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/validations/materializations.py
+-rw-r--r--   0        0        0     4526 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/validations/metrics.py
+-rw-r--r--   0        0        0     2244 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/validations/non_empty.py
+-rw-r--r--   0        0        0     6702 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/validations/unique_valid_name.py
+-rw-r--r--   0        0        0     9787 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/model/validations/validator_helpers.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/naming/__init__.py
+-rw-r--r--   0        0        0     2837 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/naming/linkable_spec_name.py
+-rw-r--r--   0        0        0     6382 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/object_utils.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/plan_conversion/__init__.py
+-rw-r--r--   0        0        0     4752 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/plan_conversion/column_resolver.py
+-rw-r--r--   0        0        0     7103 2022-04-27 23:54:18.977907 metricflow-0.93.0/metricflow/plan_conversion/dataflow_to_execution.py
+-rw-r--r--   0        0        0    61606 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/plan_conversion/dataflow_to_sql.py
+-rw-r--r--   0        0        0    24459 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/plan_conversion/instance_converters.py
+-rw-r--r--   0        0        0    10086 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/plan_conversion/node_processor.py
+-rw-r--r--   0        0        0     2089 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/plan_conversion/select_column_gen.py
+-rw-r--r--   0        0        0     7078 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/plan_conversion/spec_transforms.py
+-rw-r--r--   0        0        0     5744 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/plan_conversion/sql_dataset.py
+-rw-r--r--   0        0        0     3788 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/plan_conversion/time_spine.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/protocols/__init__.py
+-rw-r--r--   0        0        0     6301 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/protocols/sql_client.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/py.typed
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/query/__init__.py
+-rw-r--r--   0        0        0      137 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/query/query_exceptions.py
+-rw-r--r--   0        0        0    36401 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/query/query_parser.py
+-rw-r--r--   0        0        0      667 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/spec_set_transforms.py
+-rw-r--r--   0        0        0    20040 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/specs.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/optimizer/__init__.py
+-rw-r--r--   0        0        0    10064 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/optimizer/column_pruner.py
+-rw-r--r--   0        0        0     1761 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/optimizer/optimization_levels.py
+-rw-r--r--   0        0        0    29728 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/optimizer/rewriting_sub_query_reducer.py
+-rw-r--r--   0        0        0      377 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/optimizer/sql_query_plan_optimizer.py
+-rw-r--r--   0        0        0     8502 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/optimizer/sub_query_reducer.py
+-rw-r--r--   0        0        0     3356 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/optimizer/table_alias_simplifier.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/render/__init__.py
+-rw-r--r--   0        0        0     2806 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/render/big_query.py
+-rw-r--r--   0        0        0    10341 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/render/expr_renderer.py
+-rw-r--r--   0        0        0      750 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/render/redshift.py
+-rw-r--r--   0        0        0    11294 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/render/sql_plan_renderer.py
+-rw-r--r--   0        0        0     2235 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/render/sqlite.py
+-rw-r--r--   0        0        0     1113 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/sql_bind_parameters.py
+-rw-r--r--   0        0        0    41788 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/sql_exprs.py
+-rw-r--r--   0        0        0     9902 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/sql_plan.py
+-rw-r--r--   0        0        0     1371 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql/sql_plan_to_text.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql_clients/__init__.py
+-rw-r--r--   0        0        0     6603 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql_clients/base_sql_client_implementation.py
+-rw-r--r--   0        0        0     3494 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql_clients/big_query.py
+-rw-r--r--   0        0        0      693 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql_clients/common_client.py
+-rw-r--r--   0        0        0     3104 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql_clients/redshift.py
+-rw-r--r--   0        0        0     8839 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql_clients/snowflake.py
+-rw-r--r--   0        0        0     4910 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql_clients/sql_utils.py
+-rw-r--r--   0        0        0     4947 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql_clients/sqlalchemy_dialect.py
+-rw-r--r--   0        0        0     4027 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/sql_clients/sqlite.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/telemetry/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/telemetry/handlers/__init__.py
+-rw-r--r--   0        0        0     3613 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/telemetry/handlers/handlers.py
+-rw-r--r--   0        0        0      724 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/telemetry/handlers/python_log.py
+-rw-r--r--   0        0        0     2888 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/telemetry/models.py
+-rw-r--r--   0        0        0     6497 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/telemetry/reporter.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/api/__init__.py
+-rw-r--r--   0        0        0      835 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/api/conftest.py
+-rw-r--r--   0        0        0     3563 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/api/test_metricflow_client.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/cli/__init__.py
+-rw-r--r--   0        0        0     3033 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/cli/test_cli.py
+-rw-r--r--   0        0        0     2177 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/compare_df.py
+-rw-r--r--   0        0        0      579 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/conftest.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/constraints/__init__.py
+-rw-r--r--   0        0        0      523 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/constraints/test_where.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/dataflow/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/dataflow/builder/__init__.py
+-rw-r--r--   0        0        0     2264 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/dataflow/builder/test_costing.py
+-rw-r--r--   0        0        0    19494 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/dataflow/builder/test_dataflow_plan_builder.py
+-rw-r--r--   0        0        0     6996 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/dataflow/builder/test_node_data_set.py
+-rw-r--r--   0        0        0    21186 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/dataflow/builder/test_node_evaluator.py
+-rw-r--r--   0        0        0      933 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/dataflow/test_sql_table.py
+-rw-r--r--   0        0        0     1247 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/dataflow_plan_to_svg.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/dataset/__init__.py
+-rw-r--r--   0        0        0    10330 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/dataset/test_convert_data_source.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/execution/__init__.py
+-rw-r--r--   0        0        0     1491 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/execution/noop_task.py
+-rw-r--r--   0        0        0     2426 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/execution/test_sequential_executor.py
+-rw-r--r--   0        0        0     2170 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/execution/test_tasks.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.981907 metricflow-0.93.0/metricflow/test/fixtures/__init__.py
+-rw-r--r--   0        0        0     3310 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/cli_fixtures.py
+-rw-r--r--   0        0        0     3263 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/dataflow_fixtures.py
+-rw-r--r--   0        0        0     1654 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/id_fixtures.py
+-rw-r--r--   0        0        0    11044 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_fixtures.py
+-rw-r--r--   0        0        0      432 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/composite_identifier_model/materializations.yaml
+-rw-r--r--   0        0        0      600 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/composite_identifier_model/messages_source.yaml
+-rw-r--r--   0        0        0      444 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/composite_identifier_model/more_users_source.yaml
+-rw-r--r--   0        0        0      704 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/composite_identifier_model/users_source.yaml
+-rw-r--r--   0        0        0      568 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/extended_date_model/data_sources/bookings_from_sql_query_source.yaml
+-rw-r--r--   0        0        0      468 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/extended_date_model/data_sources/bookings_monthly_source.yaml
+-rw-r--r--   0        0        0      680 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/extended_date_model/data_sources/extended_bookings_source.yaml
+-rw-r--r--   0        0        0      381 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/extended_date_model/data_sources/listings_extended_source.yaml
+-rw-r--r--   0        0        0      488 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/join_types_model/bookings_source.yaml
+-rw-r--r--   0        0        0      330 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/join_types_model/listings_source.yaml
+-rw-r--r--   0        0        0      638 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/multi_hop_join_model/partitioned_data_sources/account_month_txns.yaml
+-rw-r--r--   0        0        0      481 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/multi_hop_join_model/partitioned_data_sources/bridge_table.yaml
+-rw-r--r--   0        0        0      507 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/multi_hop_join_model/partitioned_data_sources/customer_other_data.yaml
+-rw-r--r--   0        0        0      505 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/multi_hop_join_model/partitioned_data_sources/customer_table.yaml
+-rw-r--r--   0        0        0      451 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/multi_hop_join_model/partitioned_data_sources/third_hop_table.yaml
+-rw-r--r--   0        0        0      494 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/multi_hop_join_model/unpartitioned_data_sources/account_month_txns.yaml
+-rw-r--r--   0        0        0      337 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/multi_hop_join_model/unpartitioned_data_sources/bridge_table.yaml
+-rw-r--r--   0        0        0      363 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/multi_hop_join_model/unpartitioned_data_sources/customer_other_data.yaml
+-rw-r--r--   0        0        0      361 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/multi_hop_join_model/unpartitioned_data_sources/customer_table.yaml
+-rw-r--r--   0        0        0      307 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/multi_hop_join_model/unpartitioned_data_sources/third_hop_table.yaml
+-rw-r--r--   0        0        0      638 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/non_ds_model/bookings_source.yaml
+-rw-r--r--   0        0        0      636 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/non_ds_model/listings_latest.yaml
+-rw-r--r--   0        0        0     1359 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/data_sources/bookings_source.yaml
+-rw-r--r--   0        0        0      421 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/data_sources/companies.yaml
+-rw-r--r--   0        0        0      711 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/data_sources/id_verifications.yaml
+-rw-r--r--   0        0        0      959 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/data_sources/listings_latest.yaml
+-rw-r--r--   0        0        0      355 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/data_sources/lux_listing_mapping.yaml
+-rw-r--r--   0        0        0      504 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/data_sources/revenue.yaml
+-rw-r--r--   0        0        0      628 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/data_sources/user_ds_source.yaml
+-rw-r--r--   0        0        0      424 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/data_sources/users_latest.yaml
+-rw-r--r--   0        0        0      855 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/data_sources/views_source.yaml
+-rw-r--r--   0        0        0     2607 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/materializations.yaml
+-rw-r--r--   0        0        0     6205 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/metrics.yaml
+-rw-r--r--   0        0        0     3192 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/setup_fixtures.py
+-rw-r--r--   0        0        0     1546 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/sql_client_fixtures.py
+-rw-r--r--   0        0        0      280 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/sql_fixtures.py
+-rw-r--r--   0        0        0    19919 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/fixtures/table_fixtures.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/__init__.py
+-rw-r--r--   0        0        0     6212 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/configured_test_case.py
+-rw-r--r--   0        0        0     1729 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/conftest.py
+-rw-r--r--   0        0        0     5256 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_cases/itest_composite_identifier.yaml
+-rw-r--r--   0        0        0     3739 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_cases/itest_constraints.yaml
+-rw-r--r--   0        0        0     9546 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_cases/itest_cumulative_metric.yaml
+-rw-r--r--   0        0        0     3909 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_cases/itest_dimensions.yaml
+-rw-r--r--   0        0        0     1053 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_cases/itest_dundered_identifiers.yaml
+-rw-r--r--   0        0        0    11208 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_cases/itest_granularity.yaml
+-rw-r--r--   0        0        0     1241 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_cases/itest_joins.yaml
+-rw-r--r--   0        0        0     1927 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_cases/itest_measure_aggregations.yaml
+-rw-r--r--   0        0        0    11456 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_cases/itest_metrics.yaml
+-rw-r--r--   0        0        0     5422 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_cases/itest_multi_hop_join.yaml
+-rw-r--r--   0        0        0     1615 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_cases/itest_order_limit.yaml
+-rw-r--r--   0        0        0     2901 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_cases/itest_partitions.yaml
+-rw-r--r--   0        0        0     4098 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_cases/itest_simple.yaml
+-rw-r--r--   0        0        0      693 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_cases/itest_simple_non_ds.yaml
+-rw-r--r--   0        0        0     9100 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_configured_cases.py
+-rw-r--r--   0        0        0     2601 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_rendered_query.py
+-rw-r--r--   0        0        0     1445 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/integration/test_write_to_table.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/semantics/__init__.py
+-rw-r--r--   0        0        0     2432 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/semantics/test_linkable_spec_resolver.py
+-rw-r--r--   0        0        0     5934 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/test_data_source_container.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/validations/__init__.py
+-rw-r--r--   0        0        0     1339 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/validations/test_common_identifiers.py
+-rw-r--r--   0        0        0     1144 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/validations/test_data_sources.py
+-rw-r--r--   0        0        0     1163 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/validations/test_dim_names.py
+-rw-r--r--   0        0        0     7492 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/validations/test_dimension_const.py
+-rw-r--r--   0        0        0     2445 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/validations/test_element_const.py
+-rw-r--r--   0        0        0     9680 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/validations/test_identifiers.py
+-rw-r--r--   0        0        0     4273 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/validations/test_materializations.py
+-rw-r--r--   0        0        0     1629 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/validations/test_measures.py
+-rw-r--r--   0        0        0     8382 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/validations/test_metrics.py
+-rw-r--r--   0        0        0    10625 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/model/validations/test_unique_valid_name.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/plan_conversion/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/plan_conversion/instance_converters/__init__.py
+-rw-r--r--   0        0        0     6919 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/plan_conversion/instance_converters/test_create_select_columns_with_measures_aggregated.py
+-rw-r--r--   0        0        0     7219 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/plan_conversion/test_dataflow_to_execution.py
+-rw-r--r--   0        0        0    43436 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/plan_conversion/test_dataflow_to_sql_plan.py
+-rw-r--r--   0        0        0     1373 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/plan_conversion/test_time_spine.py
+-rw-r--r--   0        0        0    10672 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/plan_utils.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/prototype_utils.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/query/__init__.py
+-rw-r--r--   0        0        0     7544 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/query/test_query_parser.py
+-rw-r--r--   0        0        0     2842 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/query/test_query_parser_suggestions.py
+-rw-r--r--   0        0        0      463 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_dont_prune_if_in_where__after_pruning.sql
+-rw-r--r--   0        0        0      525 2022-04-27 23:54:18.985908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_dont_prune_if_in_where__before_pruning.sql
+-rw-r--r--   0        0        0      494 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_dont_prune_with_str_expr__after_pruning.sql
+-rw-r--r--   0        0        0      494 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_dont_prune_with_str_expr__before_pruning.sql
+-rw-r--r--   0        0        0      727 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_no_pruning__after_pruning.sql
+-rw-r--r--   0        0        0      727 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_no_pruning__before_pruning.sql
+-rw-r--r--   0        0        0      608 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_from_source__after_pruning.sql
+-rw-r--r--   0        0        0      637 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_from_source__before_pruning.sql
+-rw-r--r--   0        0        0      192 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_grandparents__after_pruning.sql
+-rw-r--r--   0        0        0      210 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_grandparents__before_pruning.sql
+-rw-r--r--   0        0        0      271 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_grandparents_in_join_query__after_pruning.sql
+-rw-r--r--   0        0        0      289 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_grandparents_in_join_query__before_pruning.sql
+-rw-r--r--   0        0        0      598 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_joined_source__after_pruning.sql
+-rw-r--r--   0        0        0      629 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_joined_source__before_pruning.sql
+-rw-r--r--   0        0        0      430 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_str_expr__after_pruning.sql
+-rw-r--r--   0        0        0      498 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_str_expr__before_pruning.sql
+-rw-r--r--   0        0        0      434 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_with_str_expr__after_pruning.sql
+-rw-r--r--   0        0        0      494 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_with_str_expr__before_pruning.sql
+-rw-r--r--   0        0        0      548 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/BigQuerySqlClient/test_convert_query_data_source__plan0.sql
+-rw-r--r--   0        0        0     2071 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/BigQuerySqlClient/test_convert_table_data_source_with_measures__plan0.sql
+-rw-r--r--   0        0        0      891 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/BigQuerySqlClient/test_convert_table_data_source_without_measures__plan0.sql
+-rw-r--r--   0        0        0      550 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/RedshiftSqlClient/test_convert_query_data_source__plan0.sql
+-rw-r--r--   0        0        0     2079 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/RedshiftSqlClient/test_convert_table_data_source_with_measures__plan0.sql
+-rw-r--r--   0        0        0      895 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/RedshiftSqlClient/test_convert_table_data_source_without_measures__plan0.sql
+-rw-r--r--   0        0        0      550 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SnowflakeSqlClient/test_convert_query_data_source__plan0.sql
+-rw-r--r--   0        0        0     2079 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SnowflakeSqlClient/test_convert_table_data_source_with_measures__plan0.sql
+-rw-r--r--   0        0        0      895 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SnowflakeSqlClient/test_convert_table_data_source_without_measures__plan0.sql
+-rw-r--r--   0        0        0      474 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SqliteSqlClient/test_convert_query_data_source__plan0.sql
+-rw-r--r--   0        0        0     1663 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SqliteSqlClient/test_convert_table_data_source_with_measures__plan0.sql
+-rw-r--r--   0        0        0      767 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SqliteSqlClient/test_convert_table_data_source_without_measures__plan0.sql
+-rw-r--r--   0        0        0     2209 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_cumulative_metric__dfp_0.xml
+-rw-r--r--   0        0        0     7389 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_distinct_values_plan__dfp_0.xml
+-rw-r--r--   0        0        0     6268 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_expr_metrics_plan__dfp_0.xml
+-rw-r--r--   0        0        0     5960 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_joined_plan__dfp_0.xml
+-rw-r--r--   0        0        0     2199 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_limit_rows_plan__dfp_0.xml
+-rw-r--r--   0        0        0    14843 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_multi_data_source_ratio_metrics_plan__dfp_0.xml
+-rw-r--r--   0        0        0    21417 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_multihop_join_plan__dfp_0.xml
+-rw-r--r--   0        0        0     4585 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_multiple_metrics_plan__dfp_0.xml
+-rw-r--r--   0        0        0     2918 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_order_by_plan__dfp_0.xml
+-rw-r--r--   0        0        0     1789 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_simple_plan__dfp_0.xml
+-rw-r--r--   0        0        0     6469 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_single_data_source_ratio_metrics_plan__dfp_0.xml
+-rw-r--r--   0        0        0     8627 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_where_constrained_plan__dfp_0.xml
+-rw-r--r--   0        0        0     4454 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_where_constrained_plan_time_dimension__dfp_0.xml
+-rw-r--r--   0        0        0     7129 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_where_constrained_with_common_linkable_plan__dfp_0.xml
+-rw-r--r--   0        0        0     9336 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_combined_metrics_plan__ep_0.xml
+-rw-r--r--   0        0        0     3100 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_joined_plan__ep_0.xml
+-rw-r--r--   0        0        0     3820 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_multihop_joined_plan__ep_0.xml
+-rw-r--r--   0        0        0     4045 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_small_combined_metrics_plan__ep_0.xml
+-rw-r--r--   0        0        0     9336 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_combined_metrics_plan__ep_0.xml
+-rw-r--r--   0        0        0     3100 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_joined_plan__ep_0.xml
+-rw-r--r--   0        0        0     3820 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_multihop_joined_plan__ep_0.xml
+-rw-r--r--   0        0        0     4045 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_small_combined_metrics_plan__ep_0.xml
+-rw-r--r--   0        0        0     9336 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_combined_metrics_plan__ep_0.xml
+-rw-r--r--   0        0        0     3100 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_joined_plan__ep_0.xml
+-rw-r--r--   0        0        0     3820 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_multihop_joined_plan__ep_0.xml
+-rw-r--r--   0        0        0     4045 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_small_combined_metrics_plan__ep_0.xml
+-rw-r--r--   0        0        0     9336 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_combined_metrics_plan__ep_0.xml
+-rw-r--r--   0        0        0     3100 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_joined_plan__ep_0.xml
+-rw-r--r--   0        0        0     3820 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_multihop_joined_plan__ep_0.xml
+-rw-r--r--   0        0        0     4045 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_small_combined_metrics_plan__ep_0.xml
+-rw-r--r--   0        0        0     4377 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/DataflowPlan/test_compute_metrics_node_simple_expr__plan0.xml
+-rw-r--r--   0        0        0     1876 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier__plan0.sql
+-rw-r--r--   0        0        0      498 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier__plan0_optimized.sql
+-rw-r--r--   0        0        0     6616 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_join__plan0.sql
+-rw-r--r--   0        0        0      982 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_join__plan0_optimized.sql
+-rw-r--r--   0        0        0     2171 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_order_by__plan0.sql
+-rw-r--r--   0        0        0      584 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql
+-rw-r--r--   0        0        0     6799 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node__plan0.sql
+-rw-r--r--   0        0        0      726 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node__plan0_optimized.sql
+-rw-r--r--   0        0        0    15499 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql
+-rw-r--r--   0        0        0     2411 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql
+-rw-r--r--   0        0        0     7002 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql
+-rw-r--r--   0        0        0     1016 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql
+-rw-r--r--   0        0        0     6850 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_simple_expr__plan0.sql
+-rw-r--r--   0        0        0      747 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql
+-rw-r--r--   0        0        0     3445 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_constrain_primary_time_dimension__plan0.sql
+-rw-r--r--   0        0        0      415 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_constrain_primary_time_dimension__plan0_optimized.sql
+-rw-r--r--   0        0        0     1639 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric__plan0.sql
+-rw-r--r--   0        0        0      698 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric__plan0_optimized.sql
+-rw-r--r--   0        0        0     1599 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_grain_to_date__plan0.sql
+-rw-r--r--   0        0        0      658 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql
+-rw-r--r--   0        0        0      942 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_ds__plan0.sql
+-rw-r--r--   0        0        0      307 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_ds__plan0_optimized.sql
+-rw-r--r--   0        0        0     1508 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window__plan0.sql
+-rw-r--r--   0        0        0      552 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window__plan0_optimized.sql
+-rw-r--r--   0        0        0     2557 2022-04-27 23:54:18.989908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql
+-rw-r--r--   0        0        0     1233 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql
+-rw-r--r--   0        0        0     2696 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_with_time_constraint__plan0.sql
+-rw-r--r--   0        0        0     1350 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql
+-rw-r--r--   0        0        0     7886 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_distinct_values__plan0.sql
+-rw-r--r--   0        0        0      697 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_distinct_values__plan0_optimized.sql
+-rw-r--r--   0        0        0     3092 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_node__plan0.sql
+-rw-r--r--   0        0        0      236 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     3320 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_with_where_constraint_node__plan0.sql
+-rw-r--r--   0        0        0      365 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_with_where_constraint_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     8009 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql
+-rw-r--r--   0        0        0     1057 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql
+-rw-r--r--   0        0        0     3741 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_limit_rows__plan0.sql
+-rw-r--r--   0        0        0      429 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_limit_rows__plan0_optimized.sql
+-rw-r--r--   0        0        0     2989 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_local_dimension_using_local_identifier__plan0.sql
+-rw-r--r--   0        0        0      446 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_local_dimension_using_local_identifier__plan0_optimized.sql
+-rw-r--r--   0        0        0     3572 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_measure_aggregation_node__plan0.sql
+-rw-r--r--   0        0        0      475 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_measure_aggregation_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     8764 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multi_join_node__plan0.sql
+-rw-r--r--   0        0        0     1166 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multi_join_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     9999 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multihop_node__plan0.sql
+-rw-r--r--   0        0        0     1255 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multihop_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     3922 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_order_by_node__plan0.sql
+-rw-r--r--   0        0        0      517 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_order_by_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     6724 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_partitioned_join__plan0.sql
+-rw-r--r--   0        0        0      863 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_partitioned_join__plan0_optimized.sql
+-rw-r--r--   0        0        0     6046 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_single_join_node__plan0.sql
+-rw-r--r--   0        0        0      617 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_single_join_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     2926 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_source_node__plan0.sql
+-rw-r--r--   0        0        0     2042 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_source_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     1880 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier__plan0.sql
+-rw-r--r--   0        0        0      498 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier__plan0_optimized.sql
+-rw-r--r--   0        0        0     6628 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_join__plan0.sql
+-rw-r--r--   0        0        0     1008 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_join__plan0_optimized.sql
+-rw-r--r--   0        0        0     2175 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_order_by__plan0.sql
+-rw-r--r--   0        0        0      584 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql
+-rw-r--r--   0        0        0     6815 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node__plan0.sql
+-rw-r--r--   0        0        0      743 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node__plan0_optimized.sql
+-rw-r--r--   0        0        0    15549 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql
+-rw-r--r--   0        0        0     2465 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql
+-rw-r--r--   0        0        0     7036 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql
+-rw-r--r--   0        0        0     1051 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql
+-rw-r--r--   0        0        0     6866 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_simple_expr__plan0.sql
+-rw-r--r--   0        0        0      786 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql
+-rw-r--r--   0        0        0     3455 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_constrain_primary_time_dimension__plan0.sql
+-rw-r--r--   0        0        0      417 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_constrain_primary_time_dimension__plan0_optimized.sql
+-rw-r--r--   0        0        0     1619 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric__plan0.sql
+-rw-r--r--   0        0        0      699 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric__plan0_optimized.sql
+-rw-r--r--   0        0        0     1618 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_grain_to_date__plan0.sql
+-rw-r--r--   0        0        0      698 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql
+-rw-r--r--   0        0        0      944 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_ds__plan0.sql
+-rw-r--r--   0        0        0      307 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_ds__plan0_optimized.sql
+-rw-r--r--   0        0        0     1514 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window__plan0.sql
+-rw-r--r--   0        0        0      577 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window__plan0_optimized.sql
+-rw-r--r--   0        0        0     2569 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql
+-rw-r--r--   0        0        0     1265 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql
+-rw-r--r--   0        0        0     2682 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_with_time_constraint__plan0.sql
+-rw-r--r--   0        0        0     1356 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql
+-rw-r--r--   0        0        0     7902 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_distinct_values__plan0.sql
+-rw-r--r--   0        0        0      707 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_distinct_values__plan0_optimized.sql
+-rw-r--r--   0        0        0     3100 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_node__plan0.sql
+-rw-r--r--   0        0        0      236 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     3328 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_with_where_constraint_node__plan0.sql
+-rw-r--r--   0        0        0      365 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_with_where_constraint_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     8025 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql
+-rw-r--r--   0        0        0     1057 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql
+-rw-r--r--   0        0        0     3749 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_limit_rows__plan0.sql
+-rw-r--r--   0        0        0      429 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_limit_rows__plan0_optimized.sql
+-rw-r--r--   0        0        0     2997 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_local_dimension_using_local_identifier__plan0.sql
+-rw-r--r--   0        0        0      446 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_local_dimension_using_local_identifier__plan0_optimized.sql
+-rw-r--r--   0        0        0     3580 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_measure_aggregation_node__plan0.sql
+-rw-r--r--   0        0        0      475 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_measure_aggregation_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     8788 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multi_join_node__plan0.sql
+-rw-r--r--   0        0        0     1166 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multi_join_node__plan0_optimized.sql
+-rw-r--r--   0        0        0    10015 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multihop_node__plan0.sql
+-rw-r--r--   0        0        0     1251 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multihop_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     3930 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_order_by_node__plan0.sql
+-rw-r--r--   0        0        0      517 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_order_by_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     6744 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_partitioned_join__plan0.sql
+-rw-r--r--   0        0        0      883 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_partitioned_join__plan0_optimized.sql
+-rw-r--r--   0        0        0     6062 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_single_join_node__plan0.sql
+-rw-r--r--   0        0        0      617 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_single_join_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     2934 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_source_node__plan0.sql
+-rw-r--r--   0        0        0     2050 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_source_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     1880 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier__plan0.sql
+-rw-r--r--   0        0        0      498 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier__plan0_optimized.sql
+-rw-r--r--   0        0        0     6628 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_join__plan0.sql
+-rw-r--r--   0        0        0     1008 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_join__plan0_optimized.sql
+-rw-r--r--   0        0        0     2175 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_order_by__plan0.sql
+-rw-r--r--   0        0        0      584 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql
+-rw-r--r--   0        0        0     6815 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node__plan0.sql
+-rw-r--r--   0        0        0      743 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node__plan0_optimized.sql
+-rw-r--r--   0        0        0    15529 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql
+-rw-r--r--   0        0        0     2445 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql
+-rw-r--r--   0        0        0     7016 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql
+-rw-r--r--   0        0        0     1031 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql
+-rw-r--r--   0        0        0     6866 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_simple_expr__plan0.sql
+-rw-r--r--   0        0        0      786 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql
+-rw-r--r--   0        0        0     3455 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_constrain_primary_time_dimension__plan0.sql
+-rw-r--r--   0        0        0      417 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_constrain_primary_time_dimension__plan0_optimized.sql
+-rw-r--r--   0        0        0     1619 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric__plan0.sql
+-rw-r--r--   0        0        0      699 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric__plan0_optimized.sql
+-rw-r--r--   0        0        0     1618 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_grain_to_date__plan0.sql
+-rw-r--r--   0        0        0      698 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql
+-rw-r--r--   0        0        0      944 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_ds__plan0.sql
+-rw-r--r--   0        0        0      307 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_ds__plan0_optimized.sql
+-rw-r--r--   0        0        0     1514 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window__plan0.sql
+-rw-r--r--   0        0        0      577 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window__plan0_optimized.sql
+-rw-r--r--   0        0        0     2569 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql
+-rw-r--r--   0        0        0     1265 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql
+-rw-r--r--   0        0        0     2682 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_with_time_constraint__plan0.sql
+-rw-r--r--   0        0        0     1356 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql
+-rw-r--r--   0        0        0     7902 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_distinct_values__plan0.sql
+-rw-r--r--   0        0        0      707 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_distinct_values__plan0_optimized.sql
+-rw-r--r--   0        0        0     3100 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_node__plan0.sql
+-rw-r--r--   0        0        0      236 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     3328 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_with_where_constraint_node__plan0.sql
+-rw-r--r--   0        0        0      365 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_with_where_constraint_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     8025 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql
+-rw-r--r--   0        0        0     1057 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql
+-rw-r--r--   0        0        0     3749 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_limit_rows__plan0.sql
+-rw-r--r--   0        0        0      429 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_limit_rows__plan0_optimized.sql
+-rw-r--r--   0        0        0     2997 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_local_dimension_using_local_identifier__plan0.sql
+-rw-r--r--   0        0        0      446 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_local_dimension_using_local_identifier__plan0_optimized.sql
+-rw-r--r--   0        0        0     3580 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_measure_aggregation_node__plan0.sql
+-rw-r--r--   0        0        0      475 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_measure_aggregation_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     8788 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multi_join_node__plan0.sql
+-rw-r--r--   0        0        0     1166 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multi_join_node__plan0_optimized.sql
+-rw-r--r--   0        0        0    10015 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multihop_node__plan0.sql
+-rw-r--r--   0        0        0     1251 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multihop_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     3930 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_order_by_node__plan0.sql
+-rw-r--r--   0        0        0      517 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_order_by_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     6744 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_partitioned_join__plan0.sql
+-rw-r--r--   0        0        0      883 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_partitioned_join__plan0_optimized.sql
+-rw-r--r--   0        0        0     6062 2022-04-27 23:54:18.993908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_single_join_node__plan0.sql
+-rw-r--r--   0        0        0      617 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_single_join_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     2934 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_source_node__plan0.sql
+-rw-r--r--   0        0        0     2050 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_source_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     1728 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier__plan0.sql
+-rw-r--r--   0        0        0      498 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier__plan0_optimized.sql
+-rw-r--r--   0        0        0     6092 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_join__plan0.sql
+-rw-r--r--   0        0        0     1008 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_join__plan0_optimized.sql
+-rw-r--r--   0        0        0     2023 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_order_by__plan0.sql
+-rw-r--r--   0        0        0      584 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql
+-rw-r--r--   0        0        0     5983 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node__plan0.sql
+-rw-r--r--   0        0        0      743 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node__plan0_optimized.sql
+-rw-r--r--   0        0        0    13913 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql
+-rw-r--r--   0        0        0     2445 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql
+-rw-r--r--   0        0        0     6184 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql
+-rw-r--r--   0        0        0     1031 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql
+-rw-r--r--   0        0        0     6034 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_simple_expr__plan0.sql
+-rw-r--r--   0        0        0      786 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql
+-rw-r--r--   0        0        0     3045 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_constrain_primary_time_dimension__plan0.sql
+-rw-r--r--   0        0        0      407 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_constrain_primary_time_dimension__plan0_optimized.sql
+-rw-r--r--   0        0        0     1541 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric__plan0.sql
+-rw-r--r--   0        0        0      673 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric__plan0_optimized.sql
+-rw-r--r--   0        0        0     1534 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_grain_to_date__plan0.sql
+-rw-r--r--   0        0        0      666 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql
+-rw-r--r--   0        0        0      868 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_ds__plan0.sql
+-rw-r--r--   0        0        0      307 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_ds__plan0_optimized.sql
+-rw-r--r--   0        0        0     1438 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window__plan0.sql
+-rw-r--r--   0        0        0      572 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window__plan0_optimized.sql
+-rw-r--r--   0        0        0     2463 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql
+-rw-r--r--   0        0        0     1248 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql
+-rw-r--r--   0        0        0     2574 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_with_time_constraint__plan0.sql
+-rw-r--r--   0        0        0     1337 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql
+-rw-r--r--   0        0        0     7070 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_distinct_values__plan0.sql
+-rw-r--r--   0        0        0      707 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_distinct_values__plan0_optimized.sql
+-rw-r--r--   0        0        0     2700 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_node__plan0.sql
+-rw-r--r--   0        0        0      236 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     2928 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_with_where_constraint_node__plan0.sql
+-rw-r--r--   0        0        0      365 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_with_where_constraint_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     7193 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql
+-rw-r--r--   0        0        0     1057 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql
+-rw-r--r--   0        0        0     3349 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_limit_rows__plan0.sql
+-rw-r--r--   0        0        0      429 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_limit_rows__plan0_optimized.sql
+-rw-r--r--   0        0        0     2565 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_local_dimension_using_local_identifier__plan0.sql
+-rw-r--r--   0        0        0      446 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_local_dimension_using_local_identifier__plan0_optimized.sql
+-rw-r--r--   0        0        0     3180 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_measure_aggregation_node__plan0.sql
+-rw-r--r--   0        0        0      475 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_measure_aggregation_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     7524 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multi_join_node__plan0.sql
+-rw-r--r--   0        0        0     1166 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multi_join_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     9231 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multihop_node__plan0.sql
+-rw-r--r--   0        0        0     1251 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multihop_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     3530 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_order_by_node__plan0.sql
+-rw-r--r--   0        0        0      517 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_order_by_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     5712 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_partitioned_join__plan0.sql
+-rw-r--r--   0        0        0      883 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_partitioned_join__plan0_optimized.sql
+-rw-r--r--   0        0        0     5230 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_single_join_node__plan0.sql
+-rw-r--r--   0        0        0      617 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_single_join_node__plan0_optimized.sql
+-rw-r--r--   0        0        0     2534 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_source_node__plan0.sql
+-rw-r--r--   0        0        0     2066 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_source_node__plan0_optimized.sql
+-rw-r--r--   0        0        0    11288 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_composite_identifier__plan0.xml
+-rw-r--r--   0        0        0    35872 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_composite_identifier_with_join__plan0.xml
+-rw-r--r--   0        0        0    13595 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_composite_identifier_with_order_by__plan0.xml
+-rw-r--r--   0        0        0    33841 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node__plan0.xml
+-rw-r--r--   0        0        0    79506 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.xml
+-rw-r--r--   0        0        0    34942 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node_ratio_from_single_data_source__plan0.xml
+-rw-r--r--   0        0        0    33940 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node_simple_expr__plan0.xml
+-rw-r--r--   0        0        0    15272 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_constrain_primary_time_dimension__plan0.xml
+-rw-r--r--   0        0        0     9065 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric__plan0.xml
+-rw-r--r--   0        0        0     9065 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_grain_to_date__plan0.xml
+-rw-r--r--   0        0        0     4867 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_no_ds__plan0.xml
+-rw-r--r--   0        0        0     9065 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_no_window__plan0.xml
+-rw-r--r--   0        0        0    13917 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_no_window_with_time_constraint__plan0.xml
+-rw-r--r--   0        0        0    13905 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_with_time_constraint__plan0.xml
+-rw-r--r--   0        0        0    40126 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_distinct_values__plan0.xml
+-rw-r--r--   0        0        0    13320 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_filter_node__plan0.xml
+-rw-r--r--   0        0        0    15261 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_filter_with_where_constraint_node__plan0.xml
+-rw-r--r--   0        0        0    42120 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_filter_with_where_constraint_on_join_dim__plan0.xml
+-rw-r--r--   0        0        0    18678 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_limit_rows__plan0.xml
+-rw-r--r--   0        0        0    14904 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_local_dimension_using_local_identifier__plan0.xml
+-rw-r--r--   0        0        0    16720 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_measure_aggregation_node__plan0.xml
+-rw-r--r--   0        0        0    40964 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_multi_join_node__plan0.xml
+-rw-r--r--   0        0        0    49219 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_multihop_node__plan0.xml
+-rw-r--r--   0        0        0    20916 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_order_by_node__plan0.xml
+-rw-r--r--   0        0        0    32547 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_partitioned_join__plan0.xml
+-rw-r--r--   0        0        0    28042 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_single_join_node__plan0.xml
+-rw-r--r--   0        0        0    12099 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_source_node__plan0.xml
+-rw-r--r--   0        0        0      100 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_engine_specific_rendering.py/SqlQueryPlan/BigQuerySqlClient/test_cast_to_timestamp__plan0.sql
+-rw-r--r--   0        0        0      101 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_engine_specific_rendering.py/SqlQueryPlan/RedshiftSqlClient/test_cast_to_timestamp__plan0.sql
+-rw-r--r--   0        0        0      101 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_engine_specific_rendering.py/SqlQueryPlan/SnowflakeSqlClient/test_cast_to_timestamp__plan0.sql
+-rw-r--r--   0        0        0       96 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_engine_specific_rendering.py/SqlQueryPlan/SqliteSqlClient/test_cast_to_timestamp__plan0.sql
+-rw-r--r--   0        0        0      572 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/BigQuerySqlClient/test_render_query__query0.sql
+-rw-r--r--   0        0        0      681 2022-04-27 23:54:18.997908 metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/BigQuerySqlClient/test_render_write_to_table_query__query0.sql
+-rw-r--r--   0        0        0      574 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/RedshiftSqlClient/test_render_query__query0.sql
+-rw-r--r--   0        0        0      683 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/RedshiftSqlClient/test_render_write_to_table_query__query0.sql
+-rw-r--r--   0        0        0      574 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SnowflakeSqlClient/test_render_query__query0.sql
+-rw-r--r--   0        0        0      683 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SnowflakeSqlClient/test_render_write_to_table_query__query0.sql
+-rw-r--r--   0        0        0      564 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SqliteSqlClient/test_render_query__query0.sql
+-rw-r--r--   0        0        0      673 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SqliteSqlClient/test_render_write_to_table_query__query0.sql
+-rw-r--r--   0        0        0      655 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_colliding_alias__after_reducing.sql
+-rw-r--r--   0        0        0      655 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_colliding_alias__before_reducing.sql
+-rw-r--r--   0        0        0      575 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_all_join_sources__after_reducing.sql
+-rw-r--r--   0        0        0     1003 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_all_join_sources__before_reducing.sql
+-rw-r--r--   0        0        0      504 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_join__after_reducing.sql
+-rw-r--r--   0        0        0      641 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_join__before_reducing.sql
+-rw-r--r--   0        0        0      205 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_sub_query__after_reducing.sql
+-rw-r--r--   0        0        0      354 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_sub_query__before_reducing.sql
+-rw-r--r--   0        0        0       62 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_component_rendering__plan0.sql
+-rw-r--r--   0        0        0      127 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_component_rendering__plan1.sql
+-rw-r--r--   0        0        0      189 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_component_rendering__plan2.sql
+-rw-r--r--   0        0        0      254 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_component_rendering__plan3.sql
+-rw-r--r--   0        0        0      275 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_component_rendering__plan4.sql
+-rw-r--r--   0        0        0      289 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_component_rendering__plan5.sql
+-rw-r--r--   0        0        0       62 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_render_limit__plan0.sql
+-rw-r--r--   0        0        0      116 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_render_order_by__plan0.sql
+-rw-r--r--   0        0        0       87 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/BigQuerySqlClient/test_render_where__plan0.sql
+-rw-r--r--   0        0        0       62 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_component_rendering__plan0.sql
+-rw-r--r--   0        0        0      127 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_component_rendering__plan1.sql
+-rw-r--r--   0        0        0      189 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_component_rendering__plan2.sql
+-rw-r--r--   0        0        0      254 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_component_rendering__plan3.sql
+-rw-r--r--   0        0        0      275 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_component_rendering__plan4.sql
+-rw-r--r--   0        0        0      289 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_component_rendering__plan5.sql
+-rw-r--r--   0        0        0       62 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_render_limit__plan0.sql
+-rw-r--r--   0        0        0      116 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_render_order_by__plan0.sql
+-rw-r--r--   0        0        0       87 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/RedshiftSqlClient/test_render_where__plan0.sql
+-rw-r--r--   0        0        0       62 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_component_rendering__plan0.sql
+-rw-r--r--   0        0        0      127 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_component_rendering__plan1.sql
+-rw-r--r--   0        0        0      189 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_component_rendering__plan2.sql
+-rw-r--r--   0        0        0      254 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_component_rendering__plan3.sql
+-rw-r--r--   0        0        0      275 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_component_rendering__plan4.sql
+-rw-r--r--   0        0        0      289 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_component_rendering__plan5.sql
+-rw-r--r--   0        0        0       62 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_render_limit__plan0.sql
+-rw-r--r--   0        0        0      116 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_render_order_by__plan0.sql
+-rw-r--r--   0        0        0       87 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SnowflakeSqlClient/test_render_where__plan0.sql
+-rw-r--r--   0        0        0       62 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_component_rendering__plan0.sql
+-rw-r--r--   0        0        0      127 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_component_rendering__plan1.sql
+-rw-r--r--   0        0        0      189 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_component_rendering__plan2.sql
+-rw-r--r--   0        0        0      254 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_component_rendering__plan3.sql
+-rw-r--r--   0        0        0      275 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_component_rendering__plan4.sql
+-rw-r--r--   0        0        0      289 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_component_rendering__plan5.sql
+-rw-r--r--   0        0        0       62 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_render_limit__plan0.sql
+-rw-r--r--   0        0        0      116 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_render_order_by__plan0.sql
+-rw-r--r--   0        0        0       87 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sql_plan_render.py/SqlQueryPlan/SqliteSqlClient/test_render_where__plan0.sql
+-rw-r--r--   0        0        0      117 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sub_query_reducer.py/SqlQueryPlan/test_reduce_sub_query__after_reducing.sql
+-rw-r--r--   0        0        0      257 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sub_query_reducer.py/SqlQueryPlan/test_reduce_sub_query__before_reducing.sql
+-rw-r--r--   0        0        0      167 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sub_query_reducer.py/SqlQueryPlan/test_rewrite_order_by_with_a_join_in_parent__after_reducing.sql
+-rw-r--r--   0        0        0      232 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_sub_query_reducer.py/SqlQueryPlan/test_rewrite_order_by_with_a_join_in_parent__before_reducing.sql
+-rw-r--r--   0        0        0      403 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_table_alias_simplifier.py/SqlQueryPlan/test_table_alias_simplification__after_alias_simplification.sql
+-rw-r--r--   0        0        0      479 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/snapshots/test_table_alias_simplifier.py/SqlQueryPlan/test_table_alias_simplification__before_alias_simplification.sql
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/sql/__init__.py
+-rw-r--r--   0        0        0     3390 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/sql/compare_sql_plan.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/sql/optimizer/__init__.py
+-rw-r--r--   0        0        0    34136 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/sql/optimizer/test_column_pruner.py
+-rw-r--r--   0        0        0    29034 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/sql/optimizer/test_rewriting_sub_query_reducer.py
+-rw-r--r--   0        0        0     8944 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/sql/optimizer/test_sub_query_reducer.py
+-rw-r--r--   0        0        0     6274 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/sql/optimizer/test_table_alias_simplifier.py
+-rw-r--r--   0        0        0     1988 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/sql/test_engine_specific_rendering.py
+-rw-r--r--   0        0        0     7909 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/sql/test_sql_expr_render.py
+-rw-r--r--   0        0        0    11429 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/sql/test_sql_plan_render.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/sql_clients/__init__.py
+-rw-r--r--   0        0        0     4380 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/sql_clients/test_sql_client.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/telemetry/__init__.py
+-rw-r--r--   0        0        0     3415 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/telemetry/test_telemetry.py
+-rw-r--r--   0        0        0     1427 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/test_object_utils.py
+-rw-r--r--   0        0        0     7061 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/test_specs.py
+-rw-r--r--   0        0        0     3326 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/test_utils.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/time/__init__.py
+-rw-r--r--   0        0        0      589 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/time/configurable_time_source.py
+-rw-r--r--   0        0        0     9898 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/test/time/test_time_granularity_solver.py
+-rw-r--r--   0        0        0        0 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/time/__init__.py
+-rw-r--r--   0        0        0      377 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/time/time_constants.py
+-rw-r--r--   0        0        0     8065 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/time/time_granularity.py
+-rw-r--r--   0        0        0    12945 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/time/time_granularity_solver.py
+-rw-r--r--   0        0        0      361 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/time/time_source.py
+-rw-r--r--   0        0        0      549 2022-04-27 23:54:19.001908 metricflow-0.93.0/metricflow/visitor.py
+-rw-r--r--   0        0        0     1465 2022-04-27 23:54:19.005908 metricflow-0.93.0/pyproject.toml
+-rw-r--r--   0        0        0     6547 2022-04-27 23:55:45.644601 metricflow-0.93.0/setup.py
+-rw-r--r--   0        0        0     1586 2022-04-27 23:55:45.645139 metricflow-0.93.0/PKG-INFO
```

### Comparing `metricflow-0.92.1/LICENSE` & `metricflow-0.93.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/cli/cli_context.py` & `metricflow-0.93.0/metricflow/cli/cli_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import logging
 
 from logging.handlers import TimedRotatingFileHandler
 from typing import Dict, Optional
 
 from metricflow.errors.errors import SqlClientCreationException, MetricFlowInitException
-from metricflow.cli.time_source import ServerTimeSource
 from metricflow.configuration.config_handler import ConfigHandler
-from metricflow.configuration.constants import (
-    CONFIG_DWH_SCHEMA,
-)
+from metricflow.configuration.constants import CONFIG_DWH_SCHEMA
 from metricflow.engine.metricflow_engine import MetricFlowEngine
 from metricflow.engine.utils import build_user_configured_model_from_config
 from metricflow.model.semantic_model import SemanticModel
-from metricflow.plan_conversion.column_resolver import DefaultColumnAssociationResolver
-from metricflow.plan_conversion.time_spine import TimeSpineSource
 from metricflow.protocols.sql_client import SqlClient
 from metricflow.sql_clients.sql_utils import make_sql_client_from_config
 from metricflow.model.objects.user_configured_model import UserConfiguredModel
 
 logger = logging.getLogger(__name__)
 
 
@@ -84,22 +79,15 @@
             return self.sql_client.health_checks(self.mf_system_schema)
         except Exception as e:
             raise SqlClientCreationException from e
 
     def _initialize_metricflow_engine(self) -> None:
         """Initialize the MetricFlowEngine."""
         try:
-            self._mf = MetricFlowEngine(
-                semantic_model=self.semantic_model,
-                sql_client=self.sql_client,
-                column_association_resolver=DefaultColumnAssociationResolver(self.semantic_model),
-                time_source=ServerTimeSource(),
-                time_spine_source=TimeSpineSource(self.sql_client, schema_name=self.mf_system_schema),
-                system_schema=self.mf_system_schema,
-            )
+            self._mf = MetricFlowEngine.from_config(self.config)
         except Exception as e:
             raise MetricFlowInitException from e
 
     @property
     def mf(self) -> MetricFlowEngine:  # noqa: D
         if self._mf is None:
             self._initialize_metricflow_engine()
```

### Comparing `metricflow-0.92.1/metricflow/cli/main.py` & `metricflow-0.93.0/metricflow/cli/main.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/cli/models.py` & `metricflow-0.93.0/metricflow/engine/models.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/cli/sample_models/customers.yaml` & `metricflow-0.93.0/metricflow/cli/sample_models/customers.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/cli/sample_models/transactions.yaml` & `metricflow-0.93.0/metricflow/cli/sample_models/transactions.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/cli/tutorial.py` & `metricflow-0.93.0/metricflow/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/cli/utils.py` & `metricflow-0.93.0/metricflow/cli/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,24 @@
     CONFIG_DWH_DIALECT,
     CONFIG_DWH_HOST,
     CONFIG_DWH_PASSWORD,
     CONFIG_DWH_PORT,
     CONFIG_DWH_SCHEMA,
     CONFIG_DWH_USER,
     CONFIG_DWH_WAREHOUSE,
+    CONFIG_EMAIL,
     CONFIG_MODEL_PATH,
 )
 from metricflow.model.validations.validator_helpers import ValidationIssueLevel
 
 logger = logging.getLogger(__name__)
 
 # MetricFlow config keys
 MF_CONFIG_KEYS = [
+    ConfigKey(key=CONFIG_EMAIL, comment="Optional"),
     ConfigKey(
         key=CONFIG_MODEL_PATH,
         value=f"{pathlib.Path.home()}/.metricflow/sample_models",
         comment="Path to directory containing defined models (Leave until after DWH setup)",
     ),
     ConfigKey(key=CONFIG_DWH_SCHEMA),
 ]
@@ -128,27 +130,18 @@
 
 # Parsers/Validators
 def convert_to_datetime(datetime_str: Optional[str]) -> Optional[dt.datetime]:
     """Callback to convert string to datetime given as an iso8601 timestamp."""
     if datetime_str is None:
         return None
 
-    if not valid_datetime(datetime_str):
-        raise click.BadParameter("must be valid iso8601 timestamp")
-
-    return dt.datetime.fromisoformat(datetime_str)
-
-
-def valid_datetime(dt_str: str) -> bool:
-    """Returns true if string is valid iso8601 timestamp, false otherwise"""
     try:
-        parse(dt_str)
+        return parse(datetime_str)
     except Exception:
-        return False
-    return True
+        raise click.BadParameter("must be valid iso8601 timestamp")
 
 
 def parse_comma_separated_inputs(value: Optional[str]) -> Optional[List[str]]:  # noqa: D
     # If comma exist, explode this into a list and return
     if value is None:
         return None
     if "," in value:
```

### Comparing `metricflow-0.92.1/metricflow/column_assoc.py` & `metricflow-0.93.0/metricflow/column_assoc.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/configuration/config_builder.py` & `metricflow-0.93.0/metricflow/configuration/config_builder.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/configuration/config_handler.py` & `metricflow-0.93.0/metricflow/configuration/config_handler.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/configuration/env_var.py` & `metricflow-0.93.0/metricflow/configuration/env_var.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/configuration/yaml_handler.py` & `metricflow-0.93.0/metricflow/configuration/yaml_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import yaml
 
-from typing import Dict
+from typing import Dict, Optional
 
 
 class YamlFileHandler:
     """Class to handle interactions with a non-nested yaml."""
 
     def __init__(self, yaml_file_path: str) -> None:  # noqa: D
         self.yaml_file_path = yaml_file_path
@@ -14,25 +14,18 @@
         """Reads the provided yaml file and loads it into a dictionary."""
         content: Dict[str, str] = {}
         if os.path.exists(self.yaml_file_path):
             with open(self.yaml_file_path) as f:
                 content = yaml.load(f, Loader=yaml.SafeLoader) or {}
         return content
 
-    def get_value(self, key: str) -> str:
+    def get_value(self, key: str) -> Optional[str]:
         """Attempts to get a corresponding value from the yaml file. Throw an error if not exists or None."""
         content = self._load_yaml()
-
-        if key not in content:
-            raise KeyError(f"Key '{key}' is missing in the yaml file '{self.yaml_file_path}'")
-
-        value = content[key]
-        if value is None:
-            raise ValueError(f"Value for key '{key}' cannot be None in the yaml file '{self.yaml_file_path}")
-        return value
+        return content.get(key)
 
     def set_value(self, key: str, value: str) -> None:
         """Sets a value to a given key in yaml file."""
         content = self._load_yaml()
         content[key] = value
         with open(self.yaml_file_path, "w") as f:
             yaml.dump(content, f)
@@ -41,7 +34,12 @@
         """Removes a key in yaml file."""
         content = self._load_yaml()
         if key not in content:
             return
         del content[key]
         with open(self.yaml_file_path, "w") as f:
             yaml.dump(content, f)
+
+    @property
+    def url(self) -> str:
+        """Returns the file url of this handler."""
+        return f"file:/{self.yaml_file_path}"
```

### Comparing `metricflow-0.92.1/metricflow/constraints/time_constraint.py` & `metricflow-0.93.0/metricflow/constraints/time_constraint.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dag/dag_to_text.py` & `metricflow-0.93.0/metricflow/dag/dag_to_text.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dag/dag_visualization.py` & `metricflow-0.93.0/metricflow/dag/dag_visualization.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dag/id_generation.py` & `metricflow-0.93.0/metricflow/dag/id_generation.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dag/mf_dag.py` & `metricflow-0.93.0/metricflow/dag/mf_dag.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dataflow/builder/costing.py` & `metricflow-0.93.0/metricflow/dataflow/builder/costing.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dataflow/builder/dataflow_plan_builder.py` & `metricflow-0.93.0/metricflow/dataflow/builder/dataflow_plan_builder.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dataflow/builder/node_data_set.py` & `metricflow-0.93.0/metricflow/dataflow/builder/node_data_set.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dataflow/builder/node_evaluator.py` & `metricflow-0.93.0/metricflow/dataflow/builder/node_evaluator.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dataflow/builder/partitions.py` & `metricflow-0.93.0/metricflow/dataflow/builder/partitions.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dataflow/dataflow_plan.py` & `metricflow-0.93.0/metricflow/dataflow/dataflow_plan.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dataflow/dataflow_plan_to_text.py` & `metricflow-0.93.0/metricflow/dataflow/dataflow_plan_to_text.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dataflow/sql_table.py` & `metricflow-0.93.0/metricflow/dataflow/sql_table.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dataset/convert_data_source.py` & `metricflow-0.93.0/metricflow/dataset/convert_data_source.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dataset/data_source_adapter.py` & `metricflow-0.93.0/metricflow/dataset/data_source_adapter.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/dataset/dataset.py` & `metricflow-0.93.0/metricflow/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/engine/metricflow_engine.py` & `metricflow-0.93.0/metricflow/engine/metricflow_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,36 +5,42 @@
 import textwrap
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Optional, List, Sequence
 
 import pandas as pd
 
-from metricflow.cli.models import Dimension, Metric
-from metricflow.cli.models import Materialization
+from metricflow.configuration.constants import CONFIG_DWH_SCHEMA
+from metricflow.configuration.yaml_handler import YamlFileHandler
 from metricflow.dataflow.builder.dataflow_plan_builder import DataflowPlanBuilder
 from metricflow.dataflow.dataflow_plan import DataflowPlan
 from metricflow.dataflow.sql_table import SqlTable
 from metricflow.dataset.convert_data_source import DataSourceToDataSetConverter
+from metricflow.engine.models import Dimension, Materialization, Metric
+from metricflow.engine.time_source import ServerTimeSource
+from metricflow.engine.utils import build_user_configured_model_from_config
 from metricflow.execution.execution_plan import ExecutionPlan, SqlQuery
 from metricflow.execution.execution_plan_to_text import execution_plan_to_text
 from metricflow.execution.executor import SequentialPlanExecutor
 from metricflow.model.semantic_model import SemanticModel
 from metricflow.object_utils import pformat_big_objects, random_id
+from metricflow.plan_conversion.column_resolver import DefaultColumnAssociationResolver
 from metricflow.plan_conversion.dataflow_to_execution import DataflowToExecutionPlanConverter
 from metricflow.plan_conversion.dataflow_to_sql import DataflowToSqlQueryPlanConverter
 from metricflow.plan_conversion.time_spine import TimeSpineSource
 from metricflow.protocols.sql_client import SqlClient
 from metricflow.query.query_parser import MetricFlowQueryParser
 from metricflow.specs import ColumnAssociationResolver
 from metricflow.specs import MetricSpec, MetricFlowQuerySpec
 from metricflow.sql.optimizer.optimization_levels import SqlQueryOptimizationLevel
 from metricflow.time.time_source import TimeSource
 from metricflow.dataset.data_source_adapter import DataSourceDataSet
 from metricflow.errors.errors import ExecutionException, MaterializationNotFoundError
+from metricflow.sql_clients.sql_utils import make_sql_client_from_config
+from metricflow.sql_clients.common_client import not_empty
 from metricflow.telemetry.models import TelemetryLevel
 from metricflow.telemetry.reporter import TelemetryReporter, log_call
 
 logger = logging.getLogger(__name__)
 _telemetry_reporter = TelemetryReporter(report_levels_higher_or_equal_to=TelemetryLevel.USAGE)
 _telemetry_reporter.add_python_log_handler()
 _telemetry_reporter.add_rudderstack_handler()
@@ -76,15 +82,15 @@
     @staticmethod
     def create_with_random_request_id(  # noqa: D
         metric_names: Sequence[str],
         group_by_names: Sequence[str],
         limit: Optional[int] = None,
         time_constraint_start: Optional[datetime.datetime] = None,
         time_constraint_end: Optional[datetime.datetime] = None,
-        where_constraint: str = None,
+        where_constraint: Optional[str] = None,
         order_by_names: Optional[Sequence[str]] = None,
         output_table: Optional[str] = None,
         sql_optimization_level: SqlQueryOptimizationLevel = SqlQueryOptimizationLevel.O4,
     ) -> MetricFlowQueryRequest:
         return MetricFlowQueryRequest(
             request_id=MetricFlowRequestId(mf_rid=f"{random_id()}"),
             metric_names=metric_names,
@@ -198,15 +204,19 @@
         Returns:
             A list of dimension values as string.
         """
         pass
 
     @abstractmethod
     def list_materializations(self) -> List[Materialization]:
-        """Retrieves a list of materialization names."""
+        """Retrieves a list of materialization names.
+
+        Returns:
+            A list of Materialization objects containing metadata.
+        """
         pass
 
     @abstractmethod
     def materialize(
         self,
         materialization_name: str,
         time_constraint_start: Optional[datetime.datetime] = None,
@@ -240,52 +250,75 @@
 
 
 class MetricFlowEngine(AbstractMetricFlowEngine):
     """Main entry point for queries."""
 
     _LOGGING_INDENT = "   "
 
-    def __init__(  # noqa: D
+    @staticmethod
+    def from_config(handler: YamlFileHandler) -> MetricFlowEngine:
+        """Initialize MetricFlowEngine via yaml config file."""
+        sql_client = make_sql_client_from_config(handler)
+        semantic_model = SemanticModel(build_user_configured_model_from_config(handler))
+        system_schema = not_empty(handler.get_value(CONFIG_DWH_SCHEMA), CONFIG_DWH_SCHEMA, handler.url)
+        return MetricFlowEngine(
+            semantic_model=semantic_model,
+            sql_client=sql_client,
+            system_schema=system_schema,
+        )
+
+    def __init__(
         self,
         semantic_model: SemanticModel,
         sql_client: SqlClient,
-        column_association_resolver: ColumnAssociationResolver,
-        time_source: TimeSource,
-        time_spine_source: TimeSpineSource,
         system_schema: str,
+        time_source: TimeSource = ServerTimeSource(),
+        column_association_resolver: Optional[ColumnAssociationResolver] = None,
+        time_spine_source: Optional[TimeSpineSource] = None,
     ) -> None:
+        """Initializer for MetricFlowEngine
+
+        For direct calls to construct MetricFlowEngine, do not pass the following parameters,
+        - time_source
+        - column_association_resolver
+        - time_spine_source
+        These parameters are mainly there to be overridden during tests.
+        """
+
         self._semantic_model = semantic_model
         self._sql_client = sql_client
-        self._column_association_resolver = column_association_resolver
+        self._column_association_resolver = column_association_resolver or (
+            DefaultColumnAssociationResolver(semantic_model)
+        )
         self._time_source = time_source
-        self._time_spine_source = time_spine_source
+        self._time_spine_source = time_spine_source or TimeSpineSource(sql_client, schema_name=system_schema)
+
         self._schema = system_schema
 
         self._source_data_sets: List[DataSourceDataSet] = []
-        self._column_association_resolver = column_association_resolver
-        converter = DataSourceToDataSetConverter(column_association_resolver=column_association_resolver)
+        converter = DataSourceToDataSetConverter(column_association_resolver=self._column_association_resolver)
         for data_source in self._semantic_model.user_configured_model.data_sources:
             data_set = converter.create_sql_source_data_set(data_source)
             self._source_data_sets.append(data_set)
             logger.info(f"Created source dataset from data source '{data_source.name}'")
 
         self._primary_time_dimension_reference = (
             self._semantic_model.data_source_semantics.primary_time_dimension_reference
         )
 
         self._dataflow_plan_builder = DataflowPlanBuilder(
             data_sets=self._source_data_sets,
             semantic_model=self._semantic_model,
             primary_time_dimension_reference=self._primary_time_dimension_reference,
-            time_spine_source=time_spine_source,
+            time_spine_source=self._time_spine_source,
         )
         self._to_sql_query_plan_converter = DataflowToSqlQueryPlanConverter[DataSourceDataSet](
             column_association_resolver=self._column_association_resolver,
             semantic_model=self._semantic_model,
-            time_spine_source=time_spine_source,
+            time_spine_source=self._time_spine_source,
         )
         self._to_execution_plan_converter = DataflowToExecutionPlanConverter(
             sql_plan_converter=self._to_sql_query_plan_converter,
             sql_plan_renderer=self._sql_client.sql_engine_attributes.sql_query_plan_renderer,
             sql_client=sql_client,
         )
         self._executor = SequentialPlanExecutor()
```

### Comparing `metricflow-0.92.1/metricflow/errors/errors.py` & `metricflow-0.93.0/metricflow/errors/errors.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/execution/execution_plan.py` & `metricflow-0.93.0/metricflow/execution/execution_plan.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/execution/execution_plan_to_text.py` & `metricflow-0.93.0/metricflow/execution/execution_plan_to_text.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/execution/executor.py` & `metricflow-0.93.0/metricflow/execution/executor.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/instances.py` & `metricflow-0.93.0/metricflow/instances.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/graph.py` & `metricflow-0.93.0/metricflow/model/graph.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/model_transformer.py` & `metricflow-0.93.0/metricflow/model/model_transformer.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/model_validator.py` & `metricflow-0.93.0/metricflow/model/model_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import copy
 import logging
 from typing import List
 
 from metricflow.model.objects.user_configured_model import UserConfiguredModel
 from metricflow.model.parsing.dir_to_model import ModelBuildResult
-from metricflow.model.validations.common_identifiers import CommonIdentifiersRule
 from metricflow.model.validations.data_sources import (
     DataSourceMeasuresUniqueRule,
     DataSourceTimeDimensionWarningsRule,
 )
 from metricflow.model.validations.dimension_const import DimensionConsistencyRule
 from metricflow.model.validations.element_const import ElementConsistencyRule
 from metricflow.model.validations.identifiers import IdentifierConfigRule, OnePrimaryIdentifierPerDataSourceRule
+from metricflow.model.validations.materializations import ValidMaterializationRule
 from metricflow.model.validations.metrics import MetricMeasuresRule, CumulativeMetricRule
 from metricflow.model.validations.non_empty import NonEmptyRule
 from metricflow.model.validations.unique_valid_name import UniqueAndValidNameRule
 from metricflow.model.validations.validator_helpers import (
     ValidationIssueType,
     ModelValidationRule,
     ValidationIssueLevel,
@@ -25,25 +25,25 @@
 logger = logging.getLogger(__name__)
 
 
 class ModelValidator:
     """A Validator that acts on UserConfiguredModel"""
 
     VALIDATION_RULES: List[ModelValidationRule] = [
-        CommonIdentifiersRule(),
         DataSourceMeasuresUniqueRule(),
         DataSourceTimeDimensionWarningsRule(),
         DimensionConsistencyRule(),
         ElementConsistencyRule(),
         IdentifierConfigRule(),
         OnePrimaryIdentifierPerDataSourceRule(),
         MetricMeasuresRule(),
         CumulativeMetricRule(),
         NonEmptyRule(),
         UniqueAndValidNameRule(),
+        ValidMaterializationRule(),
     ]
 
     @staticmethod
     def validate_model(model: UserConfiguredModel) -> ModelBuildResult:
         """Validate a model according to configured rules."""
         model_copy = copy.deepcopy(model)
 
@@ -57,15 +57,15 @@
         # If there are any errors, don't run any transforms and return the issues found.
         if any([x.level == ValidationIssueLevel.ERROR for x in issues]):
             return ModelBuildResult(model=model_copy, issues=tuple(issues))
 
         return ModelBuildResult(model=model_copy, issues=tuple(issues))
 
     @staticmethod
-    def checked_validations(model: UserConfiguredModel) -> UserConfiguredModel:
+    def checked_validations(model: UserConfiguredModel) -> UserConfiguredModel:  # chTODO: remember checked_build
         """Similar to validate(), but throws an exception if validation fails."""
         model_copy = copy.deepcopy(model)
         build_result = ModelValidator.validate_model(model_copy)
         if build_result.issues is not None:
             if any(
                 [
                     x.level == ValidationIssueLevel.WARNING or x.level == ValidationIssueLevel.FUTURE_ERROR
```

### Comparing `metricflow-0.92.1/metricflow/model/objects/common.py` & `metricflow-0.93.0/metricflow/model/objects/common.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/objects/constraints/where.py` & `metricflow-0.93.0/metricflow/model/objects/constraints/where.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/objects/data_source.py` & `metricflow-0.93.0/metricflow/model/objects/data_source.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/objects/elements/dimension.py` & `metricflow-0.93.0/metricflow/model/objects/elements/dimension.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/objects/elements/identifier.py` & `metricflow-0.93.0/metricflow/model/objects/elements/identifier.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/objects/elements/measure.py` & `metricflow-0.93.0/metricflow/model/objects/elements/measure.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/objects/materialization.py` & `metricflow-0.93.0/metricflow/model/objects/materialization.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/objects/metric.py` & `metricflow-0.93.0/metricflow/model/objects/metric.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/objects/utils.py` & `metricflow-0.93.0/metricflow/model/objects/utils.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/parsing/dir_to_model.py` & `metricflow-0.93.0/metricflow/model/parsing/dir_to_model.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/parsing/schemas.py` & `metricflow-0.93.0/metricflow/model/parsing/schemas.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/parsing/schemas_internal.py` & `metricflow-0.93.0/metricflow/model/parsing/schemas_internal.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/parsing/validation.py` & `metricflow-0.93.0/metricflow/model/parsing/validation.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/parsing/yaml_loader.py` & `metricflow-0.93.0/metricflow/model/parsing/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/semantic_model.py` & `metricflow-0.93.0/metricflow/model/semantic_model.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/semantics/data_source_container.py` & `metricflow-0.93.0/metricflow/model/semantics/data_source_container.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/semantics/linkable_spec_resolver.py` & `metricflow-0.93.0/metricflow/model/semantics/linkable_spec_resolver.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/semantics/links_new.py` & `metricflow-0.93.0/metricflow/model/semantics/links_new.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/semantics/semantic_containers.py` & `metricflow-0.93.0/metricflow/model/semantics/semantic_containers.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/transformations/boolean_measure.py` & `metricflow-0.93.0/metricflow/model/transformations/boolean_measure.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/transformations/identifiers.py` & `metricflow-0.93.0/metricflow/model/transformations/identifiers.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/transformations/names.py` & `metricflow-0.93.0/metricflow/model/transformations/names.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/transformations/proxy_measure.py` & `metricflow-0.93.0/metricflow/model/transformations/proxy_measure.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/validations/common_identifiers.py` & `metricflow-0.93.0/metricflow/model/validations/common_identifiers.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/validations/data_sources.py` & `metricflow-0.93.0/metricflow/model/validations/data_sources.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/validations/dim_names.py` & `metricflow-0.93.0/metricflow/model/validations/dim_names.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from metricflow.model.objects.metric import Metric
 from metricflow.model.objects.user_configured_model import UserConfiguredModel
 from metricflow.model.validations.validator_helpers import ModelObjectType
 from metricflow.specs import (
     MeasureReference,
     DimensionReference,
     IdentifierReference,
-    IdentifierSpec,
     DimensionSpec,
     LinklessIdentifierSpec,
 )
 
 logger = logging.getLogger(__name__)
 pp = pprint.PrettyPrinter(indent=2)
 
@@ -108,16 +107,16 @@
             for dimension in data_source.dimensions:
                 self._element_name_to_type[dimension.name.element_name] = ModelObjectType.DIMENSION
             for identifier in data_source.identifiers:
                 self._element_name_to_type[identifier.name.element_name] = ModelObjectType.IDENTIFIER
 
     def _is_identifier_valid_for_measure(self, measure_reference: MeasureReference, identifier_name: str) -> bool:
         assert measure_reference in self._measures_to_identifiers
-        identifier_spec = IdentifierSpec.parse(identifier_name)
-        return identifier_spec in self._measures_to_identifiers[measure_reference]
+        identifier_ref = IdentifierReference.parse(identifier_name)
+        return identifier_ref in self._measures_to_identifiers[measure_reference]
 
     def is_dimension_valid_for_measure(self, measure_reference: MeasureReference, dimension_name: str) -> bool:
         """Return true iff the given measure and dimension could be queried together."""
 
         logger.debug(
             f"Checking if dimension name `{dimension_name} is valid for measure `{measure_reference.element_name}` "
         )
```

### Comparing `metricflow-0.92.1/metricflow/model/validations/dimension_const.py` & `metricflow-0.93.0/metricflow/model/validations/dimension_const.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/validations/element_const.py` & `metricflow-0.93.0/metricflow/model/validations/element_const.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/validations/identifiers.py` & `metricflow-0.93.0/metricflow/model/validations/identifiers.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/validations/metrics.py` & `metricflow-0.93.0/metricflow/model/validations/metrics.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/validations/non_empty.py` & `metricflow-0.93.0/metricflow/model/validations/non_empty.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/validations/unique_valid_name.py` & `metricflow-0.93.0/metricflow/model/validations/unique_valid_name.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/model/validations/validator_helpers.py` & `metricflow-0.93.0/metricflow/model/validations/validator_helpers.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/naming/linkable_spec_name.py` & `metricflow-0.93.0/metricflow/naming/linkable_spec_name.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/object_utils.py` & `metricflow-0.93.0/metricflow/object_utils.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/plan_conversion/column_resolver.py` & `metricflow-0.93.0/metricflow/plan_conversion/column_resolver.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/plan_conversion/dataflow_to_execution.py` & `metricflow-0.93.0/metricflow/plan_conversion/dataflow_to_execution.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/plan_conversion/dataflow_to_sql.py` & `metricflow-0.93.0/metricflow/plan_conversion/dataflow_to_sql.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/plan_conversion/instance_converters.py` & `metricflow-0.93.0/metricflow/plan_conversion/instance_converters.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/plan_conversion/node_processor.py` & `metricflow-0.93.0/metricflow/plan_conversion/node_processor.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/plan_conversion/select_column_gen.py` & `metricflow-0.93.0/metricflow/plan_conversion/select_column_gen.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/plan_conversion/spec_transforms.py` & `metricflow-0.93.0/metricflow/plan_conversion/spec_transforms.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/plan_conversion/sql_dataset.py` & `metricflow-0.93.0/metricflow/plan_conversion/sql_dataset.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/plan_conversion/time_spine.py` & `metricflow-0.93.0/metricflow/plan_conversion/time_spine.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/protocols/sql_client.py` & `metricflow-0.93.0/metricflow/protocols/sql_client.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/query/query_parser.py` & `metricflow-0.93.0/metricflow/query/query_parser.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/spec_set_transforms.py` & `metricflow-0.93.0/metricflow/spec_set_transforms.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/specs.py` & `metricflow-0.93.0/metricflow/specs.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql/optimizer/column_pruner.py` & `metricflow-0.93.0/metricflow/sql/optimizer/column_pruner.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql/optimizer/optimization_levels.py` & `metricflow-0.93.0/metricflow/sql/optimizer/optimization_levels.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql/optimizer/rewriting_sub_query_reducer.py` & `metricflow-0.93.0/metricflow/sql/optimizer/rewriting_sub_query_reducer.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql/optimizer/sub_query_reducer.py` & `metricflow-0.93.0/metricflow/sql/optimizer/sub_query_reducer.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql/optimizer/table_alias_simplifier.py` & `metricflow-0.93.0/metricflow/sql/optimizer/table_alias_simplifier.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql/render/big_query.py` & `metricflow-0.93.0/metricflow/sql/render/big_query.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql/render/expr_renderer.py` & `metricflow-0.93.0/metricflow/sql/render/expr_renderer.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql/render/redshift.py` & `metricflow-0.93.0/metricflow/sql/render/redshift.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql/render/sql_plan_renderer.py` & `metricflow-0.93.0/metricflow/sql/render/sql_plan_renderer.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql/render/sqlite.py` & `metricflow-0.93.0/metricflow/sql/render/sqlite.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql/sql_bind_parameters.py` & `metricflow-0.93.0/metricflow/sql/sql_bind_parameters.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql/sql_exprs.py` & `metricflow-0.93.0/metricflow/sql/sql_exprs.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql/sql_plan.py` & `metricflow-0.93.0/metricflow/sql/sql_plan.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql/sql_plan_to_text.py` & `metricflow-0.93.0/metricflow/sql/sql_plan_to_text.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql_clients/base_sql_client_implementation.py` & `metricflow-0.93.0/metricflow/sql_clients/base_sql_client_implementation.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql_clients/big_query.py` & `metricflow-0.93.0/metricflow/sql_clients/big_query.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql_clients/common_client.py` & `metricflow-0.93.0/metricflow/sql_clients/common_client.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql_clients/redshift.py` & `metricflow-0.93.0/metricflow/sql_clients/redshift.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql_clients/snowflake.py` & `metricflow-0.93.0/metricflow/sql_clients/snowflake.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql_clients/sql_utils.py` & `metricflow-0.93.0/metricflow/sql_clients/sql_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,42 +70,42 @@
     else:
         raise ValueError(f"Unknown dialect: `{dialect}` in URL {url}")
 
 
 def make_sql_client_from_config(handler: YamlFileHandler) -> SqlClient:
     """Construct a SqlClient given a yaml file config."""
 
-    dialect = handler.get_value(CONFIG_DWH_DIALECT).upper()
-    url = f"file://{handler.yaml_file_path}"
+    url = handler.url
+    dialect = not_empty(handler.get_value(CONFIG_DWH_DIALECT), CONFIG_DWH_DIALECT, url).upper()
     if dialect == SupportedSqlEngine.BIGQUERY.name:
         path_to_creds = not_empty(handler.get_value(CONFIG_DWH_PASSWORD), CONFIG_DWH_PASSWORD, url)
         if not pathlib.Path(path_to_creds).exists:
             raise ValueError(f"`{path_to_creds}` does not contain the BigQuery credential file.")
         with open(path_to_creds, "r") as cred_file:
             creds = cred_file.read()
         return BigQuerySqlClient(password=creds)
     elif dialect == SupportedSqlEngine.SNOWFLAKE.name:
         host = not_empty(handler.get_value(CONFIG_DWH_HOST), CONFIG_DWH_HOST, url)
         user = not_empty(handler.get_value(CONFIG_DWH_USER), CONFIG_DWH_USER, url)
-        password = handler.get_value(CONFIG_DWH_PASSWORD)
+        password = not_empty(handler.get_value(CONFIG_DWH_PASSWORD), CONFIG_DWH_PASSWORD, url)
         database = not_empty(handler.get_value(CONFIG_DWH_DB), CONFIG_DWH_DB, url)
         warehouse = not_empty(handler.get_value(CONFIG_DWH_WAREHOUSE), CONFIG_DWH_WAREHOUSE, url)
         return SnowflakeSqlClient(
             host=host,
             username=user,
             password=password,
             database=database,
             url_query_params={"warehouse": warehouse},
             client_session_keep_alive=False,
         )
     elif dialect == SupportedSqlEngine.REDSHIFT.name:
         host = not_empty(handler.get_value(CONFIG_DWH_HOST), CONFIG_DWH_HOST, url)
-        port = int(handler.get_value(CONFIG_DWH_PORT))
+        port = int(not_empty(handler.get_value(CONFIG_DWH_PORT), CONFIG_DWH_PORT, url))
         user = not_empty(handler.get_value(CONFIG_DWH_USER), CONFIG_DWH_USER, url)
-        password = handler.get_value(CONFIG_DWH_PASSWORD)
+        password = not_empty(handler.get_value(CONFIG_DWH_PASSWORD), CONFIG_DWH_PASSWORD, url)
         database = not_empty(handler.get_value(CONFIG_DWH_DB), CONFIG_DWH_DB, url)
         return RedshiftSqlClient(
             host=host,
             port=port,
             username=user,
             password=password,
             database=database,
```

### Comparing `metricflow-0.92.1/metricflow/sql_clients/sqlalchemy_dialect.py` & `metricflow-0.93.0/metricflow/sql_clients/sqlalchemy_dialect.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/sql_clients/sqlite.py` & `metricflow-0.93.0/metricflow/sql_clients/sqlite.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/telemetry/handlers/handlers.py` & `metricflow-0.93.0/metricflow/telemetry/handlers/handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 logger = logging.getLogger(__name__)
 
 
 class TelemetryHandler(ABC):
     """Base class to record telemetry to some destination."""
 
     @abstractmethod
-    def _write_log(self, session_id: str, payload: PayloadType) -> None:
+    def _write_log(self, client_id: str, payload: PayloadType) -> None:
         """Subclasses should implement this to log a serialized version of the payload."""
         pass
 
     def log(
         self,
-        session_id: str,
+        client_id: str,
         function_start_event: Optional[FunctionStartEvent] = None,
         function_end_event: Optional[FunctionEndEvent] = None,
     ) -> bool:
         """Log an event to telemetry."""
         payload = TelemetryPayload(
-            session_id=session_id,
+            client_id=client_id,
             function_start_events=(function_start_event,) if function_start_event else (),
             function_end_events=(function_end_event,) if function_end_event else (),
         )
-        self._write_log(session_id, payload.dict())
+        self._write_log(client_id, payload.dict())
         return True
 
 
 class RudderstackTelemetryHandler(TelemetryHandler):
     """A telemetry client that logs data to Rudderstack."""
 
     RUDDERSTACK_EVENT_NAME = "MF_OSS"
@@ -49,56 +49,56 @@
         data_plane_url: str = TFD_DATA_PLANE,
         write_key: str = TFD_WRITE_KEY,
     ) -> None:
         self._rudderstack_client = RudderstackClient(
             write_key=write_key, host=data_plane_url, debug=False, on_error=None, send=True, sync_mode=False
         )
 
-    def _write_log(self, session_id: str, payload: PayloadType) -> None:  # noqa: D
+    def _write_log(self, client_id: str, payload: PayloadType) -> None:  # noqa: D
         """Write log to rudderstack.
 
         Added context to handle the error, but seems odd.
 
         >       msg['context']['traits']['anonymousId'] = msg['anonymousId']
         E       KeyError: 'traits'
 
         /usr/local/lib/python3.8/site-packages/rudder_analytics/client.py:243: KeyError
         """
         context: PayloadType = {"traits": {}}
         self._rudderstack_client.track(
-            anonymous_id=session_id,
+            anonymous_id=client_id,
             event=RudderstackTelemetryHandler.RUDDERSTACK_EVENT_NAME,
             timestamp=datetime.now(),
             properties=payload,
             context=context,
         )
 
 
 class ToMemoryTelemetryHandler(TelemetryHandler):
     """Records telemetry events to memory for testing purposes."""
 
     def __init__(self) -> None:  # noqa: D
         self._payloads: List[TelemetryPayload] = []
 
-    def _write_log(self, session_id: str, payload: PayloadType) -> None:  # noqa: D
+    def _write_log(self, client_id: str, payload: PayloadType) -> None:  # noqa: D
         pass
 
     @property
     def payloads(self) -> Sequence[TelemetryPayload]:  # noqa: D
         return self._payloads
 
     def log(
         self,
-        session_id: str,
+        client_id: str,
         function_start_event: Optional[FunctionStartEvent] = None,
         function_end_event: Optional[FunctionEndEvent] = None,
     ) -> bool:
         """Log an event to telemetry"""
         payload = TelemetryPayload(
-            session_id=session_id,
+            client_id=client_id,
             function_start_events=(function_start_event,) if function_start_event else (),
             function_end_events=(function_end_event,) if function_end_event else (),
         )
         if len(self._payloads) > 10:
             self._payloads.pop()
 
         self._payloads.append(payload)
```

### Comparing `metricflow-0.92.1/metricflow/telemetry/handlers/python_log.py` & `metricflow-0.93.0/metricflow/telemetry/handlers/python_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 
 class PythonLoggerTelemetryHandler(TelemetryHandler):
     """A telemetry client that logs data to the Python logger for debugging during tests."""
 
     def __init__(self, logger_level: int) -> None:  # noqa: D
         self._logger_level = logger_level
 
-    def _write_log(self, session_id: str, payload: PayloadType) -> None:  # noqa: D
+    def _write_log(self, client_id: str, payload: PayloadType) -> None:  # noqa: D
         logger.log(
             level=self._logger_level,
             msg=f"Logging telemetry payload:\n{textwrap.indent(pformat_big_objects(payload), prefix='    ')}",
         )
```

### Comparing `metricflow-0.92.1/metricflow/telemetry/models.py` & `metricflow-0.93.0/metricflow/telemetry/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,11 +94,11 @@
             exception_trace=exception_trace,
         )
 
 
 class TelemetryPayload(FrozenBaseModel):
     """Payload that can be easily serialized to JSON."""
 
-    session_id: str
+    client_id: str
     function_start_events: Tuple[FunctionStartEvent, ...] = ()
     function_end_events: Tuple[FunctionEndEvent, ...] = ()
     payload_schema: str = EVENT_SCHEMA
```

### Comparing `metricflow-0.92.1/metricflow/telemetry/reporter.py` & `metricflow-0.93.0/metricflow/telemetry/reporter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import datetime
 import functools
 import logging
 import platform
+import os
 import sys
 import time
 import traceback
 import uuid
 from hashlib import sha256
 from typing import Callable, Optional, Any
 from typing import List
 
+from metricflow.configuration.config_handler import ConfigHandler
+from metricflow.configuration.constants import CONFIG_EMAIL
 from metricflow.object_utils import random_id
 from metricflow.telemetry.handlers.handlers import (
     ToMemoryTelemetryHandler,
     TelemetryHandler,
     RudderstackTelemetryHandler,
 )
 from metricflow.telemetry.handlers.python_log import PythonLoggerTelemetryHandler
@@ -22,37 +25,41 @@
 logger = logging.getLogger(__name__)
 
 
 class TelemetryReporter:
     """Reports telemetry for improving product experience"""
 
     # Session ID to use when requesting a non-uniquely identifiable ID.
-    FULLY_ANONYMOUS_SESSION_ID = "anonymous"
+    FULLY_ANONYMOUS_CLIENT_ID = "anonymous"
+    ENV_EMAIL_OVERRIDE = "METRICFLOW_CLIENT_EMAIL"
 
     def __init__(self, report_levels_higher_or_equal_to: TelemetryLevel, fully_anonymous: bool = False) -> None:
-        """If fully_anonymous is set, use a session_id that is not unique."""
+        """If fully_anonymous is set, use a client_id that is not unique."""
         self._report_levels_higher_or_equal_to = report_levels_higher_or_equal_to
         self._fully_anonymous = fully_anonymous
+        self._email = os.getenv(TelemetryReporter.ENV_EMAIL_OVERRIDE) or ConfigHandler().get_value(CONFIG_EMAIL)
 
         if fully_anonymous:
-            self._session_id = TelemetryReporter.FULLY_ANONYMOUS_SESSION_ID
+            self._client_id = TelemetryReporter.FULLY_ANONYMOUS_CLIENT_ID
+        elif self._email:
+            self._client_id = self._email
         else:
-            self._session_id = TelemetryReporter._create_session_id()
+            self._client_id = TelemetryReporter._create_client_id()
 
         # For testing
         self._test_handler = ToMemoryTelemetryHandler()
         self._handlers: List[TelemetryHandler] = []
 
     @staticmethod
-    def _create_session_id() -> str:
+    def _create_client_id() -> str:
         """Creates an identifier for the current user based on their current environment.
 
         More specifically, this function creates a SHA-256 hash based on the system platform, release, and MAC address.
 
-        The created session ID is not guaranteed to be unique by user.
+        The created client ID is not guaranteed to be unique by user.
         """
         # getnode() returns the MAC.
         id_str = "_".join([sys.platform, platform.release(), str(uuid.getnode())])
         return sha256(id_str.encode("utf-8")).hexdigest()
 
     def add_python_log_handler(self) -> None:  # noqa: D
         self._handlers.append(PythonLoggerTelemetryHandler(logger_level=logging.INFO))
@@ -78,15 +85,15 @@
         """Logs the start of a function call when the logging level >= USAGE.
 
         invocation_id is to uniquely identify different function calls.
         """
         if TelemetryLevel.USAGE >= self._report_levels_higher_or_equal_to:
             for handler in self._handlers:
                 handler.log(
-                    session_id=self._session_id,
+                    client_id=self._client_id,
                     function_start_event=FunctionStartEvent.create(
                         event_time=datetime.datetime.now(),
                         level_name=TelemetryLevel.USAGE.name,
                         invocation_id=invocation_id,
                         module_name=module_name,
                         function_name=function_name,
                     ),
@@ -97,15 +104,15 @@
     ) -> None:
         """Similar to log_function_end, except adding the duration of the call and exception trace on error."""
         if TelemetryLevel.USAGE >= self._report_levels_higher_or_equal_to or (
             exception_trace and TelemetryLevel.EXCEPTION >= self._report_levels_higher_or_equal_to
         ):
             for handler in self._handlers:
                 handler.log(
-                    session_id=self._session_id,
+                    client_id=self._client_id,
                     function_end_event=FunctionEndEvent.create(
                         event_time=datetime.datetime.now(),
                         level_name=TelemetryLevel.USAGE.name if not exception_trace else TelemetryLevel.EXCEPTION.name,
                         invocation_id=invocation_id,
                         module_name=module_name,
                         function_name=function_name,
                         runtime=runtime,
```

### Comparing `metricflow-0.92.1/metricflow/test/cli/test_cli.py` & `metricflow-0.93.0/metricflow/test/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/compare_df.py` & `metricflow-0.93.0/metricflow/test/compare_df.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/conftest.py` & `metricflow-0.93.0/metricflow/test/conftest.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/constraints/test_where.py` & `metricflow-0.93.0/metricflow/test/constraints/test_where.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/dataflow/builder/test_costing.py` & `metricflow-0.93.0/metricflow/test/dataflow/builder/test_costing.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/dataflow/builder/test_dataflow_plan_builder.py` & `metricflow-0.93.0/metricflow/test/dataflow/builder/test_dataflow_plan_builder.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/dataflow/builder/test_node_data_set.py` & `metricflow-0.93.0/metricflow/test/dataflow/builder/test_node_data_set.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/dataflow/builder/test_node_evaluator.py` & `metricflow-0.93.0/metricflow/test/dataflow/builder/test_node_evaluator.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/dataflow/test_sql_table.py` & `metricflow-0.93.0/metricflow/test/dataflow/test_sql_table.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/dataflow_plan_to_svg.py` & `metricflow-0.93.0/metricflow/test/dataflow_plan_to_svg.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/dataset/test_convert_data_source.py` & `metricflow-0.93.0/metricflow/test/dataset/test_convert_data_source.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/execution/noop_task.py` & `metricflow-0.93.0/metricflow/test/execution/noop_task.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/execution/test_sequential_executor.py` & `metricflow-0.93.0/metricflow/test/execution/test_sequential_executor.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/execution/test_tasks.py` & `metricflow-0.93.0/metricflow/test/execution/test_tasks.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/cli_fixtures.py` & `metricflow-0.93.0/metricflow/test/fixtures/cli_fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pandas as pd
 import pytest
 
 from click.testing import CliRunner, Result
 from typing import List, Optional, Sequence
 
 from metricflow.cli.cli_context import CLIContext
-from metricflow.cli.models import Dimension, Materialization, Metric
+from metricflow.engine.models import Dimension, Materialization, Metric
 from metricflow.dataflow.sql_table import SqlTable
 from metricflow.engine.metricflow_engine import MetricFlowQueryRequest, MetricFlowQueryResult
 
 
 class MockMetricFlowEngine:
     """Mock MetricFlowEngine class as only integration is needed to be tested."""
```

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/dataflow_fixtures.py` & `metricflow-0.93.0/metricflow/test/fixtures/dataflow_fixtures.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/id_fixtures.py` & `metricflow-0.93.0/metricflow/test/fixtures/id_fixtures.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_fixtures.py` & `metricflow-0.93.0/metricflow/test/fixtures/model_fixtures.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_yamls/composite_identifier_model/messages_source.yaml` & `metricflow-0.93.0/metricflow/test/fixtures/model_yamls/composite_identifier_model/messages_source.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_yamls/composite_identifier_model/users_source.yaml` & `metricflow-0.93.0/metricflow/test/fixtures/model_yamls/composite_identifier_model/users_source.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_yamls/extended_date_model/data_sources/bookings_from_sql_query_source.yaml` & `metricflow-0.93.0/metricflow/test/fixtures/model_yamls/extended_date_model/data_sources/bookings_from_sql_query_source.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_yamls/extended_date_model/data_sources/extended_bookings_source.yaml` & `metricflow-0.93.0/metricflow/test/fixtures/model_yamls/extended_date_model/data_sources/extended_bookings_source.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_yamls/multi_hop_join_model/partitioned_data_sources/account_month_txns.yaml` & `metricflow-0.93.0/metricflow/test/fixtures/model_yamls/multi_hop_join_model/partitioned_data_sources/account_month_txns.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_yamls/non_ds_model/bookings_source.yaml` & `metricflow-0.93.0/metricflow/test/fixtures/model_yamls/non_ds_model/bookings_source.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_yamls/non_ds_model/listings_latest.yaml` & `metricflow-0.93.0/metricflow/test/fixtures/model_yamls/non_ds_model/listings_latest.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/data_sources/bookings_source.yaml` & `metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/data_sources/bookings_source.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/data_sources/id_verifications.yaml` & `metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/data_sources/id_verifications.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/data_sources/listings_latest.yaml` & `metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/data_sources/listings_latest.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/data_sources/user_ds_source.yaml` & `metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/data_sources/user_ds_source.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/data_sources/views_source.yaml` & `metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/data_sources/views_source.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/materializations.yaml` & `metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/materializations.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/model_yamls/simple_model/metrics.yaml` & `metricflow-0.93.0/metricflow/test/fixtures/model_yamls/simple_model/metrics.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/setup_fixtures.py` & `metricflow-0.93.0/metricflow/test/fixtures/setup_fixtures.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/sql_client_fixtures.py` & `metricflow-0.93.0/metricflow/test/fixtures/sql_client_fixtures.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/fixtures/table_fixtures.py` & `metricflow-0.93.0/metricflow/test/fixtures/table_fixtures.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/configured_test_case.py` & `metricflow-0.93.0/metricflow/test/integration/configured_test_case.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/conftest.py` & `metricflow-0.93.0/metricflow/test/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_cases/itest_composite_identifier.yaml` & `metricflow-0.93.0/metricflow/test/integration/test_cases/itest_composite_identifier.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_cases/itest_constraints.yaml` & `metricflow-0.93.0/metricflow/test/integration/test_cases/itest_constraints.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_cases/itest_cumulative_metric.yaml` & `metricflow-0.93.0/metricflow/test/integration/test_cases/itest_cumulative_metric.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_cases/itest_dimensions.yaml` & `metricflow-0.93.0/metricflow/test/integration/test_cases/itest_dimensions.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_cases/itest_dundered_identifiers.yaml` & `metricflow-0.93.0/metricflow/test/integration/test_cases/itest_dundered_identifiers.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_cases/itest_granularity.yaml` & `metricflow-0.93.0/metricflow/test/integration/test_cases/itest_granularity.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_cases/itest_joins.yaml` & `metricflow-0.93.0/metricflow/test/integration/test_cases/itest_joins.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_cases/itest_measure_aggregations.yaml` & `metricflow-0.93.0/metricflow/test/integration/test_cases/itest_measure_aggregations.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_cases/itest_metrics.yaml` & `metricflow-0.93.0/metricflow/test/integration/test_cases/itest_metrics.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_cases/itest_multi_hop_join.yaml` & `metricflow-0.93.0/metricflow/test/integration/test_cases/itest_multi_hop_join.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_cases/itest_order_limit.yaml` & `metricflow-0.93.0/metricflow/test/integration/test_cases/itest_order_limit.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_cases/itest_partitions.yaml` & `metricflow-0.93.0/metricflow/test/integration/test_cases/itest_partitions.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_cases/itest_simple.yaml` & `metricflow-0.93.0/metricflow/test/integration/test_cases/itest_simple.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_cases/itest_simple_non_ds.yaml` & `metricflow-0.93.0/metricflow/test/integration/test_cases/itest_simple_non_ds.yaml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_configured_cases.py` & `metricflow-0.93.0/metricflow/test/integration/test_configured_cases.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_rendered_query.py` & `metricflow-0.93.0/metricflow/test/integration/test_rendered_query.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/integration/test_write_to_table.py` & `metricflow-0.93.0/metricflow/test/integration/test_write_to_table.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/model/semantics/test_linkable_spec_resolver.py` & `metricflow-0.93.0/metricflow/test/model/semantics/test_linkable_spec_resolver.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/model/test_data_source_container.py` & `metricflow-0.93.0/metricflow/test/model/test_data_source_container.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/model/validations/test_common_identifiers.py` & `metricflow-0.93.0/metricflow/test/model/validations/test_common_identifiers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import copy
+import pytest
 import re
 from typing import Callable
 
 from metricflow.model.model_validator import ModelValidator
 from metricflow.model.objects.data_source import DataSource
 from metricflow.model.objects.user_configured_model import UserConfiguredModel
 from metricflow.specs import IdentifierSpec
 from metricflow.test.test_utils import find_data_source_with
 
 
+@pytest.mark.skip("TODO: re-enforce after validations improvements")
 def test_lonely_identifier_raises_issue(simple_model__pre_transforms: UserConfiguredModel) -> None:  # noqa: D
     model = copy.deepcopy(simple_model__pre_transforms)
     lonely_identifier_name = "hi_im_lonely"
 
     func: Callable[[DataSource], bool] = lambda data_source: len(data_source.identifiers) > 0
     data_source_with_identifiers, _ = find_data_source_with(model, func)
     data_source_with_identifiers.identifiers[0].name = IdentifierSpec.parse(lonely_identifier_name)
```

### Comparing `metricflow-0.92.1/metricflow/test/model/validations/test_data_sources.py` & `metricflow-0.93.0/metricflow/test/model/validations/test_data_sources.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/model/validations/test_dim_names.py` & `metricflow-0.93.0/metricflow/test/model/validations/test_dim_names.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/model/validations/test_dimension_const.py` & `metricflow-0.93.0/metricflow/test/model/validations/test_dimension_const.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/model/validations/test_element_const.py` & `metricflow-0.93.0/metricflow/test/model/validations/test_element_const.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/model/validations/test_identifiers.py` & `metricflow-0.93.0/metricflow/test/model/validations/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/model/validations/test_measures.py` & `metricflow-0.93.0/metricflow/test/model/validations/test_measures.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/model/validations/test_metrics.py` & `metricflow-0.93.0/metricflow/test/model/validations/test_metrics.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/model/validations/test_unique_valid_name.py` & `metricflow-0.93.0/metricflow/test/model/validations/test_unique_valid_name.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/plan_conversion/instance_converters/test_create_select_columns_with_measures_aggregated.py` & `metricflow-0.93.0/metricflow/test/plan_conversion/instance_converters/test_create_select_columns_with_measures_aggregated.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/plan_conversion/test_dataflow_to_execution.py` & `metricflow-0.93.0/metricflow/test/plan_conversion/test_dataflow_to_execution.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/plan_conversion/test_dataflow_to_sql_plan.py` & `metricflow-0.93.0/metricflow/test/plan_conversion/test_dataflow_to_sql_plan.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/plan_conversion/test_time_spine.py` & `metricflow-0.93.0/metricflow/test/plan_conversion/test_time_spine.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/plan_utils.py` & `metricflow-0.93.0/metricflow/test/plan_utils.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/query/test_query_parser.py` & `metricflow-0.93.0/metricflow/test/query/test_query_parser.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/query/test_query_parser_suggestions.py` & `metricflow-0.93.0/metricflow/test/query/test_query_parser_suggestions.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_dont_prune_if_in_where__before_pruning.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_dont_prune_if_in_where__before_pruning.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_no_pruning__after_pruning.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_no_pruning__after_pruning.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_no_pruning__before_pruning.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_no_pruning__before_pruning.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_from_source__after_pruning.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_from_source__after_pruning.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_from_source__before_pruning.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_from_source__before_pruning.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_joined_source__after_pruning.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_joined_source__after_pruning.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_joined_source__before_pruning.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_column_pruner.py/SqlQueryPlan/test_prune_joined_source__before_pruning.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/BigQuerySqlClient/test_convert_query_data_source__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/BigQuerySqlClient/test_convert_query_data_source__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/BigQuerySqlClient/test_convert_table_data_source_with_measures__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/BigQuerySqlClient/test_convert_table_data_source_with_measures__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/BigQuerySqlClient/test_convert_table_data_source_without_measures__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/BigQuerySqlClient/test_convert_table_data_source_without_measures__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/RedshiftSqlClient/test_convert_query_data_source__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/RedshiftSqlClient/test_convert_query_data_source__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/RedshiftSqlClient/test_convert_table_data_source_with_measures__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/RedshiftSqlClient/test_convert_table_data_source_with_measures__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/RedshiftSqlClient/test_convert_table_data_source_without_measures__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/RedshiftSqlClient/test_convert_table_data_source_without_measures__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SnowflakeSqlClient/test_convert_query_data_source__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SnowflakeSqlClient/test_convert_query_data_source__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SnowflakeSqlClient/test_convert_table_data_source_with_measures__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SnowflakeSqlClient/test_convert_table_data_source_with_measures__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SnowflakeSqlClient/test_convert_table_data_source_without_measures__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SnowflakeSqlClient/test_convert_table_data_source_without_measures__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SqliteSqlClient/test_convert_table_data_source_with_measures__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SqliteSqlClient/test_convert_table_data_source_with_measures__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SqliteSqlClient/test_convert_table_data_source_without_measures__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_convert_data_source.py/SqlQueryPlan/SqliteSqlClient/test_convert_table_data_source_without_measures__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_cumulative_metric__dfp_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_cumulative_metric__dfp_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_distinct_values_plan__dfp_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_distinct_values_plan__dfp_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_expr_metrics_plan__dfp_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_expr_metrics_plan__dfp_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_joined_plan__dfp_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_joined_plan__dfp_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_limit_rows_plan__dfp_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_limit_rows_plan__dfp_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_multi_data_source_ratio_metrics_plan__dfp_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_multi_data_source_ratio_metrics_plan__dfp_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_multihop_join_plan__dfp_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_multihop_join_plan__dfp_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_multiple_metrics_plan__dfp_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_multiple_metrics_plan__dfp_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_order_by_plan__dfp_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_order_by_plan__dfp_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_simple_plan__dfp_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_simple_plan__dfp_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_single_data_source_ratio_metrics_plan__dfp_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_single_data_source_ratio_metrics_plan__dfp_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_where_constrained_plan__dfp_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_where_constrained_plan__dfp_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_where_constrained_plan_time_dimension__dfp_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_where_constrained_plan_time_dimension__dfp_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_where_constrained_with_common_linkable_plan__dfp_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_plan_builder.py/DataflowPlan/test_where_constrained_with_common_linkable_plan__dfp_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_combined_metrics_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_combined_metrics_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_joined_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_joined_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_multihop_joined_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_multihop_joined_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_small_combined_metrics_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/BigQuerySqlClient/test_small_combined_metrics_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_combined_metrics_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_combined_metrics_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_joined_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_joined_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_multihop_joined_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_multihop_joined_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_small_combined_metrics_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/RedshiftSqlClient/test_small_combined_metrics_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_combined_metrics_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_combined_metrics_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_joined_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_joined_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_multihop_joined_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_multihop_joined_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_small_combined_metrics_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SnowflakeSqlClient/test_small_combined_metrics_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_combined_metrics_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_combined_metrics_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_joined_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_joined_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_multihop_joined_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_multihop_joined_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_small_combined_metrics_plan__ep_0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_execution.py/ExecutionPlan/SqliteSqlClient/test_small_combined_metrics_plan__ep_0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/DataflowPlan/test_compute_metrics_node_simple_expr__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/DataflowPlan/test_compute_metrics_node_simple_expr__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_join__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_join__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_join__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_join__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_order_by__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_order_by__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_simple_expr__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_simple_expr__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_constrain_primary_time_dimension__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_constrain_primary_time_dimension__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_grain_to_date__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_grain_to_date__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_ds__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_ds__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_with_time_constraint__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_with_time_constraint__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_distinct_values__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_distinct_values__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_distinct_values__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_distinct_values__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_with_where_constraint_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_with_where_constraint_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_limit_rows__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_limit_rows__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_local_dimension_using_local_identifier__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_local_dimension_using_local_identifier__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_measure_aggregation_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_measure_aggregation_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multi_join_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multi_join_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multi_join_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multi_join_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multihop_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multihop_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multihop_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_multihop_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_order_by_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_order_by_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_order_by_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_order_by_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_partitioned_join__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_partitioned_join__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_partitioned_join__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_partitioned_join__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_single_join_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_single_join_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_single_join_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_single_join_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_source_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_source_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_source_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/BigQuerySqlClient/test_source_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_join__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_join__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_join__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_join__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_order_by__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_order_by__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_simple_expr__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_simple_expr__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_constrain_primary_time_dimension__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_constrain_primary_time_dimension__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_grain_to_date__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_grain_to_date__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_ds__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_ds__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_with_time_constraint__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_with_time_constraint__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_distinct_values__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_distinct_values__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_distinct_values__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_distinct_values__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_with_where_constraint_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_with_where_constraint_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_limit_rows__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_limit_rows__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_local_dimension_using_local_identifier__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_local_dimension_using_local_identifier__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_measure_aggregation_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_measure_aggregation_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multi_join_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multi_join_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multi_join_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multi_join_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multihop_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multihop_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multihop_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_multihop_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_order_by_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_order_by_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_order_by_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_order_by_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_partitioned_join__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_partitioned_join__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_partitioned_join__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_partitioned_join__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_single_join_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_single_join_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_single_join_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_single_join_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_source_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_source_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_source_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/RedshiftSqlClient/test_source_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_join__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_join__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_join__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_join__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_order_by__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_order_by__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_simple_expr__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_simple_expr__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_constrain_primary_time_dimension__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_constrain_primary_time_dimension__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_grain_to_date__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_grain_to_date__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_ds__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_ds__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_with_time_constraint__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_with_time_constraint__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_distinct_values__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_distinct_values__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_distinct_values__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_distinct_values__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_with_where_constraint_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_with_where_constraint_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_limit_rows__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_limit_rows__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_local_dimension_using_local_identifier__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_local_dimension_using_local_identifier__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_measure_aggregation_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_measure_aggregation_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multi_join_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multi_join_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multi_join_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multi_join_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multihop_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multihop_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multihop_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_multihop_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_order_by_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_order_by_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_order_by_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_order_by_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_partitioned_join__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_partitioned_join__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_partitioned_join__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_partitioned_join__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_single_join_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_single_join_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_single_join_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_single_join_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_source_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_source_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_source_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SnowflakeSqlClient/test_source_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_join__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_join__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_join__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_join__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_order_by__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_order_by__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_composite_identifier_with_order_by__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_ratio_from_single_data_source__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_simple_expr__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_simple_expr__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_compute_metrics_node_simple_expr__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_constrain_primary_time_dimension__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_constrain_primary_time_dimension__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_grain_to_date__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_grain_to_date__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_grain_to_date__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_ds__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_ds__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_no_window_with_time_constraint__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_with_time_constraint__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_with_time_constraint__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_cumulative_metric_with_time_constraint__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_distinct_values__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_distinct_values__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_distinct_values__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_distinct_values__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_with_where_constraint_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_with_where_constraint_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_with_where_constraint_on_join_dim__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_filter_with_where_constraint_on_join_dim__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_limit_rows__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_limit_rows__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_local_dimension_using_local_identifier__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_local_dimension_using_local_identifier__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_measure_aggregation_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_measure_aggregation_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multi_join_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multi_join_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multi_join_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multi_join_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multihop_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multihop_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multihop_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_multihop_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_order_by_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_order_by_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_order_by_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_order_by_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_partitioned_join__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_partitioned_join__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_partitioned_join__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_partitioned_join__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_single_join_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_single_join_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_single_join_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_single_join_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_source_node__plan0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_source_node__plan0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_source_node__plan0_optimized.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/SqliteSqlClient/test_source_node__plan0_optimized.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_composite_identifier__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_composite_identifier__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_composite_identifier_with_join__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_composite_identifier_with_join__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_composite_identifier_with_order_by__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_composite_identifier_with_order_by__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node_ratio_from_multiple_data_sources__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node_ratio_from_single_data_source__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node_ratio_from_single_data_source__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node_simple_expr__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_compute_metrics_node_simple_expr__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_constrain_primary_time_dimension__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_constrain_primary_time_dimension__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_grain_to_date__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_grain_to_date__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_no_ds__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_no_ds__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_no_window__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_no_window__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_no_window_with_time_constraint__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_no_window_with_time_constraint__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_with_time_constraint__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_cumulative_metric_with_time_constraint__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_distinct_values__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_distinct_values__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_filter_node__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_filter_node__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_filter_with_where_constraint_node__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_filter_with_where_constraint_node__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_filter_with_where_constraint_on_join_dim__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_filter_with_where_constraint_on_join_dim__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_limit_rows__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_limit_rows__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_local_dimension_using_local_identifier__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_local_dimension_using_local_identifier__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_measure_aggregation_node__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_measure_aggregation_node__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_multi_join_node__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_multi_join_node__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_multihop_node__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_multihop_node__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_order_by_node__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_order_by_node__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_partitioned_join__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_partitioned_join__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_single_join_node__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_single_join_node__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_source_node__plan0.xml` & `metricflow-0.93.0/metricflow/test/snapshots/test_dataflow_to_sql_plan.py/SqlQueryPlan/test_source_node__plan0.xml`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/BigQuerySqlClient/test_render_query__query0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/BigQuerySqlClient/test_render_query__query0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/BigQuerySqlClient/test_render_write_to_table_query__query0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/BigQuerySqlClient/test_render_write_to_table_query__query0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/RedshiftSqlClient/test_render_query__query0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/RedshiftSqlClient/test_render_query__query0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/RedshiftSqlClient/test_render_write_to_table_query__query0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/RedshiftSqlClient/test_render_write_to_table_query__query0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SnowflakeSqlClient/test_render_query__query0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SnowflakeSqlClient/test_render_query__query0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SnowflakeSqlClient/test_render_write_to_table_query__query0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SnowflakeSqlClient/test_render_write_to_table_query__query0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SqliteSqlClient/test_render_query__query0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SqliteSqlClient/test_render_query__query0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SqliteSqlClient/test_render_write_to_table_query__query0.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_rendered_query.py/MetricFlowExplainResult/SqliteSqlClient/test_render_write_to_table_query__query0.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_colliding_alias__after_reducing.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_colliding_alias__after_reducing.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_colliding_alias__before_reducing.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_colliding_alias__before_reducing.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_all_join_sources__after_reducing.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_all_join_sources__after_reducing.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_all_join_sources__before_reducing.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_all_join_sources__before_reducing.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_join__before_reducing.sql` & `metricflow-0.93.0/metricflow/test/snapshots/test_rewriting_sub_query_reducer.py/SqlQueryPlan/test_reduce_join__before_reducing.sql`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/sql/compare_sql_plan.py` & `metricflow-0.93.0/metricflow/test/sql/compare_sql_plan.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/sql/optimizer/test_column_pruner.py` & `metricflow-0.93.0/metricflow/test/sql/optimizer/test_column_pruner.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/sql/optimizer/test_rewriting_sub_query_reducer.py` & `metricflow-0.93.0/metricflow/test/sql/optimizer/test_rewriting_sub_query_reducer.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/sql/optimizer/test_sub_query_reducer.py` & `metricflow-0.93.0/metricflow/test/sql/optimizer/test_sub_query_reducer.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/sql/optimizer/test_table_alias_simplifier.py` & `metricflow-0.93.0/metricflow/test/sql/optimizer/test_table_alias_simplifier.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/sql/test_engine_specific_rendering.py` & `metricflow-0.93.0/metricflow/test/sql/test_engine_specific_rendering.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/sql/test_sql_expr_render.py` & `metricflow-0.93.0/metricflow/test/sql/test_sql_expr_render.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/sql/test_sql_plan_render.py` & `metricflow-0.93.0/metricflow/test/sql/test_sql_plan_render.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/sql_clients/test_sql_client.py` & `metricflow-0.93.0/metricflow/test/sql_clients/test_sql_client.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/telemetry/test_telemetry.py` & `metricflow-0.93.0/metricflow/test/telemetry/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/test_object_utils.py` & `metricflow-0.93.0/metricflow/test/test_object_utils.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/test_specs.py` & `metricflow-0.93.0/metricflow/test/test_specs.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/test_utils.py` & `metricflow-0.93.0/metricflow/test/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import copy
 import datetime
 import logging
 
 import dateutil.parser
 from _pytest.fixtures import FixtureRequest
-from typing import Callable, Tuple
+from typing import Callable, Tuple, List
 
 from metricflow.model.objects.data_source import DataSource
+from metricflow.model.objects.materialization import Materialization
 from metricflow.model.objects.metric import Metric
 from metricflow.model.objects.user_configured_model import UserConfiguredModel
 from metricflow.protocols.sql_client import SqlClient
 
 logger = logging.getLogger(__name__)
 
 
@@ -59,7 +61,16 @@
     unless none of the metrics will work.
     """
     for index, metric in enumerate(model.metrics):
         if function(metric):
             return metric, index
 
     raise Exception("Unable to find a metric matching function criteria")
+
+
+def model_with_materialization(
+    initial_model: UserConfiguredModel, materializations: List[Materialization]
+) -> UserConfiguredModel:
+    """Returns a copy of the model but with the materialization added"""
+    model_copy = copy.deepcopy(initial_model)
+    model_copy.materializations.extend(materializations)
+    return model_copy
```

### Comparing `metricflow-0.92.1/metricflow/test/time/configurable_time_source.py` & `metricflow-0.93.0/metricflow/test/time/configurable_time_source.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/test/time/test_time_granularity_solver.py` & `metricflow-0.93.0/metricflow/test/time/test_time_granularity_solver.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/time/time_granularity.py` & `metricflow-0.93.0/metricflow/time/time_granularity.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/time/time_granularity_solver.py` & `metricflow-0.93.0/metricflow/time/time_granularity_solver.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/metricflow/visitor.py` & `metricflow-0.93.0/metricflow/visitor.py`

 * *Files identical despite different names*

### Comparing `metricflow-0.92.1/pyproject.toml` & `metricflow-0.93.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metricflow"
-version = "0.92.1"
+version = "0.93.0"
 description = ""
 authors = ["Transform <hello@transformdata.io>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.10"
 
 croniter = "^1.3.4"
```

### Comparing `metricflow-0.92.1/setup.py` & `metricflow-0.93.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['metricflow',
+ 'metricflow.api',
  'metricflow.cli',
  'metricflow.configuration',
  'metricflow.constraints',
  'metricflow.dag',
  'metricflow.dataflow',
  'metricflow.dataflow.builder',
  'metricflow.dataset',
@@ -28,14 +29,15 @@
  'metricflow.sql',
  'metricflow.sql.optimizer',
  'metricflow.sql.render',
  'metricflow.sql_clients',
  'metricflow.telemetry',
  'metricflow.telemetry.handlers',
  'metricflow.test',
+ 'metricflow.test.api',
  'metricflow.test.cli',
  'metricflow.test.constraints',
  'metricflow.test.dataflow',
  'metricflow.test.dataflow.builder',
  'metricflow.test.dataset',
  'metricflow.test.execution',
  'metricflow.test.fixtures',
@@ -130,15 +132,15 @@
  'update-checker>=0.18.0,<0.19.0']
 
 entry_points = \
 {'console_scripts': ['mf = metricflow.cli.main:cli']}
 
 setup_kwargs = {
     'name': 'metricflow',
-    'version': '0.92.1',
+    'version': '0.93.0',
     'description': '',
     'long_description': None,
     'author': 'Transform',
     'author_email': 'hello@transformdata.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `metricflow-0.92.1/PKG-INFO` & `metricflow-0.93.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metricflow
-Version: 0.92.1
+Version: 0.93.0
 Summary: 
 Author: Transform
 Author-email: hello@transformdata.io
 Requires-Python: >=3.8,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

