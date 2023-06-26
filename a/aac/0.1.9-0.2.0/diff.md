# Comparing `tmp/aac-0.1.9-py3-none-any.whl.zip` & `tmp/aac-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,204 +1,219 @@
-Zip file size: 186774 bytes, number of entries: 202
--rw-r--r--  2.0 unx      695 b- defN 23-Feb-01 23:15 aac/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Feb-01 23:15 aac/__main__.py
--rw-r--r--  2.0 unx      972 b- defN 23-Feb-01 23:15 aac/package_resources.py
--rw-r--r--  2.0 unx       57 b- defN 23-Feb-01 23:15 aac/cli/__init__.py
--rw-r--r--  2.0 unx     2096 b- defN 23-Feb-01 23:15 aac/cli/aac_command.py
--rw-r--r--  2.0 unx     2584 b- defN 23-Feb-01 23:15 aac/cli/execute.py
--rw-r--r--  2.0 unx       54 b- defN 23-Feb-01 23:15 aac/cli/builtin_commands/__init__.py
--rw-r--r--  2.0 unx     1207 b- defN 23-Feb-01 23:15 aac/cli/builtin_commands/validate/__init__.py
--rw-r--r--  2.0 unx     1476 b- defN 23-Feb-01 23:15 aac/cli/builtin_commands/validate/validate.yaml
--rw-r--r--  2.0 unx     2710 b- defN 23-Feb-01 23:15 aac/cli/builtin_commands/validate/validate_impl.py
--rw-r--r--  2.0 unx      795 b- defN 23-Feb-01 23:15 aac/cli/builtin_commands/version/__init__.py
--rw-r--r--  2.0 unx      431 b- defN 23-Feb-01 23:15 aac/cli/builtin_commands/version/version.yaml
--rw-r--r--  2.0 unx      428 b- defN 23-Feb-01 23:15 aac/cli/builtin_commands/version/version_impl.py
--rw-r--r--  2.0 unx       66 b- defN 23-Feb-01 23:15 aac/io/__init__.py
--rw-r--r--  2.0 unx      253 b- defN 23-Feb-01 23:15 aac/io/constants.py
--rw-r--r--  2.0 unx     2507 b- defN 23-Feb-01 23:15 aac/io/paths.py
--rw-r--r--  2.0 unx     2275 b- defN 23-Feb-01 23:15 aac/io/writer.py
--rw-r--r--  2.0 unx       63 b- defN 23-Feb-01 23:15 aac/io/files/__init__.py
--rw-r--r--  2.0 unx      913 b- defN 23-Feb-01 23:15 aac/io/files/aac_file.py
--rw-r--r--  2.0 unx     1626 b- defN 23-Feb-01 23:15 aac/io/files/find.py
--rw-r--r--  2.0 unx      210 b- defN 23-Feb-01 23:15 aac/io/parser/__init__.py
--rw-r--r--  2.0 unx    10005 b- defN 23-Feb-01 23:15 aac/io/parser/_parse_source.py
--rw-r--r--  2.0 unx      416 b- defN 23-Feb-01 23:15 aac/io/parser/_parser_error.py
--rw-r--r--  2.0 unx       52 b- defN 23-Feb-01 23:15 aac/lang/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 23-Feb-01 23:15 aac/lang/active_context_lifecycle_manager.py
--rw-r--r--  2.0 unx     1415 b- defN 23-Feb-01 23:15 aac/lang/constants.py
--rw-r--r--  2.0 unx     3000 b- defN 23-Feb-01 23:15 aac/lang/hierarchy.py
--rw-r--r--  2.0 unx    29109 b- defN 23-Feb-01 23:15 aac/lang/language_context.py
--rw-r--r--  2.0 unx      230 b- defN 23-Feb-01 23:15 aac/lang/language_error.py
--rw-r--r--  2.0 unx       85 b- defN 23-Feb-01 23:15 aac/lang/definitions/__init__.py
--rw-r--r--  2.0 unx     3777 b- defN 23-Feb-01 23:15 aac/lang/definitions/collections.py
--rw-r--r--  2.0 unx     7729 b- defN 23-Feb-01 23:15 aac/lang/definitions/definition.py
--rw-r--r--  2.0 unx     9139 b- defN 23-Feb-01 23:15 aac/lang/definitions/extensions.py
--rw-r--r--  2.0 unx     3136 b- defN 23-Feb-01 23:15 aac/lang/definitions/inheritance.py
--rw-r--r--  2.0 unx     7104 b- defN 23-Feb-01 23:15 aac/lang/definitions/json_schema.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Feb-01 23:15 aac/lang/definitions/lexeme.py
--rw-r--r--  2.0 unx    10713 b- defN 23-Feb-01 23:15 aac/lang/definitions/references.py
--rw-r--r--  2.0 unx     4479 b- defN 23-Feb-01 23:15 aac/lang/definitions/schema.py
--rw-r--r--  2.0 unx     5149 b- defN 23-Feb-01 23:15 aac/lang/definitions/search.py
--rw-r--r--  2.0 unx     1193 b- defN 23-Feb-01 23:15 aac/lang/definitions/source_location.py
--rw-r--r--  2.0 unx     5891 b- defN 23-Feb-01 23:15 aac/lang/definitions/structure.py
--rw-r--r--  2.0 unx      401 b- defN 23-Feb-01 23:15 aac/lang/definitions/type.py
--rw-r--r--  2.0 unx      198 b- defN 23-Feb-01 23:15 aac/persistence/__init__.py
--rw-r--r--  2.0 unx      154 b- defN 23-Feb-01 23:15 aac/persistence/state_file_error.py
--rw-r--r--  2.0 unx      695 b- defN 23-Feb-01 23:15 aac/plugins/__init__.py
--rw-r--r--  2.0 unx      511 b- defN 23-Feb-01 23:15 aac/plugins/_common.py
--rw-r--r--  2.0 unx      323 b- defN 23-Feb-01 23:15 aac/plugins/hookspecs.py
--rw-r--r--  2.0 unx     4437 b- defN 23-Feb-01 23:15 aac/plugins/plugin.py
--rw-r--r--  2.0 unx     5296 b- defN 23-Feb-01 23:15 aac/plugins/plugin_execution.py
--rw-r--r--  2.0 unx     2459 b- defN 23-Feb-01 23:15 aac/plugins/plugin_manager.py
--rw-r--r--  2.0 unx       68 b- defN 23-Feb-01 23:15 aac/plugins/contributions/__init__.py
--rw-r--r--  2.0 unx     9885 b- defN 23-Feb-01 23:15 aac/plugins/contributions/contribution_points.py
--rw-r--r--  2.0 unx     1150 b- defN 23-Feb-01 23:15 aac/plugins/contributions/plugin_contribution.py
--rw-r--r--  2.0 unx      524 b- defN 23-Feb-01 23:15 aac/plugins/contributions/contribution_types/__init__.py
--rw-r--r--  2.0 unx      353 b- defN 23-Feb-01 23:15 aac/plugins/contributions/contribution_types/contribution_type.py
--rw-r--r--  2.0 unx      957 b- defN 23-Feb-01 23:15 aac/plugins/contributions/contribution_types/definition_validation_contribution.py
--rw-r--r--  2.0 unx      859 b- defN 23-Feb-01 23:15 aac/plugins/contributions/contribution_types/primitive_validation_contribution.py
--rw-r--r--  2.0 unx       69 b- defN 23-Feb-01 23:15 aac/plugins/first_party/__init__.py
--rw-r--r--  2.0 unx     1520 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_design_doc/__init__.py
--rw-r--r--  2.0 unx     1312 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_design_doc/gen_design_doc.yaml
--rw-r--r--  2.0 unx     4290 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_design_doc/gen_design_doc_impl.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_design_doc/templates/__init__.py
--rw-r--r--  2.0 unx      257 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_design_doc/templates/datum.md.jinja2
--rw-r--r--  2.0 unx      262 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_design_doc/templates/macros.jinja2
--rw-r--r--  2.0 unx      995 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_design_doc/templates/model.md.jinja2
--rw-r--r--  2.0 unx      340 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_design_doc/templates/system-design-doc.md.jinja2
--rw-r--r--  2.0 unx      434 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_design_doc/templates/usecase.md.jinja2
--rw-r--r--  2.0 unx     1769 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_gherkin_behaviors/__init__.py
--rw-r--r--  2.0 unx      639 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_gherkin_behaviors/behavior.feature.jinja2
--rw-r--r--  2.0 unx     1181 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_gherkin_behaviors/gen_gherkin_behaviors.yaml
--rw-r--r--  2.0 unx     6986 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_gherkin_behaviors/gen_gherkin_behaviors_impl.py
--rw-r--r--  2.0 unx     1470 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_json/__init__.py
--rw-r--r--  2.0 unx      950 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_json/gen_json.yaml
--rw-r--r--  2.0 unx     1987 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_json/gen_json_impl.py
--rw-r--r--  2.0 unx     2763 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plant_uml/__init__.py
--rw-r--r--  2.0 unx     4050 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plant_uml/gen_plant_uml.yaml
--rw-r--r--  2.0 unx    12544 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plant_uml/gen_plant_uml_impl.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plant_uml/templates/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plant_uml/templates/component/__init__.py
--rw-r--r--  2.0 unx      960 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plant_uml/templates/component/component_diagram.puml.jinja2
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plant_uml/templates/object/__init__.py
--rw-r--r--  2.0 unx      258 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plant_uml/templates/object/object_diagram.puml.jinja2
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plant_uml/templates/sequence/__init__.py
--rw-r--r--  2.0 unx      300 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plant_uml/templates/sequence/sequence_diagram.puml.jinja2
--rw-r--r--  2.0 unx      204 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/GeneratePluginException.py
--rw-r--r--  2.0 unx     1441 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/__init__.py
--rw-r--r--  2.0 unx     1841 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/gen_plugin.yaml
--rw-r--r--  2.0 unx    15242 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/gen_plugin_impl.py
--rw-r--r--  2.0 unx      170 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/templates/__init__.py
--rw-r--r--  2.0 unx      170 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/templates/first_party/__init__.py
--rw-r--r--  2.0 unx     2750 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/templates/first_party/__init__.py.jinja2
--rw-r--r--  2.0 unx     1827 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/templates/first_party/plugin_impl.py.jinja2
--rw-r--r--  2.0 unx     1017 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/templates/first_party/test_plugin_impl.py.jinja2
--rw-r--r--  2.0 unx      966 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/templates/third_party/README.md.jinja2
--rw-r--r--  2.0 unx      170 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/templates/third_party/__init__.py
--rw-r--r--  2.0 unx     2734 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/templates/third_party/__init__.py.jinja2
--rw-r--r--  2.0 unx     1704 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/templates/third_party/plugin_impl.py.jinja2
--rw-r--r--  2.0 unx      935 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/templates/third_party/setup.py.jinja2
--rw-r--r--  2.0 unx      942 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/templates/third_party/test_plugin_impl.py.jinja2
--rw-r--r--  2.0 unx      761 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_plugin/templates/third_party/tox.ini.jinja2
--rw-r--r--  2.0 unx     1462 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_protobuf/__init__.py
--rw-r--r--  2.0 unx     1679 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_protobuf/gen_protobuf.yaml
--rw-r--r--  2.0 unx    19204 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_protobuf/gen_protobuf_impl.py
--rw-r--r--  2.0 unx     1006 b- defN 23-Feb-01 23:15 aac/plugins/first_party/gen_protobuf/message.proto.jinja2
--rw-r--r--  2.0 unx      811 b- defN 23-Feb-01 23:15 aac/plugins/first_party/help_dump/__init__.py
--rw-r--r--  2.0 unx      956 b- defN 23-Feb-01 23:15 aac/plugins/first_party/help_dump/help-dump.yaml
--rw-r--r--  2.0 unx      957 b- defN 23-Feb-01 23:15 aac/plugins/first_party/help_dump/help_dump_impl.py
--rw-r--r--  2.0 unx     1403 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/__init__.py
--rw-r--r--  2.0 unx     1227 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/conversion_helpers.py
--rw-r--r--  2.0 unx    11826 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/language_server.py
--rw-r--r--  2.0 unx     1414 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/lsp-server.yaml
--rw-r--r--  2.0 unx      593 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/managed_workspace_file.py
--rw-r--r--  2.0 unx     1194 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/start_lsp_server_impl.py
--rw-r--r--  2.0 unx       64 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/providers/__init__.py
--rw-r--r--  2.0 unx     4214 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/providers/code_completion_provider.py
--rw-r--r--  2.0 unx     5804 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/providers/find_references_provider.py
--rw-r--r--  2.0 unx     7384 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/providers/goto_definition_provider.py
--rw-r--r--  2.0 unx     1375 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/providers/hover_provider.py
--rw-r--r--  2.0 unx      580 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/providers/locations.py
--rw-r--r--  2.0 unx      491 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/providers/lsp_provider.py
--rw-r--r--  2.0 unx     1461 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/providers/prepare_rename_provider.py
--rw-r--r--  2.0 unx     2838 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/providers/publish_diagnostics_provider.py
--rw-r--r--  2.0 unx     6411 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/providers/rename_provider.py
--rw-r--r--  2.0 unx     7107 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/providers/semantic_tokens_provider.py
--rw-r--r--  2.0 unx     3381 b- defN 23-Feb-01 23:15 aac/plugins/first_party/lsp_server/providers/symbols.py
--rw-r--r--  2.0 unx      673 b- defN 23-Feb-01 23:15 aac/plugins/first_party/material_model/__init__.py
--rw-r--r--  2.0 unx     4710 b- defN 23-Feb-01 23:15 aac/plugins/first_party/material_model/material_model.yaml
--rw-r--r--  2.0 unx      102 b- defN 23-Feb-01 23:15 aac/plugins/first_party/material_model/material_model_impl.py
--rw-r--r--  2.0 unx     2220 b- defN 23-Feb-01 23:15 aac/plugins/first_party/plugin_management/__init__.py
--rw-r--r--  2.0 unx     5264 b- defN 23-Feb-01 23:15 aac/plugins/first_party/plugin_management/plugin-management.yaml
--rw-r--r--  2.0 unx     4411 b- defN 23-Feb-01 23:15 aac/plugins/first_party/plugin_management/plugin_management_impl.py
--rw-r--r--  2.0 unx      786 b- defN 23-Feb-01 23:15 aac/plugins/first_party/primitive_type_check/__init__.py
--rw-r--r--  2.0 unx     2256 b- defN 23-Feb-01 23:15 aac/plugins/first_party/primitive_type_check/primitive_type_check.yaml
--rw-r--r--  2.0 unx      911 b- defN 23-Feb-01 23:15 aac/plugins/first_party/primitive_type_check/validators/__init__.py
--rw-r--r--  2.0 unx     1819 b- defN 23-Feb-01 23:15 aac/plugins/first_party/primitive_type_check/validators/bool_validator.py
--rw-r--r--  2.0 unx     2226 b- defN 23-Feb-01 23:15 aac/plugins/first_party/primitive_type_check/validators/int_validator.py
--rw-r--r--  2.0 unx     1017 b- defN 23-Feb-01 23:15 aac/plugins/first_party/print_spec/__init__.py
--rw-r--r--  2.0 unx      898 b- defN 23-Feb-01 23:15 aac/plugins/first_party/print_spec/print-spec.yaml
--rw-r--r--  2.0 unx      957 b- defN 23-Feb-01 23:15 aac/plugins/first_party/print_spec/print_spec_impl.py
--rw-r--r--  2.0 unx     1667 b- defN 23-Feb-01 23:15 aac/plugins/first_party/rest_api/__init__.py
--rw-r--r--  2.0 unx     2138 b- defN 23-Feb-01 23:15 aac/plugins/first_party/rest_api/aac_rest_api_impl.py
--rw-r--r--  2.0 unx    13921 b- defN 23-Feb-01 23:15 aac/plugins/first_party/rest_api/aac_rest_app.py
--rw-r--r--  2.0 unx     1947 b- defN 23-Feb-01 23:15 aac/plugins/first_party/rest_api/rest_api.yaml
--rw-r--r--  2.0 unx       52 b- defN 23-Feb-01 23:15 aac/plugins/first_party/rest_api/models/__init__.py
--rw-r--r--  2.0 unx     1563 b- defN 23-Feb-01 23:15 aac/plugins/first_party/rest_api/models/command_model.py
--rw-r--r--  2.0 unx     1347 b- defN 23-Feb-01 23:15 aac/plugins/first_party/rest_api/models/definition_model.py
--rw-r--r--  2.0 unx     1480 b- defN 23-Feb-01 23:15 aac/plugins/first_party/rest_api/models/file_model.py
--rw-r--r--  2.0 unx     2891 b- defN 23-Feb-01 23:15 aac/plugins/first_party/specifications/__init__.py
--rw-r--r--  2.0 unx     3684 b- defN 23-Feb-01 23:15 aac/plugins/first_party/specifications/globally_unique_id.py
--rw-r--r--  2.0 unx     2757 b- defN 23-Feb-01 23:15 aac/plugins/first_party/specifications/referenced_ids_exist.py
--rw-r--r--  2.0 unx     6167 b- defN 23-Feb-01 23:15 aac/plugins/first_party/specifications/specifications.yaml
--rw-r--r--  2.0 unx     3688 b- defN 23-Feb-01 23:15 aac/plugins/first_party/specifications/specifications_impl.py
--rw-r--r--  2.0 unx      663 b- defN 23-Feb-01 23:15 aac/plugins/validators/__init__.py
--rw-r--r--  2.0 unx     2077 b- defN 23-Feb-01 23:15 aac/plugins/validators/_common.py
--rw-r--r--  2.0 unx     2538 b- defN 23-Feb-01 23:15 aac/plugins/validators/_finding_location.py
--rw-r--r--  2.0 unx     1564 b- defN 23-Feb-01 23:15 aac/plugins/validators/_validator_finding.py
--rw-r--r--  2.0 unx     2902 b- defN 23-Feb-01 23:15 aac/plugins/validators/_validator_findings.py
--rw-r--r--  2.0 unx     1749 b- defN 23-Feb-01 23:15 aac/plugins/validators/_validator_result.py
--rw-r--r--  2.0 unx     1060 b- defN 23-Feb-01 23:15 aac/plugins/validators/defined_references/__init__.py
--rw-r--r--  2.0 unx     3262 b- defN 23-Feb-01 23:15 aac/plugins/validators/defined_references/_validate_references.py
--rw-r--r--  2.0 unx     1443 b- defN 23-Feb-01 23:15 aac/plugins/validators/defined_references/defined_references.yaml
--rw-r--r--  2.0 unx     1054 b- defN 23-Feb-01 23:15 aac/plugins/validators/exclusive_fields/__init__.py
--rw-r--r--  2.0 unx     1968 b- defN 23-Feb-01 23:15 aac/plugins/validators/exclusive_fields/_exclusive_fields.py
--rw-r--r--  2.0 unx     2117 b- defN 23-Feb-01 23:15 aac/plugins/validators/exclusive_fields/exclusive_fields.yaml
--rw-r--r--  2.0 unx     1051 b- defN 23-Feb-01 23:15 aac/plugins/validators/reference_fields/__init__.py
--rw-r--r--  2.0 unx     3596 b- defN 23-Feb-01 23:15 aac/plugins/validators/reference_fields/_validate_reference_fields.py
--rw-r--r--  2.0 unx     1450 b- defN 23-Feb-01 23:15 aac/plugins/validators/reference_fields/reference_fields.yaml
--rw-r--r--  2.0 unx     1056 b- defN 23-Feb-01 23:15 aac/plugins/validators/reference_targets/__init__.py
--rw-r--r--  2.0 unx     4423 b- defN 23-Feb-01 23:15 aac/plugins/validators/reference_targets/_validate_reference_targets.py
--rw-r--r--  2.0 unx     1459 b- defN 23-Feb-01 23:15 aac/plugins/validators/reference_targets/reference_targets.yaml
--rw-r--r--  2.0 unx     1638 b- defN 23-Feb-01 23:15 aac/plugins/validators/required_fields/__init__.py
--rw-r--r--  2.0 unx     3327 b- defN 23-Feb-01 23:15 aac/plugins/validators/required_fields/_validate_required_fields.py
--rw-r--r--  2.0 unx     1496 b- defN 23-Feb-01 23:15 aac/plugins/validators/required_fields/required_fields.yaml
--rw-r--r--  2.0 unx     1012 b- defN 23-Feb-01 23:15 aac/plugins/validators/root_keys/__init__.py
--rw-r--r--  2.0 unx     1601 b- defN 23-Feb-01 23:15 aac/plugins/validators/root_keys/_validate_root_keys.py
--rw-r--r--  2.0 unx     2257 b- defN 23-Feb-01 23:15 aac/plugins/validators/root_keys/root_keys.yaml
--rw-r--r--  2.0 unx     1053 b- defN 23-Feb-01 23:15 aac/plugins/validators/subcomponent_type/__init__.py
--rw-r--r--  2.0 unx     2979 b- defN 23-Feb-01 23:15 aac/plugins/validators/subcomponent_type/_subcomponent_type.py
--rw-r--r--  2.0 unx     1493 b- defN 23-Feb-01 23:15 aac/plugins/validators/subcomponent_type/subcomponent_type.yaml
--rw-r--r--  2.0 unx     1006 b- defN 23-Feb-01 23:15 aac/plugins/validators/unique_names/__init__.py
--rw-r--r--  2.0 unx     2311 b- defN 23-Feb-01 23:15 aac/plugins/validators/unique_names/_unique_names.py
--rw-r--r--  2.0 unx     1524 b- defN 23-Feb-01 23:15 aac/plugins/validators/unique_names/unique_names.yaml
--rw-r--r--  2.0 unx     1107 b- defN 23-Feb-01 23:15 aac/plugins/validators/validator_implementation/__init__.py
--rw-r--r--  2.0 unx     2775 b- defN 23-Feb-01 23:15 aac/plugins/validators/validator_implementation/_validator_implementation.py
--rw-r--r--  2.0 unx     1470 b- defN 23-Feb-01 23:15 aac/plugins/validators/validator_implementation/validator_implementation.yaml
--rw-r--r--  2.0 unx      246 b- defN 23-Feb-01 23:15 aac/serialization/__init__.py
--rw-r--r--  2.0 unx     1076 b- defN 23-Feb-01 23:15 aac/serialization/aac_command_encoder.py
--rw-r--r--  2.0 unx      317 b- defN 23-Feb-01 23:15 aac/spec/__init__.py
--rw-r--r--  2.0 unx     3790 b- defN 23-Feb-01 23:15 aac/spec/core.py
--rw-r--r--  2.0 unx    14319 b- defN 23-Feb-01 23:15 aac/spec/spec.yaml
--rw-r--r--  2.0 unx      190 b- defN 23-Feb-01 23:15 aac/templates/__init__.py
--rw-r--r--  2.0 unx     6327 b- defN 23-Feb-01 23:15 aac/templates/engine.py
--rw-r--r--  2.0 unx      379 b- defN 23-Feb-01 23:15 aac/templates/error.py
--rw-r--r--  2.0 unx      532 b- defN 23-Feb-01 23:15 aac/validate/__init__.py
--rw-r--r--  2.0 unx     3995 b- defN 23-Feb-01 23:15 aac/validate/_collect_validators.py
--rw-r--r--  2.0 unx    10478 b- defN 23-Feb-01 23:15 aac/validate/_validate.py
--rw-r--r--  2.0 unx      214 b- defN 23-Feb-01 23:15 aac/validate/_validation_error.py
--rw-r--r--  2.0 unx    15083 b- defN 23-Feb-01 23:16 aac-0.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-01 23:16 aac-0.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 23-Feb-01 23:16 aac-0.1.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Feb-01 23:16 aac-0.1.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    21313 b- defN 23-Feb-01 23:16 aac-0.1.9.dist-info/RECORD
-202 files, 530625 bytes uncompressed, 151516 bytes compressed:  71.4%
+Zip file size: 209598 bytes, number of entries: 217
+-rw-r--r--  2.0 unx      681 b- defN 23-Jun-26 19:39 aac/__init__.py
+-rw-r--r--  2.0 unx      175 b- defN 23-Jun-26 19:39 aac/__main__.py
+-rw-r--r--  2.0 unx      972 b- defN 23-Jun-26 19:39 aac/package_resources.py
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-26 19:39 aac/cli/__init__.py
+-rw-r--r--  2.0 unx     2096 b- defN 23-Jun-26 19:39 aac/cli/aac_command.py
+-rw-r--r--  2.0 unx     2743 b- defN 23-Jun-26 19:39 aac/cli/execute.py
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-26 19:39 aac/cli/builtin_commands/__init__.py
+-rw-r--r--  2.0 unx     1207 b- defN 23-Jun-26 19:39 aac/cli/builtin_commands/validate/__init__.py
+-rw-r--r--  2.0 unx     1470 b- defN 23-Jun-26 19:39 aac/cli/builtin_commands/validate/validate.yaml
+-rw-r--r--  2.0 unx     3110 b- defN 23-Jun-26 19:39 aac/cli/builtin_commands/validate/validate_impl.py
+-rw-r--r--  2.0 unx      795 b- defN 23-Jun-26 19:39 aac/cli/builtin_commands/version/__init__.py
+-rw-r--r--  2.0 unx      435 b- defN 23-Jun-26 19:39 aac/cli/builtin_commands/version/version.yaml
+-rw-r--r--  2.0 unx      428 b- defN 23-Jun-26 19:39 aac/cli/builtin_commands/version/version_impl.py
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-26 19:39 aac/io/__init__.py
+-rw-r--r--  2.0 unx      253 b- defN 23-Jun-26 19:39 aac/io/constants.py
+-rw-r--r--  2.0 unx     2507 b- defN 23-Jun-26 19:39 aac/io/paths.py
+-rw-r--r--  2.0 unx     2275 b- defN 23-Jun-26 19:39 aac/io/writer.py
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-26 19:39 aac/io/files/__init__.py
+-rw-r--r--  2.0 unx      925 b- defN 23-Jun-26 19:39 aac/io/files/aac_file.py
+-rw-r--r--  2.0 unx     1628 b- defN 23-Jun-26 19:39 aac/io/files/find.py
+-rw-r--r--  2.0 unx      427 b- defN 23-Jun-26 19:39 aac/io/parser/__init__.py
+-rw-r--r--  2.0 unx     4849 b- defN 23-Jun-26 19:39 aac/io/parser/_cache.py
+-rw-r--r--  2.0 unx      534 b- defN 23-Jun-26 19:39 aac/io/parser/_cache_manager.py
+-rw-r--r--  2.0 unx     7610 b- defN 23-Jun-26 19:39 aac/io/parser/_parse_source.py
+-rw-r--r--  2.0 unx      415 b- defN 23-Jun-26 19:39 aac/io/parser/_parser_error.py
+-rw-r--r--  2.0 unx     4629 b- defN 23-Jun-26 19:39 aac/io/parser/_yaml.py
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-26 19:39 aac/lang/__init__.py
+-rw-r--r--  2.0 unx     1603 b- defN 23-Jun-26 19:39 aac/lang/active_context_lifecycle_manager.py
+-rw-r--r--  2.0 unx     3210 b- defN 23-Jun-26 19:39 aac/lang/constants.py
+-rw-r--r--  2.0 unx     4139 b- defN 23-Jun-26 19:39 aac/lang/hierarchy.py
+-rw-r--r--  2.0 unx    30160 b- defN 23-Jun-26 19:39 aac/lang/language_context.py
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-26 19:39 aac/lang/language_error.py
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-26 19:39 aac/lang/definitions/__init__.py
+-rw-r--r--  2.0 unx     3777 b- defN 23-Jun-26 19:39 aac/lang/definitions/collections.py
+-rw-r--r--  2.0 unx     9179 b- defN 23-Jun-26 19:39 aac/lang/definitions/definition.py
+-rw-r--r--  2.0 unx    11643 b- defN 23-Jun-26 19:39 aac/lang/definitions/extensions.py
+-rw-r--r--  2.0 unx     3136 b- defN 23-Jun-26 19:39 aac/lang/definitions/inheritance.py
+-rw-r--r--  2.0 unx     7104 b- defN 23-Jun-26 19:39 aac/lang/definitions/json_schema.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jun-26 19:39 aac/lang/definitions/lexeme.py
+-rw-r--r--  2.0 unx     3921 b- defN 23-Jun-26 19:39 aac/lang/definitions/metadata_structure.py
+-rw-r--r--  2.0 unx     9943 b- defN 23-Jun-26 19:39 aac/lang/definitions/references.py
+-rw-r--r--  2.0 unx     7827 b- defN 23-Jun-26 19:39 aac/lang/definitions/schema.py
+-rw-r--r--  2.0 unx     5149 b- defN 23-Jun-26 19:39 aac/lang/definitions/search.py
+-rw-r--r--  2.0 unx     1193 b- defN 23-Jun-26 19:39 aac/lang/definitions/source_location.py
+-rw-r--r--  2.0 unx     3495 b- defN 23-Jun-26 19:39 aac/lang/definitions/structural_node.py
+-rw-r--r--  2.0 unx     5891 b- defN 23-Jun-26 19:39 aac/lang/definitions/structure.py
+-rw-r--r--  2.0 unx      401 b- defN 23-Jun-26 19:39 aac/lang/definitions/type.py
+-rw-r--r--  2.0 unx      198 b- defN 23-Jun-26 19:39 aac/persistence/__init__.py
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-26 19:39 aac/persistence/state_file_error.py
+-rw-r--r--  2.0 unx      695 b- defN 23-Jun-26 19:39 aac/plugins/__init__.py
+-rw-r--r--  2.0 unx      704 b- defN 23-Jun-26 19:39 aac/plugins/_common.py
+-rw-r--r--  2.0 unx      323 b- defN 23-Jun-26 19:39 aac/plugins/hookspecs.py
+-rw-r--r--  2.0 unx     4627 b- defN 23-Jun-26 19:39 aac/plugins/plugin.py
+-rw-r--r--  2.0 unx     5296 b- defN 23-Jun-26 19:39 aac/plugins/plugin_execution.py
+-rw-r--r--  2.0 unx     2864 b- defN 23-Jun-26 19:39 aac/plugins/plugin_manager.py
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-26 19:39 aac/plugins/contributions/__init__.py
+-rw-r--r--  2.0 unx     9885 b- defN 23-Jun-26 19:39 aac/plugins/contributions/contribution_points.py
+-rw-r--r--  2.0 unx     1150 b- defN 23-Jun-26 19:39 aac/plugins/contributions/plugin_contribution.py
+-rw-r--r--  2.0 unx      524 b- defN 23-Jun-26 19:39 aac/plugins/contributions/contribution_types/__init__.py
+-rw-r--r--  2.0 unx      353 b- defN 23-Jun-26 19:39 aac/plugins/contributions/contribution_types/contribution_type.py
+-rw-r--r--  2.0 unx     1118 b- defN 23-Jun-26 19:39 aac/plugins/contributions/contribution_types/definition_validation_contribution.py
+-rw-r--r--  2.0 unx     1022 b- defN 23-Jun-26 19:39 aac/plugins/contributions/contribution_types/primitive_validation_contribution.py
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-26 19:39 aac/plugins/first_party/__init__.py
+-rw-r--r--  2.0 unx     2514 b- defN 23-Jun-26 19:39 aac/plugins/first_party/active_context/__init__.py
+-rw-r--r--  2.0 unx     6501 b- defN 23-Jun-26 19:39 aac/plugins/first_party/active_context/active_context.yaml
+-rw-r--r--  2.0 unx     3947 b- defN 23-Jun-26 19:39 aac/plugins/first_party/active_context/active_context_impl.py
+-rw-r--r--  2.0 unx     1520 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_design_doc/__init__.py
+-rw-r--r--  2.0 unx     1284 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_design_doc/gen_design_doc.yaml
+-rw-r--r--  2.0 unx     4429 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_design_doc/gen_design_doc_impl.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_design_doc/templates/__init__.py
+-rw-r--r--  2.0 unx      254 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_design_doc/templates/datum.md.jinja2
+-rw-r--r--  2.0 unx      260 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_design_doc/templates/macros.jinja2
+-rw-r--r--  2.0 unx      988 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_design_doc/templates/model.md.jinja2
+-rw-r--r--  2.0 unx      334 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_design_doc/templates/system-design-doc.md.jinja2
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_design_doc/templates/usecase.md.jinja2
+-rw-r--r--  2.0 unx     1760 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_gherkin_behaviors/__init__.py
+-rw-r--r--  2.0 unx      639 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_gherkin_behaviors/behavior.feature.jinja2
+-rw-r--r--  2.0 unx     1156 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_gherkin_behaviors/gen_gherkin_behaviors.yaml
+-rw-r--r--  2.0 unx     7000 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_gherkin_behaviors/gen_gherkin_behaviors_impl.py
+-rw-r--r--  2.0 unx     1470 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_json/__init__.py
+-rw-r--r--  2.0 unx      997 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_json/gen_json.yaml
+-rw-r--r--  2.0 unx     2006 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_json/gen_json_impl.py
+-rw-r--r--  2.0 unx     2763 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plant_uml/__init__.py
+-rw-r--r--  2.0 unx     4334 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plant_uml/gen_plant_uml.yaml
+-rw-r--r--  2.0 unx    12572 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plant_uml/gen_plant_uml_impl.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plant_uml/templates/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plant_uml/templates/component/__init__.py
+-rw-r--r--  2.0 unx      960 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plant_uml/templates/component/component_diagram.puml.jinja2
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plant_uml/templates/object/__init__.py
+-rw-r--r--  2.0 unx      255 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plant_uml/templates/object/object_diagram.puml.jinja2
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plant_uml/templates/sequence/__init__.py
+-rw-r--r--  2.0 unx      297 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plant_uml/templates/sequence/sequence_diagram.puml.jinja2
+-rw-r--r--  2.0 unx      204 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/GeneratePluginException.py
+-rw-r--r--  2.0 unx     1442 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/__init__.py
+-rw-r--r--  2.0 unx     1780 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/gen_plugin.yaml
+-rw-r--r--  2.0 unx    17121 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/gen_plugin_impl.py
+-rw-r--r--  2.0 unx      170 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/templates/__init__.py
+-rw-r--r--  2.0 unx      170 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/templates/first_party/__init__.py
+-rw-r--r--  2.0 unx     2700 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/templates/first_party/__init__.py.jinja2
+-rw-r--r--  2.0 unx     1821 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/templates/first_party/plugin_impl.py.jinja2
+-rw-r--r--  2.0 unx     1036 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/templates/first_party/test_plugin_impl.py.jinja2
+-rw-r--r--  2.0 unx      931 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/templates/third_party/README.md.jinja2
+-rw-r--r--  2.0 unx      170 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/templates/third_party/__init__.py
+-rw-r--r--  2.0 unx     2685 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/templates/third_party/__init__.py.jinja2
+-rw-r--r--  2.0 unx     1698 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/templates/third_party/plugin_impl.py.jinja2
+-rw-r--r--  2.0 unx      954 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/templates/third_party/setup.py.jinja2
+-rw-r--r--  2.0 unx      961 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/templates/third_party/test_plugin_impl.py.jinja2
+-rw-r--r--  2.0 unx      761 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_plugin/templates/third_party/tox.ini.jinja2
+-rw-r--r--  2.0 unx     1462 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_protobuf/__init__.py
+-rw-r--r--  2.0 unx     2632 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_protobuf/gen_protobuf.yaml
+-rw-r--r--  2.0 unx    19919 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_protobuf/gen_protobuf_impl.py
+-rw-r--r--  2.0 unx     1006 b- defN 23-Jun-26 19:39 aac/plugins/first_party/gen_protobuf/message.proto.jinja2
+-rw-r--r--  2.0 unx      811 b- defN 23-Jun-26 19:39 aac/plugins/first_party/help_dump/__init__.py
+-rw-r--r--  2.0 unx      906 b- defN 23-Jun-26 19:39 aac/plugins/first_party/help_dump/help-dump.yaml
+-rw-r--r--  2.0 unx      965 b- defN 23-Jun-26 19:39 aac/plugins/first_party/help_dump/help_dump_impl.py
+-rw-r--r--  2.0 unx     1403 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/__init__.py
+-rw-r--r--  2.0 unx     1227 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/conversion_helpers.py
+-rw-r--r--  2.0 unx    11791 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/language_server.py
+-rw-r--r--  2.0 unx     1481 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/lsp-server.yaml
+-rw-r--r--  2.0 unx      593 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/managed_workspace_file.py
+-rw-r--r--  2.0 unx     1197 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/start_lsp_server_impl.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/providers/__init__.py
+-rw-r--r--  2.0 unx     4430 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/providers/code_completion_provider.py
+-rw-r--r--  2.0 unx     2593 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/providers/document_link_provider.py
+-rw-r--r--  2.0 unx     5799 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/providers/find_references_provider.py
+-rw-r--r--  2.0 unx     7275 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/providers/goto_definition_provider.py
+-rw-r--r--  2.0 unx     1523 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/providers/hover_provider.py
+-rw-r--r--  2.0 unx      580 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/providers/locations.py
+-rw-r--r--  2.0 unx      467 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/providers/lsp_provider.py
+-rw-r--r--  2.0 unx     1461 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/providers/prepare_rename_provider.py
+-rw-r--r--  2.0 unx     3712 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/providers/publish_diagnostics_provider.py
+-rw-r--r--  2.0 unx     8796 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/providers/rename_provider.py
+-rw-r--r--  2.0 unx     6989 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/providers/semantic_tokens_provider.py
+-rw-r--r--  2.0 unx     3589 b- defN 23-Jun-26 19:39 aac/plugins/first_party/lsp_server/providers/symbols.py
+-rw-r--r--  2.0 unx     2220 b- defN 23-Jun-26 19:39 aac/plugins/first_party/plugin_management/__init__.py
+-rw-r--r--  2.0 unx     4969 b- defN 23-Jun-26 19:39 aac/plugins/first_party/plugin_management/plugin-management.yaml
+-rw-r--r--  2.0 unx     4411 b- defN 23-Jun-26 19:39 aac/plugins/first_party/plugin_management/plugin_management_impl.py
+-rw-r--r--  2.0 unx     1138 b- defN 23-Jun-26 19:39 aac/plugins/first_party/primitive_type_check/__init__.py
+-rw-r--r--  2.0 unx    16042 b- defN 23-Jun-26 19:39 aac/plugins/first_party/primitive_type_check/primitive_type_check.yaml
+-rw-r--r--  2.0 unx      932 b- defN 23-Jun-26 19:39 aac/plugins/first_party/primitive_type_check/validators/__init__.py
+-rw-r--r--  2.0 unx     1933 b- defN 23-Jun-26 19:39 aac/plugins/first_party/primitive_type_check/validators/bool_validator.py
+-rw-r--r--  2.0 unx     1974 b- defN 23-Jun-26 19:39 aac/plugins/first_party/primitive_type_check/validators/date_validator.py
+-rw-r--r--  2.0 unx     2156 b- defN 23-Jun-26 19:39 aac/plugins/first_party/primitive_type_check/validators/file_validator.py
+-rw-r--r--  2.0 unx     2326 b- defN 23-Jun-26 19:39 aac/plugins/first_party/primitive_type_check/validators/int_validator.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jun-26 19:39 aac/plugins/first_party/primitive_type_check/validators/num_validator.py
+-rw-r--r--  2.0 unx     1800 b- defN 23-Jun-26 19:39 aac/plugins/first_party/primitive_type_check/validators/reference_validator.py
+-rw-r--r--  2.0 unx     1852 b- defN 23-Jun-26 19:39 aac/plugins/first_party/primitive_type_check/validators/string_validator.py
+-rw-r--r--  2.0 unx     1017 b- defN 23-Jun-26 19:39 aac/plugins/first_party/print_spec/__init__.py
+-rw-r--r--  2.0 unx      899 b- defN 23-Jun-26 19:39 aac/plugins/first_party/print_spec/print-spec.yaml
+-rw-r--r--  2.0 unx      967 b- defN 23-Jun-26 19:39 aac/plugins/first_party/print_spec/print_spec_impl.py
+-rw-r--r--  2.0 unx     1662 b- defN 23-Jun-26 19:39 aac/plugins/first_party/rest_api/__init__.py
+-rw-r--r--  2.0 unx     2135 b- defN 23-Jun-26 19:39 aac/plugins/first_party/rest_api/aac_rest_api_impl.py
+-rw-r--r--  2.0 unx    16354 b- defN 23-Jun-26 19:39 aac/plugins/first_party/rest_api/aac_rest_app.py
+-rw-r--r--  2.0 unx     1973 b- defN 23-Jun-26 19:39 aac/plugins/first_party/rest_api/rest_api.yaml
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-26 19:39 aac/plugins/first_party/rest_api/models/__init__.py
+-rw-r--r--  2.0 unx     1563 b- defN 23-Jun-26 19:39 aac/plugins/first_party/rest_api/models/command_model.py
+-rw-r--r--  2.0 unx     1347 b- defN 23-Jun-26 19:39 aac/plugins/first_party/rest_api/models/definition_model.py
+-rw-r--r--  2.0 unx     1480 b- defN 23-Jun-26 19:39 aac/plugins/first_party/rest_api/models/file_model.py
+-rw-r--r--  2.0 unx     1544 b- defN 23-Jun-26 19:39 aac/plugins/first_party/specifications/__init__.py
+-rw-r--r--  2.0 unx      994 b- defN 23-Jun-26 19:39 aac/plugins/first_party/specifications/specifications.yaml
+-rw-r--r--  2.0 unx     3697 b- defN 23-Jun-26 19:39 aac/plugins/first_party/specifications/specifications_impl.py
+-rw-r--r--  2.0 unx      812 b- defN 23-Jun-26 19:39 aac/plugins/validators/__init__.py
+-rw-r--r--  2.0 unx     2302 b- defN 23-Jun-26 19:39 aac/plugins/validators/_common.py
+-rw-r--r--  2.0 unx     2538 b- defN 23-Jun-26 19:39 aac/plugins/validators/_finding_location.py
+-rw-r--r--  2.0 unx     1564 b- defN 23-Jun-26 19:39 aac/plugins/validators/_validator_finding.py
+-rw-r--r--  2.0 unx     2902 b- defN 23-Jun-26 19:39 aac/plugins/validators/_validator_findings.py
+-rw-r--r--  2.0 unx     1701 b- defN 23-Jun-26 19:39 aac/plugins/validators/_validator_result.py
+-rw-r--r--  2.0 unx     1060 b- defN 23-Jun-26 19:39 aac/plugins/validators/defined_references/__init__.py
+-rw-r--r--  2.0 unx     3353 b- defN 23-Jun-26 19:39 aac/plugins/validators/defined_references/_validate_references.py
+-rw-r--r--  2.0 unx     1648 b- defN 23-Jun-26 19:39 aac/plugins/validators/defined_references/defined_references.yaml
+-rw-r--r--  2.0 unx     1063 b- defN 23-Jun-26 19:39 aac/plugins/validators/exclusive_fields/__init__.py
+-rw-r--r--  2.0 unx     2022 b- defN 23-Jun-26 19:39 aac/plugins/validators/exclusive_fields/_validate_exclusive_fields.py
+-rw-r--r--  2.0 unx     2417 b- defN 23-Jun-26 19:39 aac/plugins/validators/exclusive_fields/exclusive_fields.yaml
+-rw-r--r--  2.0 unx     1051 b- defN 23-Jun-26 19:39 aac/plugins/validators/reference_fields/__init__.py
+-rw-r--r--  2.0 unx     3599 b- defN 23-Jun-26 19:39 aac/plugins/validators/reference_fields/_validate_reference_fields.py
+-rw-r--r--  2.0 unx     1681 b- defN 23-Jun-26 19:39 aac/plugins/validators/reference_fields/reference_fields.yaml
+-rw-r--r--  2.0 unx     1056 b- defN 23-Jun-26 19:39 aac/plugins/validators/reference_targets/__init__.py
+-rw-r--r--  2.0 unx     4612 b- defN 23-Jun-26 19:39 aac/plugins/validators/reference_targets/_validate_reference_targets.py
+-rw-r--r--  2.0 unx     1683 b- defN 23-Jun-26 19:39 aac/plugins/validators/reference_targets/reference_targets.yaml
+-rw-r--r--  2.0 unx     1787 b- defN 23-Jun-26 19:39 aac/plugins/validators/required_fields/__init__.py
+-rw-r--r--  2.0 unx     3372 b- defN 23-Jun-26 19:39 aac/plugins/validators/required_fields/_validate_required_fields.py
+-rw-r--r--  2.0 unx     1726 b- defN 23-Jun-26 19:39 aac/plugins/validators/required_fields/required_fields.yaml
+-rw-r--r--  2.0 unx     1049 b- defN 23-Jun-26 19:39 aac/plugins/validators/requirement_references/__init__.py
+-rw-r--r--  2.0 unx     2696 b- defN 23-Jun-26 19:39 aac/plugins/validators/requirement_references/_validate_requirement_references.py
+-rw-r--r--  2.0 unx     1644 b- defN 23-Jun-26 19:39 aac/plugins/validators/requirement_references/requirement_references.yaml
+-rw-r--r--  2.0 unx     1012 b- defN 23-Jun-26 19:39 aac/plugins/validators/root_keys/__init__.py
+-rw-r--r--  2.0 unx     1640 b- defN 23-Jun-26 19:39 aac/plugins/validators/root_keys/_validate_root_keys.py
+-rw-r--r--  2.0 unx     2461 b- defN 23-Jun-26 19:39 aac/plugins/validators/root_keys/root_keys.yaml
+-rw-r--r--  2.0 unx     1062 b- defN 23-Jun-26 19:39 aac/plugins/validators/subcomponent_type/__init__.py
+-rw-r--r--  2.0 unx     3028 b- defN 23-Jun-26 19:39 aac/plugins/validators/subcomponent_type/_validate_subcomponent_type.py
+-rw-r--r--  2.0 unx     1714 b- defN 23-Jun-26 19:39 aac/plugins/validators/subcomponent_type/subcomponent_type.yaml
+-rw-r--r--  2.0 unx     1015 b- defN 23-Jun-26 19:39 aac/plugins/validators/unique_names/__init__.py
+-rw-r--r--  2.0 unx     2365 b- defN 23-Jun-26 19:39 aac/plugins/validators/unique_names/_validate_unique_names.py
+-rw-r--r--  2.0 unx     1675 b- defN 23-Jun-26 19:39 aac/plugins/validators/unique_names/unique_names.yaml
+-rw-r--r--  2.0 unx     1049 b- defN 23-Jun-26 19:39 aac/plugins/validators/unique_requirement_ids/__init__.py
+-rw-r--r--  2.0 unx     3698 b- defN 23-Jun-26 19:39 aac/plugins/validators/unique_requirement_ids/_validate_unique_requirement_ids.py
+-rw-r--r--  2.0 unx     1689 b- defN 23-Jun-26 19:39 aac/plugins/validators/unique_requirement_ids/unique_requirement_ids.yaml
+-rw-r--r--  2.0 unx     1129 b- defN 23-Jun-26 19:39 aac/plugins/validators/validator_implementation/__init__.py
+-rw-r--r--  2.0 unx     2317 b- defN 23-Jun-26 19:39 aac/plugins/validators/validator_implementation/_validate_validator_implementation.py
+-rw-r--r--  2.0 unx     1722 b- defN 23-Jun-26 19:39 aac/plugins/validators/validator_implementation/validator_implementation.yaml
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-26 19:39 aac/serialization/__init__.py
+-rw-r--r--  2.0 unx     1076 b- defN 23-Jun-26 19:39 aac/serialization/aac_command_encoder.py
+-rw-r--r--  2.0 unx      317 b- defN 23-Jun-26 19:39 aac/spec/__init__.py
+-rw-r--r--  2.0 unx     4140 b- defN 23-Jun-26 19:39 aac/spec/core.py
+-rw-r--r--  2.0 unx    18876 b- defN 23-Jun-26 19:39 aac/spec/spec.yaml
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-26 19:39 aac/templates/__init__.py
+-rw-r--r--  2.0 unx     6327 b- defN 23-Jun-26 19:39 aac/templates/engine.py
+-rw-r--r--  2.0 unx      379 b- defN 23-Jun-26 19:39 aac/templates/error.py
+-rw-r--r--  2.0 unx      532 b- defN 23-Jun-26 19:39 aac/validate/__init__.py
+-rw-r--r--  2.0 unx     3995 b- defN 23-Jun-26 19:39 aac/validate/_collect_validators.py
+-rw-r--r--  2.0 unx    11286 b- defN 23-Jun-26 19:39 aac/validate/_validate.py
+-rw-r--r--  2.0 unx      214 b- defN 23-Jun-26 19:39 aac/validate/_validation_error.py
+-rw-r--r--  2.0 unx    15070 b- defN 23-Jun-26 19:40 aac-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 19:40 aac-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-26 19:40 aac-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-26 19:40 aac-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    23105 b- defN 23-Jun-26 19:40 aac-0.2.0.dist-info/RECORD
+217 files, 610762 bytes uncompressed, 171332 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -57,20 +57,29 @@
 
 Filename: aac/io/files/find.py
 Comment: 
 
 Filename: aac/io/parser/__init__.py
 Comment: 
 
+Filename: aac/io/parser/_cache.py
+Comment: 
+
+Filename: aac/io/parser/_cache_manager.py
+Comment: 
+
 Filename: aac/io/parser/_parse_source.py
 Comment: 
 
 Filename: aac/io/parser/_parser_error.py
 Comment: 
 
+Filename: aac/io/parser/_yaml.py
+Comment: 
+
 Filename: aac/lang/__init__.py
 Comment: 
 
 Filename: aac/lang/active_context_lifecycle_manager.py
 Comment: 
 
 Filename: aac/lang/constants.py
@@ -102,26 +111,32 @@
 
 Filename: aac/lang/definitions/json_schema.py
 Comment: 
 
 Filename: aac/lang/definitions/lexeme.py
 Comment: 
 
+Filename: aac/lang/definitions/metadata_structure.py
+Comment: 
+
 Filename: aac/lang/definitions/references.py
 Comment: 
 
 Filename: aac/lang/definitions/schema.py
 Comment: 
 
 Filename: aac/lang/definitions/search.py
 Comment: 
 
 Filename: aac/lang/definitions/source_location.py
 Comment: 
 
+Filename: aac/lang/definitions/structural_node.py
+Comment: 
+
 Filename: aac/lang/definitions/structure.py
 Comment: 
 
 Filename: aac/lang/definitions/type.py
 Comment: 
 
 Filename: aac/persistence/__init__.py
@@ -168,14 +183,23 @@
 
 Filename: aac/plugins/contributions/contribution_types/primitive_validation_contribution.py
 Comment: 
 
 Filename: aac/plugins/first_party/__init__.py
 Comment: 
 
+Filename: aac/plugins/first_party/active_context/__init__.py
+Comment: 
+
+Filename: aac/plugins/first_party/active_context/active_context.yaml
+Comment: 
+
+Filename: aac/plugins/first_party/active_context/active_context_impl.py
+Comment: 
+
 Filename: aac/plugins/first_party/gen_design_doc/__init__.py
 Comment: 
 
 Filename: aac/plugins/first_party/gen_design_doc/gen_design_doc.yaml
 Comment: 
 
 Filename: aac/plugins/first_party/gen_design_doc/gen_design_doc_impl.py
@@ -339,14 +363,17 @@
 
 Filename: aac/plugins/first_party/lsp_server/providers/__init__.py
 Comment: 
 
 Filename: aac/plugins/first_party/lsp_server/providers/code_completion_provider.py
 Comment: 
 
+Filename: aac/plugins/first_party/lsp_server/providers/document_link_provider.py
+Comment: 
+
 Filename: aac/plugins/first_party/lsp_server/providers/find_references_provider.py
 Comment: 
 
 Filename: aac/plugins/first_party/lsp_server/providers/goto_definition_provider.py
 Comment: 
 
 Filename: aac/plugins/first_party/lsp_server/providers/hover_provider.py
@@ -369,23 +396,14 @@
 
 Filename: aac/plugins/first_party/lsp_server/providers/semantic_tokens_provider.py
 Comment: 
 
 Filename: aac/plugins/first_party/lsp_server/providers/symbols.py
 Comment: 
 
-Filename: aac/plugins/first_party/material_model/__init__.py
-Comment: 
-
-Filename: aac/plugins/first_party/material_model/material_model.yaml
-Comment: 
-
-Filename: aac/plugins/first_party/material_model/material_model_impl.py
-Comment: 
-
 Filename: aac/plugins/first_party/plugin_management/__init__.py
 Comment: 
 
 Filename: aac/plugins/first_party/plugin_management/plugin-management.yaml
 Comment: 
 
 Filename: aac/plugins/first_party/plugin_management/plugin_management_impl.py
@@ -399,17 +417,32 @@
 
 Filename: aac/plugins/first_party/primitive_type_check/validators/__init__.py
 Comment: 
 
 Filename: aac/plugins/first_party/primitive_type_check/validators/bool_validator.py
 Comment: 
 
+Filename: aac/plugins/first_party/primitive_type_check/validators/date_validator.py
+Comment: 
+
+Filename: aac/plugins/first_party/primitive_type_check/validators/file_validator.py
+Comment: 
+
 Filename: aac/plugins/first_party/primitive_type_check/validators/int_validator.py
 Comment: 
 
+Filename: aac/plugins/first_party/primitive_type_check/validators/num_validator.py
+Comment: 
+
+Filename: aac/plugins/first_party/primitive_type_check/validators/reference_validator.py
+Comment: 
+
+Filename: aac/plugins/first_party/primitive_type_check/validators/string_validator.py
+Comment: 
+
 Filename: aac/plugins/first_party/print_spec/__init__.py
 Comment: 
 
 Filename: aac/plugins/first_party/print_spec/print-spec.yaml
 Comment: 
 
 Filename: aac/plugins/first_party/print_spec/print_spec_impl.py
@@ -438,20 +471,14 @@
 
 Filename: aac/plugins/first_party/rest_api/models/file_model.py
 Comment: 
 
 Filename: aac/plugins/first_party/specifications/__init__.py
 Comment: 
 
-Filename: aac/plugins/first_party/specifications/globally_unique_id.py
-Comment: 
-
-Filename: aac/plugins/first_party/specifications/referenced_ids_exist.py
-Comment: 
-
 Filename: aac/plugins/first_party/specifications/specifications.yaml
 Comment: 
 
 Filename: aac/plugins/first_party/specifications/specifications_impl.py
 Comment: 
 
 Filename: aac/plugins/validators/__init__.py
@@ -480,15 +507,15 @@
 
 Filename: aac/plugins/validators/defined_references/defined_references.yaml
 Comment: 
 
 Filename: aac/plugins/validators/exclusive_fields/__init__.py
 Comment: 
 
-Filename: aac/plugins/validators/exclusive_fields/_exclusive_fields.py
+Filename: aac/plugins/validators/exclusive_fields/_validate_exclusive_fields.py
 Comment: 
 
 Filename: aac/plugins/validators/exclusive_fields/exclusive_fields.yaml
 Comment: 
 
 Filename: aac/plugins/validators/reference_fields/__init__.py
 Comment: 
@@ -513,45 +540,63 @@
 
 Filename: aac/plugins/validators/required_fields/_validate_required_fields.py
 Comment: 
 
 Filename: aac/plugins/validators/required_fields/required_fields.yaml
 Comment: 
 
+Filename: aac/plugins/validators/requirement_references/__init__.py
+Comment: 
+
+Filename: aac/plugins/validators/requirement_references/_validate_requirement_references.py
+Comment: 
+
+Filename: aac/plugins/validators/requirement_references/requirement_references.yaml
+Comment: 
+
 Filename: aac/plugins/validators/root_keys/__init__.py
 Comment: 
 
 Filename: aac/plugins/validators/root_keys/_validate_root_keys.py
 Comment: 
 
 Filename: aac/plugins/validators/root_keys/root_keys.yaml
 Comment: 
 
 Filename: aac/plugins/validators/subcomponent_type/__init__.py
 Comment: 
 
-Filename: aac/plugins/validators/subcomponent_type/_subcomponent_type.py
+Filename: aac/plugins/validators/subcomponent_type/_validate_subcomponent_type.py
 Comment: 
 
 Filename: aac/plugins/validators/subcomponent_type/subcomponent_type.yaml
 Comment: 
 
 Filename: aac/plugins/validators/unique_names/__init__.py
 Comment: 
 
-Filename: aac/plugins/validators/unique_names/_unique_names.py
+Filename: aac/plugins/validators/unique_names/_validate_unique_names.py
 Comment: 
 
 Filename: aac/plugins/validators/unique_names/unique_names.yaml
 Comment: 
 
+Filename: aac/plugins/validators/unique_requirement_ids/__init__.py
+Comment: 
+
+Filename: aac/plugins/validators/unique_requirement_ids/_validate_unique_requirement_ids.py
+Comment: 
+
+Filename: aac/plugins/validators/unique_requirement_ids/unique_requirement_ids.yaml
+Comment: 
+
 Filename: aac/plugins/validators/validator_implementation/__init__.py
 Comment: 
 
-Filename: aac/plugins/validators/validator_implementation/_validator_implementation.py
+Filename: aac/plugins/validators/validator_implementation/_validate_validator_implementation.py
 Comment: 
 
 Filename: aac/plugins/validators/validator_implementation/validator_implementation.yaml
 Comment: 
 
 Filename: aac/serialization/__init__.py
 Comment: 
@@ -585,23 +630,23 @@
 
 Filename: aac/validate/_validate.py
 Comment: 
 
 Filename: aac/validate/_validation_error.py
 Comment: 
 
-Filename: aac-0.1.9.dist-info/METADATA
+Filename: aac-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: aac-0.1.9.dist-info/WHEEL
+Filename: aac-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: aac-0.1.9.dist-info/entry_points.txt
+Filename: aac-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: aac-0.1.9.dist-info/top_level.txt
+Filename: aac-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aac-0.1.9.dist-info/RECORD
+Filename: aac-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aac/__init__.py

```diff
@@ -8,19 +8,19 @@
     major = sys.version_info.major
     print(f"Python version {major}.{minor} is too low; AaC requires at least Python version 3.9 or higher to run.")
     exit(1)
 
 import logging
 import os
 
-__version__ = "0.1.9"
+__version__ = "0.2.0"
 __log_file_name__ = os.path.join(os.path.dirname(__file__), "aac.log")
 
 logging.basicConfig(
-    format="%(asctime)s::%(module)s::%(filename)s::L%(lineno)d::%(levelname)s::%(message)s",
+    format="%(asctime)s::%(pathname)s:%(lineno)d::%(levelname)s::%(message)s",
     filename=__log_file_name__,
     encoding="utf-8",
     level=logging.DEBUG,
     datefmt="%m/%d/%Y %H:%M:%S",
 )
 
 __all__ = ("__version__",)
```

## aac/__main__.py

```diff
@@ -1,12 +1,10 @@
 """Main entry point."""
-
 import sys
 
 if sys.argv[0].endswith("__main__.py"):
     sys.argv[0] = "aac"
 
 
 if __name__ == "__main__":
     from aac.cli.execute import cli
-
     cli()
```

## aac/cli/execute.py

```diff
@@ -1,13 +1,14 @@
 """The entry-point for the command line interface for the aac tool."""
 
 import sys
-from click import Argument, Command, Option, ParamType, Parameter, Path, UNPROCESSED, echo, group, types
+from click import Argument, Command, Option, ParamType, Parameter, Path, UNPROCESSED, group, secho, types
 
 from aac.cli.aac_command import AacCommand, AacCommandArgument
+from aac.io.parser._parser_error import ParserError
 from aac.lang.active_context_lifecycle_manager import get_active_context
 from aac.persistence import ACTIVE_CONTEXT_STATE_FILE_NAME
 from aac.plugins.plugin_execution import PluginExecutionResult
 
 
 @group(context_settings=dict(help_option_names=["-h", "--help"]))
 def cli():
@@ -15,15 +16,15 @@
     pass
 
 
 @cli.result_callback()
 def output_result(result: PluginExecutionResult):
     """Output the message from the result of executing the CLI command."""
     error_occurred = not result.is_success()
-    echo(result.get_messages_as_string(), err=error_occurred, color=True)
+    secho(result.get_messages_as_string(), err=error_occurred, color=True)
 
     get_active_context().export_to_file(ACTIVE_CONTEXT_STATE_FILE_NAME)
 
     if error_occurred:
         sys.exit(result.status_code.value)
 
 
@@ -57,16 +58,20 @@
 
         return not arg.name.startswith("-")
 
     return Command(
         name=command.name,
         callback=command.callback,
         params=[to_click_parameter(arg) for arg in command.arguments],
-        help=command.description,
+        short_help=command.description,
         no_args_is_help=len([arg for arg in command.arguments if is_required_arg(arg)]) > 0,
     )
 
 
-active_context = get_active_context()
+try:
+    active_context = get_active_context()
+except ParserError as error:
+    raise ParserError(error.source, error.errors) from None
+
 commands = [to_click_command(cmd) for cmd in active_context.get_plugin_commands()]
 for command in commands:
     cli.add_command(command)
```

## aac/cli/builtin_commands/validate/validate.yaml

```diff
@@ -1,35 +1,34 @@
-model:
-  name: validate
-  description: Validate the provided Architecture-as-Code definition file.
-  behavior:
+plugin:
+  name: Validate
+  description: An AaC plugin that validates the definition(s) in a file.
+  commands:
     - name: validate
-      type: command
-      description: Validate the AaC definition file.
+      helpText: Validate one, or more, AaC definitions in a file.
       input:
         - name: architecture-file
           type: file
           python_type: str
           description: The path to the AaC file to be validated.
         - name: --definition-name
           type: string
           python_type: str
           description: |
             The name of one definition to validate. (optional)
             This argument will cause only the definition provided by the argument to be validated.
       acceptance:
-        - scenario: The definitions are valid
+        - scenario: The definitions are valid.
           given:
             - The file path at {{validate.input.architecture-file}} exists.
             - The contents of {{validate.input.architecture-file}} are a valid AaC definition.
           when:
             - The aac application is run with the validate command.
           then:
             - A successful validation status is displayed to the user.
-        - scenario: The definitions are invalid
+        - scenario: The definitions are invalid.
           given:
             - The file path at {{validate.input.architecture-file}} exists.
             - The contents of {{validate.input.architecture-file}} do not represent a valid AaC definition.
           when:
             - The aac application is run with the validate command.
           then:
             - A validation failure status is displayed to the user.
```

## aac/cli/builtin_commands/validate/validate_impl.py

```diff
@@ -1,23 +1,23 @@
-"""AaC Plugin implementation module for the validate plugin."""
-# NOTE: It is safe to edit this file.
-# This file is only initially generated by the aac gen-plugin, and it won't be overwritten if the file already exists.
+"""AaC Plugin implementation module for the Validate plugin."""
+
+
 import logging
+
 from os import linesep
 from typing import Optional
 
+from aac.io.parser import parse, ParserError
 from aac.lang.active_context_lifecycle_manager import get_active_context
-
+from aac.lang.definitions.collections import get_definition_by_name
 from aac.plugins import PluginError
 from aac.plugins.plugin_execution import PluginExecutionResult, plugin_result
 from aac.validate import validated_source, validated_definition
-from aac.io.parser import parse
-from aac.lang.definitions.collections import get_definition_by_name
 
-plugin_name = "validate"
+plugin_name = "Validate"
 
 
 def validate(architecture_file: str, definition_name: Optional[str] = None) -> PluginExecutionResult:
     """
     Validate the AaC definition file.
 
     Args:
@@ -34,38 +34,47 @@
     with plugin_result(plugin_name, _validate) as result:
         return result
 
 
 def _validate_definition_in_file(file_path, definition_name) -> str:
     success_message = f"'{definition_name}' in {file_path} is valid."
 
-    definitions_in_file = parse(file_path)
-    definition_to_validate = get_definition_by_name(definition_name, definitions_in_file)
-    if definition_to_validate:
-        with validated_definition(definition_to_validate):
-            return success_message
+    try:
+        definitions_in_file = parse(file_path)
+    except ParserError as error:
+        raise ParserError(error.source, error.errors) from None
     else:
-        active_context = get_active_context()
-        target_definition = active_context.get_definition_by_name(definition_name)
-
-        possible_source_message = ""
-        if target_definition:
-            possible_source_message = f"Definition '{definition_name}' can be found in '{target_definition.source.uri}'"
-
-        possible_definitions_in_file = [definition.name for definition in definitions_in_file]
-
-        missing_definition_error_message = linesep.join(
-            [
-                f"'{definition_name}' was not found in the file.",
-                f"Definitions available in '{file_path}' are {possible_definitions_in_file}",
-                possible_source_message
-            ]
-        )
+        definition_to_validate = get_definition_by_name(definition_name, definitions_in_file)
+        if definition_to_validate:
+            with validated_definition(definition_to_validate) as result:
+                return _get_validation_success_message(success_message, result)
+        else:
+            active_context = get_active_context()
+            target_definition = active_context.get_definition_by_name(definition_name)
 
-        logging.error(missing_definition_error_message)
-        raise PluginError(missing_definition_error_message)
+            possible_source_message = ""
+            if target_definition:
+                possible_source_message = f"Definition '{definition_name}' can be found in '{target_definition.source.uri}'"
+
+            possible_definitions_in_file = [definition.name for definition in definitions_in_file]
+
+            missing_definition_error_message = linesep.join(
+                [
+                    f"'{definition_name}' was not found in the file.",
+                    f"Definitions available in '{file_path}' are {possible_definitions_in_file}",
+                    possible_source_message
+                ]
+            )
+            logging.error(missing_definition_error_message)
+            raise PluginError(missing_definition_error_message)
 
 
 def _validate_context_and_file(file_path) -> str:
     success_message = f"{file_path} is valid."
-    with validated_source(file_path):
-        return success_message
+    with validated_source(file_path) as result:
+        return _get_validation_success_message(success_message, result)
+
+
+def _get_validation_success_message(default_message, validation_result) -> str:
+    plugin_messages = validation_result.get_messages_as_string()
+    return_message = f"{default_message}{linesep}{plugin_messages}"
+    return return_message
```

## aac/cli/builtin_commands/version/version.yaml

```diff
@@ -1,13 +1,12 @@
-model:
-  name: version
-  description: Outputs Architecture-as-Code Python package version
-  behavior:
+plugin:
+  name: Version
+  description: An AaC plugin that outputs the Architecture-as-Code Python package version.
+  commands:
     - name: version
-      type: command
-      description: Print the AaC package version
+      helpText: Print the AaC package version.
       acceptance:
-        - scenario: Output the AaC package version
+        - scenario: Output the AaC package version.
           when:
             - The aac application is run with the version command.
           then:
             - The AaC Python package version is written to the console.
```

## aac/cli/builtin_commands/version/version_impl.py

```diff
@@ -1,13 +1,13 @@
-"""AaC Plugin implementation module for the version plugin."""
+"""AaC Plugin implementation module for the Version plugin."""
 
 from aac import __version__
 from aac.plugins.plugin_execution import PluginExecutionResult, plugin_result
 
-plugin_name = "version"
+plugin_name = "Version"
 
 
 def version() -> PluginExecutionResult:
     """Print the AaC package version."""
 
     def get_current_version():
         return __version__
```

## aac/io/files/aac_file.py

```diff
@@ -1,12 +1,12 @@
 """File metadata and management class for AaC."""
 from attr import attrib, attrs, validators
 
 
-@attrs(eq=False)
+@attrs(hash=False, eq=False)
 class AaCFile:
     """
     An Architecture-as-Code file containing AaC definitions.
 
     Attributes:
         uri (str): The file's URI path
         is_user_editable (bool): True if the file can be edited by the user, otherwise false
```

## aac/io/files/find.py

```diff
@@ -30,14 +30,14 @@
     _, file_ext = os.path.splitext(filepath)
 
     is_valid_aac_file = False
     if file_ext == YAML_DOCUMENT_EXTENSION or file_ext == AAC_DOCUMENT_EXTENSION:
         try:
             parse(filepath)
         except ParserError as error:
-            logging.info(f"File '{filepath}' is not a valid AaC file. Reason: {error.errors}")
+            logging.error(f"File '{filepath}' is not a valid AaC file. Reason: {error.errors}")
         except Exception as error:
-            logging.info(f"File '{filepath}' could not be parsed. Reason: {error}")
+            logging.error(f"File '{filepath}' could not be parsed. Reason: {error}")
         else:
             is_valid_aac_file = True
 
     return is_valid_aac_file
```

## aac/io/parser/__init__.py

```diff
@@ -1,9 +1,15 @@
 """AaC Parser and related functions submodule."""
 
 from aac.io.parser._parse_source import parse
 from aac.io.parser._parser_error import ParserError
+from aac.io.parser._yaml import scan_yaml, parse_yaml
+from aac.io.parser._cache_manager import get_cache, reset_cache
 
 __all__ = (
     ParserError.__name__,
     parse.__name__,
+    scan_yaml.__name__,
+    parse_yaml.__name__,
+    get_cache.__name__,
+    reset_cache.__name__,
 )
```

## aac/io/parser/_parse_source.py

```diff
@@ -1,30 +1,37 @@
-"""Parse Architecture-as-Code YAML files.
+"""
+Parse Architecture-as-Code YAML files.
 
 The AaC parser reads a YAML file, performs validation (if not suppressed) and provides
 the caller with a dictionary of the content keyed by the named type.  This allows you
 to find a certain type in a model by just looking for that key.
 """
 import logging
-import yaml
+
+from copy import deepcopy
 from os import path, linesep
 from typing import Optional
-from yaml.parser import ParserError as YAMLParserError
+from yaml import Mark, Token, StreamStartToken, StreamEndToken, DocumentStartToken
 
 from aac.io.constants import DEFAULT_SOURCE_URI
 from aac.io.files.aac_file import AaCFile
-from aac.io.parser._parser_error import ParserError
+from aac.io.parser._cache_manager import get_cache
 from aac.io.paths import sanitize_filesystem_path
+from aac.lang.constants import DEFINITION_FIELD_FILES, DEFINITION_FIELD_NAME, ROOT_KEY_IMPORT
 from aac.lang.definitions.definition import Definition
 from aac.lang.definitions.lexeme import Lexeme
 from aac.lang.definitions.source_location import SourceLocation
 
 
+YAML_CACHE = get_cache()
+
+
 def parse(source: str, source_uri: Optional[str] = None) -> list[Definition]:
-    """Parse the Architecture-as-Code (AaC) definition(s) from the provided source.
+    """
+    Parse the Architecture-as-Code (AaC) definition(s) from the provided source.
 
     Args:
         source (str): Must be either a file path to an AaC yaml file or a string containing AaC definitions.
         source_uri (Optional[str]): Overrides and sets the source_uri
 
     Returns:
         A list of Definition objects containing the internal representation of the definition and metadata
@@ -39,197 +46,135 @@
         if path.lexists(sanitized_source):
             is_file = True
 
     return _parse_file(sanitized_source) if is_file else _parse_str(source_uri or DEFAULT_SOURCE_URI, source)
 
 
 def _parse_file(arch_file: str) -> list[Definition]:
-    """Parse an Architecture-as-Code YAML file and return the definitions in it.
+    """
+    Parse an Architecture-as-Code YAML file and return the definitions in it.
 
     Args:
         arch_file (str): The Architecture-as-Code YAML file to be parsed.
 
     Returns:
         The AaC definitions extracted from the specified file.
     """
     definition_lists = [_parse_str(file, _read_file_content(file)) for file in _get_files_to_process(arch_file)]
     return [definition for definition_list in definition_lists for definition in definition_list]
 
 
 def _parse_str(source: str, model_content: str) -> list[Definition]:
-    """Parse a string containing one or more YAML model definitions.
+    """
+    Parse a string containing one or more YAML model definitions.
 
     Args:
         source:  The file the content came from (to help with better logging)
         model_content:  The YAML to parse
 
     Returns:
         The AaC definitions that were built from the model contents.
     """
 
-    def mark_to_source_location(start: yaml.error.Mark, end: yaml.error.Mark) -> SourceLocation:
+    def mark_to_source_location(start: Mark, end: Mark) -> SourceLocation:
         return SourceLocation(start.line, start.column, start.index, end.column - start.column)
 
     def get_lexemes_for_definition(value_tokens, content_start, content_end) -> list[Lexeme]:
         definition_tokens = [token for token in value_tokens if is_token_between_locations(token, content_start, content_end)]
         definition_lexemes = []
         for token in definition_tokens:
             location = mark_to_source_location(token.start_mark, token.end_mark)
             definition_lexemes.append(Lexeme(location, source, token.value))
         return definition_lexemes
 
     def is_token_between_locations(token, inclusive_line_start: int, inclusive_line_end: int) -> list[Lexeme]:
         return token.start_mark.line >= inclusive_line_start and token.end_mark.line <= inclusive_line_end
 
-    yaml_tokens = _scan_yaml(model_content)
-    value_tokens = [token for token in yaml_tokens if hasattr(token, "value")]
-    doc_start_token = [token for token in yaml_tokens if isinstance(token, yaml.tokens.StreamStartToken)]
-    doc_end_token = [token for token in yaml_tokens if isinstance(token, yaml.tokens.StreamEndToken)]
-    doc_segment_tokens = [token for token in yaml_tokens if isinstance(token, yaml.tokens.DocumentStartToken)]
+    yaml_tokens: list[Token] = YAML_CACHE.scan_string(model_content)
+    value_tokens: list[Token] = [token for token in yaml_tokens if hasattr(token, "value")]
+    doc_start_token: list[StreamStartToken] = [token for token in yaml_tokens if isinstance(token, StreamStartToken)]
+    doc_end_token: list[StreamEndToken] = [token for token in yaml_tokens if isinstance(token, StreamEndToken)]
+    doc_segment_tokens: list[DocumentStartToken] = [token for token in yaml_tokens if isinstance(token, DocumentStartToken)]
     doc_tokens = [*doc_start_token, *doc_segment_tokens, *doc_end_token]
 
+    yaml_dicts: list[dict] = deepcopy(YAML_CACHE.parse_string(model_content))
+
     source_files: dict[str, AaCFile] = {}
     definitions: list[Definition] = []
     for doc_token_index in range(0, len(doc_tokens) - 1):
         start_doc_token = doc_tokens[doc_token_index]
         end_doc_token = doc_tokens[doc_token_index + 1]
 
         content_start_line = start_doc_token.start_mark.line
-        content_end_line = end_doc_token.end_mark.line
-
-        end_of_file_offset = 1 if isinstance(end_doc_token, yaml.tokens.StreamEndToken) else 0
+        content_end_line = end_doc_token.end_mark.line + (1 if isinstance(end_doc_token, StreamEndToken) else 0)
 
-        yaml_text = linesep.join(model_content.splitlines()[content_start_line:content_end_line + end_of_file_offset])
+        yaml_text = linesep.join(model_content.splitlines()[content_start_line:content_end_line])
         yaml_text += linesep
 
         if yaml_text.strip():
             definition_lexemes = get_lexemes_for_definition(value_tokens, content_start_line, content_end_line)
-            root_yaml, *_ = _parse_yaml(source, yaml_text)
-
-            if "import" in root_yaml:
-                del root_yaml["import"]
-
-            root_type, *_ = root_yaml.keys()
-            definition_name = root_yaml.get(root_type, {}).get("name")
-            source_file = source_files.get(source)
 
-            if not source_file:
-                source_file = AaCFile(source, True, False)
-                source_files[source] = source_file
-
-            definitions.append(Definition(definition_name, yaml_text, source_file, definition_lexemes, root_yaml))
+            if yaml_dicts:
+                source_file = source_files.get(source)
+                if not source_file:
+                    source_file = AaCFile(source, True, False)
+                    source_files[source] = source_file
+
+                root_yaml = yaml_dicts.pop(0)
+                root_type, *_ = root_yaml.keys()
+                definition_name = root_yaml.get(root_type, {}).get(DEFINITION_FIELD_NAME, "")
+
+                new_definition = Definition(
+                    name=definition_name,
+                    content=yaml_text,
+                    source=source_file,
+                    meta_structure=None,
+                    lexemes=definition_lexemes,
+                    structure=root_yaml,
+                )
+                definitions.append(new_definition)
         else:
-            logging.info(f"Skipping empty content between {start_doc_token}:L{content_start_line} and {end_doc_token}:L{content_end_line} in source {source}")
+            logging.info(
+                f"Skipping empty content between {start_doc_token}:L{content_start_line} and {end_doc_token}:L{content_end_line} in source {source}"
+            )
             logging.debug(f"Source: {source} Content:{model_content}")
             logging.debug(f"Content lines:{model_content.splitlines()}")
 
     return definitions
 
 
-def _parse_yaml(source: str, content: str) -> list[dict]:
-    """Parse content as a YAML string and return the resulting structure.
-
-    Args:
-        source (str): The source of the YAML content. Used to provide better error messages.
-        content (str): The YAML content to be parsed.
-
-    Returns:
-        The parsed YAML content.
-
-    Raises:
-        If the YAML is invalid, a ParserError is raised.
-        If the model is not a dictionary, a ParserError is raised.
-        If the model does not have (at least) a "name" field, a ParserError is raised.
-    """
-    try:
-        models = list(yaml.load_all(content, Loader=yaml.SafeLoader))
-        _error_if_not_yaml(source, content, models)
-        _error_if_not_complete(source, content, models)
-        return models
-    except YAMLParserError as error:
-        raise ParserError(source, [f"Failed to parse file, invalid YAML {error.context} {error.problem}", content])
-    except Exception as error:
-        raise ParserError(source, [f"Failed to parse file, invalid YAML {error}", content])
-
-
-def _scan_yaml(content):
-    return list(yaml.scan(content, Loader=yaml.SafeLoader))
-
-
-def _error_if_not_yaml(source, content, models):
-    """Raise a ParserError if the model is not a YAML model we can parse."""
-
-    def is_model(model):
-        """Return True if the model is further parseable."""
-        return isinstance(model, dict)
-
-    # Iterate over each model and test if it is considered a valid model.
-    if not all(map(is_model, models)):
-        raise ParserError(source, ["provided content was not YAML", content])
-
-
-def _error_if_not_complete(source, content, models):
-    """Raise a ParserError if the model is incomplete."""
-
-    def is_import(model):
-        """Return True if the model is an import declaration."""
-        type, *_ = model.keys()
-        return type == "import"
-
-    def assert_definition_has_name(model):
-        """Throws a ParserError if the definition doesn't have a name property."""
-        type, *_ = model.keys()
-        has_name = model.get(type) and model.get(type).get("name")
-        if not has_name:
-            raise ParserError(source, [f"Definition is missing field 'name': {content}"])
-
-    # Raise an error if any of the loaded YAML models are incomplete.
-    models_without_imports = list(filter(lambda m: not is_import(m), models))
-    all(map(assert_definition_has_name, models_without_imports))
-
-
 def _read_file_content(arch_file: str) -> str:
     """
     Read file content method extracts text content from the specified file.
 
     Args:
         arch_file: The file to read.
 
     Returns:
         The contents of the file as a string.
     """
-    arch_file_path = arch_file
-    with open(arch_file_path, "r") as file:
+    with open(arch_file, "r") as file:
         return file.read()
 
 
-def _recurse_imports(arch_file_path: str, existing: set) -> set:
-    """Recursive portion of _get_files_to_process that keeps track of history so that we can handle circular imports.
+def _get_files_to_process(arch_file_path: str) -> list[str]:
+    """
+    Return a list of all files referenced in the model.
 
-    Discovered an issue during testing where if there exists a cycle in the import sequence across files, the parser
-    will recurse until it crashes.  Unfortunately this led to an error message to the user saying the initial file was
-    invalid yaml, which it was not, creating confusion.  Now this just eliminates duplications when discovered in the
-    import sequence avoiding the issue.
-    """
-    existing.add(arch_file_path)
-    content = _read_file_content(arch_file_path)
-    roots = _parse_yaml(arch_file_path, content)
-    roots_with_imports = [root for root in roots if "import" in root.keys()]
+    Traverse the import path starting from the specified file and return a list of all files referenced by the model.
+    """
+
+    def collect_imports(arch_file_path: str, unique_imports: set[str]) -> set[str]:
+        unique_imports.add(arch_file_path)
+        structures = [structure for structure in YAML_CACHE.parse_file(arch_file_path) if structure.get(ROOT_KEY_IMPORT)]
+        imports = [imp for root in structures for imp in root.get(ROOT_KEY_IMPORT, {}).get(DEFINITION_FIELD_FILES, [])]
 
-    for root in roots_with_imports:
-        for imp in root["import"]:
+        for imp in imports:
             arch_file_dir = path.dirname(path.realpath(arch_file_path))
             parse_path = path.join(arch_file_dir, imp.removeprefix(f".{path.sep}"))
             sanitized_path = sanitize_filesystem_path(parse_path)
-            if sanitized_path not in existing:
-                existing.update(_recurse_imports(sanitized_path, existing))
-
-    return existing
+            if sanitized_path not in unique_imports:
+                unique_imports.update(collect_imports(sanitized_path, unique_imports))
 
+        return unique_imports
 
-def _get_files_to_process(arch_file_path: str) -> list[str]:
-    """Return a list of all files referenced in the model.
-
-    Traverse the import path starting from the specified Arch-as-Code file and returns a list of
-    all files referenced by the model.
-    """
-    return list(_recurse_imports(arch_file_path, set()))
+    return list(collect_imports(arch_file_path, set()))
```

## aac/io/parser/_parser_error.py

```diff
@@ -1,10 +1,9 @@
 """Custom ParserError class that represents errors encountered during the parsing process."""
 from attr import Factory, attrib, attrs, validators
 
 
 @attrs
 class ParserError(BaseException):
     """An error that represents a file that could not be parsed."""
-
     source: str = attrib(validator=validators.instance_of(str))
     errors: list[str] = attrib(default=Factory(list), validator=validators.instance_of(list))
```

## aac/lang/active_context_lifecycle_manager.py

```diff
@@ -1,9 +1,8 @@
 """This module manages a singleton instance of LanguageContext and its lifecycle."""
-
 from aac.lang.language_context import LanguageContext
 from aac.persistence import ACTIVE_CONTEXT_STATE_FILE_NAME
 from aac.plugins.plugin_manager import get_plugins
 from aac.spec import get_aac_spec
 
 
 ACTIVE_CONTEXT = None
@@ -17,16 +16,16 @@
         reload_context: If true, the active context will be rebuilt and plugins/extension reapplied.
 
     Returns:
         The managed instance of LanguageContext
     """
     global ACTIVE_CONTEXT
 
-    if False and not ACTIVE_CONTEXT and not reload_context:  # Disabling persistence for performance reasons.
-        ACTIVE_CONTEXT = LanguageContext()
+    if not ACTIVE_CONTEXT and not reload_context:
+        ACTIVE_CONTEXT = get_initialized_language_context(core_spec_only=True)
         ACTIVE_CONTEXT.import_from_file(ACTIVE_CONTEXT_STATE_FILE_NAME)
 
     if not ACTIVE_CONTEXT or reload_context or not ACTIVE_CONTEXT.is_initialized:
         ACTIVE_CONTEXT = get_initialized_language_context()
 
     return ACTIVE_CONTEXT
```

## aac/lang/constants.py

```diff
@@ -2,45 +2,91 @@
 This module provides string constants for strings used in the Core AaC Spec.
 
 These values aren't expected to change often; it's expected that any deviation
 between these values and the core spec will be caught by testing.
 """
 
 # Root Keys
-ROOT_KEY_IMPORT = "import"
+ROOT_KEY_COMMAND_GROUP = "command_group"
 ROOT_KEY_ENUM = "enum"
-ROOT_KEY_SCHEMA = "schema"
+ROOT_KEY_EXTENSION = "ext"
+ROOT_KEY_IMPORT = "import"
 ROOT_KEY_MODEL = "model"
+ROOT_KEY_PLUGIN = "plugin"
+ROOT_KEY_SCHEMA = "schema"
+ROOT_KEY_SPECIFICATION = "spec"
 ROOT_KEY_USECASE = "usecase"
-ROOT_KEY_EXTENSION = "ext"
 ROOT_KEY_VALIDATION = "validation"
 
 # Common Definition Field Names
+DEFINITION_FIELD_ACCEPTANCE = "acceptance"
+DEFINITION_FIELD_ACTION = "action"
 DEFINITION_FIELD_ADD = "add"
 DEFINITION_FIELD_ARGUMENTS = "arguments"
 DEFINITION_FIELD_BEHAVIOR = "behavior"
+DEFINITION_FIELD_COMMANDS = "commands"
+DEFINITION_FIELD_COMPONENTS = "components"
+DEFINITION_FIELD_DEFINITION_SOURCES = "definitionSources"
+DEFINITION_FIELD_DEFINITION_VALIDATIONS = "definitionValidations"
 DEFINITION_FIELD_DESCRIPTION = "description"
+DEFINITION_FIELD_DISPLAY = "display"
 DEFINITION_FIELD_EXTENSION_ENUM = "enumExt"
 DEFINITION_FIELD_EXTENSION_SCHEMA = "schemaExt"
 DEFINITION_FIELD_FIELDS = "fields"
+DEFINITION_FIELD_FILES = "files"
+DEFINITION_FIELD_GIVEN = "given"
+DEFINITION_FIELD_GROUP = "group"
+DEFINITION_FIELD_HELP_TEXT = "helpText"
+DEFINITION_FIELD_IMPORT = "import"
 DEFINITION_FIELD_INHERITS = "inherits"
+DEFINITION_FIELD_INPUT = "input"
 DEFINITION_FIELD_NAME = "name"
+DEFINITION_FIELD_OUTPUT = "output"
+DEFINITION_FIELD_PARTICIPANTS = "participants"
+DEFINITION_FIELD_PRIMITIVE_VALIDATIONS = "primitiveValidations"
 DEFINITION_FIELD_REQUIRED = "required"
+DEFINITION_FIELD_SCENARIO = "scenario"
+DEFINITION_FIELD_SOURCE = "source"
+DEFINITION_FIELD_STATE = "state"
+DEFINITION_FIELD_STEP = "step"
+DEFINITION_FIELD_STEPS = "steps"
+DEFINITION_FIELD_TAGS = "tags"
+DEFINITION_FIELD_TARGET = "target"
+DEFINITION_FIELD_THEN = "then"
 DEFINITION_FIELD_TYPE = "type"
 DEFINITION_FIELD_VALIDATION = "validation"
+DEFINITION_FIELD_VALIDATIONS = "validations"
 DEFINITION_FIELD_VALUES = "values"
+DEFINITION_FIELD_WHEN = "when"
 
 # Core AaC Definition Names
-DEFINITION_NAME_PRIMITIVES = "Primitives"
-DEFINITION_NAME_ROOT = "root"
-DEFINITION_NAME_SCHEMA = "schema"
-DEFINITION_NAME_MODEL = "model"
+DEFINITION_NAME_BEHAVIOR = "Behavior"
+DEFINITION_NAME_BEHAVIOR_TYPE = "BehaviorType"
+DEFINITION_NAME_ENUM = "Enum"
+DEFINITION_NAME_EXTENSION = "Extension"
 DEFINITION_NAME_FIELD = "Field"
+DEFINITION_NAME_MODEL = "Model"
+DEFINITION_NAME_PRIMITIVES = "Primitives"
+DEFINITION_NAME_REQUIREMENT = "Requirement"
+DEFINITION_NAME_REQUIREMENT_REFERENCE = "RequirementReference"
+DEFINITION_NAME_ROOT = "Root"
+DEFINITION_NAME_SCENARIO = "Scenario"
+DEFINITION_NAME_SCHEMA = "Schema"
+DEFINITION_NAME_SPECIFICATION = "Specification"
+DEFINITION_NAME_VALIDATION = "Validation"
+DEFINITION_NAME_VALIDATION_REFERENCE = "ValidationReference"
 
 # Core AaC Primitive Types
-PRIMITIVE_TYPE_STRING = "string"
-PRIMITIVE_TYPE_INT = "int"
-PRIMITIVE_TYPE_NUMBER = "number"
 PRIMITIVE_TYPE_BOOL = "bool"
 PRIMITIVE_TYPE_DATE = "date"
+PRIMITIVE_TYPE_DIRECTORY = "directory"
 PRIMITIVE_TYPE_FILE = "file"
+PRIMITIVE_TYPE_INT = "int"
+PRIMITIVE_TYPE_NUMBER = "number"
 PRIMITIVE_TYPE_REFERENCE = "reference"
+PRIMITIVE_TYPE_STRING = "string"
+
+# Core AaC Behavior Types
+BEHAVIOR_TYPE_PUBLISH_SUBSCRIBE = "PUB_SUB"
+BEHAVIOR_TYPE_REQUEST_RESPONSE = "REQUEST_RESPONSE"
+BEHAVIOR_TYPE_STARTUP = "STARTUP"
+BEHAVIOR_TYPE_TIMER = "TIMER"
```

## aac/lang/hierarchy.py

```diff
@@ -3,57 +3,78 @@
 from typing import Optional
 
 from aac.lang.constants import (
     DEFINITION_FIELD_FIELDS,
     DEFINITION_FIELD_NAME,
     DEFINITION_FIELD_TYPE,
     DEFINITION_NAME_ROOT,
-    DEFINITION_NAME_SCHEMA,
+    ROOT_KEY_SCHEMA,
 )
 from aac.lang.language_context import LanguageContext
 from aac.lang.definitions.collections import get_definition_by_name
 from aac.lang.definitions.definition import Definition
 from aac.lang.definitions.search import search_definition
+from aac.lang.definitions.schema import get_definition_schema
 
 
 def get_definition_ancestry(definition: Definition, context: LanguageContext) -> list[Definition]:
-    """Return an ordered list of ancestor definitions starting with the root definition and ending with the argument."""
+    """
+    Return an ordered list of ancestor definitions starting with the root definition and ending with the argument.
+
+    This function traverses the list of the definition's schema definitions all the way back to `Schema`. For instance,
+    if you passed a `model` root key definition to this function, it would return itself, the `Model` definition, and
+    the `Schema` definition. This is because a definition with the `model` root key is defined by the schema `Model` definition
+    which is in turn defined by the `Schema` definition.
+
+    Args:
+        definition (Definition): The definition to search for ancestors of.
+        context (LanguageContext): The language context containing the definition's schema.
+
+    Returns:
+        A list of definitions that define the schema and the schema's parent schemas.
+    """
 
     ancestors_list = []
-    found_self_defined_ancestor = False
-    ancestor_definition: Optional[Definition] = definition
 
-    # If the definition key isn't defined, return the schema definition as the only ancestor.
+    # If the definition key isn't defined, return an empty ancestor list.
     if definition.get_root_key() not in context.get_root_keys():
-        ancestors_list.append(get_root_definition_by_key(DEFINITION_NAME_SCHEMA, context.definitions))
-        found_self_defined_ancestor = True
+        ancestors_list.append(get_root_definition_by_key(ROOT_KEY_SCHEMA, context.definitions))
+        logging.error(f"The definition '{definition.name}' does not have a defined root key '{definition.get_root_key()}'.")
+    else:
+        found_self_defined_ancestor = False
+        ancestor_definition: Optional[Definition] = definition
 
-    # Loop until we get to the root definition defining itself.
-    while not found_self_defined_ancestor and ancestor_definition:
-        found_self_defined_ancestor = ancestor_definition.name == ancestor_definition.get_root_key()
-        ancestors_list.append(ancestor_definition)
-        ancestor_definition = get_root_definition_by_key(ancestor_definition.get_root_key(), context.definitions)
+        # Loop until we get to `Schema` defining itself.
+        while not found_self_defined_ancestor and ancestor_definition:
+            ancestor_root_schema = get_definition_schema(ancestor_definition, context)
+            found_self_defined_ancestor = ancestor_definition == ancestor_root_schema
+            ancestors_list.append(ancestor_definition)
+            ancestor_definition = get_root_definition_by_key(ancestor_definition.get_root_key(), context.definitions)
 
     ancestors_list.reverse()
     return ancestors_list
 
 
-def get_root_definition_by_key(root_key: str, parsed_definitions: list[Definition]) -> Optional[Definition]:
+def get_root_definition_by_key(root_key: str, definitions: list[Definition]) -> Optional[Definition]:
     """
-    Return the parsed definition that defines a root key structure or None if not found.
+    Return the definition that defines the structure of the root key.
+
+    This function is useful for looking up the schema definition that defines a root key. For instance, if you
+    passed the root key 'model' and the definitions list contains the Root and Model definitions, then this
+    function will return the Model definition.
 
     Args:
-        root_key (str): The root key from a Definition
-        parsed_definitions (list[Definition]): A list of definitions to search, must include the root Definition.
+        root_key (str): The root key to search for
+        definitions (list[Definition]): A list of definitions to search, must include the root Definition.
 
     Return:
-        An optional Definition that defines the structure of the root key.
+        A Definition that defines the structure of the root key, or None if not found.
     """
-    root_definition = get_definition_by_name(DEFINITION_NAME_ROOT, parsed_definitions)
-    root_fields = search_definition(root_definition, [DEFINITION_NAME_SCHEMA, DEFINITION_FIELD_FIELDS])
+    root_definition = get_definition_by_name(DEFINITION_NAME_ROOT, definitions)
+    root_fields = search_definition(root_definition, [ROOT_KEY_SCHEMA, DEFINITION_FIELD_FIELDS])
 
     root_key_fields = list(filter(lambda field: (field.get(DEFINITION_FIELD_NAME) == root_key), root_fields))
     root_key_count = len(root_key_fields)
 
     root_key_field = None
     if root_key_count < 1:
         logging.error(f"Failed to find field based on root key.\nField name: {root_key}\nAvailable Fields:{root_fields}")
@@ -61,8 +82,8 @@
         root_key_field = root_key_fields[0]
 
         if root_key_count > 1:
             logging.error(
                 f"Found multiple fields when only expected to find one.\nField name: {root_key}\nReturned Fields:{root_key_fields}"
             )
 
-        return get_definition_by_name(root_key_field.get(DEFINITION_FIELD_TYPE), parsed_definitions)
+        return get_definition_by_name(root_key_field.get(DEFINITION_FIELD_TYPE), definitions)
```

## aac/lang/language_context.py

```diff
@@ -9,14 +9,15 @@
 from typing import Optional
 from uuid import UUID
 
 from aac import __version__
 from aac.cli.aac_command import AacCommand
 from aac.io.files.aac_file import AaCFile
 from aac.io.parser import parse
+from aac.io.parser._parser_error import ParserError
 from aac.io.paths import sanitize_filesystem_path
 from aac.io.writer import write_file, write_definitions_to_file
 from aac.lang.constants import (
     DEFINITION_FIELD_NAME,
     DEFINITION_NAME_PRIMITIVES,
     DEFINITION_NAME_ROOT,
     ROOT_KEY_ENUM,
@@ -30,14 +31,17 @@
 from aac.lang.language_error import LanguageError
 from aac.persistence.state_file_error import StateFileError
 from aac.plugins.contributions.contribution_points import DefinitionValidationContribution, PrimitiveValidationContribution
 from aac.plugins.plugin import Plugin
 from aac.plugins.plugin_manager import get_plugins
 
 
+MISSING_TYPE = "missing_type"
+
+
 @attrs(slots=True, auto_attribs=True)
 class LanguageContext:
     """
     A management and utility class for the contextual AaC domain-specific language.
 
     Because the AaC DSL is self-defining, self-validating, and highly extensible, the DSL
     structure and rules are highly dependent on contextual definition sources such as active
@@ -58,15 +62,15 @@
     # Private attribute - don't reference outside of this class.
     definitions_dictionary: dict[UUID, Definition] = attrib(
         init=False, default=Factory(dict), validator=validators.instance_of(dict)
     )
 
     # Definition Methods
 
-    def add_definition_to_context(self, definition: Definition):
+    def add_definition_to_context(self, definition: Definition) -> None:
         """
         Add the Definition to the list of definitions in the LanguageContext.
 
         Args:
             definition: The Definition to add to the context.
         """
         new_definition = definition.copy()
@@ -77,39 +81,31 @@
             self.definitions.append(new_definition)
         else:
             logging.debug(
                 f"Did not add definition '{new_definition.name}' to the context because one already exists with the same name."
             )
 
         if definition.get_inherits():
-            # This import is located here because the inheritance module uses the language context for lookup, causing a circular dependency at initialization
+            # This import is located here because the inheritance module uses the language context for lookup,
+            #   causing a circular dependency at initialization
             from aac.lang.definitions.inheritance import apply_inherited_attributes_to_definition
 
             apply_inherited_attributes_to_definition(new_definition, self)
 
         if definition.is_extension():
-            target_definition_name = definition.get_type()
+            target_definition_name = definition.get_type() or MISSING_TYPE
             target_definition = self.get_definition_by_name(target_definition_name)
 
             if target_definition:
-                definitions_with_target_definition_name = [
-                    definition for definition in self.definitions if target_definition.name == definition.name
-                ]
-
-                if len(definitions_with_target_definition_name) > 1:
-                    raise LanguageError(
-                        f"Duplicate target definitions found ({len(definitions_with_target_definition_name)}) with name '{target_definition_name}'."
-                    )
-
                 apply_extension_to_definition(new_definition, target_definition)
 
             else:
-                logging.error(f"Failed to find the target defintion '{target_definition_name}' in the context.")
+                logging.error(f"Failed to find the target definition '{target_definition_name}' in the context.")
 
-    def add_definitions_to_context(self, definitions: list[Definition]):
+    def add_definitions_to_context(self, definitions: list[Definition]) -> None:
         """
         Add the list of Definitions to the list of definitions in the LanguageContext, any extensions are added last.
 
         Args:
             definitions: The list of Definitions to add to the context.
         """
 
@@ -117,15 +113,15 @@
             """This is a simple attempt to resolve dependencies between definitions with inheritance. This is a temporary inadequacy."""
             sorted_definitions: dict[str, Definition] = OrderedDict()
 
             for definition in definitions:
                 sorted_definitions[definition.name] = definition
 
             for definition in definitions:
-                inherited_definition_names = definition.get_inherits()
+                inherited_definition_names = definition.get_inherits() or []
                 for inherited_definition_name in inherited_definition_names:
                     if inherited_definition_name in sorted_definitions:
                         sorted_definitions.move_to_end(definition.name)
 
             return list(sorted_definitions.values())
 
         extension_definitions = get_definitions_by_root_key(ROOT_KEY_EXTENSION, definitions)
@@ -135,65 +131,65 @@
         child_definitions = [definition for definition in schema_definitions if definition.get_inherits() is not None]
         sorted_child_definitions = simple_dependency_sort_for_definitions_with_inheritance(child_definitions)
         child_definition_names = [definition.name for definition in child_definitions]
         secondary_definitions = child_definition_names + extension_definition_names
 
         initial_definitions = [definition for definition in definitions if definition.name not in secondary_definitions]
 
-        for definition in initial_definitions:
-            self.add_definition_to_context(definition)
+        all_definitions = [*initial_definitions, *sorted_child_definitions, *extension_definitions]
 
-        for definition in sorted_child_definitions:
+        for definition in all_definitions:
             self.add_definition_to_context(definition)
 
-        for extension_definition in extension_definitions:
-            self.add_definition_to_context(extension_definition)
-
-    def add_definitions_from_uri(self, uri: str, names: list[str]):
+    def add_definitions_from_uri(self, uri: str, names: Optional[list[str]] = None) -> None:
         """
         Load the definitions from the provided file URI.
 
         Args:
             uri (str): The file URI from which to load definitions.
             names (list[str]): The list of the names of the definitions that should be loaded into
-                the context.
+                the context. If names is not provided, import all definitions. (default: None)
         """
         if lexists(uri):
-            definitions = [definition for definition in parse(uri) if definition.name in names]
-            self.update_definitions_in_context(list(set(self.definitions).intersection(definitions)))
-            self.add_definitions_to_context(list(set(definitions).difference(self.definitions)))
+            try:
+                definitions = [definition for definition in parse(uri) if not names or definition.name in names]
+            except ParserError as error:
+                raise ParserError(error.source, error.errors) from None
+            else:
+                self.update_definitions_in_context(list(set(definitions).intersection(self.definitions)))
+                self.add_definitions_to_context(list(set(definitions).difference(self.definitions)))
         else:
             logging.warn(f"Skipping {uri} as it could not be found.")
 
-    def remove_definition_from_context(self, definition: Definition):
+    def remove_definition_from_context(self, definition: Definition) -> None:
         """
         Remove the Definition from the list of definitions in the LanguageContext.
 
         Args:
             definition (Definition): The Definition to remove from the context.
         """
-        if definition.uid in self.definitions_dictionary:
+        if definition.uid in self.definitions_dictionary and self._is_definition_editable(definition):
             definition.source.is_loaded_in_context = False
             self.definitions_dictionary.pop(definition.uid)
             self.definitions.remove(definition)
         else:
             definitions_in_context = self.get_defined_types()
             logging.error(
                 f"Definition not present in context, can't be removed. '{definition.name}' not in '{definitions_in_context}'"
             )
 
         if definition.is_extension():
-            target_definition_name = definition.get_type()
+            target_definition_name = definition.get_type() or MISSING_TYPE
             target_definition = self.get_definition_by_name(target_definition_name)
             if target_definition:
                 remove_extension_from_definition(definition, target_definition)
             else:
-                logging.error(f"Failed to find the target defintion '{target_definition_name}' in the context.")
+                logging.error(f"Failed to find the target definition '{target_definition_name}' in the context.")
 
-    def remove_definitions_from_context(self, definitions: list[Definition]):
+    def remove_definitions_from_context(self, definitions: list[Definition]) -> None:
         """
         Remove the list of Definitions from the list of definitions in the LanguageContext, any extensions are removed last.
 
         Args:
             definitions (list[Definition]): The list of Definitions to remove from the context.
         """
         extension_definitions = get_definitions_by_root_key(ROOT_KEY_EXTENSION, definitions)
@@ -205,32 +201,34 @@
         for definition in non_extension_definitions:
             if definition not in extension_definitions:
                 self.remove_definition_from_context(definition)
 
         for extension_definition in extension_definitions:
             self.remove_definition_from_context(extension_definition)
 
-    def update_definition_in_context(self, definition: Definition):
+    def update_definition_in_context(self, definition: Definition) -> None:
         """
         Update the Definition in the list of definitions in the LanguageContext, if it exists.
 
         Args:
             definition (Definition): The Definition to update in the context.
         """
-        old_definition = self.definitions_dictionary.get(definition.uid)
-        if old_definition:
+
+        if definition.uid in self.definitions_dictionary:
+            old_definition = self.definitions_dictionary.get(definition.uid)
+
             self.remove_definition_from_context(old_definition)
             self.add_definition_to_context(definition)
-        else:
+        elif definition.uid not in self.definitions_dictionary:
             definitions_in_context = self.get_defined_types()
             missing_target_definition = f"Definition not present in context, can't be updated. '{definition.name}' with uid '{definition.uid}' not present in '{definitions_in_context}'"
             logging.error(missing_target_definition)
             raise LanguageError(missing_target_definition)
 
-    def update_definitions_in_context(self, definitions: list[Definition]):
+    def update_definitions_in_context(self, definitions: list[Definition]) -> None:
         """
         Update the list of Definitions in the list of definitions in the LanguageContext, any extensions are added last.
 
         Args:
             definitions (list[Definition]): The list of Definitions to update in the context.
         """
         extension_definitions = get_definitions_by_root_key(ROOT_KEY_EXTENSION, definitions)
@@ -255,27 +253,34 @@
         Returns:
             A list of strings, one entry for each root key in the LanguageContext.
 
             These keys may differ from those provided by the core spec since the LanguageContext applies definitions
             from active plugins and user files, which may extend the set of root keys.
             See :py:func:`aac.spec.get_root_keys()` for the list of root keys provided by the unaltered core AaC DSL.
         """
-        return [field.get(DEFINITION_FIELD_NAME) for field in self.get_root_fields()]
+        return [str(field.get(DEFINITION_FIELD_NAME)) for field in self.get_root_fields()]
 
     def get_root_fields(self) -> list[dict]:
         """
         Get the list of root fields as defined in the LanguageContext.
 
         Returns:
             A list of dictionaries, one dictionary for each root field including name and type.
 
             These fields may differ from those provided by the core spec since the LanguageContext applies definitions
             from active plugins and user files, which may extend the set of root fields.
         """
-        return self.get_definition_by_name(DEFINITION_NAME_ROOT).get_fields()
+        root_definition = self.get_definition_by_name(DEFINITION_NAME_ROOT)
+
+        if root_definition:
+            return root_definition.get_fields() or []
+        else:
+            raise LanguageError(
+                f"Unable to get the '{DEFINITION_NAME_ROOT}' definition. Check that AaC has the core-spec loaded."
+            )
 
     def get_root_keys_definition(self) -> Definition:
         """
         Return the root keys type definition in the LanguageContext.
 
         Returns:
             The definition that defines the root key types.
@@ -320,15 +325,15 @@
         Returns:
             A list of strings, one entry for each primitive type defined in the LanguageContext.
 
             These types may differ from those provided by the core spec since the LanguageContext applies definitions
             from active plugins and user files, which may extend the set of root keys.
             See :py:func:`aac.spec.get_primitives()` for the list of root keys provided by the unaltered core AaC DSL.
         """
-        return self.get_primitives_definition().get_values()
+        return deepcopy(self.get_primitives_definition().get_values()) or []
 
     def get_defined_types(self) -> list[str]:
         """
         Return a list of strings containing the names of all the definitions in the LanguageContext.
 
         Returns:
             A list of strings, one entry for each definition name available in the LanguageContext.
@@ -396,15 +401,17 @@
             if len(definition_to_return) > 0:
                 if len(definition_to_return) > 1:
                     logging.info(
                         f"Multiple definitions found with the same name '{definition_name}' found in context. Returning the first one."
                     )
                 return definition_to_return[0]
             else:
-                logging.info(f"Failed to find the definition named '{definition_name}' in the context.")
+                logging.info(
+                    f"Failed to find the definition named '{definition_name}' in the context of '{self.get_defined_types()}'."
+                )
         else:
             logging.error(f"No definition name was provided to {self.get_definition_by_name.__name__}")
 
     def get_definition_by_uid(self, uid: UUID) -> Optional[Definition]:
         """
         Return the definition with the corresponding uid, or None if not found.
 
@@ -579,15 +586,19 @@
         """
         sanitized_file_uri = sanitize_filesystem_path(file_uri)
         definitions_in_file = self.get_definitions_by_file_uri(sanitized_file_uri)
 
         if len(definitions_in_file) > 0:
             write_definitions_to_file(definitions_in_file, sanitized_file_uri)
             self.remove_definitions_from_context(definitions_in_file)
-            self.add_definitions_to_context(parse(sanitized_file_uri))
+            try:
+                self.add_definitions_to_context(parse(sanitized_file_uri))
+            except ParserError as error:
+                raise ParserError(error.source, error.errors) from None
+
         elif lexists(sanitized_file_uri):
             logging.info(f"Deleting {sanitized_file_uri} since there are no definitions for the file in the context.")
             remove(sanitized_file_uri)
 
     def get_file_in_context_by_uri(self, uri: str) -> Optional[AaCFile]:
         """
         Return the AaCFile object by uri from the context or None if the file isn't in the context.
@@ -608,63 +619,78 @@
 
         Args:
             file_uri (str): The source file URI to filter on.
 
         Returns:
             A list of definitions belonging to the target file.
         """
-        return [definition for definition in self.definitions if file_uri == definition.source.uri]
+        return [definition for definition in self.definitions if str(file_uri) == str(definition.source.uri)]
 
     def import_from_file(self, file_uri: str) -> None:
         """
         Load the language context from filename.
 
         Args:
             file_uri (str): The name of the file from which to load the language context.
         """
 
         def decode_state_file():
             with open(file_uri) as state_file:
                 object = json.loads(state_file.read()) or {}
-                return (
-                    object.get("aac_version"),
-                    object.get("files"),
-                    object.get("definitions"),
-                    object.get("plugins"),
-                )
+                return object.get("aac_version"), object.get("plugins")
 
         if lexists(file_uri):
-            version, files, definitions, plugins = decode_state_file()
+            version, plugins = decode_state_file()
 
             if version != __version__:
                 raise StateFileError(
                     f"Version mismatch: State file written using version {version}; current AaC version {__version__}"
                 )
 
-            for file in files:
-                self.add_definitions_from_uri(sanitize_filesystem_path(file), definitions)
+            # Make sure to clear the state of the context before importing a state file.
+            self.clear()
 
             for plugin in plugins:
                 self.activate_plugin_by_name(plugin)
 
             self.is_initialized = True
+        else:
+            self.is_initialized = False
+            logging.warning(f"The file {file_uri} could not be imported to initialize the active context.")
 
     def export_to_file(self, file_uri: str) -> None:
         """
         Write the language context to disk.
 
         Args:
             file_uri (str): The name of the file in which to store the language context.
         """
         data = dict(
             aac_version=__version__,
-            files=[file.uri for file in self.get_files_in_context()],
-            definitions=self.get_defined_types(),
             plugins=[plugin.name for plugin in self.get_active_plugins()],
         )
         write_file(file_uri, json.dumps(data, indent=2), True)
 
     # Misc Helper Functions
 
-    def copy(self) -> 'LanguageContext':
+    def copy(self) -> "LanguageContext":
         """Return a deep copy of the context."""
         return deepcopy(self)
+
+    def clear(self) -> None:
+        """Remove all definitions and plugins from the language context."""
+        self.is_initialized = False
+        self.plugins = []
+
+    # Private methods
+
+    def _is_definition_editable(self, definition: Definition) -> bool:
+        """Returns true if the definition can be edited, otherwise false. No source also returns false."""
+        is_editable = False
+        if definition.source:
+            is_editable = definition.source.is_user_editable
+        else:
+            logging.error(
+                f"Definition '{definition.name}' was not modified, because its source '{definition.source.uri or 'no-source'}' is not editable."
+            )
+
+        return is_editable
```

## aac/lang/definitions/definition.py

```diff
@@ -3,95 +3,116 @@
 
 import copy
 import logging
 import yaml
 
 from attr import Factory, attrib, attrs, validators
 from typing import Any, Optional
-from uuid import UUID, uuid4
+from uuid import UUID, uuid5, NAMESPACE_DNS
 
 from aac.io.files.aac_file import AaCFile
 from aac.lang.constants import (
     DEFINITION_FIELD_DESCRIPTION,
     DEFINITION_FIELD_EXTENSION_ENUM,
     DEFINITION_FIELD_EXTENSION_SCHEMA,
     DEFINITION_FIELD_FIELDS,
+    DEFINITION_FIELD_FILES,
+    ROOT_KEY_IMPORT,
     DEFINITION_FIELD_INHERITS,
     DEFINITION_FIELD_TYPE,
     DEFINITION_FIELD_VALIDATION,
     DEFINITION_FIELD_VALUES,
     ROOT_KEY_ENUM,
     ROOT_KEY_EXTENSION,
     ROOT_KEY_SCHEMA,
 )
+
 from aac.lang.definitions.lexeme import Lexeme
+from aac.lang.definitions.structural_node import StructuralNode
 
 
-@attrs(hash=False)
+@attrs(hash=False, eq=False)
 class Definition:
     """An Architecture-as-Code definition.
 
     Attributes:
         uid (UUID): A unique identifier for selecting the specific definition.
         name (str): The name of the definition
         content (str): The original source textual representation of the definition.
         source (AaCFile): The source document containing the definition.
         lexemes (list[Lexeme]): A list of lexemes for each item in the parsed definition.
         structure (dict): The dictionary representation of the definition.
+        meta_structure (Optional[StructuralNode]): The node-based representation of the definition's structure and collated metadata
     """
 
     uid: UUID = attrib(init=False, validator=validators.instance_of(UUID))
     name: str = attrib(validator=validators.instance_of(str))
     content: str = attrib(validator=validators.instance_of(str))
     source: AaCFile = attrib(validator=validators.instance_of(AaCFile))
     lexemes: list[Lexeme] = attrib(default=Factory(list), validator=validators.instance_of(list))
     structure: dict = attrib(default=Factory(dict), validator=validators.instance_of(dict))
+    meta_structure: Optional[StructuralNode] = attrib(
+        default=None, validator=validators.optional(validators.instance_of(StructuralNode))
+    )
 
     def __attrs_post_init__(self):
         """Post-init hook."""
-        self.uid = uuid4()
+        self.uid = uuid5(NAMESPACE_DNS, str(self.__hash__()))
+        if self.is_import():
+            self.name = str(self.uid)
 
     def __hash__(self) -> int:
         """Return the hash of this Definition."""
         return hash(self.name)
 
+    def __eq__(self, obj):
+        """Equals function for the Definition."""
+
+        def is_equal() -> bool:
+            equal = self.name == obj.name
+            equal = equal and self.structure == obj.structure
+            return equal
+
+        return isinstance(obj, Definition) and is_equal()
+
     def get_root_key(self) -> str:
         """Return the root key for the parsed definition."""
         return list(self.structure.keys())[0]
 
     # Get Field Functions
 
     def get_top_level_fields(self) -> dict[str, dict]:
         """
         Return a dictionary of the top-level fields that are populated in the definition where the key is the field name.
 
         Schema/data definitions will return their top-level fields, including a "fields" field. Because schema/data
-        is self-defining, it may be easy to confuse the intention of this function and assume that it will returns the
+        is self-defining, it may be easy to confuse the intention of this function and assume that it returns the
         entries in a schema/data definition's `fields` field, which is not the case.
 
         The resulting structure is not a copy, but a reference to the Definition's underlying structure. Editing this
         data structure will alter the fields in the Definition.
         """
-        fields = self.structure.get(self.get_root_key())
+        fields = self.structure.get(self.get_root_key(), {})
 
         if not fields:
             logging.debug(f"Failed to find any fields defined in the definition. Definition:\n{self.structure}")
-            fields = {}
 
         return fields
 
     def get_description(self) -> Optional[str]:
         """Return the description for the current definition, or None if it isn't defined."""
         fields = self.get_top_level_fields()
-        return fields.get(DEFINITION_FIELD_DESCRIPTION)
+        description = fields.get(DEFINITION_FIELD_DESCRIPTION)
+        return str(description) if description else None
 
     def get_type(self) -> Optional[str]:
         """Return the string for the extension type field, or None if the field isn't defined."""
         fields = self.get_top_level_fields()
-        return fields.get(DEFINITION_FIELD_TYPE)
+        type_field = fields.get(DEFINITION_FIELD_TYPE)
+        return str(type_field) if type_field else None
 
     def get_validations(self) -> Optional[list[dict]]:
         """Return a list of validation entry dictionaries, or None if the field isn't defined."""
         fields = self.get_top_level_fields()
         return fields.get(DEFINITION_FIELD_VALIDATION)
 
     def get_inherits(self) -> Optional[list[str]]:
@@ -105,52 +126,65 @@
         return fields.get(DEFINITION_FIELD_VALUES)
 
     def get_fields(self) -> Optional[list[dict]]:
         """Return a list of field dictionaries, or None if there are no fields defined."""
         fields = self.get_top_level_fields()
         return fields.get(DEFINITION_FIELD_FIELDS)
 
+    def get_imports(self) -> Optional[list[str]]:
+        """Return a list of imported files, or None if the definition is not import."""
+        imports = self.get_top_level_fields()
+        return imports.get(DEFINITION_FIELD_FILES)
+
     # Type Test Functions
 
     def is_extension(self) -> bool:
-        """Returns true if the definition is an extension definition."""
+        """Return true if the definition is an extension definition."""
         return self.get_root_key() == ROOT_KEY_EXTENSION
 
     def is_schema_extension(self) -> bool:
-        """Returns true if the definition is a schema extension definition."""
+        """Return true if the definition is a schema extension definition."""
         definition = self.get_top_level_fields()
         return DEFINITION_FIELD_EXTENSION_SCHEMA in definition and isinstance(
             definition[DEFINITION_FIELD_EXTENSION_SCHEMA], dict
         )
 
     def is_enum_extension(self) -> bool:
-        """Returns true if the definition is an enum extension definition."""
+        """Return true if the definition is an enum extension definition."""
         definition = self.get_top_level_fields()
         return DEFINITION_FIELD_EXTENSION_ENUM in definition and isinstance(definition[DEFINITION_FIELD_EXTENSION_ENUM], dict)
 
     def is_schema(self) -> bool:
-        """Returns true if the definition is a schema definition."""
+        """Return true if the definition is a schema definition."""
         return self.get_root_key() == ROOT_KEY_SCHEMA
 
     def is_enum(self) -> bool:
-        """Returns true if the definition is an enum definition."""
+        """Return true if the definition is an enum definition."""
         return self.get_root_key() == ROOT_KEY_ENUM
 
+    def is_import(self) -> bool:
+        """Return True if the definition is an import definition."""
+        return self.get_root_key() == ROOT_KEY_IMPORT
+
     # IO Functions
 
     def to_yaml(self) -> str:
         """Return a yaml string based on the current state of the definition including extensions."""
         return yaml.dump(self.structure, sort_keys=False)
 
     # Misc Functions
 
     def copy(self) -> Definition:
         """Return a deep copy of the definition."""
         return copy.deepcopy(self)
 
+    def get_source_file(self) -> AaCFile:
+        """Returns the AaCFile the definition can be found in."""
+        return self.source
+
     def get_lexeme_with_value(
         self,
         search_value: Any,
         prefix_values: Optional[list[Any]] = None,
         suffix_values: Optional[list[Any]] = None,
     ) -> Optional[Lexeme]:
         """
```

## aac/lang/definitions/extensions.py

```diff
@@ -1,10 +1,20 @@
 """Module for handling Definitions and Extensions."""
 
 import logging
+from aac.lang.constants import (
+    DEFINITION_FIELD_ADD,
+    DEFINITION_FIELD_ARGUMENTS,
+    DEFINITION_FIELD_EXTENSION_ENUM,
+    DEFINITION_FIELD_EXTENSION_SCHEMA,
+    DEFINITION_FIELD_FIELDS,
+    DEFINITION_FIELD_NAME,
+    DEFINITION_FIELD_VALIDATION,
+    DEFINITION_FIELD_VALUES,
+)
 
 from aac.lang.definitions.definition import Definition
 from aac.lang.language_error import LanguageError
 
 
 def apply_extension_to_definition(extension_definition: Definition, target_definition: Definition) -> None:
     """
@@ -21,31 +31,31 @@
     extension_additional_content = _get_extension_additional_content_dict(extension_definition)
     extension_field_name = _get_extension_field_name(extension_definition)
 
     original_field_values = target_definition_fields_dict.get(extension_field_name)
     if original_field_values is not None:
         updated_values = []
 
-        if extension_additional_content is not None and "add" in extension_additional_content:
-            new_values = extension_additional_content.get("add") or []
+        if extension_additional_content is not None and DEFINITION_FIELD_ADD in extension_additional_content:
+            new_values = extension_additional_content.get(DEFINITION_FIELD_ADD) or []
             if extension_definition.is_enum_extension():
                 updated_values = _combine_enum_values(original_field_values, new_values)
             else:
                 updated_values = _combine_schema_fields(original_field_values, new_values)
 
             target_definition_fields_dict[extension_field_name] = updated_values
             _add_extension_required_fields_to_definition(target_definition_fields_dict, extension_additional_content)
 
         else:
-            missing_ext_content_message = f"Error when attempting to applying extension '{extension_definition.name}'. The extension is missing the appropriate extension content field '{target_definition.get_root_key()}Ext'"
+            missing_ext_content_message = f"Error when attempting to apply extension '{extension_definition.name}'. The extension is missing the appropriate extension content field '{target_definition.get_root_key()}Ext'"
             logging.error(missing_ext_content_message)
             raise LanguageError(missing_ext_content_message)
 
     else:
-        extension_type = "enum" if extension_definition.is_enum_extension() else "schema"
+        extension_type = get_extension_definition_type(extension_definition)
         incorrect_target_error_message = f"Attempted to apply the extension '{extension_definition.name}' ({extension_type}) to an incompatible target definition '{target_definition.name}' ({target_definition.get_root_key()})"
         logging.error(incorrect_target_error_message)
 
 
 def remove_extension_from_definition(extension_definition: Definition, target_definition: Definition) -> None:
     """
     Remove the extension from the definition it modifies.
@@ -56,116 +66,160 @@
 
     Raises:
         LanguageError: Raised when there is an unrecoverable internal error when removing an extension
     """
     target_definition_fields = target_definition.get_top_level_fields()
     extension_additional_content = _get_extension_additional_content_dict(extension_definition)
     extension_field_name = _get_extension_field_name(extension_definition)
+    extension_target_field = target_definition_fields.get(extension_field_name)
 
-    if target_definition_fields.get(extension_field_name):
-        elements_to_remove = extension_additional_content.get("add")
+    if extension_target_field:
+        elements_to_remove = extension_additional_content.get(DEFINITION_FIELD_ADD)
         if not isinstance(elements_to_remove, list):
             elements_to_remove = [elements_to_remove]
 
         for element_to_remove in elements_to_remove:
-            target_definition_fields[extension_field_name].remove(element_to_remove)
+
+            if extension_definition.is_schema_extension():
+                field_name_to_remove = element_to_remove.get(DEFINITION_FIELD_NAME, "")
+                _remove_schema_extension_from_fields(field_name_to_remove, extension_target_field)
+            elif extension_definition.is_enum_extension():
+                _remove_enum_extension_from_values(element_to_remove, extension_target_field)
+            else:
+                logging.error(
+                    f"Unrecognized extension type found in '{extension_definition}'. Valid types are '{DEFINITION_FIELD_EXTENSION_ENUM}' and '{DEFINITION_FIELD_EXTENSION_SCHEMA}'"
+                )
     else:
         missing_target_error_message = f"Attempted to remove a missing extension field from the target. Extension name '{extension_definition.name}' target definition '{target_definition.name}'"
         logging.error(missing_target_error_message)
         raise LanguageError(missing_target_error_message)
 
     _remove_extension_required_fields_to_definition(target_definition_fields, extension_additional_content)
 
 
+def get_extension_definition_type(definition: Definition) -> str:
+    """Returns the extension's substructure type based on whether the extension is extending an enum or schema definition."""
+    return DEFINITION_FIELD_EXTENSION_ENUM if definition.is_enum_extension() else DEFINITION_FIELD_EXTENSION_SCHEMA
+
+
+def _remove_schema_extension_from_fields(field_name_to_remove: str, target_definition_fields: list[dict]):
+    """Specifically remove the extension's field from the target definition's fields."""
+    matching_fields = [field for field in target_definition_fields if field.get(DEFINITION_FIELD_NAME) == field_name_to_remove]
+
+    if len(matching_fields) == 0:
+        logging.error(f"Failed to find the field '{field_name_to_remove}' in the target fields '{target_definition_fields}'")
+    else:
+        matching_field, *_ = matching_fields
+        target_definition_fields.remove(matching_field)
+
+
+def _remove_enum_extension_from_values(enum_to_remove: str, target_enum_values: list[str]):
+    """Specifically remove the extension's enum value from the target definition's enum values."""
+    if enum_to_remove not in target_enum_values:
+        logging.error(f"Failed to find the enum value '{enum_to_remove}' in the target values '{target_enum_values}'")
+    else:
+        target_enum_values.remove(enum_to_remove)
+
+
 def _get_extension_additional_content_dict(extension_definition: Definition) -> dict:
     """Return the extension's additive information fields based on the extension's sub-type (enumExt/dataExt)."""
     extension_definition_fields = extension_definition.get_top_level_fields()
-    extension_type = "enum" if extension_definition.is_enum_extension() else "schema"
-    ext_type = f"{extension_type}Ext"
-    return extension_definition_fields.get(ext_type)
+    extension_type = get_extension_definition_type(extension_definition)
+    return extension_definition_fields.get(extension_type)
 
 
 def _get_extension_field_name(extension_definition: Definition) -> str:
     """Get the appropriate field name (values/fields) for the extension's additional content."""
-    return "values" if extension_definition.is_enum_extension() else "fields"
+    return DEFINITION_FIELD_VALUES if extension_definition.is_enum_extension() else DEFINITION_FIELD_FIELDS
 
 
 def _combine_enum_values(original_values: list[str], new_values: list[str]) -> list[str]:
     """Return a list of all unique original and new enum values combined together."""
     return list(set(original_values + new_values))
 
 
 def _combine_schema_fields(original_fields: list[dict], new_fields: list[dict]) -> list[dict]:
     """Return a list of all unique original and new data fields combined together."""
-    updated_fields_dict = {value.get("name"): value for value in original_fields}
-    unique_new_fields = [field for field in new_fields if field.get("name") not in updated_fields_dict.keys()]
-    new_fields_dict = {value.get("name"): value for value in unique_new_fields}
+    updated_fields_dict = {value.get(DEFINITION_FIELD_NAME): value for value in original_fields}
+    unique_new_fields = [field for field in new_fields if field.get(DEFINITION_FIELD_NAME) not in updated_fields_dict.keys()]
+    new_fields_dict = {value.get(DEFINITION_FIELD_NAME): value for value in unique_new_fields}
     updated_fields_dict.update(new_fields_dict)
     return list(updated_fields_dict.values())
 
 
 def _remove_enum_values(target_values: list, values_to_remove: list) -> list:
     """Return a list of the target values sans any of the values to remove."""
     dict_of_values_to_remove = {value: value for value in values_to_remove}
     updated_values_list = {value: value for value in target_values if value not in dict_of_values_to_remove}
     return list(updated_values_list.values())
 
 
 def _remove_schema_fields(target_fields: list, fields_to_remove: list):
     """Return a list of the target fields sans any of the fields to remove."""
-    dict_of_fields_to_remove = {field.get("name"): field for field in fields_to_remove}
-    updated_fields_list = {field.get("name"): field for field in target_fields if field.get("name") not in dict_of_fields_to_remove}
+    dict_of_fields_to_remove = {field.get(DEFINITION_FIELD_NAME): field for field in fields_to_remove}
+    updated_fields_list = {
+        field.get(DEFINITION_FIELD_NAME): field
+        for field in target_fields
+        if field.get(DEFINITION_FIELD_NAME) not in dict_of_fields_to_remove
+    }
     return list(updated_fields_list.values())
 
 
-def _add_extension_required_fields_to_definition(target_definition_fields: dict, extension_additional_content_fields: dict) -> None:
+def _add_extension_required_fields_to_definition(
+    target_definition_fields: dict, extension_additional_content_fields: dict
+) -> None:
     """Add any additional required fields from the extension to the target definition."""
     extension_required_fields = extension_additional_content_fields.get("required")
     definition_validations = _get_definition_validations(target_definition_fields)
 
     if not definition_validations:
-        target_definition_fields["validation"] = []
+        target_definition_fields[DEFINITION_FIELD_VALIDATION] = []
 
     required_fields_validation = _get_required_fields_validation_for_definition(target_definition_fields)
     if extension_required_fields:
-        target_definition_fields["validation"].append(required_fields_validation)
-        required_fields_validation["arguments"].extend(extension_required_fields)
+        target_definition_fields[DEFINITION_FIELD_VALIDATION].append(required_fields_validation)
+        required_fields_validation[DEFINITION_FIELD_ARGUMENTS].extend(extension_required_fields)
 
 
-def _remove_extension_required_fields_to_definition(target_definition_fields: dict, extension_additional_content_fields: dict) -> None:
+def _remove_extension_required_fields_to_definition(
+    target_definition_fields: dict, extension_additional_content_fields: dict
+) -> None:
     """Remove the extension's required fields from the target definition's required fields."""
     target_required_fields = []
     definition_validations = _get_definition_validations(target_definition_fields)
     extension_required_fields = extension_additional_content_fields.get("required") or []
 
     if definition_validations:
         required_fields_validation = _get_required_fields_validation_for_definition(target_definition_fields)
-        target_required_fields = required_fields_validation.get("arguments")
+        target_required_fields = required_fields_validation.get(DEFINITION_FIELD_ARGUMENTS)
 
     for required_field in extension_required_fields:
         if required_field in target_required_fields:
             target_required_fields.remove(required_field)
         else:
             logging.error(
                 f"Extension-applied required field '{required_field}' is not present in target dictionary: '{target_definition_fields}'"
             )
 
 
 def _get_required_fields_validation_string() -> str:
     """Return the name of the required fields validation."""
-    from aac.plugins.validators.required_fields import PLUGIN_NAME
-    return PLUGIN_NAME
+    from aac.plugins.validators.required_fields import VALIDATION_NAME
+
+    return VALIDATION_NAME
 
 
 def _get_required_fields_validation_for_definition(definition_fields: dict) -> dict:
     """Return the required fields validation on the specified definition."""
     definition_validations = _get_definition_validations(definition_fields)
     required_fields_validation_name = _get_required_fields_validation_string()
-    required_fields_validation = [v for v in definition_validations if v.get("name") == required_fields_validation_name]
-    empty_required_fields_validation = {"name": required_fields_validation_name, "arguments": []}
+    required_fields_validation = [
+        v for v in definition_validations if v.get(DEFINITION_FIELD_NAME) == required_fields_validation_name
+    ]
+    empty_required_fields_validation = {DEFINITION_FIELD_NAME: required_fields_validation_name, DEFINITION_FIELD_ARGUMENTS: []}
 
     return required_fields_validation[0] if required_fields_validation else empty_required_fields_validation
 
 
 def _get_definition_validations(definition_fields: dict) -> list[dict]:
     """Return the list of validation definitions for the specified definition."""
     return definition_fields.get("validation") or []
```

## aac/lang/definitions/references.py

```diff
@@ -58,104 +58,100 @@
         if enum_reference.name in root_definitions_type_to_key_dict.keys():
             instances_of_referencing_root_key = language_context.get_definitions_by_root_key(root_definitions_type_to_key_dict.get(enum_reference.name))
             definitions_referencing_enum_value.extend(instances_of_referencing_root_key)
 
     return definitions_referencing_enum_value
 
 
-def is_reference_format_valid(reference_field_value: str = None) -> tuple[bool, str]:
-    """Returns boolean and string tuple indicating if the reference field is properly formatted for processing."""
-    # This assumes input is not None
-    if reference_field_value is None:
-        return False, "Reference must have content"
-
-    found_invalid_segment = False
-    message = "Reference OK"
-
-    for segment in reference_field_value.split('.'):
-
-        # Rule: segment must have content
-        if len(segment) == 0:
-            message = "Failed rule: segment must have content"
-            found_invalid_segment = True
-            break
-
-        open_peren = segment.find('(')
-        close_peren = segment.find(')')
-        equals = segment.find('=')
-
-        # Rule: if there is an open peren designating a selector, there must be a corresponding close peren...and vice versa
-        if not ((open_peren < 0 and close_peren < 0) or (open_peren > 0 and close_peren > 0)):
-            message = "Failed rule: if there is an open peren designating a selector, there must be a corresponding close peren...and vice versa"
-            found_invalid_segment = True
-            break
-
-        # Rule:  if there is a selector, it must contain an equals with content on either side
-        if open_peren >= 0 and (equals < 0 or (open_peren + 1 == equals) or (equals + 1 == close_peren)):
-            message = "Failed rule: if there is a selector, it must contain an equals with content on either side"
-            found_invalid_segment = True
-            break
-
-        # break the segment into it's parts (i.e. key(selector_field=selector_value))
-        key, selector, selector_field, selector_value = _get_reference_segment_content(segment)
-
-        # Rule: there must be content before the selector
-        if len(key) == 0:
-            message = "Failed rule: there must be content before the selector"
-            found_invalid_segment = True
-            break
-
-        # Rule: names only contain allowed values
-        if _has_disallowed_characters(key) or (len(selector_field) > 0 and _has_disallowed_characters(selector_field)):
-            message = "Failed rule: names only contain allowed values"
-            found_invalid_segment = True
-            break
+def is_reference_format_valid(reference_field_value: str) -> bool:
+    """Return whether the reference field is properly formatted for processing."""
 
-    return not found_invalid_segment, message
+    def is_valid_segment(segment: str) -> bool:
+        return (
+            len(segment) > 0
+            and _has_matched_parentheses(segment)
+            and _has_selector_field_and_selector_value(segment)
+            and _refers_to_element(segment)
+            and _is_valid_name(segment)
+        )
 
+    if reference_field_value:
+        valid_segments = [is_valid_segment(segment) for segment in reference_field_value.split(".")]
+        return all(valid_segments)
 
-def _has_disallowed_characters(test_me: str) -> bool:
+    return False
+
+
+def _has_matched_parentheses(segment: str) -> bool:
+    open_paren = segment.find("(")
+    close_paren = segment.find(")")
+    return (open_paren < 0 and close_paren < 0) or (open_paren > 0 and close_paren > open_paren)
+
+
+def _has_selector_field_and_selector_value(segment: str) -> bool:
+    open_paren = segment.find("(")
+    close_paren = segment.find(")")
+    equal_sign = segment.find("=")
+    return (open_paren < 0 and close_paren < 0 and equal_sign < 0) or (
+        open_paren > 0 and equal_sign > open_paren + 1 and equal_sign < close_paren - 1
+    )
+
+
+def _refers_to_element(segment: str) -> bool:
+    element, *_ = _get_reference_segment_content(segment)
+    return len(element) > 0
+
+
+def _is_valid_name(segment: str) -> bool:
+    element, _, selector_field, _ = _get_reference_segment_content(segment)
+    return _no_disallowed_characters(element) and (_no_disallowed_characters(selector_field) if selector_field else True)
+
+
+def _no_disallowed_characters(segment: str) -> bool:
     disallowed = set("~`!@#$%^&*()=+\\|[]{}'\";:/?,.<> ")
-    return any((c in disallowed) for c in test_me)
+    return len(disallowed.intersection(segment)) == 0
 
 
 def get_reference_target_definitions(reference_field_value: str, language_context: LanguageContext) -> list[Definition]:
     """
     Return a list containing the referenced definitions.
 
+    Search the language context for target definitions which satisfy the reference.  A matching
+    definition must have all fields referenced in the selector and must contain fields which satisfy
+    any selectors defined in the reference.
+
+    It is assumed that `reference_field_value` is a properly formatted reference primitive field.
+    If it is not, an empty list will be returned.  You can test this using the
+    `is_reference_format_valid()` method prior to getting the reference target definitions if you
+    have any uncertainty.
+
     Args:
         reference_field_value (str): The definition that is being referenced
         language_context (LanguageContext): The language context to search.
-
-    Search the language context for target definitions which satisfy the reference.  A matching definition
-    must have all fields referenced in the selector and must contain fields which satisfy any selectors defined in
-    the reference.
-
-    It is assumed that the reference_field_value is a properly formatted reference primitive field.  If it is not,
-    an empty list will be returned.  You can test this using the is_reference_format_valid() method prior to getting
-    the reference target definitions if you have any uncertainty.
     """
 
     # Check that input is not None and is valid
-    if not is_reference_format_valid(reference_field_value)[0]:
+    if not is_reference_format_valid(reference_field_value):
         return []
 
     # First get the root element and optional selector
-    segments = reference_field_value.split('.')
+    segments = reference_field_value.split(".")
 
     # get the root so we can pull the right definitions from the language context
     root, _, _, _ = _get_reference_segment_content(segments[0])
 
     # recursively filter through the definitions by filtering out definitions using selectors
     keepers = _process_segment([], segments, language_context.get_definitions_by_root_key(root), language_context)
 
     return keepers
 
 
-def _process_segment(prefix: list[str], segments: list[str], definitions: list[Definition], language_context: LanguageContext) -> list[Definition]:
+def _process_segment(
+    prefix: list[str], segments: list[str], definitions: list[Definition], language_context: LanguageContext
+) -> list[Definition]:
     """This should process segments recursively."""
     if len(segments) == 0:
         # everything has been processed, so return what was found in the previous recursion
         return definitions
 
     keepers = []
     key, selector, selector_field, selector_value = _get_reference_segment_content(segments[0])
@@ -186,16 +182,17 @@
                 keepers.append(definition)
     else:
         # no root level selector, so just keep all definitions and move on
         keepers.extend(definitions)
     return keepers
 
 
-def _process_non_root(key: str, prefix: list[str], selector: str, selector_field: str, selector_value: str, definitions: list[Definition]) -> list[Definition]:
-    # initialize return value as empty string
+def _process_non_root(
+    key: str, prefix: list[str], selector: str, selector_field: str, selector_value: str, definitions: list[Definition]
+) -> list[Definition]:
     keepers = []
     for definition in definitions:
         top_level_fields = definition.get_top_level_fields()
         dict_list = _drill_into_nested_dict(prefix[1:], top_level_fields)
 
         for def_dict in dict_list:
             if key in def_dict.keys():
@@ -231,21 +228,20 @@
         elif isinstance(next_level, dict):
             items_to_return = _drill_into_nested_dict(search_keys[1:], next_level)
 
     return items_to_return
 
 
 def _get_reference_segment_content(segment: str) -> tuple:
-
     element = ""
     selector = ""
     selector_field = ""
     selector_value = ""
-    if segment.find('(') > 0:
-        element = segment.partition('(')[0]
-        selector = segment[segment.find('(') + 1:segment.find(')')]
+    if segment.find("(") > 0:
+        element = segment.partition("(")[0]
+        selector = segment[segment.find("(") + 1:segment.find(")")]
         selector_field, selector_value = selector.split("=")
-        selector_value = selector_value.strip('\"')  # remove quotes if they exist
+        selector_value = selector_value.strip('"')  # remove quotes if they exist
     else:
         element = segment
 
     return (element, selector, selector_field, selector_value)
```

## aac/lang/definitions/schema.py

```diff
@@ -1,10 +1,16 @@
 """Provide functions for dealing with definition schemas and their relationships."""
 import logging
 from typing import Optional
+from aac.lang.constants import (
+    DEFINITION_FIELD_FIELDS,
+    DEFINITION_FIELD_NAME,
+    DEFINITION_FIELD_TYPE,
+    DEFINITION_NAME_PRIMITIVES,
+)
 
 from aac.lang.language_context import LanguageContext
 from aac.lang.definitions.definition import Definition
 
 
 def get_definition_schema(source_definition: Definition, context: LanguageContext) -> Optional[Definition]:
     """Return the root definition schema for the source definition."""
@@ -12,27 +18,29 @@
         return None
 
     root_schema_definitions = get_root_schema_definitions(context)
     definition_root_key = source_definition.get_root_key()
     definition_schema = root_schema_definitions.get(definition_root_key)
 
     if not definition_schema:
-        logging.error(f"Failed to find schema definition for '{source_definition.name}' with root key: '{definition_root_key}'.")
+        logging.error(
+            f"Failed to find schema definition for '{source_definition.name}' with root key: '{definition_root_key}'."
+        )
 
     return definition_schema
 
 
 def get_root_schema_definitions(context: LanguageContext) -> dict[str, Definition]:
     """Return a dictionary of root keys to definitions."""
     root_definitions_entries = context.get_root_fields()
 
     root_definitions_dict = {}
     for root in root_definitions_entries:
-        root_name = root.get("name")
-        root_type = root.get("type")
+        root_name = root.get(DEFINITION_FIELD_NAME)
+        root_type = root.get(DEFINITION_FIELD_TYPE)
 
         # We only care about definitions, which excludes primitive types
         if context.is_definition_type(root_type):
             root_definition = context.get_definition_by_name(root_type)
 
             if not root_definition:
                 logging.error(f"Failed to find definition named '{root_type}' for root key: {root_name}.")
@@ -50,15 +58,15 @@
     schema_definition_fields = []
     if schema_definition:
         schema_definition_fields = schema_definition.get_top_level_fields()
 
         if "fields" not in schema_definition_fields:
             logging.error(f"Definition schema '{schema_definition.name}' does not specify any defined fields.")
         else:
-            schema_defined_fields = {field.get("name"): field for field in schema_definition_fields.get("fields")}
+            schema_defined_fields = _convert_fields_list_to_dict(schema_definition_fields.get(DEFINITION_FIELD_FIELDS))
 
     else:
         logging.error(f"Failed to find schema for definition key: {source_definition.get_root_key()}")
 
     return schema_defined_fields
 
 
@@ -78,24 +86,88 @@
         A list of dictionaries that match instances of the sub-definition type.
     """
     substructure_definitions = {}
 
     def _get_sub_definitions(schema_definition: Definition, fields):
 
         for field_dict in fields:
-            field_type = field_dict.get("type")
+            field_type = field_dict.get(DEFINITION_FIELD_TYPE)
 
             if not field_type:
                 logging.debug(
                     f"Failed to find the field definition for {field_type} in the defined fields {fields} of '{schema_definition.name}'."
                 )
 
             if context.is_definition_type(field_type) and field_type not in substructure_definitions:
                 field_definition = context.get_definition_by_name(field_type)
                 substructure_definitions[field_type] = field_definition
 
                 if not field_definition.is_enum():
-                    _get_sub_definitions(field_definition, field_definition.get_top_level_fields().get("fields"))
+                    _get_sub_definitions(
+                        field_definition, field_definition.get_top_level_fields().get(DEFINITION_FIELD_FIELDS)
+                    )
 
     top_level_fields = list(get_schema_defined_fields(source_definition, context).values())
     _get_sub_definitions(source_definition, top_level_fields)
     return list(substructure_definitions.values())
+
+
+def get_schema_for_field(
+    source_definition: Definition, field_keys: list[str], context: LanguageContext
+) -> Optional[Definition]:
+    """
+    Return the schema definition that defines the structure for the field specified by the keys listed in field_keys.
+
+    For example, if you wanted to know the definition for ['model','component'] you'd get 'Field' because components is an array of `Field`.
+
+    Args:
+        source_definition (Definition): The definition to search.
+        field_keys (list[str]): The list of keys used to identify the target field in the source definition.
+        context (LanguageContext): The language context, used to navigate the structure and lookup definitions.
+
+    Returns:
+        The schema that defines the field structure, the enum definition defined for an enum field, or the primitives definition for primitive fields.
+    """
+    keys_to_traverse = field_keys.copy()
+    definition_to_return = None
+
+    def _traverse_key(fields: dict) -> Optional[Definition]:
+        field_schema_definition = None
+
+        key_to_traverse = keys_to_traverse.pop(0)
+        field_to_traverse = fields.get(key_to_traverse, {})
+
+        field_type = str(field_to_traverse.get(DEFINITION_FIELD_TYPE, ""))
+
+        if field_type:
+            if context.is_definition_type(field_type):
+                field_schema_definition = context.get_definition_by_name(field_type)
+                fields_to_traverse = field_schema_definition.get_top_level_fields().get(DEFINITION_FIELD_FIELDS, {})
+                traverse_fields_dict = _convert_fields_list_to_dict(fields_to_traverse)
+
+                if len(keys_to_traverse) > 0 and field_schema_definition:
+                    field_schema_definition = _traverse_key(traverse_fields_dict)
+
+            elif context.is_primitive_type(field_type):
+                field_schema_definition = context.get_definition_by_name(DEFINITION_NAME_PRIMITIVES)
+            else:
+                # Assumed to be enum as enums and primitives are the only terminal types
+                field_schema_definition = context.get_enum_definition_by_type(field_type)
+
+        else:
+            # In the case of no field-type, we're assumed to be at a terminal value (enum or primitive value)
+            field_schema_definition = context.get_enum_definition_by_type(key_to_traverse)
+
+        return field_schema_definition
+
+    if len(keys_to_traverse) > 1:
+        keys_to_traverse.pop(0)  # Go ahead and pop the root key since we don't specifically need it.
+        definition_to_return = _traverse_key(get_schema_defined_fields(source_definition, context))
+    elif len(keys_to_traverse) > 0 and keys_to_traverse[0] == source_definition.get_root_key():
+        definition_to_return = get_definition_schema(source_definition, context)
+
+    return definition_to_return
+
+
+def _convert_fields_list_to_dict(fields: list[dict]) -> dict[str, dict]:
+    """Converts the usual list of fields into a dictionary where the field name is the key."""
+    return {field.get(DEFINITION_FIELD_NAME): field for field in fields}
```

## aac/plugins/_common.py

```diff
@@ -1,13 +1,15 @@
 """Common utilities usable by all the plugins."""
-
 from aac.io.parser import parse
+from aac.io.parser._parser_error import ParserError
 from aac.lang.definitions.definition import Definition
 from aac.package_resources import get_resource_file_contents, get_resource_file_path
 
 
 def get_plugin_definitions_from_yaml(package, filename) -> list[Definition]:
     """Return the parsed plugin definitions from the plugin definition file."""
-    return parse(
-        get_resource_file_contents(package, filename),
-        get_resource_file_path(package, filename)
-    )
+    try:
+        yaml_definitions = parse(get_resource_file_contents(package, filename), get_resource_file_path(package, filename))
+    except ParserError as error:
+        raise ParserError(error.source, error.errors) from None
+    else:
+        return yaml_definitions
```

## aac/plugins/plugin.py

```diff
@@ -1,8 +1,9 @@
 """Plugin metadata class."""
+import copy
 from attr import Factory, attrib, attrs, validators
 
 from aac.cli.aac_command import AacCommand
 from aac.lang.definitions.definition import Definition
 from aac.plugins.contributions.contribution_points import ContributionPoints
 from aac.plugins.contributions.contribution_types import DefinitionValidationContribution, PrimitiveValidationContribution
 
@@ -87,7 +88,11 @@
                 by the definition.
         """
         self.contributions.register_definitions(self.name, definitions)
 
     def get_definitions(self) -> list[Definition]:
         """Get the definitions provided by this plugin."""
         return self.contributions.get_definitions_by_plugin_name(self.name)
+
+    def copy(self) -> "Plugin":
+        """Return a deepcopy of the plugin, good for modifying the plugin without altering cached plugins."""
+        return copy.deepcopy(self)
```

## aac/plugins/plugin_manager.py

```diff
@@ -2,14 +2,19 @@
 from importlib import import_module
 from pluggy import PluginManager
 
 from aac.plugins import hookspecs, PLUGIN_PROJECT_NAME
 from aac.plugins.plugin import Plugin
 
 
+# Using an installed plugin cache for performance. This will causes issues if users try to
+#   install new plugins without restarting AaC.
+INSTALLED_PLUGINS = []
+
+
 def get_plugin_manager() -> PluginManager:
     """
     Get the plugin manager and automatically registers first-party internal plugins.
 
     Returns:
         The plugin manager.
     """
@@ -27,40 +32,42 @@
         "gen_protobuf",
         "gen_design_doc",
         "gen_gherkin_behaviors",
         "gen_plant_uml",
         "specifications",
         "print_spec",
         "lsp_server",
-        "material_model",
         "help_dump",
         "rest_api",
         "primitive_type_check",
         "plugin_management",
+        "active_context",
     ]
 
     # register "built-in" commands
     builtin_command_plugins_package = "aac.cli.builtin_commands"
     builtin_command_plugins = [
         "validate",
         "version",
     ]
 
     # register "built-in" validation plugins
     validator_plugins_package = "aac.plugins.validators"
     validator_plugins = [
         "defined_references",
-        "required_fields",
-        "validator_implementation",
         "exclusive_fields",
-        "subcomponent_type",
-        "root_keys",
         "reference_fields",
         "reference_targets",
+        "required_fields",
+        "requirement_references",
+        "root_keys",
+        "subcomponent_type",
         "unique_names",
+        "unique_requirement_ids",
+        "validator_implementation",
     ]
 
     def register_plugin(plugin, package):
         plugin_module = import_module(f"{package}.{plugin}")
         plugin_manager.register(plugin_module)
 
     [register_plugin(name, first_party_plugins_package) for name in first_party_plugins]
@@ -68,13 +75,17 @@
     [register_plugin(name, validator_plugins_package) for name in validator_plugins]
 
     return plugin_manager
 
 
 def get_plugins() -> list[Plugin]:
     """
-    Get a list of all the plugins available in the AaC package.
+    Get a list of all the system-wide plugins available to activate in the AaC package.
 
     Returns:
-        A list of plugins that are currently registered.
+        A list of plugins that are currently installed on the system.
     """
-    return get_plugin_manager().hook.get_plugin()
+    global INSTALLED_PLUGINS
+    if not INSTALLED_PLUGINS:
+        INSTALLED_PLUGINS = get_plugin_manager().hook.get_plugin()
+
+    return [plugin.copy() for plugin in INSTALLED_PLUGINS]
```

## aac/plugins/contributions/contribution_types/definition_validation_contribution.py

```diff
@@ -1,25 +1,32 @@
 """Rule Validation Contribution class."""
+
 from __future__ import annotations
+
+from typing import Callable, Optional
+
 from attr import attrib, attrs, validators
 
 from aac.lang.definitions.definition import Definition
 
 
 @attrs(hash=False)
 class DefinitionValidationContribution:
     """
-    A class that contains all the relevant information to manage and execute definition validation contributions with the validation process.
+    A contribution for validating a definition.
+
+    A class that contains all the relevant information to manage and execute definition validation
+    contributions with the validation process.
 
     Attributes:
-        name: A string with the name of the command argument
-        definition: The AaC definition of the Validator Plugin
-        validation_function: The validation callback function
+        name (str): A string with the name of the command argument.
+        definition (str): The AaC definition of the Validator Plugin.
+        validation_function (Optional[Callable]): The validation callback function.
     """
 
     name: str = attrib(validator=validators.instance_of(str))
     definition: Definition = attrib(validator=validators.instance_of(Definition))
-    validation_function: callable = attrib(validator=validators.is_callable())
+    validation_function: Optional[Callable] = attrib(validator=validators.optional(validators.is_callable()))
 
     def __hash__(self) -> int:
         """Return the hash of this DefinitionValidationContribution."""
         return hash(self.name)
```

## aac/plugins/contributions/contribution_types/primitive_validation_contribution.py

```diff
@@ -1,23 +1,30 @@
 """Type Validation Contribution class."""
+
 from __future__ import annotations
+
+from typing import Callable, Optional
+
 from attr import attrib, attrs, validators
 
 
 @attrs(hash=False)
 class PrimitiveValidationContribution:
     """
-    A class that contains all the relevant information to manage and execute type validator contributions against type-value enums in the validation process.
+    A contribution for validating a primitive value.
+
+    A class that contains all the relevant information to manage and execute type validator
+    contributions against type-value enums in the validation process.
 
     Attributes:
-        name: The name of the enum validator
-        primitive_type: The enum type
-        validation_function: The validation callback function
+        name (str): The name of the enum validator
+        primitive_type (str): The enum type
+        validation_function (Optional[Callable]): The validation callback function
     """
 
     name: str = attrib(validator=validators.instance_of(str))
     primitive_type: str = attrib(validator=validators.instance_of(str))
-    validation_function: callable = attrib(validator=validators.is_callable())
+    validation_function: Optional[Callable] = attrib(validator=validators.optional(validators.is_callable()))
 
     def __hash__(self) -> int:
         """Return the hash of this TypeValidationContribution."""
         return hash(self.name)
```

## aac/plugins/first_party/gen_design_doc/gen_design_doc.yaml

```diff
@@ -1,14 +1,14 @@
-model:
-  name: gen-design-doc
-  description: gen-design-doc is an Architecture-as-Code plugin that generates a System Design Document from Architecture-as-Code models.
-  behavior:
+plugin:
+  name: Generate System Design Document
+  description: An AaC plugin that generates a System Design Document from AaC definitions.
+  commands:
     - name: gen-design-doc
-      type: command
-      description: Generate a System Design Document from Architecture-as-Code models.
+      group: Generation
+      helpText: Generate a System Design Document from Architecture-as-Code models.
       input:
         - name: architecture-file
           type: file
           python_type: str
           description: An AaC file containing the modeled system for which to generate the System Design document.
         - name: output-directory
           type: directory
```

## aac/plugins/first_party/gen_design_doc/gen_design_doc_impl.py

```diff
@@ -1,27 +1,28 @@
-"""AaC Plugin implementation module for the aac-gen-design-doc plugin."""
+"""AaC Plugin implementation module for the Generate System Design Document plugin."""
 
 import os
 
 from jinja2 import Template
 
 
+from aac.lang.constants import ROOT_KEY_MODEL, ROOT_KEY_SCHEMA, ROOT_KEY_USECASE
 from aac.lang.definitions.collections import get_definitions_by_root_key
 from aac.lang.definitions.definition import Definition
 from aac.plugins.plugin_execution import PluginExecutionResult, plugin_result
 from aac.plugins.validators.required_fields import get_required_fields
 from aac.templates.engine import (
     TemplateOutputFile,
     generate_template,
     load_templates,
     write_generated_templates_to_file,
 )
 from aac.validate import validated_source
 
-plugin_name = "gen-design-doc"
+plugin_name = "Generate System Design Document"
 
 
 def gen_design_doc(architecture_file: str, output_directory: str) -> PluginExecutionResult:
     """
     Generate a System Design Document from Architecture-as-Code models.
 
     Args:
@@ -52,17 +53,17 @@
 def _get_parsed_models(architecture_file: str) -> list[Definition]:
     with validated_source(architecture_file) as result:
         return result.definitions if isinstance(result.definitions, list) else [result.definitions]
 
 
 def _make_template_properties(parsed_definitions: list[Definition], arch_file: str) -> dict:
     title = _get_document_title(arch_file)
-    models = _get_and_prepare_definitions_by_type(parsed_definitions, "model")
-    usecases = _get_and_prepare_definitions_by_type(parsed_definitions, "usecase")
-    interfaces = _get_and_prepare_definitions_by_type(parsed_definitions, "schema")
+    models = _get_and_prepare_definitions_by_type(parsed_definitions, ROOT_KEY_MODEL)
+    usecases = _get_and_prepare_definitions_by_type(parsed_definitions, ROOT_KEY_USECASE)
+    interfaces = _get_and_prepare_definitions_by_type(parsed_definitions, ROOT_KEY_SCHEMA)
     return {
         "title": title,
         "models": models,
         "usecases": usecases,
         "interfaces": interfaces,
     }
 
@@ -83,15 +84,15 @@
 
 def _get_and_prepare_definitions_by_type(parsed_definitions: list[Definition], aac_type: str) -> list[dict]:
     def get_definition_structure_with_required_fields(interface_definition: Definition):
         return interface_definition.structure | {"required_fields": get_required_fields(interface_definition)}
 
     filtered_definitions = get_definitions_by_root_key(aac_type, parsed_definitions)
     definition_template_properties = []
-    if aac_type == "schema":
+    if aac_type == ROOT_KEY_SCHEMA:
         definition_template_properties = [
             get_definition_structure_with_required_fields(definition) for definition in filtered_definitions
         ]
     else:
         definition_template_properties = [definition.structure for definition in filtered_definitions]
 
     return definition_template_properties
```

## aac/plugins/first_party/gen_design_doc/templates/datum.md.jinja2

```diff
@@ -1,10 +1,12 @@
-{%- for i in interfaces %}
+{% for i in interfaces %}
 {% set datum = i.schema %}
+
 ### Schema: {{ datum.name }}
 
 #### Fields
 {% for field in datum.fields %}
-- {{ field.type }} {{ field.name }}{%- if field.name in i.required_fields %} (required){%- endif %}
-{%- endfor %}
 
-{%- endfor %}
+- {{ field.type }} {{ field.name }}{% if field.name in i.required_fields %} (required){% endif %}
+{% endfor %}
+
+{% endfor %}
```

## aac/plugins/first_party/gen_design_doc/templates/macros.jinja2

```diff
@@ -1,11 +1,11 @@
 {% macro description(map) %}
-{%- if map and 'description' in map and map.description %}
+{% if map and 'description' in map and map.description %}
 {{ map.description }}
-{%- endif %}
+{% endif %}
 {% endmacro %}
 
 {% macro print_fields(fields) %}
 {% for field in fields %}
 - {{ field.type }} {{ field.name }}
-{%- endfor %}
-{% endmacro %}
+{% endfor %}
+{% endmacro %}
```

## aac/plugins/first_party/gen_design_doc/templates/model.md.jinja2

```diff
@@ -1,51 +1,59 @@
 {% from 'macros.jinja2' import description, print_fields %}
 
-{%- for m in models %}
+{% for m in models %}
 {% set model = m.model %}
+
 ### Model: {{ model.name }}
 
 {{ description(model) }}
 
-{%- if 'components' in model -%}
+{% if 'components' in model %}
+
 #### Components
 {{ print_fields(model.components) }}
 {% endif %}
 
 #### Behavior
 {% for behavior in model.behavior %}
+
 ***{{ behavior.name }}***
 
 {{ description(behavior) }}
 
 This is a {{ behavior.type }} type of behavior.
 
-{% if 'input' in behavior -%}
+{% if 'input' in behavior %}
+
 **Inputs**
+
 {{ print_fields(behavior.input) }}
 {% endif %}
 
-{%- if 'output' in behavior -%}
+{% if 'output' in behavior %}
+
 **Outputs**
+
 {{ print_fields(behavior.output) }}
 {% endif %}
 
 {% for acceptance in behavior.acceptance %}
 
 **Scenario: {{ acceptance.scenario }}**
 
 *Procedure:*
-{%- if 'given' in acceptance %}
+{% if 'given' in acceptance %}
+
 {% for given in acceptance.given %}
 1. Given {{ given }}
-{%- endfor %}
-{%- endif %}
-{%- for when in acceptance.when %}
+{% endfor %}
+{% endif %}
+{% for when in acceptance.when %}
 1. When {{ when }}
-{%- endfor %}
-{%- for then in acceptance.then %}
+{% endfor %}
+{% for then in acceptance.then %}
 1. Then {{ then }}
-{%- endfor %}
 {% endfor %}
-{%- endfor %}
+{% endfor %}
+{% endfor %}
 
-{%- endfor %}
+{% endfor %}
```

## aac/plugins/first_party/gen_design_doc/templates/system-design-doc.md.jinja2

```diff
@@ -1,19 +1,19 @@
 # {{ title }}
 
-{%- if interfaces | length > 0 %}
+{% if interfaces | length > 0 %}
 
 ## Interfaces
 {% include 'datum.md.jinja2' with context %}
-{%- endif %}
+{% endif %}
 
-{%- if models | length > 0 %}
+{% if models | length > 0 %}
 
 ## System Components
 {% include 'model.md.jinja2' with context %}
-{%- endif %}
+{% endif %}
 
-{%- if usecases | length > 0 %}
+{% if usecases | length > 0 %}
 
 ## Use Cases
 {% include 'usecase.md.jinja2' with context %}
-{%- endif %}
+{% endif %}
```

## aac/plugins/first_party/gen_design_doc/templates/usecase.md.jinja2

```diff
@@ -1,22 +1,24 @@
 {% from 'macros.jinja2' import description, print_fields %}
-{%- for u in usecases %}
+{% for u in usecases %}
 {% set usecase = u.usecase %}
+
 ### Usecase: {{ usecase.name }}
 
 {{ description(usecase) }}
 
 #### Participants
+
 {{ print_fields(usecase.participants) }}
 
 #### Steps
 
 {% for steps in usecase.steps %}
 
 ***{{ steps.step }}***
 
-- **Source:** {{ steps.source }}
-- **Target:** {{ steps.target }}
-- **Action:** {{ steps.action }}
-{%- endfor %}
+ **Source:** {{ steps.source }}
+ **Target:** {{ steps.target }}
+ **Action:** {{ steps.action }}
+{% endfor %}
 
-{%- endfor %}
+{% endfor %}
```

## aac/plugins/first_party/gen_gherkin_behaviors/__init__.py

```diff
@@ -36,15 +36,15 @@
             "directory",
         ),
     ]
 
     plugin_commands = [
         AacCommand(
             "gen-gherkin-behaviors",
-            "Generate Gherkin feature files from Arch-as-Code model behavior scenarios.",
+            "Generate Gherkin feature files from AaC model behavior scenarios.",
             gen_gherkin_behaviors,
             gen_gherkin_behaviors_arguments,
         ),
     ]
 
     return plugin_commands
```

## aac/plugins/first_party/gen_gherkin_behaviors/gen_gherkin_behaviors.yaml

```diff
@@ -1,23 +1,23 @@
-model:
-  name: aac-gen-gherkin-behaviors
-  description: aac-gen-gherkin-behaviors is an Architecture-as-Code plugin that generates Gherkin feature files from model behavior scenarios.
-  behavior:
+plugin:
+  name: Generate Gherkin Feature Files
+  description: An AaC plugin that generates Gherkin feature files from model behavior scenarios.
+  commands:
     - name: gen-gherkin-behaviors
-      type: command
-      description: Generate Gherkin feature files from Arch-as-Code model behavior scenarios.
+      group: Generation
+      helpText: Generate Gherkin feature files from AaC model behavior scenarios.
       input:
         - name: architecture-file
           type: file
           python_type: str
-          description: The yaml file containing the data models to generate as Gherkin feature files.
+          description: The YAML file containing the data models from which to generate Gherkin feature files.
         - name: output-directory
           type: directory
           python_type: str
-          description: The directory to write the generated Gherkin feature files to.
+          description: The directory into which the generated Gherkin feature files will be written.
       acceptance:
         - scenario: Output Gherkin feature files for behavior scenarios in an Architecture model.
           given:
             - The {{gen-gherkin-behaviors.input.architecture-file}} contains a valid architecture.
           when:
             - The aac app is run with the gen-gherkin-behaviors command and a valid architecture file.
           then:
```

## aac/plugins/first_party/gen_gherkin_behaviors/gen_gherkin_behaviors_impl.py

```diff
@@ -1,16 +1,16 @@
-"""AaC Plugin implementation module for the aac-gen-gherkin-behaviors plugin."""
+"""AaC Plugin implementation module for the Generate Gherkin Feature Files plugin."""
 
 from aac.lang.definitions.collections import get_models_by_type, convert_parsed_definitions_to_dict_definition
 from aac.plugins import PluginError
 from aac.plugins.plugin_execution import PluginExecutionResult, plugin_result
 from aac.templates.engine import TemplateOutputFile, generate_template, load_templates, write_generated_templates_to_file
 from aac.validate import validated_source
 
-plugin_name = "gen-gherkin-behaviors"
+plugin_name = "Generate Gherkin Feature Files"
 
 
 def gen_gherkin_behaviors(architecture_file: str, output_directory: str) -> PluginExecutionResult:
     """
     Generate Gherkin feature files from Arch-as-Code model behavior scenarios.
 
     Args:
```

## aac/plugins/first_party/gen_json/gen_json.yaml

```diff
@@ -1,24 +1,24 @@
-model:
-  name: gen-json
-  description: An Architecture-as-Code plugin that generates json representations of the AaC yaml DSL.
-  behavior:
+plugin:
+  name: Generate JSON
+  description: An AaC plugin that generates JSON representations of one, or more, AaC definitions.
+  commands:
     - name: gen-json
-      type: command
-      description: Generate JSON representation of AaC yaml DSL
+      group: Generation
+      helpText: Generate a JSON representation of one, or more, AaC definitions.
       input:
         - name: architecture-files
           type: file
           python_type: list[str]
-          description: File paths to AaC file(s) containing models to parse and print as JSON.
+          description: File paths to AaC file(s) containing definitions to output as JSON.
         - name: --output-directory
           type: directory
           python_type: str
-          description: Directory in which JSON files will be written
+          description: The directory into which JSON files will be written.
       acceptance:
-        - scenario: Output JSON representation.
+        - scenario: Output a JSON representation of AaC definitions.
           given:
             - The {{gen-json.input.architecture-files}} contains a valid model.
           when:
             - The aac app is run with the gen-json command.
           then:
             - JSON representation is output to the user or to the user defined output directory.
```

## aac/plugins/first_party/gen_json/gen_json_impl.py

```diff
@@ -1,20 +1,21 @@
-"""A plugin to print JSON schema of AaC model files."""
+"""AaC Plugin implementation module for the Generate JSON plugin."""
 
 import json
 import os
+
 from typing import Optional
 
 from aac.io.writer import write_file
 from aac.lang.definitions.collections import convert_parsed_definitions_to_dict_definition
 from aac.plugins.plugin_execution import PluginExecutionResult, PluginExecutionStatusCode, plugin_result
 from aac.validate import validated_source
 
 
-plugin_name = "gen-json"
+plugin_name = "Generate JSON"
 
 
 def print_json(architecture_files: list[str], output_directory: Optional[str] = None) -> PluginExecutionResult:
     """
     Print the parsed_models from the parsed architecture_files values in JSON format.
 
     Args:
```

## aac/plugins/first_party/gen_plant_uml/gen_plant_uml.yaml

```diff
@@ -1,23 +1,29 @@
-model:
-  name: aac-plantuml
-  description: aac-plantuml is a Architecture-as-Code plugin that enables Plant UML content to be generated from Arch-as-Code models.
-  behavior:
+plugin:
+  name: Generate PlantUML Diagrams
+  description: |
+    An AaC plugin that enables PlantUML diagrams to be generated from AaC
+    definitions.
+  commands:
     - name: puml-component
-      type: command
-      description: Converts an AaC model to Plant ULM component diagram
+      group: Generation
+      helpText: Converts an AaC-defined system to a PlantUML component diagram.
       input:
         - name: architecture-file
           type: file
           python_type: str
-          description: Path to a yaml file containing an AaC usecase from which to generate a Plant UML component diagram.
+          description: |
+            A path to a YAML file containing an AaC-defined system from which to
+            generate a PlantUML component diagram.
         - name: output-directory
           type: directory
           python_type: str
-          description: Output directory for the PlantUML (.puml) diagram file
+          description: |
+            The output directory into which the PlantUML (.puml) diagram file
+            will be written.
       acceptance:
         - scenario: Output PlantUML component diagram for valid architecture.
           given:
             - The {{puml.input.architecture-file}} contains a valid model.
           when:
             - The aac app is run with the puml-component command.
           then:
@@ -27,25 +33,29 @@
             - The {{puml.input.architecture-file}} contains a valid model.
             - The positional argument {{puml.input.output-directory}} contains a valid filepath.
           when:
             - The aac app is run with the puml-component command.
           then:
             - A PlantUML component diagram of the model is generated to a .puml file.
     - name: puml-sequence
-      type: command
-      description: Converts an AaC usecase to Plant ULM sequence diagram
+      group: Generation
+      helpText: Converts an AaC-defined usecase to PlantUML sequence diagram.
       input:
         - name: architecture-file
           type: file
           python_type: str
-          description: Path to a yaml file containing an AaC usecase from which to generate a Plant UML sequence diagram.
+          description: |
+            A path to a YAML file containing an AaC-defined usecase from which
+            to generate a PlantUML sequence diagram.
         - name: output-directory
           type: directory
           python_type: str
-          description: Output directory for the PlantUML (.puml) diagram file
+          description: |
+            The output directory into which the PlantUML (.puml) diagram file
+            will be written.
       acceptance:
         - scenario: Output PlantUML sequence diagram for valid use case.
           given:
             - The {{puml.input.architecture-file}} contains a valid model.
           when:
             - The aac app is run with the puml-sequence command.
           then:
@@ -55,25 +65,29 @@
             - The {{puml.input.architecture-file}} contains a valid model.
             - The positional argument {{puml.input.output-directory}} contains a valid filepath.
           when:
             - The aac app is run with the puml-sequence command.
           then:
             - A PlantUML sequence diagram of the model is generated to a .puml file.
     - name: puml-object
-      type: command
-      description: Converts an AaC model to Plant ULM object diagram
+      group: Generation
+      helpText: Convert an AaC-defined system to PlantUML object diagram.
       input:
         - name: architecture-file
           type: file
           python_type: str
-          description: Path to a yaml file containing an AaC usecase from which to generate a Plant UML object diagram.
+          description: |
+            A path to a YAML file containing an AaC-defined system from which to
+            generate a PlantUML object diagram.
         - name: output-directory
           type: directory
           python_type: str
-          description: Output directory for the PlantUML (.puml) diagram file
+          description: |
+            The output directory into which the PlantUML (.puml) diagram file
+            will be written.
       acceptance:
         - scenario: Output PlantUML object diagram for valid model.
           given:
             - The {{puml.input.architecture-file}} contains a valid model.
           when:
             - The aac app is run with the puml-object command.
           then:
```

## aac/plugins/first_party/gen_plant_uml/gen_plant_uml_impl.py

```diff
@@ -1,21 +1,22 @@
-"""AaC Plugin implementation module for the aac-plantuml plugin."""
+"""AaC Plugin implementation module for the Generate PlantUML Diagrams plugin."""
 
 import os
+
 from typing import Callable
 
 from aac.lang.active_context_lifecycle_manager import get_active_context
 from aac.lang.definitions.collections import get_definitions_by_root_key
 from aac.lang.definitions.definition import Definition
 from aac.lang.definitions.search import search_definition
 from aac.plugins.plugin_execution import PluginExecutionResult, plugin_result
-from aac.validate import validated_source
 from aac.templates.engine import generate_templates, load_templates, write_generated_templates_to_file
+from aac.validate import validated_source
 
-plugin_name = "gen-plant-uml"
+plugin_name = "Generate PlantUML Diagrams"
 PLANT_UML_FILE_EXTENSION = ".puml"
 COMPONENT_STRING = "component"
 OBJECT_STRING = "object"
 SEQUENCE_STRING = "sequence"
 FILE_NAME_CHARACTERS_TO_REPLACE = ".!@#$%^&*();,\\/?[]{}`~|'"
```

## aac/plugins/first_party/gen_plant_uml/templates/object/object_diagram.puml.jinja2

```diff
@@ -1,10 +1,10 @@
 @startuml {{title}} Object Diagram
 title {{title}} Object Diagram
-{%- for object in objects %}
+{% for object in objects %}
 object {{object}}
-{%- endfor %}
+{% endfor %}
 
-{%- for object_hierarchy in object_hierarchies %}
+{% for object_hierarchy in object_hierarchies %}
 {{object_hierarchy.parent}} *-- {{object_hierarchy.child}}
-{%- endfor %}
-@enduml
+{% endfor %}
+@enduml
```

## aac/plugins/first_party/gen_plant_uml/templates/sequence/sequence_diagram.puml.jinja2

```diff
@@ -1,10 +1,10 @@
 @startuml {{title}} Sequence Diagram
 title {{title}} Sequence Diagram
-{%- for participant in participants %}
+{% for participant in participants %}
 participant {{participant.type}} as {{participant.name}}
-{%- endfor %}
+{% endfor %}
 
-{%- for sequence in sequences %}
+{% for sequence in sequences %}
 {{sequence.source}} -> {{sequence.target}} : {{sequence.action}}
-{%- endfor %}
-@enduml
+{% endfor %}
+@enduml
```

## aac/plugins/first_party/gen_plugin/__init__.py

```diff
@@ -16,14 +16,15 @@
 
     Returns:
         A collection of information about the plugin and what it contributes.
     """
     plugin = Plugin(plugin_name)
     plugin.register_commands(_get_plugin_commands())
     plugin.register_definitions(_get_plugin_definitions())
+
     return plugin
 
 
 def _get_plugin_commands():
     command_arguments = [
         AacCommandArgument(
             "architecture-file",
```

## aac/plugins/first_party/gen_plugin/gen_plugin.yaml

```diff
@@ -1,19 +1,19 @@
-model:
-  name: gen-plugin
-  description: An Architecture-as-Code plugin that generates opinionated plugin stubs for easier and quicker plugin development.
-  behavior:
+plugin:
+  name: Generate Plugin
+  description: An AaC plugin that generates opinionated plugin stubs for easier and quicker plugin development.
+  commands:
     - name: gen-plugin
-      type: command
-      description: Generate
+      group: Generation
+      helpText: Generate stubs for an AaC plugin.
       input:
         - name: architecture-file
           type: file
           python_type: str
-          description: filepath to the architecture file.
+          description: The path to the architecture file with the plugin definition.
       acceptance:
         - scenario: Generate first party plugin stub files.
           given:
             - The {{gen-plugin.input.architecture-file}} contains a valid model.
             - The {{gen-plugin.input.architecture-file}} is in the AaC repository under the directory path "src/aac/plugins/".
           when:
             - The aac app is run with the gen-plugin command.
@@ -23,15 +23,14 @@
           given:
             - The {{gen-plugin.input.architecture-file}} contains a valid model.
           when:
             - The aac app is run with the gen-plugin command.
             - The value of {{gen-plugin.input.architecture-file}} does not contain "src/aac/plugins/".
           then:
             - Stubbed third party plugin files are not generated.
-
 ---
 enum:
   name: PythonDataType
   values:
     - str
     - int
     - float
@@ -54,14 +53,7 @@
       add:
         - name: python_type
           type: PythonDataType
         - name: number_of_arguments
           type: int
         - name: default
           type: PythonDataType
----
-ext:
-   name: CommandBehaviorType
-   type: BehaviorType
-   enumExt:
-      add:
-         - command
```

## aac/plugins/first_party/gen_plugin/gen_plugin_impl.py

```diff
@@ -1,28 +1,47 @@
-"""
-A plugin to generate new plugins based on a specifically structured AaC model file.
+"""AaC Plugin implementation module for the Generate Plugin plugin."""
 
-The plugin AaC model must define behaviors using the command BehaviorType.  Each
-defined behavior becomes a new command for the aac CLI.
-"""
 import logging
-import yaml
 
-from os import path, rename, makedirs
+from os import makedirs, path, rename
+from typing import Any
 
-from aac.lang.definitions.collections import convert_parsed_definitions_to_dict_definition, get_models_by_type
-from aac.lang.definitions.search import search
+from aac import __version__
+from aac.io.parser import parse, ParserError
+from aac.lang.constants import (
+    DEFINITION_FIELD_COMMANDS,
+    DEFINITION_FIELD_DEFINITION_SOURCES,
+    DEFINITION_FIELD_DISPLAY,
+    DEFINITION_FIELD_GROUP,
+    DEFINITION_FIELD_HELP_TEXT,
+    DEFINITION_FIELD_INPUT,
+    DEFINITION_FIELD_NAME,
+    DEFINITION_FIELD_OUTPUT,
+    DEFINITION_FIELD_TYPE,
+    ROOT_KEY_ENUM,
+    ROOT_KEY_EXTENSION,
+    ROOT_KEY_PLUGIN,
+    ROOT_KEY_SCHEMA,
+    ROOT_KEY_VALIDATION,
+)
+from aac.lang.definitions.collections import get_definitions_by_root_key
 from aac.lang.definitions.definition import Definition
-from aac.templates.engine import TemplateOutputFile, generate_templates, load_templates, write_generated_templates_to_file
 from aac.plugins import OperationCancelled
 from aac.plugins.first_party.gen_plugin.GeneratePluginException import GeneratePluginException
 from aac.plugins.plugin_execution import PluginExecutionResult, plugin_result
-from aac.validate import validated_source
+from aac.templates.engine import (
+    TemplateOutputFile,
+    generate_templates,
+    load_templates,
+    write_generated_templates_to_file,
+)
+from aac.validate import validated_definitions
 
-plugin_name = "gen-plugin"
+
+plugin_name = "Generate Plugin"
 
 PLUGIN_TYPE_FIRST_STRING = "first"
 PLUGIN_TYPE_THIRD_STRING = "third"
 
 EXPECTED_FIRST_PARTY_DIRECTORY_PATH = str(path.join("src", "aac", "plugins"))
 
 
@@ -51,25 +70,44 @@
         raise OperationCancelled(f"Move {architecture_file_path} to the desired directory and retry.")
 
     with plugin_result(plugin_name, _generate_plugin) as result:
         return result
 
 
 def _generate_plugin_files_to_directory(architecture_file_path: str, plugin_output_directory: str, plugin_type: str) -> str:
-    with validated_source(architecture_file_path) as validation_result:
-        definitions = validation_result.definitions
-        templates = list(
+    with validated_definitions(_collect_all_plugin_definitions(architecture_file_path)) as validation_result:
+        templates: list = list(
             _prepare_and_generate_plugin_files(
-                definitions, plugin_type, architecture_file_path, plugin_output_directory
+                validation_result.definitions, plugin_type, architecture_file_path, plugin_output_directory
             ).values()
         )
         write_generated_templates_to_file(templates)
         return f"Successfully created a {plugin_type}-party plugin in {plugin_output_directory}"
 
 
+def _collect_all_plugin_definitions(architecture_file_path: str) -> list[Definition]:
+
+    def get_definition_source_path(pathspec: str) -> str:
+        return pathspec if pathspec.startswith(path.sep) else path.join(path.dirname(architecture_file_path), pathspec)
+
+    plugin_definitions = []
+
+    try:
+        definitions = parse(architecture_file_path)
+    except ParserError as error:
+        raise ParserError(error.source, error.errors) from None
+    else:
+        plugin, *_ = get_definitions_by_root_key(ROOT_KEY_PLUGIN, definitions)
+        definition_sources = plugin.get_top_level_fields().get(DEFINITION_FIELD_DEFINITION_SOURCES, [])
+        definition_sources_definitions = [definition for path in definition_sources for definition in parse(get_definition_source_path(path))]
+        plugin_definitions = definitions + definition_sources_definitions
+
+    return plugin_definitions
+
+
 def _is_plugin_in_aac_repository(architecture_file_path: str) -> bool:
     """
     Returns true if the architecture file path is inside the AaC repository.
 
     Performs a basic check against the file path of the architecture as code plugin file
         to determine if the file's path matches  some partial structure that matches
         the directory hierarchy of the project.
@@ -77,15 +115,15 @@
     Args:
         architecture_file_path: str the full path to the architecture file and output directory
     """
     return EXPECTED_FIRST_PARTY_DIRECTORY_PATH in architecture_file_path
 
 
 def _apply_output_template_properties(
-    output_files: list[TemplateOutputFile],
+    output_files: dict[str, TemplateOutputFile],
     overwite_files: list[str],
     plugin_implementation_name,
 ):
     """
     Apply post-generation settings to the files prior to them being written to the filesystem.
 
     Args:
@@ -113,20 +151,20 @@
 def _get_template_output_directories(plugin_type: str, architecture_file_path: str, plugin_name: str) -> dict[str, str]:
     """Returns a manually maintained list of templates and their output directories."""
 
     architecture_file_directory_path = path.dirname(architecture_file_path)
 
     # First party files are generated at the same level as the architecture file
     first_party_directories = {
-        "test_plugin_impl.py.jinja2": path.join("tests", "plugins"),
+        "test_plugin_impl.py.jinja2": path.join("tests", "plugins", "first_party"),
         "plugin_impl.py.jinja2": architecture_file_directory_path,
         "__init__.py.jinja2": architecture_file_directory_path,
     }
 
-    # Third party files are generated a level belowthe architecture file
+    # Third party files are generated a level below the architecture file
     third_party_directories = {
         "test_plugin_impl.py.jinja2": "tests",
         "README.md.jinja2": "",
         "__init__.py.jinja2": plugin_name,
         "plugin_impl.py.jinja2": plugin_name,
         "setup.py.jinja2": "",
         "tox.ini.jinja2": "",
@@ -141,100 +179,101 @@
     """Generates the Jinja2 templates with the template properties."""
     directories = {name: path.join(output_directory, output_file) for name, output_file in output_directories.items()}
     return generate_templates(load_templates(__package__, f"templates/{plugin_type}_party"), directories, template_properties)
 
 
 def _prepare_and_generate_plugin_files(
     definitions: list[Definition], plugin_type: str, architecture_file_path: str, output_directory: str
-) -> dict[str, list[TemplateOutputFile]]:
+) -> dict[str, TemplateOutputFile]:
     """
-    Parse the model and generate the plugin template accordingly.
+    Parse the plugin definitions and generate the plugin template accordingly.
 
     Args:
-        parsed_models (dict[str, dict]): Dict representing the plugin models.
+        definitions (list[Definition]): A list of definitions
         plugin_type (str): A string representing the plugin type {PLUGIN_TYPE_FIRST_STRING, PLUGIN_TYPE_THIRD_STRING}
         architecture_file_path (str): The filepath to the architecture file used to generate the plugin.
         output_directory (str): The directory in which to output the generated plugin files.
 
     Returns:
         List of TemplateOutputFile objects that contain the compiled templates
 
     Raises:
         GeneratePluginException: An error encountered during the plugin generation process.
     """
-    parsed_definitions_dictionary = convert_parsed_definitions_to_dict_definition(definitions)
-    template_properties = _gather_template_properties(parsed_definitions_dictionary, architecture_file_path, plugin_type)
-
-    plugin_name = template_properties.get("plugin").get("name")
-    plugin_implementation_name = template_properties.get("plugin").get("implementation_name")
+    template_properties = _gather_template_properties(definitions, architecture_file_path, plugin_type)
 
+    plugin_name = template_properties.get(ROOT_KEY_PLUGIN, {}).get(DEFINITION_FIELD_NAME)
+    plugin_implementation_name = template_properties.get(ROOT_KEY_PLUGIN, {}).get("implementation_name")
     plugin_implementation_name = _convert_to_implementation_name(plugin_name)
+
     templates_to_overwrite = _get_overwriteable_templates()
     template_output_directories = _get_template_output_directories(
         plugin_type, architecture_file_path, plugin_implementation_name
     )
 
     if plugin_type == PLUGIN_TYPE_THIRD_STRING:
-        new_architecture_file_location = _get_new_architecture_file_path(
-            architecture_file_path, output_directory, plugin_implementation_name
-        )
-        _move_architecture_file_to_plugin_root(architecture_file_path, new_architecture_file_location)
+        template_properties["aac_version"] = __version__
+        new_sources = {}
+        definition_sources = {definition.source.uri for definition in definitions}
+        for source in definition_sources:
+            new_sources[source] = _get_updated_file_path(source, output_directory, plugin_implementation_name)
+            _move_architecture_file_to_plugin_root(source, new_sources[source])
 
         for definition in definitions:
-            definition.source.uri = new_architecture_file_location
+            definition.source.uri = new_sources.get(definition.source.uri)
 
     generated_templates = _generate_template_files(
         plugin_type, output_directory, template_output_directories, template_properties
     )
 
     _apply_output_template_properties(generated_templates, templates_to_overwrite, plugin_implementation_name)
 
     return generated_templates
 
 
 def _gather_template_properties(
-    parsed_models: dict[str, dict], architecture_file_path: str, plugin_type: str
-) -> dict[str, any]:
+    parsed_definitions: list[Definition], architecture_file_path: str, plugin_type: str
+) -> dict[str, Any]:
     """
     Analyzes the models and returns the necessary template data to generate the plugin.
 
     Args:
-        parsed_models (dict[str, dict]): Dict representing the plugin models
-        architecture_file_path (str): The filepath to the architecture file used to generate the plugin
-        plugin_type (str): Whether the plugin is first or third party
+        parsed_definitions (list[Definition]): A list of plugin definitions.
+        architecture_file_path (str): The filepath to the architecture file used to generate the plugin.
+        plugin_type (str): Whether the plugin is first or third party.
 
     Returns:
         A dictionary of properties to be used when generating the jinja templates.
     """
+    plugins = get_definitions_by_root_key(ROOT_KEY_PLUGIN, parsed_definitions)
+    if len(plugins) != 1:
+        raise GeneratePluginException("Plugin AaC YAML must contain one, and only one, plugin definition.")
 
-    # Ensure model is present and valid, get the plugin name
-    plugin_models = get_models_by_type(parsed_models, "model")
-    if len(plugin_models.keys()) != 1:
-        raise GeneratePluginException("Plugin Arch-as-Code yaml must contain one and only one model.")
-
-    plugin_model = list(plugin_models.values())[0].get("model")
-    plugin_name = plugin_model.get("name")
-    plugin_implementation_name = _convert_to_implementation_name(plugin_name)
+    plugin, *_ = plugins
+    plugin_implementation_name = _convert_to_implementation_name(plugin.name)
 
     # Prepare template variables/properties
-    behaviors = search(plugin_model, ["behavior"])
-    commands = _gather_commands(behaviors)
+    commands = _gather_command_properties(plugin)
 
     plugin = {
-        "name": plugin_name,
+        DEFINITION_FIELD_NAME: plugin.name,
         "implementation_name": plugin_implementation_name,
     }
 
     plugin_aac_definitions = [
-        _add_definitions_yaml_string(definition) for definition in _gather_plugin_aac_definitions(parsed_models)
+        {
+            "root_key": definition.get_root_key(),
+            "type_name": definition.name,
+            "yaml": definition.to_yaml(),
+        } for definition in _gather_plugin_aac_definitions(parsed_definitions)
     ]
 
     package_name = path.basename(path.dirname(architecture_file_path))
     architecture_file = {
-        "name": path.basename(architecture_file_path),
+        DEFINITION_FIELD_NAME: path.basename(architecture_file_path),
         "package_name": f"first_party.{package_name}" if plugin_type == PLUGIN_TYPE_FIRST_STRING else package_name,
     }
 
     template_properties = {
         "plugin": plugin,
         "commands": commands,
         "plugin_definitions": plugin_aac_definitions,
@@ -251,15 +290,15 @@
     Args:
         template_name (str): The template's name
         plugin_name (str): The plugin's name
 
     Returns:
         A string containing the customized/pythonic file name.
     """
-    return template_name.replace(".jinja2", "").replace("plugin", plugin_name)
+    return template_name.replace(".jinja2", "").replace("plugin", plugin_name.lower())
 
 
 def _is_user_desired_output_directory(architecture_file_path: str) -> bool:
     """
     Confirms with the user that they're comfortable with the target generation directory.
 
     Args:
@@ -279,86 +318,87 @@
             first = False
 
         confirmation = input(f"Do you want to generate an AaC plugin in the directory {output_dir}/? [y/n]")
 
     return confirmation in ["y", "Y"]
 
 
-def _gather_commands(behaviors: dict) -> list[dict]:
+def _gather_command_properties(plugin_definition: Definition) -> list[dict]:
     """
-    Parse the plugin model's behaviors and return a list of commands derived from the plugin's behavior.
+    Parse the plugin definition's commands and return a list of each command's template properties.
 
     Args:
-        behaviors: The plugin's modeled behaviors
+        plugin_definition (Definition): The plugin definition.
 
     Returns:
-        list of command-type behaviors dicts
+        A list of template property dicts for the plugin's commands.
     """
 
     def modify_command_input_output_entry(in_out_entry: dict):
         """Modify the input and output entries of a behavior definition to reduce complexity in the templates."""
         python_type = in_out_entry.get("python_type")
 
-        in_out_entry["name"] = in_out_entry.get("name").removeprefix("--")
+        in_out_entry[DEFINITION_FIELD_NAME] = in_out_entry.get(DEFINITION_FIELD_NAME).removeprefix("--")
 
         if python_type:
-            in_out_entry["type"] = python_type
+            in_out_entry[DEFINITION_FIELD_TYPE] = python_type
             in_out_entry["python_type_default"] = type(python_type)
 
         return in_out_entry
 
     commands = []
 
-    for behavior in behaviors:
-        behavior_name = behavior["name"]
-        behavior_description = behavior["description"]
-        behavior_type = behavior.get("type")
-
-        if behavior_type != "command":
-            continue
+    for cmd in plugin_definition.get_top_level_fields().get(DEFINITION_FIELD_COMMANDS, []):
+        command = {}
 
         # First line should end with a period. flake8(D400)
-        if not behavior_description.endswith("."):
-            behavior_description = f"{behavior_description}."
-
-        if behavior.get("input"):
-            behavior["input"] = list(map(modify_command_input_output_entry, behavior.get("input")))
-
-        behavior["description"] = behavior_description
-        behavior["implementation_name"] = _convert_to_implementation_name(behavior_name)
-        commands.append(behavior)
+        command_help_text = cmd.get(DEFINITION_FIELD_HELP_TEXT)
+        if not command_help_text.endswith("."):
+            command_help_text = f"{command_help_text}."
+
+        command_input = cmd.get(DEFINITION_FIELD_INPUT)
+        if command_input:
+            command[DEFINITION_FIELD_INPUT] = [modify_command_input_output_entry(i) for i in command_input]
+
+        command_output = cmd.get(DEFINITION_FIELD_OUTPUT)
+        if command_output:
+            command[DEFINITION_FIELD_OUTPUT] = [modify_command_input_output_entry(o) for o in command_output]
+
+        command_name = cmd.get(DEFINITION_FIELD_NAME)
+        command[DEFINITION_FIELD_NAME] = command_name
+        command[DEFINITION_FIELD_HELP_TEXT] = command_help_text
+        command[DEFINITION_FIELD_DISPLAY] = cmd.get(DEFINITION_FIELD_NAME, command_name)
+        command[DEFINITION_FIELD_GROUP] = cmd.get(DEFINITION_FIELD_GROUP)
+        command["implementation_name"] = _convert_to_implementation_name(command_name)
+        commands.append(command)
 
     return commands
 
 
-def _gather_plugin_aac_definitions(parsed_models: dict[str, dict]) -> list[dict]:
+def _gather_plugin_aac_definitions(parsed_definitions: list[Definition]) -> list[Definition]:
     """
     Gather all AaC definitions declared by the model.
 
     Args:
-        parsed_models (dict[str, dict]): Dict representing the plugin models
+        parsed_definitions (list[Definition]): The list of plugin definitions.
 
     Returns:
         A list of AaC definitions provided by the plugin
     """
-    extension_definitions = list(get_models_by_type(parsed_models, "ext").values())
-    schema_definitions = list(get_models_by_type(parsed_models, "schema").values())
-    enum_definitions = list(get_models_by_type(parsed_models, "enum").values())
-
-    return extension_definitions + schema_definitions + enum_definitions
-
+    validation_definitions = get_definitions_by_root_key(ROOT_KEY_VALIDATION, parsed_definitions)
+    extension_definitions = get_definitions_by_root_key(ROOT_KEY_EXTENSION, parsed_definitions)
+    schema_definitions = get_definitions_by_root_key(ROOT_KEY_SCHEMA, parsed_definitions)
+    enum_definitions = get_definitions_by_root_key(ROOT_KEY_ENUM, parsed_definitions)
 
-def _add_definitions_yaml_string(model: dict) -> dict:
-    model["yaml"] = yaml.dump(model)
-    return model
+    return validation_definitions + extension_definitions + schema_definitions + enum_definitions
 
 
 def _convert_to_implementation_name(original_name: str) -> str:
     """Converts a plugin name to a pythonic version for implementation."""
-    return original_name.replace("-", "_")
+    return original_name.replace("-", "_").replace(" ", "_").lower()
 
 
 def _get_repository_root_directory_from_path(system_path: str) -> str:
     """Returns the root of the AaC Repository from a path within the repository's plugins directory."""
     target_index = system_path.find(EXPECTED_FIRST_PARTY_DIRECTORY_PATH)
 
     if target_index < 0:
@@ -366,19 +406,19 @@
         raise (
             GeneratePluginException(f"Expected file path '{system_path}' to contain '{EXPECTED_FIRST_PARTY_DIRECTORY_PATH}'.")
         )
 
     return system_path[:target_index]
 
 
-def _get_new_architecture_file_path(architecture_file_path: str, output_directory: str, generated_plugin_name: str) -> str:
+def _get_updated_file_path(architecture_file_path: str, output_directory: str, generated_plugin_name: str) -> str:
     """Return the new file path to which the plugin architecture file will be moved."""
     architecture_file_path = path.join(output_directory, architecture_file_path)
     file_name = path.basename(architecture_file_path)
     new_file_path = path.join(output_directory, generated_plugin_name, file_name)
     return new_file_path
 
 
 def _move_architecture_file_to_plugin_root(architecture_file_path: str, new_file_path: str) -> None:
-    """Moves the architecture file to the plugin root directory."""
+    """Move the architecture file to the plugin root directory."""
     makedirs(path.dirname(new_file_path), exist_ok=True)
     rename(architecture_file_path, new_file_path)
```

## aac/plugins/first_party/gen_plugin/templates/first_party/__init__.py.jinja2

```diff
@@ -50,24 +50,23 @@
     {% endif %}
     {% endfor %}
 
     plugin_commands = [
         {% for command in commands %}
         AacCommand(
             "{{command.name}}",
-            "{{command.description}}",
+            "{{command.helpText}}",
             {{command.implementation_name}}{% if command.input is defined %},
             {{command.implementation_name}}_arguments,{% endif +%}
         ),
         {% endfor %}
     ]
 
     return plugin_commands
 {% endif %}
 {% if plugin_definitions | length > 0 %}
 {# Leave a blank line here since we want 2 space if the expression is true and one if it's false#}
-{% set yaml_file_joiner = joiner("\n---\n") %}
 
 def _get_plugin_definitions():
     return get_plugin_definitions_from_yaml(__package__, "{{architecture_file.name}}")
 
 {% endif %}
```

## aac/plugins/first_party/gen_plugin/templates/first_party/plugin_impl.py.jinja2

```diff
@@ -6,16 +6,16 @@
 
 plugin_name = "{{plugin.name}}"
 {% for command in commands %}
 {% set comma_joiner = joiner(", ") %}
 
 def {{command.implementation_name}}({% for command_input in command.input %}{{comma_joiner()}}{{command_input.name | trim('-') | replace('-', '_')}}: {{command_input.python_type}}{% endfor %}) -> PluginExecutionResult:
     """
-    {% if command.description is defined %}
-    {{command.description}}
+    {% if command.helpText is defined %}
+    {{command.helpText}}
     {% else %}
     TODO: Write a description
     {% endif %}
     {% if command.input is defined %}
 
     Args:
     {%- for command_input in command.input +%}
```

## aac/plugins/first_party/gen_plugin/templates/first_party/test_plugin_impl.py.jinja2

```diff
@@ -1,15 +1,15 @@
 from unittest import TestCase
 
 from aac.plugins.plugin_execution import PluginExecutionStatusCode
 {% set comma_joiner = joiner(", ") %}
 from aac.plugins.{{architecture_file.package_name}}.{{plugin.implementation_name}}_impl import {% for command in commands %}{{comma_joiner()}}{{command.implementation_name}}{% endfor %}
 
 
-class Test{{plugin.name | title | replace('-', '')}}(TestCase):
+class Test{{plugin.name | title | replace('-', '') | replace(' ', '')}}(TestCase):
     {% for command in commands %}
     def test_{{command.implementation_name}}(self):
         # TODO: Write tests for {{command.implementation_name}}
 
         {% for argument in command.input %}
         {{argument.name | replace('-', '_')}} = {{argument.type}}()
         {% endfor %}
```

## aac/plugins/first_party/gen_plugin/templates/third_party/README.md.jinja2

```diff
@@ -2,20 +2,20 @@
 
 ## Plugin Commands
 
 {% for command in commands %}
 
 ### Command: {{command.name}}
 
-{{command.description}}
+{{command.helpText}}
 
 Example shell usage:
 
 ```bash
-(.env) $ aac {{command.name}} -h
+(.env) $ aac {{command.display or command.name}} -h
 ```
 
 #### Command arguments
 
 - `-h`, `--help`: Shows a help message
 {% if command.input is defined %}
 {% for command_input in command.input %}
@@ -25,18 +25,17 @@
 {% endfor %}
 
 {% if plugin_definitions | length > 0 %}
 
 ## Plugin Extensions and Definitions
 
 {% for def in plugin_definitions %}
-{% set type = def | rejectattr('yaml') | list | first %}
 
-### {{type | title}} - {{def[type].name}}
+### {{def.root_key | title}} - {{def.type_name}}
 
-TODO: Add descriptive information about {{def[type].name}}
+TODO: Add descriptive information about {{def.type_name}}
 
 ```yaml
 {{def.yaml}}
 ```
 {% endfor %}
 {% endif %}
```

## aac/plugins/first_party/gen_plugin/templates/third_party/__init__.py.jinja2

```diff
@@ -1,8 +1,9 @@
 """The {{plugin.name}} plugin module."""
+
 # NOTE: It is safe to edit this file.
 # This file is only initially generated by aac gen-plugin, and it won't be overwritten if the file already exists.
 
 from aac.cli.aac_command import AacCommand, AacCommandArgument
 from aac.plugins import hookimpl
 from aac.plugins.plugin import Plugin
 {% if plugin_definitions | length > 0 %}
@@ -50,24 +51,23 @@
     {% endif %}
     {% endfor %}
 
     plugin_commands = [
         {% for command in commands %}
         AacCommand(
             "{{command.name}}",
-            "{{command.description}}",
+            "{{command.helpText}}",
             {{command.implementation_name}}{% if command.input is defined %},
             {{command.implementation_name}}_arguments,{% endif +%}
         ),
         {% endfor %}
     ]
 
     return plugin_commands
 {% endif %}
 {% if plugin_definitions | length > 0 %}
 {# Leave a blank line here since we want 2 space if the expression is true and one if it's false#}
-{% set yaml_file_joiner = joiner("\n---\n") %}
 
 def _get_plugin_definitions():
     return get_plugin_definitions_from_yaml(__package__, "{{architecture_file.name}}")
 
 {% endif %}
```

## aac/plugins/first_party/gen_plugin/templates/third_party/plugin_impl.py.jinja2

```diff
@@ -6,16 +6,16 @@
 
 plugin_name = "{{plugin.name}}"
 {% for command in commands %}
 {%+ set comma_joiner = joiner(", ") %}
 
 def {{command.implementation_name}}({% for command_input in command.input %}{{comma_joiner()}}{{command_input.name | trim('-') }}: {{command_input.python_type}}{% endfor %}) -> PluginExecutionResult:
     """
-    {% if command.description is defined %}
-    {{command.description}}
+    {% if command.helpText is defined %}
+    {{command.helpText}}
     {% else %}
     TODO: Write a description
     {% endif %}
     {% if command.input is defined %}
 
     Args:
     {%- for command_input in command.input +%}
```

## aac/plugins/first_party/gen_plugin/templates/third_party/setup.py.jinja2

```diff
@@ -4,25 +4,25 @@
 
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     readme_description = fh.read()
 
 runtime_dependencies = [
-    "aac"
+    "aac ~= {{aac_version}}"
 ]
 
 test_dependencies = [
-    "nose2 >= 0.10.0",
-    "coverage >= 6.0",
-    "flake8 >= 3.9",
-    "flake8-docstrings >= 1.6.0",
-    "flake8-fixme >= 1.1.1",
-    "flake8-eradicate >= 1.2.0",
-    "flake8-assertive >= 1.3.0",
+    "nose2 ~= 0.10.0",
+    "coverage ~= 6.0",
+    "flake8 ~= 4.0",
+    "flake8-docstrings ~= 1.6.0",
+    "flake8-fixme ~= 1.1.1",
+    "flake8-eradicate ~= 1.2.0",
+    "flake8-assertive ~= 1.3.0",
 ]
 
 setup(
     version="0.0.1",
     name="{{plugin.name}}",
     packages=find_packages(where=".", exclude="tests"),
     package_data={"": ["*.aac", "*.jinja2", "*.yaml"]},
```

## aac/plugins/first_party/gen_plugin/templates/third_party/test_plugin_impl.py.jinja2

```diff
@@ -2,15 +2,15 @@
 
 from aac.plugins.plugin_execution import PluginExecutionStatusCode
 
 {%+ set comma_joiner = joiner(", ") %}
 from {{plugin.implementation_name}}.{{plugin.implementation_name}}_impl import {% for command in commands %}{{comma_joiner()}}{{command.implementation_name}}{% endfor %}
 
 
-class Test{{plugin.name | title | replace('-', '')}}(TestCase):
+class Test{{plugin.name | title | replace('-', '') | replace(' ', '')}}(TestCase):
 
     {% for command in commands %}
     def test_{{command.implementation_name}}(self):
         # TODO: Write tests for {{command.implementation_name}}
 
         {% for argument in command.input %}
         {{argument.name}} = {{argument.type}}()
```

## aac/plugins/first_party/gen_protobuf/gen_protobuf.yaml

```diff
@@ -1,23 +1,27 @@
-model:
-  name: gen-protobuf
-  description: gen-protobuf is an Architecture-as-Code plugin that generates protobuf message definitions from Architecture-as-Code models.
-  behavior:
+plugin:
+  name: Generate Protobuf Messages
+  description: An AaC plugin that generates Protobuf message definitions from AaC definitions.
+  commands:
     - name: gen-protobuf
-      type: command
-      description: Generate protobuf messages from Arch-as-Code models
+      group: Generation
+      helpText: Generate Protobuf messages from AaC definitions.
       input:
         - name: architecture-file
           type: file
           python_type: str
-          description: The yaml file containing the data models to generate as Protobuf messages.
+          description: |
+            The YAML file containing the schema definitions from which to
+            generate Protobuf messages.
         - name: output-directory
           type: directory
           python_type: str
-          description: The directory to write the generated Protobuf messages to.
+          description: |
+            The output directory into which the generated Protobuf messages will
+            be written.
       acceptance:
         - scenario: Output protobuf messages for behavior input/output entries in an Architecture model.
           given:
             - The {{gen-protobuf.input.architecture-file}} contains a valid architecture.
           when:
             - The aac app is run with the gen-protobuf command and a valid architecture file.
           then:
@@ -38,22 +42,58 @@
       - sint64
       - fixed32
       - fixed64
       - bool
       - string
       - bytes
 ---
+schema:
+  name: Map
+  description: Defines a map/key-value pair data structure, and the typing.
+  fields:
+    - name: name
+      type: string
+      description: The name of the Map type
+    - name: key_type
+      type: string
+      description: The key type for elements in the map.
+    - name: value_type
+      type: string
+      description: The value type for elements in the map.
+  validation:
+    - name: Required fields are present
+      arguments:
+        - name
+        - key_type
+        - value_type
+---
+schema:
+  name: KeyValuePair
+  description: Defines a key-value pair, use in list to create key-value pairs in AaC.
+  fields:
+    - name: key
+      type: string
+      description: The key map entry.
+    - name: value
+      type: string
+      description: The value map entry.
+  validation:
+    - name: Required fields are present
+      arguments:
+        - key
+        - value
+---
 ext:
    name: SchemaMessageOptions
-   type: schema
+   type: Schema
    schemaExt:
       add:
         - name: protobuf_message_options
           type: KeyValuePair[]
 ---
 ext:
    name: EnumMessageOptions
-   type: enum
+   type: Enum
    schemaExt:
       add:
         - name: protobuf_message_options
-          type: KeyValuePair[]
+          type: KeyValuePair[]
```

## aac/plugins/first_party/gen_protobuf/gen_protobuf_impl.py

```diff
@@ -1,25 +1,38 @@
-"""AaC Plugin implementation module for the aac-gen-protobuf plugin."""
+"""AaC Plugin implementation module for the Generate Protobuf Messages plugin."""
 
 import logging
 import os
 import re
 
+from aac.lang.constants import (
+    DEFINITION_FIELD_BEHAVIOR,
+    DEFINITION_FIELD_DESCRIPTION,
+    DEFINITION_FIELD_FIELDS,
+    DEFINITION_FIELD_INPUT,
+    DEFINITION_FIELD_NAME,
+    DEFINITION_FIELD_OUTPUT,
+    DEFINITION_FIELD_TYPE,
+    DEFINITION_FIELD_VALUES,
+    ROOT_KEY_ENUM,
+    ROOT_KEY_MODEL,
+    ROOT_KEY_SCHEMA,
+)
 from aac.lang.definitions.definition import Definition
 from aac.lang.definitions.type import is_array_type, remove_list_type_indicator
 from aac.lang.definitions.collections import get_definitions_by_root_key
 from aac.lang.definitions.search import search_definition
 from aac.lang.active_context_lifecycle_manager import get_active_context
 from aac.lang.language_context import LanguageContext
 from aac.plugins import PluginError
 from aac.plugins.plugin_execution import PluginExecutionResult, plugin_result
 from aac.templates.engine import TemplateOutputFile, generate_template, load_templates, write_generated_templates_to_file
 from aac.validate import validated_source
 
-plugin_name = "gen-protobuf"
+plugin_name = "Generate Protobuf Messages"
 
 
 def gen_protobuf(architecture_file: str, output_directory: str) -> PluginExecutionResult:
     """
     Gen-protobuf plugin command entry point. Generate protobuf messages from Arch-as-Code models.
 
     Args:
@@ -44,15 +57,15 @@
     # Validate the source AaC file and its contents
     with validated_source(architecture_file) as validation_result:
         loaded_templates = load_templates(__package__, ".")
 
         # Get the validated model definitions
         validated_definitions = validation_result.definitions
         get_active_context().add_definitions_to_context(validated_definitions)
-        model_definitions = get_definitions_by_root_key("model", validated_definitions)
+        model_definitions = get_definitions_by_root_key(ROOT_KEY_MODEL, validated_definitions)
 
         model_interface_messages = _get_model_interface_data_structures(model_definitions)
         protobuf_message_template_properties = _get_message_template_properties(model_interface_messages)
 
         generated_template_messages = _generate_protobuf_messages(
             loaded_templates,
             output_directory,
@@ -91,45 +104,48 @@
             all_message_definitions.update(message_sub_structures)
 
     return all_message_definitions
 
 
 def _get_model_behavior_input_output_definitions(model_definition: Definition) -> dict[str, Definition]:
     """Return a list of definitions that are defined in the input and output of model behavior's."""
-    model_behavior_keys = ["model", "behavior"]
+    model_behavior_keys = [ROOT_KEY_MODEL, DEFINITION_FIELD_BEHAVIOR]
 
     model_interface_messages = []
-    model_interface_messages += search_definition(model_definition, model_behavior_keys + ["input"])
-    model_interface_messages += search_definition(model_definition, model_behavior_keys + ["output"])
-    model_interface_message_names = [field.get("type") for field in model_interface_messages]
+    model_interface_messages += search_definition(model_definition, model_behavior_keys + [DEFINITION_FIELD_INPUT])
+    model_interface_messages += search_definition(model_definition, model_behavior_keys + [DEFINITION_FIELD_OUTPUT])
+    model_interface_message_names = [field.get(DEFINITION_FIELD_TYPE) for field in model_interface_messages]
 
     active_context = get_active_context()
     interface_definitions = [active_context.get_definition_by_name(name) for name in model_interface_message_names]
 
     return {interface_def.name: interface_def for interface_def in interface_definitions}
 
 
 def _get_embedded_data_structures(schema_definition: Definition, active_context: LanguageContext) -> dict[str, Definition]:
     """Return a dict of schema definition structures that make up the structure of the definition."""
 
     interface_message_substructures = {}
-    definition_names_to_traverse = set([field.get("type") for field in schema_definition.get_top_level_fields().get("fields")])
+    definition_names_to_traverse = set(
+        [field.get(DEFINITION_FIELD_TYPE) for field in schema_definition.get_top_level_fields().get(DEFINITION_FIELD_FIELDS)]
+    )
 
     while len(definition_names_to_traverse) > 0:
         target_definition_name = definition_names_to_traverse.pop()
         target_definition = active_context.get_definition_by_name(target_definition_name)
 
         if target_definition:
 
             if target_definition.name not in interface_message_substructures:
                 interface_message_substructures[target_definition.name] = target_definition
 
             if target_definition.is_schema():
                 target_definition_field_types = [
-                    field.get("type") for field in target_definition.get_top_level_fields().get("fields")
+                    field.get(DEFINITION_FIELD_TYPE)
+                    for field in target_definition.get_top_level_fields().get(DEFINITION_FIELD_FIELDS)
                 ]
 
                 # filter out already visited definitions
                 filtered_target_field_types = list(
                     filter(lambda type: type not in interface_message_substructures, target_definition_field_types)
                 )
                 definition_names_to_traverse.update(filtered_target_field_types)
@@ -178,15 +194,15 @@
         imports (list): A list of model imports
         options (dict): A list of message options
 
     Returns:
         A dictionary containing the properties in a consistent structure.
     """
     active_context = get_active_context()
-    file_type = "enum" if active_context.is_enum_type(name) else "schema"
+    file_type = ROOT_KEY_ENUM if active_context.is_enum_type(name) else ROOT_KEY_SCHEMA
 
     # Check if the value is a string, then format the string value it properly for protobuf.
     for option_entry in options:
         option_value = option_entry.get("value")
 
         if type(option_value) is str:
             option_entry["value"] = f'"{option_value}"'
@@ -197,17 +213,17 @@
     name = _sanitize_string_to_pascal_case(name)
 
     # Format the enum values
     enums = [_sanitize_string_to_snake_case(enum).upper() for enum in enums]
 
     # Format the field strings
     for field in fields:
-        field["name"] = _sanitize_string_to_snake_case(field.get("name"))
-        if field["type"] not in active_context.get_primitive_types():
-            field["type"] = _sanitize_string_to_pascal_case(field.get("type"))
+        field[DEFINITION_FIELD_NAME] = _sanitize_string_to_snake_case(field.get(DEFINITION_FIELD_NAME))
+        if field[DEFINITION_FIELD_TYPE] not in active_context.get_primitive_types():
+            field[DEFINITION_FIELD_TYPE] = _sanitize_string_to_pascal_case(field.get(DEFINITION_FIELD_TYPE))
 
     return {
         "message_name": name,
         "message_description": description,
         "file_type": file_type,
         "enums": enums,
         "fields": fields,
@@ -224,16 +240,16 @@
         enum_definition (dict): An enum definition as a dictionary
 
     Returns:
          A dictionary containing the template generation properties.
     """
     enum_name = enum_definition.name
     enum_definition_fields = enum_definition.get_top_level_fields()
-    enum_values = enum_definition_fields.get("values") or []
-    enum_description = enum_definition_fields.get("description") or ""
+    enum_values = enum_definition_fields.get(DEFINITION_FIELD_VALUES) or []
+    enum_description = enum_definition_fields.get(DEFINITION_FIELD_DESCRIPTION) or ""
     description_as_proto_comment = _convert_description_to_protobuf_comment(enum_description)
     definition_options = enum_definition_fields.get("protobuf_message_options") or []
 
     return _to_template_properties_dict(enum_name, description_as_proto_comment, enums=enum_values, options=definition_options)
 
 
 def _get_schema_properties(interface_structures: dict[str, Definition], data_definition: Definition) -> dict[str, any]:
@@ -245,27 +261,27 @@
         data_model (dict): A data model definition as a dictionary
 
     Returns:
          A dictionary containing the template generation properties.
     """
     active_context = get_active_context()
     definition_fields = data_definition.get_top_level_fields()
-    structure_fields = definition_fields.get("fields")
+    structure_fields = definition_fields.get(DEFINITION_FIELD_FIELDS)
 
     definition_name = data_definition.name
-    definition_description = definition_fields.get("description") or ""
+    definition_description = definition_fields.get(DEFINITION_FIELD_DESCRIPTION) or ""
     definition_description_as_proto_comment = _convert_description_to_protobuf_comment(definition_description)
     definition_options = definition_fields.get("protobuf_message_options") or []
 
     message_fields = []
     message_imports = []
     for field in structure_fields:
-        proto_field_name = field.get("name")
-        proto_field_description = field.get("description") or ""
-        proto_field_type = field.get("type")
+        proto_field_name = field.get(DEFINITION_FIELD_NAME)
+        proto_field_description = field.get(DEFINITION_FIELD_DESCRIPTION) or ""
+        proto_field_type = field.get(DEFINITION_FIELD_TYPE)
         sanitized_proto_field_type = remove_list_type_indicator(proto_field_type)
         description_as_proto_comment = _convert_description_to_protobuf_comment(proto_field_description, 1)
 
         message_fields.append(
             {
                 "name": proto_field_name,
                 "description": description_as_proto_comment,
@@ -435,15 +451,15 @@
     return converted_string
 
 
 def _convert_description_to_protobuf_comment(description: str, indent_level: int = 0) -> str:
     """
     Return the description as a protobuf multiline comment.
 
-    The returned string is expected to slot into a template multitine comment like such:
+    The returned string is expected to slot into a template multiline comment like such:
         1. The first line isn't indented or starred
         2. every subsequent line break is indented and starred
     """
     space_indent = "  "
     additional_space_indent = space_indent * indent_level
 
     if description:
@@ -458,15 +474,15 @@
             comment_newline_value = os.linesep
             comment_line_prefix = f"{additional_space_indent} * "
 
             # if the first line in the description, don't add a line prefix
             if i == 0:
                 comment_line_prefix = ""
 
-            # if the final line in the description, don't add a line seperator
+            # if the final line in the description, don't add a line separator
             if i == len(description_newlines) - 1:
                 comment_newline_value = " */"
 
             formatted_multiline_comment += f"{comment_line_prefix}{comment_line}{comment_newline_value}"
     else:
         formatted_multiline_comment = ""
```

## aac/plugins/first_party/help_dump/help-dump.yaml

```diff
@@ -1,17 +1,16 @@
-model:
-  name: help-dump
+plugin:
+  name: Dump AaC Commands
   description: |
-    An Architecture-as-Code plugin that produces a consistently-formatted representation of all the commands, command
-    arguments, and descriptions for each.
-  behavior:
+    An AaC plugin that produces a consistently-formatted representation of all
+    the AaC commands and their corresponding attributes.
+  commands:
     - name: help-dump
-      type: command
-      description: |
-        Produce a formatted string containing all commands, their arguments, and each of their descriptions.
+      group: Internal
+      helpText: Produce a formatted string containing all AaC commands and their attributes.
       output:
         - name: help-output
           type: string
           python_type: str
           description: The formatted string with all commands, etc.
       acceptance:
         - scenario: Output formatted help string.
```

## aac/plugins/first_party/help_dump/help_dump_impl.py

```diff
@@ -1,16 +1,16 @@
-"""AaC Plugin implementation module for the help-dump plugin."""
+"""AaC Plugin implementation module for the Dump Commands plugin."""
 
 import json
 
 from aac.lang.active_context_lifecycle_manager import get_active_context
 from aac.plugins.plugin_execution import PluginExecutionResult, plugin_result
 from aac.serialization import AacCommandEncoder
 
-plugin_name = "help-dump"
+plugin_name = "Dump Commands"
 
 
 def help_dump() -> PluginExecutionResult:
     """
     Produce a formatted string containing all commands, their arguments, and each of their descriptions.
 
     Returns:
```

## aac/plugins/first_party/lsp_server/language_server.py

```diff
@@ -1,19 +1,18 @@
 """The Architecture-as-Code Language Server."""
 import difflib
 import logging
-
 from asyncio import ensure_future
 from os import linesep
-from typing import Optional
-
+from typing import Any, Optional
 from pygls.lsp import (
     CompletionOptions,
     CompletionParams,
     DefinitionParams,
+    DocumentLinkParams,
     DidChangeTextDocumentParams,
     DidCloseTextDocumentParams,
     DidOpenTextDocumentParams,
     HoverParams,
     PublishDiagnosticsParams,
     ReferenceParams,
     RenameParams,
@@ -23,18 +22,20 @@
 )
 from pygls.protocol import LanguageServerProtocol
 from pygls.server import LanguageServer
 from pygls.uris import to_fs_path
 
 from aac import __version__ as AAC_VERSION
 from aac.io.parser import parse
+from aac.io.parser._parser_error import ParserError
 from aac.lang.active_context_lifecycle_manager import get_initialized_language_context
 from aac.lang.language_context import LanguageContext
 from aac.plugins.first_party.lsp_server.managed_workspace_file import ManagedWorkspaceFile
 from aac.plugins.first_party.lsp_server.providers.code_completion_provider import CodeCompletionProvider
+from aac.plugins.first_party.lsp_server.providers.document_link_provider import DocumentLinkProvider
 from aac.plugins.first_party.lsp_server.providers.find_references_provider import FindReferencesProvider
 from aac.plugins.first_party.lsp_server.providers.goto_definition_provider import GotoDefinitionProvider
 from aac.plugins.first_party.lsp_server.providers.hover_provider import HoverProvider
 from aac.plugins.first_party.lsp_server.providers.lsp_provider import LspProvider
 from aac.plugins.first_party.lsp_server.providers.prepare_rename_provider import PrepareRenameProvider
 from aac.plugins.first_party.lsp_server.providers.publish_diagnostics_provider import PublishDiagnosticsProvider
 from aac.plugins.first_party.lsp_server.providers.rename_provider import RenameProvider
@@ -82,18 +83,19 @@
         self.configure_providers()
         self.setup_features()
 
     def configure_providers(self):
         """Configure and setup the providers that make LSP functionality available for the AaC LSP server."""
         self.providers[methods.COMPLETION] = self.providers.get(methods.COMPLETION, CodeCompletionProvider())
         self.providers[methods.DEFINITION] = self.providers.get(methods.DEFINITION, GotoDefinitionProvider())
-        self.providers[methods.REFERENCES] = self.providers.get(methods.REFERENCES, FindReferencesProvider())
+        self.providers[methods.DOCUMENT_LINK] = self.providers.get(methods.DOCUMENT_LINK, DocumentLinkProvider())
         self.providers[methods.HOVER] = self.providers.get(methods.HOVER, HoverProvider())
-        self.providers[methods.RENAME] = self.providers.get(methods.RENAME, RenameProvider())
         self.providers[methods.PREPARE_RENAME] = self.providers.get(methods.PREPARE_RENAME, PrepareRenameProvider())
+        self.providers[methods.REFERENCES] = self.providers.get(methods.REFERENCES, FindReferencesProvider())
+        self.providers[methods.RENAME] = self.providers.get(methods.RENAME, RenameProvider())
         self.providers[methods.TEXT_DOCUMENT_SEMANTIC_TOKENS_FULL] = self.providers.get(
             methods.TEXT_DOCUMENT_SEMANTIC_TOKENS_FULL, SemanticTokensProvider()
         )
         self.providers[methods.TEXT_DOCUMENT_PUBLISH_DIAGNOSTICS] = self.providers.get(
             methods.TEXT_DOCUMENT_PUBLISH_DIAGNOSTICS, PublishDiagnosticsProvider()
         )
 
@@ -104,20 +106,21 @@
         self.feature(methods.TEXT_DOCUMENT_DID_OPEN)(did_open)
         self.feature(methods.TEXT_DOCUMENT_DID_CLOSE)(did_close)
         self.feature(methods.TEXT_DOCUMENT_DID_CHANGE)(did_change)
 
         trigger_and_commit_chars = self.providers.get(methods.COMPLETION).get_trigger_characters()
         completion_options = CompletionOptions(trigger_characters=trigger_and_commit_chars)
         self.feature(methods.COMPLETION, completion_options)(handle_completion)
-        self.feature(methods.HOVER)(handle_hover)
         self.feature(methods.DEFINITION)(handle_goto_definition)
+        self.feature(methods.DOCUMENT_LINK)(handle_document_link)
+        self.feature(methods.HOVER)(handle_hover)
+        self.feature(methods.PREPARE_RENAME)(handle_prepare_rename)
         self.feature(methods.REFERENCES)(handle_references)
         self.feature(methods.RENAME)(handle_rename)
         self.feature(methods.TEXT_DOCUMENT_PUBLISH_DIAGNOSTICS)(handle_publish_diagnostics)
-        self.feature(methods.PREPARE_RENAME)(handle_prepare_rename)
 
         semantic_tokens_legend = self.providers.get(methods.TEXT_DOCUMENT_SEMANTIC_TOKENS_FULL).get_semantic_tokens_legend()
         self.feature(methods.TEXT_DOCUMENT_SEMANTIC_TOKENS_FULL, semantic_tokens_legend)(handle_semantic_tokens)
 
 
 async def did_open(ls: AacLanguageServer, params: DidOpenTextDocumentParams):
     """Text document did open notification."""
@@ -128,15 +131,22 @@
 
     if not managed_file:
         managed_file = ManagedWorkspaceFile(file_uri)
         ls.workspace_files[file_uri] = managed_file
 
     managed_file.is_client_managed = True
     file_path = to_fs_path(file_uri)
-    ls.language_context.add_definitions_to_context(parse(file_path))
+    try:
+        file_definitions = parse(file_path)
+    except ParserError as error:
+        raise ParserError(error.source, error.errors) from None
+    if file_definitions:
+        ls.language_context.add_definitions_to_context(file_definitions)
+    else:
+        logging.error(f"Failed to parse definitions from document {file_path}")
 
     ensure_future(handle_publish_diagnostics(ls, PublishDiagnosticsParams(uri=params.text_document.uri, diagnostics=[])))
 
 
 async def did_close(ls: AacLanguageServer, params: DidCloseTextDocumentParams):
     """Text document did close notification."""
     logging.info(f"Text document closed by LSP client {params.text_document.uri}.")
@@ -150,101 +160,96 @@
     """Text document did change notification."""
     document_path = to_fs_path(params.text_document.uri)
     logging.info(f"Text document altered by LSP client {document_path}.")
 
     ensure_future(handle_publish_diagnostics(ls, PublishDiagnosticsParams(uri=params.text_document.uri, diagnostics=[])))
 
     file_content = params.content_changes[0].text
-    incoming_definitions_dict = {definition.name: definition for definition in parse(file_content, document_path)}
-    new_definitions = []
-    altered_definitions = []
-
-    old_definitions = ls.language_context.get_definitions_by_file_uri(document_path)
-    old_definitions_to_update_dict = {
-        definition.name: definition for definition in old_definitions if definition.name in incoming_definitions_dict
-    }
-    old_definitions_to_delete = [
-        definition for definition in old_definitions if definition.name not in incoming_definitions_dict
-    ]
-
-    for incoming_definition_name, incoming_definition in incoming_definitions_dict.items():
-        old_definition = old_definitions_to_update_dict.get(incoming_definition_name)
-
-        if old_definition:
-            incoming_definition.uid = old_definition.uid
-            altered_definitions.append(incoming_definition)
-
-            old_definition_lines = old_definition.to_yaml().split(linesep)
-            altered_definition_lines = incoming_definition.to_yaml().split(linesep)
-            changes = linesep.join(list(difflib.ndiff(old_definition_lines, altered_definition_lines))).strip()
-            logging.info(f"Updating definition: {old_definition.name}.\n Differences:\n{changes}")
-        else:
-            logging.info(f"Adding definition: {incoming_definition.name}.")
-            new_definitions.append(incoming_definition)
-
-    ls.language_context.add_definitions_to_context(new_definitions)
-    ls.language_context.update_definitions_in_context(altered_definitions)
-    ls.language_context.remove_definitions_from_context(old_definitions_to_delete)
+    try:
+        incoming_definitions_dict = {definition.name: definition for definition in parse(file_content, document_path)}
+    except ParserError as error:
+        raise ParserError(error.source, error.errors) from None
+    else:
+        new_definitions = []
+        altered_definitions = []
+
+        old_definitions = ls.language_context.get_definitions_by_file_uri(document_path)
+        old_definitions_to_update_dict = {
+            definition.name: definition for definition in old_definitions if definition.name in incoming_definitions_dict
+        }
+        old_definitions_to_delete = [
+            definition for definition in old_definitions if definition.name not in incoming_definitions_dict
+        ]
+
+        for incoming_definition_name, incoming_definition in incoming_definitions_dict.items():
+            old_definition = old_definitions_to_update_dict.get(incoming_definition_name)
+
+            if old_definition:
+                incoming_definition.uid = old_definition.uid
+                altered_definitions.append(incoming_definition)
+
+                old_definition_lines = old_definition.to_yaml().split(linesep)
+                altered_definition_lines = incoming_definition.to_yaml().split(linesep)
+                changes = linesep.join(list(difflib.ndiff(old_definition_lines, altered_definition_lines))).strip()
+                logging.info(f"Updating definition: {old_definition.name}.\n Differences:\n{changes}")
+            else:
+                logging.info(f"Adding definition: {incoming_definition.name}.")
+                new_definitions.append(incoming_definition)
+
+        ls.language_context.add_definitions_to_context(new_definitions)
+        ls.language_context.update_definitions_in_context(altered_definitions)
+        ls.language_context.remove_definitions_from_context(old_definitions_to_delete)
 
 
 async def handle_completion(ls: AacLanguageServer, params: CompletionParams):
     """Handle the completion request."""
-    code_completion_provider = ls.providers.get(methods.COMPLETION)
-    completion_results = code_completion_provider.handle_request(ls, params)
-    logging.debug(f"Completion results: {completion_results}")
-    return completion_results
+    return _provider_handle_request(methods.COMPLETION, ls, params)
+
+
+async def handle_document_link(ls: AacLanguageServer, params: DocumentLinkParams):
+    """Handle the completion request."""
+    return _provider_handle_request(methods.DOCUMENT_LINK, ls, params)
 
 
 async def handle_hover(ls: AacLanguageServer, params: HoverParams):
     """Handle the hover request."""
-    hover_provider = ls.providers.get(methods.HOVER)
-    hover_results = hover_provider.handle_request(ls, params)
-    logging.debug(f"Hover results: {hover_results}")
-    return hover_results
+    return _provider_handle_request(methods.HOVER, ls, params)
 
 
 async def handle_goto_definition(ls: AacLanguageServer, params: DefinitionParams):
     """Handle the goto definition request."""
-    goto_definition_provider = ls.providers.get(methods.DEFINITION)
-    goto_definition_results = goto_definition_provider.handle_request(ls, params)
-    logging.debug(f"Goto Definition results: {goto_definition_results}")
-    return goto_definition_results
+    return _provider_handle_request(methods.DEFINITION, ls, params)
 
 
 async def handle_references(ls: AacLanguageServer, params: ReferenceParams):
     """Handle the find references request."""
-    find_references_provider = ls.providers.get(methods.REFERENCES)
-    find_references_results = find_references_provider.handle_request(ls, params)
-    logging.debug(f"Find references results: {find_references_results}")
-    return find_references_results
+    return _provider_handle_request(methods.REFERENCES, ls, params)
 
 
 async def handle_rename(ls: AacLanguageServer, params: RenameParams):
     """Handle the rename definition request."""
-    rename_provider = ls.providers.get(methods.RENAME)
-    rename_results = rename_provider.handle_request(ls, params)
-    logging.debug(f"Rename results: {rename_results}")
-    return rename_results
+    return _provider_handle_request(methods.RENAME, ls, params)
 
 
 async def handle_prepare_rename(ls: AacLanguageServer, params: RenameParams):
     """Handle the prepare rename definition request."""
-    prepare_rename_provider = ls.providers.get(methods.PREPARE_RENAME)
-    prepare_rename_results = prepare_rename_provider.handle_request(ls, params)
-    logging.debug(f"Prepare rename results: {prepare_rename_results}")
-    return prepare_rename_results
+    return _provider_handle_request(methods.PREPARE_RENAME, ls, params)
 
 
 async def handle_semantic_tokens(ls: AacLanguageServer, params: SemanticTokensParams):
     """Handle the semantic tokens request."""
-    semantic_tokens_provider = ls.providers.get(methods.TEXT_DOCUMENT_SEMANTIC_TOKENS_FULL)
-    semantic_tokens_results = semantic_tokens_provider.handle_request(ls, params)
-    logging.debug(f"Semantic tokens results: {semantic_tokens_results}")
-    return semantic_tokens_results
+    return _provider_handle_request(methods.TEXT_DOCUMENT_SEMANTIC_TOKENS_FULL, ls, params)
 
 
 async def handle_publish_diagnostics(ls: AacLanguageServer, params: PublishDiagnosticsParams):
     """Handle the publish diagnostics request."""
-    publish_diagnostics_provider = ls.providers.get(methods.TEXT_DOCUMENT_PUBLISH_DIAGNOSTICS)
-    diagnostics_results = await publish_diagnostics_provider.handle_request(ls, params)
-    logging.debug(f"Publish Diagnostics results: {diagnostics_results}")
-    return diagnostics_results
+    return _provider_handle_request(methods.TEXT_DOCUMENT_PUBLISH_DIAGNOSTICS, ls, params)
+
+
+def _provider_handle_request(provider_name: str, ls: AacLanguageServer, params: Any):
+    provider = ls.providers.get(provider_name)
+
+    if provider:
+        results = provider.handle_request(ls, params)
+        return results
+    else:
+        logging.warning(f"No provider found for '{provider_name}'.")
```

## aac/plugins/first_party/lsp_server/lsp-server.yaml

```diff
@@ -1,39 +1,39 @@
-model:
-  name: lsp-server
-  description: Start the LSP server
-  behavior:
+plugin:
+  name: LSP Server
+  description: An AaC plugin that can be used to start the AaC LSP server.
+  commands:
     - name: start-lsp-io
-      type: command
-      description: Start the AaC Language Server Protocol (LSP) server in IO mode
+      group: Backend
+      helpText: Start the AaC Language Server Protocol (LSP) server in IO mode.
       acceptance:
-        - scenario: Start the LSP server in IO mode
+        - scenario: Start the LSP server in IO mode.
           given:
             - The LSP server is not currently running.
           when:
             - The aac application is run with the start-lsp-io command.
           then:
             - The AaC LSP server is started in IO mode.
-            - Messages to and from the LSP occur over system IO
+            - Messages to and from the LSP occur over system IO.
     - name: start-lsp-tcp
-      type: command
-      description: Start the AaC Language Server Protocol (LSP) server in TCP mode
+      group: Backend
+      helpText: Start the AaC Language Server Protocol (LSP) server in TCP mode.
       input:
         - name: --host
           type: string
           python_type: str
-          description: The host address to bind the TCP server to.
+          description: The host address to which the TCP server will be bound.
           default: 127.0.0.1
         - name: --port
           type: number
           python_type: int
-          description: The host port to bing the TCP server to.
+          description: The host port to which the TCP server will be bound.
           default: 5007
       acceptance:
-        - scenario: Start the LSP server in TCP mode
+        - scenario: Start the LSP server in TCP mode.
           given:
             - The LSP server is not currently running.
           when:
             - The aac application is run with the start-lsp-tcp command.
           then:
             - The AaC LSP server is started in TCP mode.
-            - Messages to and from the LSP occur over a TCP connection
+            - Messages to and from the LSP occur over a TCP connection.
```

## aac/plugins/first_party/lsp_server/start_lsp_server_impl.py

```diff
@@ -1,14 +1,15 @@
-"""AaC Plugin implementation module for the start-lsp plugin."""
+"""AaC Plugin implementation module for the LSP Server plugin."""
 
 from typing import Callable
+
 from aac.plugins.first_party.lsp_server.language_server import AacLanguageServer
 from aac.plugins.plugin_execution import PluginExecutionResult, plugin_result
 
-plugin_name = "start-lsp"
+plugin_name = "LSP Server"
 
 
 def start_lsp_io():
     """Start the LSP server in IO mode."""
     aac_language_server = AacLanguageServer()
     return _start_lsp(aac_language_server.start_io)
```

## aac/plugins/first_party/lsp_server/providers/code_completion_provider.py

```diff
@@ -4,14 +4,15 @@
 import logging
 from attr import Factory, attrib, attrs, validators
 
 from pygls.lsp import CompletionParams, CompletionList, CompletionItem, CompletionItemKind
 from pygls.server import LanguageServer
 
 from aac.io.parser import parse
+from aac.io.parser._parser_error import ParserError
 from aac.lang.active_context_lifecycle_manager import get_active_context
 from aac.lang.definitions.collections import get_definitions_by_root_key
 from aac.lang.definitions.definition import Definition
 from aac.plugins.first_party.lsp_server.providers.lsp_provider import LspProvider
 
 SPACE_TRIGGER = " "
 
@@ -67,27 +68,31 @@
     if primitives_definition:
         primitive_references = {field: "Primitive type" for field in active_context.get_primitive_types()}
 
     schema_definition_references = _convert_definitions_to_name_description_dict(
         active_context.get_definitions_by_root_key("schema")
     )
 
-    file_definitions = parse(_get_code_completion_parent_text_file(language_server, params))
-    file_schema_references = _convert_definitions_to_name_description_dict(
-        get_definitions_by_root_key("schema", file_definitions)
-    )
-    available_references = primitive_references | schema_definition_references | file_schema_references
-
-    return CompletionList(
-        is_incomplete=False,
-        items=[
-            CompletionItem(label=name, kind=CompletionItemKind.Reference, documentation=description)
-            for name, description in available_references.items()
-        ],
-    )
+    try:
+        file_definitions = parse(_get_code_completion_parent_text_file(language_server, params))
+    except ParserError as error:
+        raise ParserError(error.source, error.errors) from None
+    else:
+        file_schema_references = _convert_definitions_to_name_description_dict(
+            get_definitions_by_root_key("schema", file_definitions)
+        )
+        available_references = primitive_references | schema_definition_references | file_schema_references
+
+        return CompletionList(
+            is_incomplete=False,
+            items=[
+                CompletionItem(label=name, kind=CompletionItemKind.Reference, documentation=description)
+                for name, description in available_references.items()
+            ],
+        )
 
 
 def _get_code_completion_parent_text_file(language_server: LanguageServer, params: CompletionParams):
     return language_server.workspace.documents.get(params.text_document.uri).source
 
 
 def _convert_definitions_to_name_description_dict(definitions: list[Definition]) -> dict:
```

## aac/plugins/first_party/lsp_server/providers/find_references_provider.py

```diff
@@ -70,15 +70,15 @@
         if SymbolType.DEFINITION_NAME in symbol_types:
             definition_to_find = language_context.get_definition_by_name(name)
             if not definition_to_find:
                 logging.warn(f"Can't find references for non-definition {name}")
             else:
                 locations.extend(self.get_definition_name_reference_locations(definition_to_find, language_context))
 
-        if SymbolType.ROOT_KEY_NAME in symbol_types:
+        if SymbolType.ROOT_KEY in symbol_types:
             locations.extend(self.get_root_key_reference_locations(name, language_context))
 
         return locations
 
     def get_definition_name_reference_locations(
         self, definition_to_find: Definition, language_context: LanguageContext
     ) -> list[Location]:
```

## aac/plugins/first_party/lsp_server/providers/goto_definition_provider.py

```diff
@@ -72,15 +72,15 @@
                 locations.extend(self.get_definition_name_lexeme_location(definition_to_find))
 
         if SymbolType.ENUM_VALUE_TYPE in symbol_types:
             definition_to_find = language_context.get_enum_definition_by_type(name)
             if definition_to_find:
                 locations.extend(self.get_enum_value_lexeme_location(definition_to_find, name))
 
-        if SymbolType.ROOT_KEY_NAME in symbol_types:
+        if SymbolType.ROOT_KEY in symbol_types:
             definition_to_find = language_context.get_root_keys_definition()
             if definition_to_find:
                 locations.extend(self.get_root_key_definition_lexeme_location(definition_to_find, name))
 
         return locations
 
     def get_definition_name_lexeme_location(self, definition: Definition) -> list[Location]:
@@ -90,19 +90,16 @@
         Args:
             definition (Definition): The definition to pull the name lexeme from.
 
 
         Returns:
             A list, probably consisting of only one element, of locations corresponding to lexemes of definition names
         """
-        def filter_lexeme_by_reference_name(lexeme: Lexeme) -> bool:
-            return lexeme.value == definition.name
-
         locations = []
-        referencing_lexemes = filter(filter_lexeme_by_reference_name, definition.lexemes)
+        referencing_lexemes = [lexeme for lexeme in definition.lexemes if lexeme.value == definition.name]
         for lexeme in referencing_lexemes:
             previous_lexeme = definition.lexemes[definition.lexemes.index(lexeme) - 1]
             if "name" in previous_lexeme.value:
                 locations.append(get_location_from_lexeme(lexeme))
 
         return locations
```

## aac/plugins/first_party/lsp_server/providers/hover_provider.py

```diff
@@ -13,16 +13,23 @@
 
 class HoverProvider(LspProvider):
     """Provide useful contextual information for the named item being hovered over."""
 
     def handle_request(self, language_server: LanguageServer, params: HoverParams) -> Optional[Hover]:
         """Return the YAML representation of the item at the specified position."""
         document: Optional[Document] = language_server.workspace.documents.get(params.text_document.uri)
-        position = params.position
-        symbol = get_symbol_at_position(document.source, position.line, position.character)
 
-        if symbol is not None:
-            name = remove_list_type_indicator(symbol).strip(":")
-            definition = language_server.language_context.get_definition_by_name(name)
-            return definition and Hover(
-                contents=MarkupContent(kind=MarkupKind.Markdown, value=f"```\n{definition.content}\n```")
-            )
+        return_hover = None
+        if document:
+            position = params.position
+            symbol = get_symbol_at_position(document.source, position.line, position.character)
+
+            if symbol is not None:
+                name = remove_list_type_indicator(symbol).strip(":")
+                definition = language_server.language_context.get_definition_by_name(name)
+
+                if definition:
+                    return_hover = Hover(
+                        contents=MarkupContent(kind=MarkupKind.Markdown, value=f"```\n{definition.content}\n```")
+                    )
+
+        return return_hover
```

## aac/plugins/first_party/lsp_server/providers/lsp_provider.py

```diff
@@ -1,15 +1,14 @@
 """A module containing a base LSP provider."""
-
 from abc import abstractmethod
+from typing import Any
 
-from pygls.lsp.types.basic_structures import Model
 from pygls.server import LanguageServer
 
 
 class LspProvider:
     """A base class used to handle specific LSP requests."""
 
     @abstractmethod
-    def handle_request(self, language_server: LanguageServer, params: Model):
+    def handle_request(self, language_server: LanguageServer, params: Any) -> Any:
         """Handle the specific request."""
         raise NotImplementedError("All LspProviders must implement the handle_request method.")
```

## aac/plugins/first_party/lsp_server/providers/publish_diagnostics_provider.py

```diff
@@ -1,43 +1,67 @@
 """Module for PublishDiagnostics Provider which handles publishing of diagnostics for AaC Language Server."""
-
-from typing import Optional
-
+import logging
 from pygls.lsp import Diagnostic, DiagnosticSeverity, PublishDiagnosticsParams
 from pygls.server import LanguageServer
 from pygls.uris import to_fs_path
+from typing import Optional
 
 from aac.io.parser import parse
+from aac.io.parser._parser_error import ParserError
 from aac.plugins.first_party.lsp_server.conversion_helpers import source_location_to_range
 from aac.plugins.first_party.lsp_server.providers.lsp_provider import LspProvider
 from aac.plugins.validators._validator_finding import ValidatorFinding, FindingSeverity
 from aac.validate._validate import _validate_definitions
 
 
 class PublishDiagnosticsProvider(LspProvider):
     """Handler for Publishing Diagnostics for AaC LSP."""
 
-    async def handle_request(self, ls: LanguageServer, params: PublishDiagnosticsParams) -> list[Diagnostic]:
+    def handle_request(self, ls: LanguageServer, params: PublishDiagnosticsParams) -> list[Diagnostic]:
         """Handle publishing validation findings as diagnostics."""
         self.language_server = ls
         diagnostics = self.get_diagnostics(params.uri)
         ls.publish_diagnostics(params.uri, diagnostics)
         return diagnostics
 
     def get_diagnostics(self, document_uri: str) -> list[Diagnostic]:
         """Add the Diagnostics found on document_uri."""
         findings = self.get_findings_for_document(document_uri)
         return [self.finding_to_diagnostic(finding) for finding in findings]
 
     def get_findings_for_document(self, document_uri: str) -> list[ValidatorFinding]:
-        """Return all the ValidatorFindings for the specified document."""
-        document = self.language_server.workspace.get_document(document_uri)
-        parsed_definitions = parse(document.source, to_fs_path(document_uri))
-        result = _validate_definitions(parsed_definitions, self.language_server.language_context, validate_context=False)
-        return result.findings.get_all_findings()
+        """
+        Return all the ValidatorFindings for the specified document.
+
+        Args:
+            self (PublishDiagnosticsProvider): Instance of class.
+            document_uri (str): Specified document.
+
+        Returns:
+            List of ValidatorFindings for the definitions within the specified document.
+        """
+        findings = []
+
+        if self.language_server.workspace:
+            document = self.language_server.workspace.get_document(document_uri)
+
+            if document:
+                try:
+                    parsed_definitions = parse(document.source, to_fs_path(document_uri))
+                except ParserError as error:
+                    raise ParserError(error.source, error.errors) from None
+                else:
+                    result = _validate_definitions(parsed_definitions, self.language_server.language_context, validate_context=False)
+                    findings = result.findings.get_all_findings()
+            else:
+                logging.debug(f"Can't provide diagnostics, {document_uri} not found in the workspace.")
+        else:
+            logging.debug("Can't provide diagnostics, the workspace doesn't exist in the LSP.")
+
+        return findings
 
     def finding_to_diagnostic(self, finding: ValidatorFinding) -> Diagnostic:
         """Convert a ValidatorFinding to an LSP Diagnostic."""
         severity = self.finding_severity_to_diagnostic_severity(finding.severity)
         return Diagnostic(
             range=source_location_to_range(finding.location.location),
             severity=severity.value if severity else None,
```

## aac/plugins/first_party/lsp_server/providers/rename_provider.py

```diff
@@ -1,14 +1,15 @@
 """Module for the Rename Provider which handles requests to rename symbols."""
 
 import logging
-from typing import Optional
+from typing import List, Optional
 from pygls.server import LanguageServer
 from pygls.lsp.types import Position, RenameParams, WorkspaceEdit, TextEdit, TextDocumentIdentifier
 from pygls.workspace import Document
+from aac.lang.constants import DEFINITION_FIELD_NAME, DEFINITION_FIELD_TYPE
 
 from aac.lang.definitions.definition import Definition
 from aac.lang.language_context import LanguageContext
 from aac.lang.definitions.references import get_definition_type_references_from_list, get_enum_references_from_context
 from aac.lang.definitions.type import remove_list_type_indicator
 from aac.lang.definitions.lexeme import Lexeme
 from aac.plugins.first_party.lsp_server.providers.symbols import (
@@ -19,15 +20,15 @@
 from aac.plugins.first_party.lsp_server.providers.locations import get_location_from_lexeme
 from aac.plugins.first_party.lsp_server.providers.lsp_provider import LspProvider
 
 
 class RenameProvider(LspProvider):
     """Handles the rename requests."""
 
-    def handle_request(self, language_server: LanguageServer, params: RenameParams) -> WorkspaceEdit:
+    def handle_request(self, language_server: LanguageServer, params: RenameParams) -> Optional[WorkspaceEdit]:
         """Return the workspace edit consisting of text edits for the rename request."""
         self.language_server = language_server
         return self.get_rename_edits(
             self.language_server.workspace.documents, params.text_document.uri, params.position, params.new_name
         )
 
     def get_rename_edits(
@@ -48,84 +49,127 @@
             A workspace edit consisting of the text edits spanning all pertinent instances of the selected symbol, or None.
         """
         document = documents.get(current_uri)
         workspace_edit = None
 
         if document:
             symbol = get_symbol_at_position(document.source, position.line, position.character)
-            edits = self._get_rename_edits(symbol, new_name) if symbol else {}
 
             if symbol:
+                edits = self._get_rename_edits(symbol, new_name)
+
                 try:
                     workspace_edit = WorkspaceEdit(text_document=TextDocumentIdentifier(uri=document.uri), changes=edits)
                 except Exception as error:
                     logging.error(error)
 
         return workspace_edit
 
-    def _get_rename_edits(self, symbol: str, new_name: str) -> dict[str, TextEdit]:
+    def _get_rename_edits(self, symbol: str, new_name: str) -> dict[str, list[TextEdit]]:
         """Returns the list of text edits based on the selected symbol's type."""
-        if not symbol:
-            return None
 
-        language_context = self.language_server.language_context
+        # Strip any ':' that accompany yaml keys from the incoming replacement text
+        sanitized_new_name = new_name.strip(":")
+        text_to_replace = remove_list_type_indicator(symbol)
 
-        name = remove_list_type_indicator(symbol).strip(":")
-        symbol_types = get_possible_symbol_types(name, language_context)
+        language_context = self.language_server.language_context
+        symbol_types = get_possible_symbol_types(text_to_replace, language_context)
 
         edits = {}
         if SymbolType.DEFINITION_NAME in symbol_types:
-            definition_to_find = language_context.get_definition_by_name(name)
+            definition_to_find = language_context.get_definition_by_name(text_to_replace)
             if not definition_to_find:
-                logging.warn(f"Can't find references for non-definition {name}")
+                logging.warn(f"Can't find references for non-definition {text_to_replace}")
             else:
-                edits = self._get_definition_name_text_edits(new_name, definition_to_find, language_context)
+                edits = self._get_definition_name_text_edits(sanitized_new_name, definition_to_find, language_context)
 
         if SymbolType.ENUM_VALUE_TYPE in symbol_types:
-            enum_to_find = language_context.get_enum_definition_by_type(name)
+            enum_to_find = language_context.get_enum_definition_by_type(text_to_replace)
             if not enum_to_find:
-                logging.warn(f"Can't find references for non-enum {name}")
+                logging.warn(f"Can't find references for non-enum {text_to_replace}")
             else:
-                edits = self._get_enum_value_type_text_edits(name, new_name, enum_to_find, language_context)
+                edits = self._get_enum_value_type_text_edits(text_to_replace, sanitized_new_name, enum_to_find, language_context)
+
+        if SymbolType.ROOT_KEY in symbol_types:
+            root_fields = language_context.get_root_fields()
+            key_schema_field, *_ = [field for field in root_fields if field.get(DEFINITION_FIELD_NAME) == text_to_replace]
+            definition_to_find = language_context.get_definition_by_name(key_schema_field.get(DEFINITION_FIELD_TYPE))
+
+            if not definition_to_find:
+                logging.critical(f"Can't find the source definition definition '{text_to_replace}'.")
+            else:
+                edits = self._get_root_key_text_edits(text_to_replace, sanitized_new_name, definition_to_find, language_context)
 
         return edits
 
     def _get_definition_name_text_edits(
         self, new_name: str, definition_to_find: Definition, language_context: LanguageContext
-    ) -> dict[str, TextEdit]:
+    ) -> dict[str, list[TextEdit]]:
         """Returns a dictionary of document uri to TextEdits where the uri is the key and the list of edits the value."""
-        edits = {}
+        edits: dict[str, list] = {}
         definition_references = get_definition_type_references_from_list(definition_to_find, language_context.definitions)
         definitions_to_alter = [*definition_references, definition_to_find]
 
-        for definition in definitions_to_alter:
-
-            def filter_lexeme_by_reference_name(lexeme: Lexeme) -> bool:
-                return remove_list_type_indicator(lexeme.value) == definition_to_find.name
-
-            reference_lexemes = filter(filter_lexeme_by_reference_name, definition.lexemes)
-
-            for lexeme_to_replace in reference_lexemes:
-                document_edits = edits.get(lexeme_to_replace.source, [])
-                replacement_range = get_location_from_lexeme(lexeme_to_replace).range
-                document_edits.append(TextEdit(range=replacement_range, new_text=new_name))
-                edits[str(lexeme_to_replace.source)] = document_edits
+        for definition in _filter_editable_definitions(definitions_to_alter):
+            reference_lexemes = [
+                lexeme for lexeme in definition.lexemes if remove_list_type_indicator(lexeme.value) == definition_to_find.name
+            ]
+            self._add_edits_from_lexemes(new_name, reference_lexemes, edits)
 
         return edits
 
     def _get_enum_value_type_text_edits(
         self, old_value: str, new_value: str, definition_to_find: Definition, language_context: LanguageContext
-    ) -> dict[str, TextEdit]:
+    ) -> dict[str, list[TextEdit]]:
         """Returns a dictionary of enum value type uri to TextEdits where the uri is the key and the list of edits is the value."""
-        edits = {}
+        edits: dict[str, list] = {}
         enum_references = get_enum_references_from_context(definition_to_find, language_context)
         enum_references_to_alter = [*enum_references, definition_to_find]
 
-        for definition in enum_references_to_alter:
-            reference_lexemes = [lexeme for lexeme in definition.lexemes if remove_list_type_indicator(lexeme.value) == old_value]
-            for lexeme_to_replace in reference_lexemes:
-                document_edits = edits.get(lexeme_to_replace.source, [])
-                replacement_range = get_location_from_lexeme(lexeme_to_replace).range
-                document_edits.append(TextEdit(range=replacement_range, new_text=new_value))
-                edits[str(lexeme_to_replace.source)] = document_edits
+        for definition in _filter_editable_definitions(enum_references_to_alter):
+            reference_lexemes = [
+                lexeme for lexeme in definition.lexemes if remove_list_type_indicator(lexeme.value) == old_value
+            ]
+            self._add_edits_from_lexemes(new_value, reference_lexemes, edits)
+
+        return edits
+
+    def _get_root_key_text_edits(
+        self, old_value: str, new_value: str, definition_to_find: Definition, language_context: LanguageContext
+    ) -> dict[str, list[TextEdit]]:
+        """Returns a dictionary of uri to TextEdits where the uri is the key and the list of edits is the value."""
+        edits: dict[str, list] = {}
+
+        definitions_with_root_key = language_context.get_definitions_by_root_key(old_value)
+        root_key_references = get_definition_type_references_from_list(definition_to_find, language_context.definitions)
+        definitions_to_alter = [*definitions_with_root_key, *root_key_references, definition_to_find]
+
+        for definition in _filter_editable_definitions(definitions_to_alter):
+            reference_lexemes = [
+                lexeme for lexeme in definition.lexemes if remove_list_type_indicator(lexeme.value) == old_value
+            ]
+            self._add_edits_from_lexemes(new_value, reference_lexemes, edits)
 
         return edits
+
+    def _add_edits_from_lexemes(self, new_value: str, reference_lexemes: list[Lexeme], edits_list: dict[str, list]):
+        """Converts lexemes to edits and adds them to the edits dictionary."""
+        edits: dict = {}
+
+        logging.error(f"Lexemes to replace {reference_lexemes}")
+        for lexeme_to_replace in reference_lexemes:
+            lexeme_source = str(lexeme_to_replace.source)
+            replacement_range = get_location_from_lexeme(lexeme_to_replace).range
+            edit = TextEdit(range=replacement_range, new_text=new_value)
+
+            source_edits_list = edits_list.get(lexeme_source)
+            if not source_edits_list:
+                edits_list[lexeme_source] = [edit]
+            else:
+                source_edits_list.append(edit)
+
+        return edits
+
+
+def _filter_editable_definitions(definitions_to_filter: List[Definition]) -> List[Definition]:
+    filtered_definitions = {definition for definition in definitions_to_filter if definition.source.is_user_editable}
+    return list(filtered_definitions)
```

## aac/plugins/first_party/lsp_server/providers/semantic_tokens_provider.py

```diff
@@ -1,17 +1,17 @@
 """Module for the Semantic Tokens Provider which handles."""
 
 from typing import Any, Callable, Optional
 
 from pygls.lsp import SemanticTokenModifiers, SemanticTokenTypes, SemanticTokens, SemanticTokensLegend, SemanticTokensParams
-from pygls.server import LanguageServer
 from pygls.uris import to_fs_path
+from pygls.server import LanguageServer
 from yaml import Token
 
-from aac.io.parser._parse_source import _scan_yaml
+from aac.io.parser import get_cache
 from aac.lang.language_context import LanguageContext
 from aac.plugins.first_party.lsp_server.providers.lsp_provider import LspProvider
 from aac.spec.core import get_root_keys, _get_aac_spec_file_path
 
 
 def _is_enum(token: Token, language_context: LanguageContext) -> bool:
     """Return whether the provided token is an Enum token type."""
@@ -31,15 +31,15 @@
 
 def _is_struct(token: Token, language_context: LanguageContext) -> bool:
     """Return whether the provided token is a Struct token type."""
     definition = language_context.get_definition_by_name(token.value)
     return definition.is_schema() if definition else False
 
 
-def _is_string(token: Token, language_context: LanguageContext) -> bool:
+def _is_string(token: Token, _) -> bool:
     """Return whether the provided token represents a string value."""
     is_explicit_string = hasattr(token, "style") and token.style and token.style in "|'\""
     contains_spaces = any(map(lambda ch: ch.isspace(), token.value))
     return is_explicit_string or contains_spaces
 
 
 def _is_macro(token: Token, language_context: LanguageContext) -> bool:
@@ -82,24 +82,23 @@
     }
 
     def handle_request(self, language_server: LanguageServer, params: SemanticTokensParams) -> SemanticTokens:
         """Handle the semantic tokens request."""
         self.language_server = language_server
 
         token_data = []
-        with open(to_fs_path(params.text_document.uri), mode="r") as file:
-            prev_token, *tokens = _scan_yaml(file.read())
-            tokens = [token for token in tokens if hasattr(token, "value")]
-            for token in tokens:
-                semantic_token_data = self.convert_to_semantic_token(prev_token, token)
-                if semantic_token_data:
-                    token_data.extend(list(semantic_token_data))
-                    prev_token = token
+        prev_token, *tokens = get_cache().scan_file(to_fs_path(params.text_document.uri))
+        tokens = [token for token in tokens if hasattr(token, "value")]
+        for token in tokens:
+            semantic_token_data = self.convert_to_semantic_token(prev_token, token)
+            if semantic_token_data:
+                token_data.extend(list(semantic_token_data))
+                prev_token = token
 
-            return SemanticTokens(data=token_data)
+        return SemanticTokens(data=token_data)
 
     def get_semantic_tokens_legend(self) -> SemanticTokensLegend:
         """Return the legend for interpreting the semantic tokens codes."""
 
         def get_names(values) -> list[str]:
             return [value.name for value in values]
```

## aac/plugins/first_party/lsp_server/providers/symbols.py

```diff
@@ -7,15 +7,15 @@
 
 
 class SymbolType(Enum):
     """Enums classifying the symbol type. Leveraged by providers to tailor responses."""
 
     DEFINITION_NAME = 1
     ENUM_VALUE_TYPE = 2
-    ROOT_KEY_NAME = 3
+    ROOT_KEY = 3
 
 
 def get_possible_symbol_types(name: str, language_context: LanguageContext) -> list[SymbolType]:
     """
     Return a list of enums indicating what kind of symbol this may be based on the language context.
 
     Args:
@@ -32,15 +32,15 @@
         symbol_types.append(SymbolType.DEFINITION_NAME)
 
     enum_definition = language_context.get_enum_definition_by_type(name)
     if enum_definition:
         symbol_types.append(SymbolType.ENUM_VALUE_TYPE)
 
     if name in language_context.get_root_keys():
-        symbol_types.append(SymbolType.ROOT_KEY_NAME)
+        symbol_types.append(SymbolType.ROOT_KEY)
 
     return symbol_types
 
 
 def get_symbol_at_position(content: str, line: int, column: int) -> Optional[str]:
     """
     Return the word at or adjacent to the offset location.
@@ -69,30 +69,36 @@
     symbol_range = None
 
     if line_with_symbol != "":
         adjusted_column = column if column < len(line_with_symbol) else column - 1
         on_symbol = not line_with_symbol[adjusted_column].isspace()
 
         if on_symbol:
-
             symbol_start = 0
             # Reversed range from the adjusted column to the 0 element in the line
             for i in range(adjusted_column, -1, -1):
-                if line_with_symbol[i].isspace():
+                if line_with_symbol[i] == ":":
                     break
 
                 symbol_start = i
 
-            symbol_end = len(line_with_symbol)
+            symbol_end = len(line_with_symbol) - 1
             for i in range(adjusted_column, len(line_with_symbol)):
-                if line_with_symbol[i].isspace():
+                if line_with_symbol[i] == ":":
                     break
 
                 symbol_end = i
 
+            # Strip the whitespace
+            while line_with_symbol[symbol_start].isspace():
+                symbol_start += 1
+
+            while line_with_symbol[symbol_end].isspace():
+                symbol_end -= 1
+
             # Have to add 1 to the end index since slice ends are exclusive.
             symbol_end += 1
 
             start_position = Position(line=line, character=symbol_start)
             end_position = Position(line=line, character=symbol_end)
             symbol_range = Range(start=start_position, end=end_position)
```

## aac/plugins/first_party/plugin_management/plugin-management.yaml

```diff
@@ -1,14 +1,14 @@
-model:
-  name: plugin-management
-  description: An AaC plugin that manages which plugins available in the language context.
-  behavior:
+plugin:
+  name: Plugin Management
+  description: An AaC plugin that manages which plugins are available in the language context.
+  commands:
     - name: list-plugins
-      type: command
-      description: Display a list of available plugins.
+      group: Management
+      helpText: Display a list of available plugins.
       input:
         - name: --all
           type: bool
           python_type: bool
           description: Display a list of all the installed AaC plugins.
         - name: --active
           type: bool
@@ -22,92 +22,92 @@
         - name: plugins
           type: string[]
           python_type: list[str]
           description: The list of plugin names.
       acceptance:
         - scenario: Display a list of all installed plugins.
           when:
-            - The command is run with the {{plugin-management.input.--all}} flag.
+            - The command is run with the {{list-plugins.input.--all}} flag.
           then:
             - A list of all plugins installed on the system will be displayed.
         - scenario: Display a list of all plugins that are active on the system.
           when:
-            - The command is run with the {{plugin-management.input.--active}} flag.
+            - The command is run with the {{list-plugins.input.--active}} flag.
           then:
             - A list of all plugins installed on the system that are active will be displayed.
         - scenario: Display a list of all plugins that are installed but not active on the system.
           when:
-            - The command is run with the {{plugin-management.input.--inactive}} flag.
+            - The command is run with the {{list-plugins.input.--inactive}} flag.
           then:
             - A list of all plugins installed on the system that are inactive will be displayed.
         - scenario: Help displayed when no flags given.
           when:
             - The command is run without arguments.
           then:
             - The command help text is displayed.
         - scenario: Error when multiple flags given.
           when:
             - More than one flag is provided.
           then:
             - An error is displayed to the user stating that flags are mutually exclusive.
     - name: activate-plugin
-      type: command
-      description: Activate a plugin that's available and inactive on the system.
+      group: Management
+      helpText: Activate a plugin that's available and inactive on the system.
       input:
         - name: name
           type: string
           python_type: str
           description: The name of the plugin to be activated.
       acceptance:
         - scenario: Plugin is activated.
           given:
-            - The plugin named {{plugin-management.activate-plugin.plugin-name}} is installed on the system.
-            - The plugin named {{plugin-management.activate-plugin.plugin-name}} is inactive on the system.
+            - The plugin named {{activate-plugin.input.name}} is installed on the system.
+            - The plugin named {{activate-plugin.input.name}} is inactive on the system.
           when:
-            - The command is run with {{plugin-management.activate-plugin.plugin-name}}.
+            - The command is run with {{activate-plugin.input.name}}.
           then:
-            - The plugin named {{plugin-management.activate-plugin.plugin-name}} is activated.
+            - The plugin named {{activate-plugin.input.name}} is activated.
         - scenario: Error when plugin is not installed.
           given:
-            - The plugin named {{plugin-management.activate-plugin.plugin-name}} is not installed on the system.
+            - The plugin named {{activate-plugin.input.name}} is not installed on the system.
           when:
-            - The command is run with {{plugin-management.activate-plugin.plugin-name}}.
+            - The command is run with {{activate-plugin.input.name}}.
           then:
             - An error message is displayed to the user stating the plugin is not installed on the system.
         - scenario: Error when plugin is active.
           given:
-            - The plugin named {{plugin-management.activate-plugin.plugin-name}} is active.
+            - The plugin named {{activate-plugin.input.name}} is active.
           when:
-            - The command is run with {{plugin-management.activate-plugin.plugin-name}}.
+            - The command is run with {{activate-plugin.input.name}}.
           then:
             - An error message is displayed to the user stating the plugin is active.
     - name: deactivate-plugin
-      type: command
-      description: Deactivate a plugin that's available and active on the system.
+      group: Management
+      helpText: Deactivate a plugin that's available and active on the system.
       input:
         - name: name
           type: string
           python_type: str
           description: The name of the plugin to be deactivated.
       acceptance:
         - scenario: Plugin is deactivated.
           given:
-            - The plugin named {{plugin-management.activate-plugin.plugin-name}} is installed on the system.
-            - The plugin named {{plugin-management.activate-plugin.plugin-name}} is active on the system.
+            - The plugin named {{deactivate-plugin.input.name}} is installed on the system.
+            - The plugin named {{deactivate-plugin.input.name}} is active on the system.
           when:
-            - The command is run with {{plugin-management.activate-plugin.plugin-name}}.
+            - The command is run with {{deactivate-plugin.input.name}}.
           then:
-            - The plugin named {{plugin-management.activate-plugin.plugin-name}} is deactivated.
+            - The plugin named {{deactivate-plugin.input.name}} is deactivated.
         - scenario: Error when plugin is not installed.
           given:
-            - The plugin named {{plugin-management.activate-plugin.plugin-name}} is not installed on the system.
+            - The plugin named {{deactivate-plugin.input.name}} is not installed on the system.
           when:
-            - The command is run with {{plugin-management.activate-plugin.plugin-name}}.
+            - The command is run with {{deactivate-plugin.input.name}}.
           then:
             - An error message is displayed to the user stating the plugin is not installed on the system.
         - scenario: Error when plugin is not active.
           given:
-            - The plugin named {{plugin-management.activate-plugin.plugin-name}} is inactive.
+            - The plugin named {{deactivate-plugin.input.name}} is inactive.
           when:
-            - The command is run with {{plugin-management.activate-plugin.plugin-name}}.
+            - The command is run with {{deactivate-plugin.input.name}}.
           then:
             - An error message is displayed to the user stating the plugin is inactive.
```

## aac/plugins/first_party/plugin_management/plugin_management_impl.py

```diff
@@ -1,17 +1,17 @@
-"""AaC Plugin implementation module for the plugin-management plugin."""
+"""AaC Plugin implementation module for the Plugin Management plugin."""
 
 import logging
 
 from aac.lang.active_context_lifecycle_manager import get_active_context
 from aac.plugins import PluginError
 from aac.plugins.plugin_execution import PluginExecutionResult, plugin_result
 from aac.plugins.plugin_manager import get_plugins
 
-plugin_name = "plugin-management"
+plugin_name = "Plugin Management"
 
 
 def list_plugins(all: bool, active: bool, inactive: bool) -> PluginExecutionResult:
     """
     Display a list of available plugins.
 
     Args:
```

## aac/plugins/first_party/primitive_type_check/__init__.py

```diff
@@ -1,12 +1,21 @@
 """The primitive-type-checking plugin module."""
 
 from aac.plugins import hookimpl
 from aac.plugins.contributions.contribution_types import PrimitiveValidationContribution
-from aac.plugins.first_party.primitive_type_check.validators import int_validator, bool_validator, plugin_name
+from aac.plugins.first_party.primitive_type_check.validators import (
+    plugin_name,
+    int_validator,
+    bool_validator,
+    file_validator,
+    num_validator,
+    date_validator,
+    reference_validator,
+    string_validator,
+)
 from aac.plugins.plugin import Plugin
 
 
 @hookimpl
 def get_plugin() -> Plugin:
     """
     Returns information about the plugin.
@@ -16,8 +25,16 @@
     """
     plugin = Plugin(plugin_name)
     plugin.register_primitive_validations(_get_primitive_validations())
     return plugin
 
 
 def _get_primitive_validations() -> list[PrimitiveValidationContribution]:
-    return [int_validator.get_validator(), bool_validator.get_validator()]
+    return [
+        int_validator.get_validator(),
+        bool_validator.get_validator(),
+        file_validator.get_validator(),
+        num_validator.get_validator(),
+        date_validator.get_validator(),
+        reference_validator.get_validator(),
+        string_validator.get_validator(),
+    ]
```

## aac/plugins/first_party/primitive_type_check/primitive_type_check.yaml

```diff
@@ -1,47 +1,339 @@
-model:
-  name: primitive-type-checking
+plugin:
+  name: Primitive Type Checking
   description: |
-    Primitive Type Checking is an Architecture-as-Code plugin that provides
-    primitive type validations for the primitive enum types defined in the core specification.
-  behavior:
+    An AaC plugin that enables primitive type checking for the primitive enum
+    types defined in the core specification.
+  primitiveValidators:
+    - name: Validate String Primitives
     - name: Validate Integer Primitives
-      type: request-response
-      description:
+    - name: Validate Number Primitives
+    - name: Validate Boolean Primitives
+    - name: Validate Date Primitives
+    - name: Validate File Primitives
+    - name: Validate Directory Primitives
+    - name: Validate Reference Primitives
+---
+validation:
+  name: Validate String Primitives
+  description: Provides validation for the primitive AaC type string.
+  behavior:
+    - name: validate string primitive
+      description: Provides an error message if the value in a string field is not parsed as a string.
+      type: REQUEST_RESPONSE
       input:
         - name: input
           type: ValidatorInput
       output:
         - name: results
           type: ValidatorOutput
       acceptance:
-        - scenario: Successfully Validate an Integer Primitive Value
+        - scenario: Successfully validate a string primitive value.
           given:
-            - The ValidatorInput content consists of valid AaC definitions
-            - The ValidatorInput contains at least one definition field that is defined as being type `int`
-            - The value in the primitive `int` field is a non-string whole number
+            - The ValidatorInput content consists of valid AaC definitions.
+            - The ValidatorInput contains at least one definition field that is defined as being type `string`.
+            - The value in the primitive `string` field is a YAML value that can be interpreted as a `string`.
           when:
-            - The input is validated
+            - The input is validated.
           then:
-            - The ValidatorOutput does not indicate any errors
-            - The ValidatorOutput does not indicate any warnings
-            - The ValidatorOutput indicates the primitive value under test is valid
-        - scenario: Fail to Validate an Integer Primitive Value is A Float
+            - The ValidatorOutput does not indicate any errors.
+            - The ValidatorOutput does not indicate any warnings.
+            - The ValidatorOutput indicates the primitive value under test is valid.
+        - scenario: Fail to validate a string primitive value that is numeric.
           given:
-            - The ValidatorInput content consists of valid AaC definitions
-            - The ValidatorInput contains at least one definition field that is defined as being type `int`
-            - The value in the primitive `int` field is a decimal number
+            - The ValidatorInput content consists of AaC definitions.
+            - The ValidatorInput contains at least one definition field that is defined as being type `string`.
+            - The value in the primitive `string` field is a decimal number.
           when:
-            - The input is validated
+            - The input is validated.
           then:
-            - The ValidatorOutput indicates an error
-            - The ValidatorOutput indicates the primitive value under test is invalid
-        - scenario: Fail to Validate an Integer Primitive Value Is a String
+            - The ValidatorOutput indicates an error.
+            - The ValidatorOutput indicates the primitive value under test is invalid.
+        - scenario: Fail to validate a string primitive value that is null.
+          given:
+            - The ValidatorInput content consists of AaC definitions.
+            - The ValidatorInput contains at least one definition field that is defined as being type `string`.
+            - The value in the primitive `string` field is `null`.
+          when:
+            - The input is validated.
+          then:
+            - The ValidatorOutput indicates an error.
+            - The ValidatorOutput indicates the primitive value under test is invalid.
+---
+validation:
+  name: Validate Integer Primitives
+  description: Provides validation for the primitive AaC type int.
+  behavior:
+    - name: validate integer primitive
+      description: Provides an error message if the value in an int field is not parsed as an integer.
+      type: REQUEST_RESPONSE
+      input:
+        - name: input
+          type: ValidatorInput
+      output:
+        - name: results
+          type: ValidatorOutput
+      acceptance:
+        - scenario: Successfully validate an integer primitive value.
           given:
-            - The ValidatorInput content consists of valid AaC definitions
-            - The ValidatorInput contains at least one definition field that is defined as being type `int`
-            - The value in the primitive `int` field contains alphabetical letters or punctuation marks
+            - The ValidatorInput content consists of valid AaC definitions.
+            - The ValidatorInput contains at least one definition field that is defined as being type `int`.
+            - The value in the primitive `int` field is a non-string whole number.
           when:
-            - The input is validated
+            - The input is validated.
           then:
-            - The ValidatorOutput indicates an error
-            - The ValidatorOutput indicates the primitive value under test is invalid
+            - The ValidatorOutput does not indicate any errors.
+            - The ValidatorOutput does not indicate any warnings.
+            - The ValidatorOutput indicates the primitive value under test is valid.
+        - scenario: Fail to validate an integer primitive value that is a float.
+          given:
+            - The ValidatorInput content consists of AaC definitions.
+            - The ValidatorInput contains at least one definition field that is defined as being type `int`.
+            - The value in the primitive `int` field is a decimal number.
+          when:
+            - The input is validated.
+          then:
+            - The ValidatorOutput indicates an error.
+            - The ValidatorOutput indicates the primitive value under test is invalid.
+        - scenario: Fail to validate an integer primitive value that is a string.
+          given:
+            - The ValidatorInput content consists of AaC definitions.
+            - The ValidatorInput contains at least one definition field that is defined as being type `int`.
+            - The value in the primitive `int` field contains alphabetical letters or punctuation marks.
+          when:
+            - The input is validated.
+          then:
+            - The ValidatorOutput indicates an error.
+            - The ValidatorOutput indicates the primitive value under test is invalid.
+---
+validation:
+  name: Validate Number Primitives
+  description: Provides validation for the primitive AaC type number.
+  behavior:
+  - name: validate number primitive
+    description: Provides an error message if the value in a number field is not parsed as a number.
+    type: REQUEST_RESPONSE
+    input:
+      - name: input
+        type: ValidatorInput
+    output:
+      - name: results
+        type: ValidatorOutput
+    acceptance:
+      - scenario: Successfully validate a number primitive value.
+        given:
+          - The ValidatorInput content consists of valid AaC definitions.
+          - The ValidatorInput contains at least one definition field that is defined as being type `number`.
+          - The value in the primitive `number` field is a non-string whole number.
+        when:
+          - The input is validated.
+        then:
+          - The ValidatorOutput does not indicate any errors.
+          - The ValidatorOutput does not indicate any warnings.
+          - The ValidatorOutput indicates the primitive value under test is valid.
+      - scenario: Successfully validate a number primitive value that is an integer.
+        given:
+          - The ValidatorInput content consists of AaC definitions.
+          - The ValidatorInput contains at least one definition field that is defined as being type `number`.
+          - The value in the primitive `number` field is an integer.
+        when:
+          - The input is validated.
+        then:
+          - The ValidatorOutput does not indicate any errors.
+          - The ValidatorOutput does not indicate any warnings.
+          - The ValidatorOutput indicates the primitive value under test is valid.
+      - scenario: Fail to validate a number primitive value that is a string.
+        given:
+          - The ValidatorInput content consists of AaC definitions.
+          - The ValidatorInput contains at least one definition field that is defined as being type `number`.
+          - The value in the primitive `number` field contains alphabetical letters or punctuation marks.
+        when:
+          - The input is validated.
+        then:
+          - The ValidatorOutput indicates an error.
+          - The ValidatorOutput indicates the primitive value under test is invalid.
+---
+validation:
+  name: Validate Boolean Primitives
+  description: Provides validation for the primitive AaC type bool.
+  behavior:
+  - name: validate boolean primitive
+    description: Provides an error message if the value in a bool field is not parsed as a boolean (True/False).
+    type: REQUEST_RESPONSE
+    input:
+      - name: input
+        type: ValidatorInput
+    output:
+      - name: results
+        type: ValidatorOutput
+    acceptance:
+      - scenario: Successfully validate a boolean primitive value.
+        given:
+          - The ValidatorInput content consists of valid AaC definitions.
+          - The ValidatorInput contains at least one definition field that is defined as being type `bool`.
+          - The value in the primitive `bool` field is a valid boolean YAML value.
+        when:
+          - The input is validated.
+        then:
+          - The ValidatorOutput does not indicate any errors.
+          - The ValidatorOutput does not indicate any warnings.
+          - The ValidatorOutput indicates the primitive value under test is valid.
+      - scenario: Fail to validate an integer primitive value is a non-boolean string.
+        given:
+          - The ValidatorInput content consists of AaC definitions.
+          - The ValidatorInput contains at least one definition field that is defined as being type `bool`.
+          - The value in the primitive `bool` field contains alphabetical letters or punctuation marks that don't represent a YAML boolean value.
+        when:
+          - The input is validated.
+        then:
+          - The ValidatorOutput indicates an error.
+          - The ValidatorOutput indicates the primitive value under test is invalid.
+---
+validation:
+  name: Validate Date Primitives
+  description: Provides validation for the primitive AaC type date.
+  behavior:
+  - name: validate date primitive
+    description: Provides an error message if the value in a date field is not parsed as a date.
+    type: REQUEST_RESPONSE
+    input:
+      - name: input
+        type: ValidatorInput
+    output:
+      - name: results
+        type: ValidatorOutput
+    acceptance:
+      - scenario: Successfully validate a date primitive value.
+        given:
+          - The ValidatorInput content consists of valid AaC definitions.
+          - The ValidatorInput contains at least one definition field that is defined as being type `date`.
+          - The value in the primitive `date` field is a valid date YAML value.
+        when:
+          - The input is validated.
+        then:
+          - The ValidatorOutput does not indicate any errors.
+          - The ValidatorOutput does not indicate any warnings.
+          - The ValidatorOutput indicates the primitive value under test is valid.
+      - scenario: Fail to validate a date primitive value that is a non-date string.
+        given:
+          - The ValidatorInput content consists of AaC definitions.
+          - The ValidatorInput contains at least one definition field that is defined as being type `date`.
+          - The value in the primitive `date` field contains alphabetical letters or punctuation marks that don't represent a YAML date value.
+        when:
+          - The input is validated.
+        then:
+          - The ValidatorOutput indicates an error.
+          - The ValidatorOutput indicates the primitive value under test is invalid.
+---
+validation:
+  name: Validate File Primitives
+  description: Provides validation for the primitive AaC type file.
+  behavior:
+  - name: validate file primitive
+    description: Provides an error message if the value in a file field is not a valid file on the file system.
+    type: REQUEST_RESPONSE
+    input:
+      - name: input
+        type: ValidatorInput
+    output:
+      - name: results
+        type: ValidatorOutput
+    acceptance:
+      - scenario: Successfully validate a file primitive value.
+        given:
+          - The ValidatorInput content consists of valid AaC definitions.
+          - The ValidatorInput contains at least one definition field that is defined as being type `file`.
+          - The value in the primitive `file` field is a valid path to a file.
+          - The specified file path exists on the file system.
+        when:
+          - The input is validated.
+        then:
+          - The ValidatorOutput does not indicate any errors.
+          - The ValidatorOutput does not indicate any warnings.
+          - The ValidatorOutput indicates the primitive value under test is valid.
+      - scenario: Warn when validating a file primitive value that does not exist.
+        given:
+          - The ValidatorInput content consists of valid AaC definitions.
+          - The ValidatorInput contains at least one definition field that is defined as being type `file`.
+          - The value in the primitive `file` field represents a file path.
+          - The specified file path does not exist on the file system.
+        when:
+          - The input is validated.
+        then:
+          - The ValidatorOutput indicates a warning.
+          - The ValidatorOutput indicates the primitive value under test does not exist.
+---
+validation:
+  name: Validate Directory Primitives
+  description: Provides validation for the primitive AaC type directory.
+  behavior:
+  - name: validate directory primitive
+    description: Provides an error message if the value in a directory field is not a valid directory on the filesystem.
+    type: REQUEST_RESPONSE
+    input:
+      - name: input
+        type: ValidatorInput
+    output:
+      - name: results
+        type: ValidatorOutput
+    acceptance:
+      - scenario: Successfully validate a directory primitive value.
+        given:
+          - The ValidatorInput content consists of valid AaC definitions.
+          - The ValidatorInput contains at least one definition field that is defined as being type `directory`.
+          - The value in the primitive `directory` field is a valid path to a directory.
+          - The specified directory path exists on the file system.
+        when:
+          - The input is validated.
+        then:
+          - The ValidatorOutput does not indicate any errors.
+          - The ValidatorOutput does not indicate any warnings.
+          - The ValidatorOutput indicates the primitive value under test is valid.
+      - scenario: Warn when validating a directory primitive value that does not exist.
+        given:
+          - The ValidatorInput content consists of valid AaC definitions.
+          - The ValidatorInput contains at least one definition field that is defined as being type `directory`.
+          - The value in the primitive `directory` field represents a directory path.
+          - The specified directory path does not exist on the file system.
+        when:
+          - The input is validated.
+        then:
+          - The ValidatorOutput indicates a warning.
+          - The ValidatorOutput indicates the primitive value under test does not exist.
+---
+validation:
+  name: Validate Reference Primitives
+  description: Provides validation for the primitive AaC type reference.
+  behavior:
+  - name: validate reference primitive
+    description: Provides an error message if the value in a reference field is not a reference to another definition.
+    type: REQUEST_RESPONSE
+    input:
+      - name: input
+        type: ValidatorInput
+    output:
+      - name: results
+        type: ValidatorOutput
+    acceptance:
+      - scenario: Successfully validate a reference primitive value.
+        given:
+          - The ValidatorInput content consists of valid AaC definitions.
+          - The ValidatorInput contains at least one definition field that is defined as being type `reference`.
+          - The value in the primitive `reference` field is the name of an AaC definition.
+          - The specified definition exists in the active context.
+        when:
+          - The input is validated.
+        then:
+          - The ValidatorOutput does not indicate any errors.
+          - The ValidatorOutput does not indicate any warnings.
+          - The ValidatorOutput indicates the primitive value under test is valid.
+      - scenario: Error when validating a reference primitive value that does not exist.
+        given:
+          - The ValidatorInput content consists of valid AaC definitions.
+          - The ValidatorInput contains at least one definition field that is defined as being type `reference`.
+          - The value in the primitive `reference` field is a string value.
+          - The specified reference does not exist in the active context.
+        when:
+          - The input is validated.
+        then:
+          - The ValidatorOutput indicates an error.
+          - The ValidatorOutput indicates the primitive value under test is not a valid reference to a definition.
```

## aac/plugins/first_party/primitive_type_check/validators/__init__.py

```diff
@@ -8,18 +8,18 @@
     PRIMITIVE_TYPE_NUMBER,
     PRIMITIVE_TYPE_REFERENCE,
     PRIMITIVE_TYPE_STRING,
 )
 
 
 def _create_validator_name(enum_type: str) -> str:
-    return f"{enum_type}_enum_validator"
+    return f"Validate {enum_type.capitalize()} Primitives"
 
 
-plugin_name = "primitive-type-check"
+plugin_name = "Primitive Type Checking"
 
 STRING_VALIDATION_NAME = _create_validator_name(PRIMITIVE_TYPE_STRING)
 INT_VALIDATION_NAME = _create_validator_name(PRIMITIVE_TYPE_INT)
 NUMBER_VALIDATION_NAME = _create_validator_name(PRIMITIVE_TYPE_NUMBER)
 BOOL_VALIDATION_NAME = _create_validator_name(PRIMITIVE_TYPE_BOOL)
 DATE_VALIDATION_NAME = _create_validator_name(PRIMITIVE_TYPE_DATE)
 FILE_VALIDATION_NAME = _create_validator_name(PRIMITIVE_TYPE_FILE)
```

## aac/plugins/first_party/primitive_type_check/validators/bool_validator.py

```diff
@@ -1,39 +1,42 @@
-"""Module for the various type contributions provided by this plugin."""
+"""Module for validating primitive boolean types."""
+
 from typing import Any, Optional
 
 from aac.lang.constants import PRIMITIVE_TYPE_BOOL
 from aac.lang.definitions.definition import Definition
+from aac.lang.language_context import LanguageContext
 from aac.plugins.contributions.contribution_types import PrimitiveValidationContribution
 from aac.plugins.first_party.primitive_type_check.validators import BOOL_VALIDATION_NAME
 from aac.plugins.validators._validator_finding import ValidatorFinding, FindingSeverity, FindingLocation
 
 
 def get_validator() -> PrimitiveValidationContribution:
     """Return the Primitive Validator for 'boolean'."""
     return PrimitiveValidationContribution(BOOL_VALIDATION_NAME, PRIMITIVE_TYPE_BOOL, validate_bool)
 
 
-def validate_bool(definition: Definition, value_to_validate: Any) -> Optional[ValidatorFinding]:
+def validate_bool(definition: Definition, value_to_validate: Any, _: LanguageContext) -> Optional[ValidatorFinding]:
     """
     Returns a Validation finding if the type isn't valid, otherwise None.
 
     This function is intended to be used in the Validation apparatus, and for this result
     to be collated with other finding into a larger ValidatorResult.
 
     Arge:
         definition (Definition): The definition that the value belongs to.
         value_to_validate (Any): The value to be tested.
+        _ (LanguageContext): The current LanguageContext.
 
     Returns:
         A ValidatorFinding if the value is not a boolean or None.
     """
 
     is_invalid = not isinstance(value_to_validate, bool)
     finding = None
     if is_invalid:
         lexeme, *_ = [lexeme for lexeme in definition.lexemes if lexeme.value.lower() == str(value_to_validate.lower())]
-        finding_message = f"{value_to_validate} is not a valid value for boolean type {PRIMITIVE_TYPE_BOOL}"
+        finding_message = f"{value_to_validate} is not a valid value for boolean type {PRIMITIVE_TYPE_BOOL}."
         finding_location = FindingLocation.from_lexeme(BOOL_VALIDATION_NAME, lexeme)
         finding = ValidatorFinding(definition, FindingSeverity.ERROR, finding_message, finding_location)
 
     return finding
```

## aac/plugins/first_party/primitive_type_check/validators/int_validator.py

```diff
@@ -1,48 +1,50 @@
-"""Module for the various type contributions provided by this plugin."""
+"""Module for validating primitive integer types."""
 
 import logging
+
 from typing import Any, Optional
 
 from aac.lang.constants import PRIMITIVE_TYPE_INT
 from aac.lang.definitions.definition import Definition
+from aac.lang.language_context import LanguageContext
 from aac.plugins.contributions.contribution_types.primitive_validation_contribution import PrimitiveValidationContribution
 from aac.plugins.first_party.primitive_type_check.validators import INT_VALIDATION_NAME
 from aac.plugins.validators import FindingLocation
 from aac.plugins.validators._validator_finding import FindingSeverity, ValidatorFinding
 
 
 def get_validator() -> PrimitiveValidationContribution:
     """Return the Primitive Validator for 'int'."""
     return PrimitiveValidationContribution(INT_VALIDATION_NAME, PRIMITIVE_TYPE_INT, validate_integer)
 
 
-def validate_integer(definition: Definition, value_to_validate: Any) -> Optional[ValidatorFinding]:
+def validate_integer(definition: Definition, value_to_validate: Any, _: LanguageContext) -> Optional[ValidatorFinding]:
     """
     Returns a Validation finding if the type isn't valid, otherwise None.
 
     This function is intended to be used in the Validation apparatus, and for this result
         to be collated with other findings into a larger ValidatorResult.
 
     Args:
         definition (Definition): The definition that the value belongs to.
         value_to_validate (Any): The value to test.
+        _ (LanguageContext): The current LanguageContext.
 
     Returns:
         A ValidatorFinding if the value is not an integer, or None.
     """
     is_invalid = False
     try:
         type_casted_int = int(value_to_validate)
         # assert that the conversion didn't alter the contents, like in the case of float -> int.
         is_invalid = str(type_casted_int) != str(value_to_validate)
     except Exception as error:
         is_invalid = True
         logging.debug(f"{PRIMITIVE_TYPE_INT} validation failed for value {value_to_validate} with error:\n{error}")
-        pass
 
     finding = None
     if is_invalid:
         finding_message = f"{value_to_validate} is not a valid value for the enum type {PRIMITIVE_TYPE_INT}"
         lexeme = definition.get_lexeme_with_value(value_to_validate)
         finding_location = FindingLocation.from_lexeme(INT_VALIDATION_NAME, lexeme)
         finding = ValidatorFinding(definition, FindingSeverity.ERROR, finding_message, finding_location)
```

## aac/plugins/first_party/print_spec/print-spec.yaml

```diff
@@ -1,22 +1,22 @@
-model:
-  name: print-spec
-  description: Print the AaC core specification
-  behavior:
+plugin:
+  name: Print Core Spec
+  description: Print the AaC core specification.
+  commands:
     - name: print-spec
-      type: command
-      description: Print the AaC model describing core AaC data types and enumerations.
+      group: Query
+      helpText: Print the AaC model describing core AaC data types and enumerations.
       acceptance:
-        - scenario: Print the AaC Core specification
+        - scenario: Print the AaC Core specification.
           when:
             - The aac application is run with the print-spec command.
           then:
             - The AaC core specification is written to the console.
     - name: print-active-context
-      type: command
-      description: Print the AaC active language context including data types and enumerations added by plugins.
+      group: Query
+      helpText: Print the AaC active language context including data types and enumerations added by plugins.
       acceptance:
-        - scenario: Print the AaC active language context
+        - scenario: Print the AaC active language context.
           when:
             - The aac application is run with the print-active-context command.
           then:
             - The AaC active language context definitions are written to the console.
```

## aac/plugins/first_party/print_spec/print_spec_impl.py

```diff
@@ -1,15 +1,15 @@
-"""AaC Plugin implementation module for the print-spec plugin."""
+"""AaC Plugin implementation module for the Print Core Spec plugin."""
 
 from aac.lang.active_context_lifecycle_manager import get_active_context
 from aac.plugins.plugin_execution import PluginExecutionResult, plugin_result
 from aac.spec.core import get_aac_spec_as_yaml
 
 
-plugin_name = "print-spec"
+plugin_name = "Print Core Spec"
 
 
 def print_spec() -> PluginExecutionResult:
     """Print the AaC model describing core AaC data types and enumerations."""
     with plugin_result(plugin_name, get_aac_spec_as_yaml) as result:
         return result
```

## aac/plugins/first_party/rest_api/__init__.py

```diff
@@ -47,15 +47,15 @@
         AacCommand(
             "rest-api",
             "Start a RESTful interface for interacting with and managing AaC.",
             rest_api,
             rest_api_arguments,
         ),
         AacCommand(
-            "generate-openapi-spec",
+            "gen-openapi-spec",
             "Write the OpenAPI schema to a JSON file.",
             generate_api_spec,
             generate_api_spec_arguments,
         ),
     ]
 
     return plugin_commands
```

## aac/plugins/first_party/rest_api/aac_rest_api_impl.py

```diff
@@ -1,20 +1,21 @@
-"""AaC Plugin implementation module for the aac-rest-api plugin."""
+"""AaC Plugin implementation module for the REST API plugin."""
 
-from fastapi.openapi.utils import get_openapi
 import asyncio
 import json
 import logging
 import os
 import uvicorn
 
+from fastapi.openapi.utils import get_openapi
+
 from aac.plugins.plugin_execution import PluginExecutionResult, plugin_result
 from aac.plugins.first_party.rest_api.aac_rest_app import app, refresh_available_files_in_workspace
 
-plugin_name = "rest-api"
+plugin_name = "REST API"
 
 
 def rest_api(host: str = "0.0.0.0", port: int = 8000) -> PluginExecutionResult:
     """
     Start a RESTful interface for interacting with and managing AaC.
 
     Args:
```

## aac/plugins/first_party/rest_api/aac_rest_app.py

```diff
@@ -1,19 +1,21 @@
 """Module for configuring and maintaining the restful application and its routes."""
-from fastapi import FastAPI, HTTPException, BackgroundTasks, responses
+from fastapi import FastAPI, HTTPException, BackgroundTasks, responses, exceptions, Request
 from http import HTTPStatus
 import logging
 import os
 
 from aac.cli.aac_command import AacCommand
 from aac.io.files.aac_file import AaCFile
 from aac.io.files.find import find_aac_files, is_aac_file
 from aac.io.paths import sanitize_filesystem_path
 from aac.io.parser import parse
+from aac.io.parser._parser_error import ParserError
 from aac.lang.active_context_lifecycle_manager import get_active_context
+from aac.lang.constants import DEFINITION_FIELD_TYPE, DEFINITION_FIELD_NAME
 from aac.lang.definitions.json_schema import get_definition_json_schema
 from aac.lang.language_error import LanguageError
 from aac.plugins.plugin_execution import PluginExecutionStatusCode
 from aac.plugins.first_party.rest_api.models.command_model import (
     CommandModel,
     CommandRequestModel,
     CommandResponseModel,
@@ -59,28 +61,38 @@
 
         return file_model
     else:
         _report_error_response(HTTPStatus.NOT_FOUND, f"File {uri} not found in the context.")
 
 
 @app.post("/files/import", status_code=HTTPStatus.NO_CONTENT)
-def import_files_to_context(file_models: list[FilePathModel]):
-    """Import the list of files into the context."""
+def import_files_to_context(file_models: list[FilePathModel]) -> None:
+    """
+    Import the list of files into the context.
+
+    Args:
+        file_models (list[FilePathModel]): List of file models for import.
+
+    """
     files_to_import = set([str(model.uri) for model in file_models])
     valid_aac_files = set(filter(is_aac_file, files_to_import))
     invalid_files = files_to_import.difference(valid_aac_files)
 
     if len(invalid_files) > 0:
         _report_error_response(
             HTTPStatus.BAD_REQUEST,
             f"Invalid files were asked to imported. Invalid files: {invalid_files}.",
         )
     else:
-        new_file_definitions = [parse(file) for file in valid_aac_files]
-        list(map(get_active_context().add_definitions_to_context, new_file_definitions))
+        try:
+            new_file_definitions = [parse(file) for file in valid_aac_files]
+        except ParserError as error:
+            raise ParserError(error.source, error.errors) from None
+        else:
+            list(map(get_active_context().add_definitions_to_context, new_file_definitions))
 
 
 @app.put("/file", status_code=HTTPStatus.NO_CONTENT)
 def rename_file_uri(rename_request: FilePathRenameModel) -> None:
     """Update a file's uri. (Rename file)."""
     active_context = get_active_context()
     current_file_path = sanitize_filesystem_path(str(rename_request.current_file_uri))
@@ -231,14 +243,54 @@
     else:
         _report_error_response(
             HTTPStatus.NOT_FOUND,
             f"Definition {name} not found in the context; failed to delete definitions.",
         )
 
 
+# Language Context Support
+
+@app.get("/context/schema", status_code=HTTPStatus.OK, response_model=DefinitionModel)
+def get_root_key_schema(key: str):
+    """
+    Returns the JSON schema for the given root key, or HTTPStatus.NOT_FOUND not found if the key doesn't exist.
+
+    Returns:
+        200 HTTPStatus.OK if successful.
+        404 HTTPStatus.NOT_FOUND if the key doesn't exist.
+    """
+    active_context = get_active_context()
+    key_fields = active_context.get_root_fields()
+    matching_keys = [key_field for key_field in key_fields if key_field.get(DEFINITION_FIELD_NAME) == key]
+
+    if not matching_keys:
+        _report_error_response(HTTPStatus.NOT_FOUND, f"No root key found called {key}.")
+    else:
+        key_definition_name = matching_keys[0].get(DEFINITION_FIELD_TYPE, "")
+        schema_definition = active_context.get_definition_by_name(key_definition_name)
+
+        if not schema_definition:
+            _report_error_response(HTTPStatus.NOT_FOUND, f"Unable to get the schema definition {key_definition_name}.")
+        else:
+            schema_model = to_definition_model(schema_definition)
+            schema_model.json_schema = get_definition_json_schema(schema_definition, active_context)
+            return schema_model
+
+
+@app.get("/context/root_keys", status_code=HTTPStatus.OK, response_model=list[str])
+def get_language_context_root_keys():
+    """
+    Returns a list of root keys from the active context.
+
+    Returns:
+        200 HTTPStatus.OK
+    """
+    return get_active_context().get_root_keys()
+
+
 # AaC Plugin Commands
 
 
 @app.get("/commands", status_code=HTTPStatus.OK, response_model=list[CommandModel])
 def get_aac_commands():
     """Return a list of all available plugin commands."""
     aac_and_plugin_commands = _get_rest_api_compatible_commands()
@@ -286,17 +338,21 @@
     AVAILABLE_AAC_FILES = list(_get_available_files_in_workspace())
 
     # Update the active context with any missing files
     active_context = get_active_context()
     files_in_context = {file.uri for file in active_context.get_files_in_context()}
     available_files = {file.uri for file in AVAILABLE_AAC_FILES}
     missing_files = available_files.difference(files_in_context)
-    definition_lists_from_missing_files = [parse(file_uri) for file_uri in missing_files]
-    definitions_to_add = {definition.name: definition for definition_list in definition_lists_from_missing_files for definition in definition_list}
-    active_context.add_definitions_to_context(list(definitions_to_add.values()))
+    try:
+        definition_lists_from_missing_files = [parse(file_uri) for file_uri in missing_files]
+    except ParserError as error:
+        raise ParserError(error.source, error.errors) from None
+    else:
+        definitions_to_add = {definition.name: definition for definition_list in definition_lists_from_missing_files for definition in definition_list}
+        active_context.add_definitions_to_context(list(definitions_to_add.values()))
 
 
 def _report_error_response(code: HTTPStatus, error: str):
     logging.error(error)
     raise HTTPException(
         status_code=code,
         detail=error,
@@ -324,7 +380,13 @@
 # Error Handlers
 
 
 @app.exception_handler(LanguageError)
 async def language_error_exception_handler(request, exc):
     """If a `LanguageError` exception is encountered, then return a 400 BAD Request with the exception's message."""
     return responses.PlainTextResponse(str(exc), status_code=400)
+
+
+@app.exception_handler(exceptions.RequestValidationError)
+async def validation_exception_handler(request: Request, exc: exceptions.RequestValidationError):
+    """If a `exceptions.RequestValidationError` exception is encountered, then return a 422 UNPROCESSABLE ENTITY with the exception's message."""
+    _report_error_response(HTTPStatus.UNPROCESSABLE_ENTITY, str(exc))
```

## aac/plugins/first_party/rest_api/rest_api.yaml

```diff
@@ -1,47 +1,49 @@
-model:
-  name: aac-rest-api
-  description: Provides a RESTful API for managing and interacting with the AaC Python package.
-  behavior:
+plugin:
+  name: REST API
+  description: |
+    An AaC plugin that provides a RESTful API for managing and interacting with
+    the AaC Python package.
+  commands:
     - name: rest-api
-      type: command
-      description: Start a RESTful interface for interacting with and managing AaC.
+      group: Backend
+      helpText: Start a RESTful interface for interacting with and managing AaC.
       input:
         - name: --host
           type: string
           python_type: str
           description: Set the hostname of the service. Useful for operating behind proxies.
           defualt: 0.0.0.0
         - name: --port
           type: int
           python_type: int
           description: The port to which the RESTful service will be bound.
           default: 8080
       acceptance:
-        - scenario: Start the RESTful API without arguments
+        - scenario: Start the RESTful API without arguments.
           when:
             - The aac app is run with the rest-api command.
           then:
-            - The RESTful API is accessible on the default port value
-        - scenario: Start the RESTful API with arguments
+            - The RESTful API is accessible on the default port value.
+        - scenario: Start the RESTful API with arguments.
           given:
             - The {{rest-api.input.--host}} contains a valid hostname.
             - The {{rest-api.input.--port}} contains a valid, open port.
           when:
             - The aac app is run with the rest-api command.
           then:
-            - The RESTful API is accessible on the port specified by the port argument
-            - The RESTful API returns links to itself with the hostname specified by the host argument
-    - name: generate-openapi-spec
-      type: command
-      description: Write the OpenAPI schema to a JSON file.
+            - The RESTful API is accessible on the port specified by the port argument.
+            - The RESTful API returns links to itself with the hostname specified by the host argument.
+    - name: gen-openapi-spec
+      group: Generation
+      helpText: Write the OpenAPI schema to a JSON file.
       input:
         - name: output_directory
           type: directory
           python_type: str
-          description: The output directory in which to write the AaC OpenAPI JSON file
+          description: The output directory in which to write the AaC OpenAPI JSON file.
       acceptance:
         - scenario: Output the OpenAPI specification to file.
           when:
             - The aac app is run with the generate-openapi-spec command.
           then:
             - The OpenAPI schema is written to the output directory in a JSON file.
```

## aac/plugins/first_party/specifications/__init__.py

```diff
@@ -1,18 +1,14 @@
 """The specifications plugin module."""
-import logging
 
 from aac.cli.aac_command import AacCommand, AacCommandArgument
-from aac.lang.definitions.collections import get_definition_by_name
 from aac.lang.definitions.definition import Definition
 from aac.plugins import hookimpl
-from aac.plugins.plugin import Plugin, DefinitionValidationContribution
+from aac.plugins.plugin import Plugin
 from aac.plugins.first_party.specifications.specifications_impl import plugin_name, spec_csv
-from aac.plugins.first_party.specifications.globally_unique_id import validate_unique_ids
-from aac.plugins.first_party.specifications.referenced_ids_exist import validate_referenced_ids
 from aac.plugins._common import get_plugin_definitions_from_yaml
 
 
 @hookimpl
 def get_plugin() -> Plugin:
     """
     Returns information about the plugin.
@@ -20,16 +16,14 @@
     Returns:
         A collection of information about the plugin and what it contributes.
     """
     plugin = Plugin(plugin_name)
     plugin_definitions = _get_plugin_definitions()
     plugin.register_commands(_get_plugin_commands())
     plugin.register_definitions(plugin_definitions)
-    plugin.register_definition_validations(_get_validations(plugin_definitions))
-    logging.info("Spec plugin created.")
 
     return plugin
 
 
 def _get_plugin_commands():
     spec_csv_arguments = [
         AacCommandArgument(
@@ -54,22 +48,7 @@
     ]
 
     return plugin_commands
 
 
 def _get_plugin_definitions() -> list[Definition]:
     return get_plugin_definitions_from_yaml(__package__, "specifications.yaml")
-
-
-def _get_validations(plugin_definitions: list[Definition]) -> list[DefinitionValidationContribution]:
-    global_id_validation_definition = get_definition_by_name("Requirement ID is unique", plugin_definitions)
-    id_exists_validation_definition = get_definition_by_name("Referenced IDs exist", plugin_definitions)
-
-    validations = []
-    if global_id_validation_definition and id_exists_validation_definition:
-        global_id_validation = DefinitionValidationContribution(global_id_validation_definition.name, global_id_validation_definition, validate_unique_ids)
-        id_exists_validation = DefinitionValidationContribution(id_exists_validation_definition.name, id_exists_validation_definition, validate_referenced_ids)
-        validations = [global_id_validation, id_exists_validation]
-    else:
-        logging.error("Failed to source expected specification validation definitions.")
-
-    return validations
```

## aac/plugins/first_party/specifications/specifications.yaml

```diff
@@ -1,222 +1,25 @@
-model:
-  name: specifications
-  description: aac-spec is a Architecture-as-Code plugin that enables requirement definition and traceability in Architecture-as-Code models.
-  behavior:
+plugin:
+  name: Specifications
+  description: An AaC plugin that enables requirement definition and traceability in Architecture-as-Code.
+  commands:
     - name: spec-csv
-      type: command
-      description: Generates a comma separated value file (i.e. Excel file) listing requirements.
+      group: Generation
+      helpText: Generate a CSV file listing requirements.
       input:
         - name: architecture-file
           type: file
           python_type: str
-          description:  The file to convert into csv.
+          description:  The file to convert into CSV.
         - name: output-directory
           type: file
           python_type: str
-          description: The directory where the csv file should be placed.
+          description: The directory into which the CSV file will be generated.
       acceptance:
-        - scenario: Valid spec is converted to csv.
+        - scenario: A CSV file is generated from a valid specification.
           given:
-            - The {{spec-validate.input.architecture-file}} contains a valid architecture specification.
+            - The {{spec-csv.input.architecture-file}} contains a valid architecture specification.
           when:
             - The aac app is run with the spec-csv command.
           then:
-            - A message saying spec csv generation was successful is printed to the console.
-            - a csv file is generated.
----
-validation:
-  name: Referenced IDs exist
-  description: Verifies ids in a requirement reference exist within the context.
-  behavior:
-    - name: Verify that requirement references exist.
-      type: request-response
-      description:
-      input:
-        - name: input
-          type: ValidatorInput
-      output:
-        - name: results
-          type: ValidatorOutput
-      acceptance:
-        - scenario: Successfully Validate a requirement reference id exists
-          given:
-            - The ValidatorInput content consists of valid AaC definitions.
-            - The ValidatorInput contains some AaC fields that reference requirement ids.
-          when:
-            - The input is validation
-          then:
-            - The ValidatorOutput does not indicate any errors
-            - The ValidatorOutput does not indicate any warnings
-            - The ValidatorOutput indicates the definition under test is valid
-        - scenario: Fail to validate a definition's requirement reference fields
-          given:
-            - The ValidatorInput content consists of otherwise valid AaC definitions.
-            - The ValidatorInput contains at least one requirement reference id that does not exist.
-          when:
-            - The ValidatorInput is validated
-          then:
-            - The ValidatorOutput has errors
-            - The ValidatorOutput errors indicate that there are invalid requirement id references
----
-validation:
-  name: Requirement ID is unique
-  description: Verifies ids in a requirement ID is globally unique within the context.
-  behavior:
-    - name: Verify that requirement ids are globally unique.
-      type: request-response
-      description:
-      input:
-        - name: input
-          type: ValidatorInput
-      output:
-        - name: results
-          type: ValidatorOutput
-      acceptance:
-        - scenario: Successfully Validate a requirement id uniqueness
-          given:
-            - The ValidatorInput content consists of valid AaC definitions.
-            - The ValidatorInput contains some AaC spec definitions where requirement ids are unique.
-          when:
-            - The input is validation
-          then:
-            - The ValidatorOutput does not indicate any errors
-            - The ValidatorOutput does not indicate any warnings
-            - The ValidatorOutput indicates the definition under test is valid
-        - scenario: Fail to validate a requirement id uniqueness
-          given:
-            - The ValidatorInput content consists of otherwise valid AaC definitions.
-            - The ValidatorInput contains some AaC spec definition where duplicate requirement ids are present.
-          when:
-            - The ValidatorInput is validated
-          then:
-            - The ValidatorOutput has errors
-            - The ValidatorOutput errors indicate that there are non-unique requirement ids
----
-ext:
-  name: addLoggingToBehaviorType
-  type: BehaviorType
-  enumExt:
-    add:
-      - logging
----
-ext:
-  name: addSpecificationToRoot
-  type: root
-  schemaExt:
-    add:
-      - name: spec
-        type: Specification
----
-ext:
-  name: addSpecTraceToModel
-  type: model
-  schemaExt:
-    add:
-      - name: requirements
-        type: RequirementReference
----
-ext:
-  name: addSpecTraceToBehavior
-  type: Behavior
-  schemaExt:
-    add:
-      - name: requirements
-        type: RequirementReference
----
-ext:
-  name: addSpecTraceToSchema
-  type: schema
-  schemaExt:
-    add:
-      - name: requirements
-        type: RequirementReference
----
-schema:
-  name: Specification
-  fields:
-    - name: name
-      type: string
-    - name: description
-      type: string
-    - name: sections
-      type: SpecSection[]
-    - name: requirements
-      type: Requirement[]
-  required:
-    - name
-  validation:
-    - name: Required fields are present
-      arguments:
-        - name
----
-schema:
-  name: SpecSection
-  fields:
-    - name: name
-      type: string
-    - name: description
-      type: string
-    - name: requirements
-      type: Requirement[]
-  required:
-    - name
-  validation:
-    - name: Required fields are present
-      arguments:
-        - name
----
-schema:
-  name: Requirement
-  fields:
-    - name: id
-      type: string
-    - name: shall
-      type: string
-    - name: parent
-      type: RequirementReference
-    - name: child
-      type: RequirementReference
-    - name: attributes
-      type: RequirementAttribute[]
-  required:
-    - id
-    - shall
-  validation:
-    - name: Required fields are present
-      arguments:
-        - id
-        - shall
-    - name: Requirement ID is unique
-      arguments:
-        - id
----
-schema:
-  name: RequirementAttribute
-  fields:
-    - name: name
-      type: string
-    - name: value
-      type: string
-  required:
-    - name
-    - value
-  validation:
-    - name: Required fields are present
-      arguments:
-        - name
-        - value
----
-schema:
-  name: RequirementReference
-  fields:
-    - name: ids
-      type: string[]
-  required:
-    - ids
-  validation:
-    - name: Required fields are present
-      arguments:
-        - ids
-    - name: Referenced IDs exist
-      arguments:
-        - ids
+            - A message saying spec CSV generation was successful is printed to the console.
+            - A CSV file is generated.
```

## aac/plugins/first_party/specifications/specifications_impl.py

```diff
@@ -1,17 +1,19 @@
-"""AaC Plugin implementation module for the aac-spec plugin."""
+"""AaC Plugin implementation module for the Specifications plugin."""
+
 import csv
+
 from os import path, makedirs
 from typing import List
 
 from aac.lang.definitions.definition import Definition
 from aac.plugins.plugin_execution import PluginExecutionResult, plugin_result
 from aac.validate import validated_source
 
-plugin_name = "specification"
+plugin_name = "Specifications"
 
 
 def spec_csv(architecture_file: str, output_directory: str) -> PluginExecutionResult:
     """
     Generate a csv requirements table from a specification definition.
 
     Args:
@@ -34,15 +36,15 @@
             makedirs(output_directory)
 
         file_counter = 0
         for spec_name in reqs.keys():
             file_name = spec_name + ".csv"
             file_name = file_name.replace(" ", "_")
             output_path = path.join(output_directory, file_name)
-            with open(output_path, 'w') as output:
+            with open(output_path, "w") as output:
                 writer = csv.DictWriter(output, fieldnames=field_names)
                 writer.writeheader()
                 writer.writerows(reqs[spec_name])
                 file_counter = file_counter + 1
 
         return f"{file_counter} CSV spec files written to {output_directory}"
```

## aac/plugins/validators/__init__.py

```diff
@@ -1,17 +1,20 @@
 """A plugins sub-module specifically for 1st party validator plugins."""
 
+from aac.plugins.validators._validator_finding import FindingSeverity, ValidatorFinding
 from aac.plugins.validators._validator_findings import ValidatorFindings
 from aac.plugins.validators._finding_location import FindingLocation
 from aac.plugins.validators._validator_result import ValidatorResult
 from aac.plugins.validators._common import (
     get_validation_definition_from_plugin_yaml,
     get_validation_definition_from_plugin_definitions,
 )
 
 __all__ = (
     ValidatorResult.__name__,
+    ValidatorFinding.__name__,
     ValidatorFindings.__name__,
     FindingLocation.__name__,
+    FindingSeverity.__name__,
     get_validation_definition_from_plugin_yaml.__name__,
     get_validation_definition_from_plugin_definitions.__name__,
 )
```

## aac/plugins/validators/_common.py

```diff
@@ -1,12 +1,12 @@
 """Module for common, shared functions specifically for the validator subclass of plugins."""
-
 from typing import Callable
-from aac.io.parser import parse
 
+from aac.io.parser import parse
+from aac.io.parser._parser_error import ParserError
 from aac.lang.definitions.collections import get_definitions_by_root_key
 from aac.lang.definitions.definition import Definition
 from aac.plugins import PluginError
 from aac.plugins.contributions.contribution_types import DefinitionValidationContribution
 
 
 def get_validation_definition_from_plugin_yaml(plugin_definitions_string: str) -> Definition:
@@ -15,15 +15,20 @@
 
     Args:
         plugin_definitions_string (str): The definitions as a yaml string
 
     Returns:
         The validation definition for the plugin.
     """
-    return get_validation_definition_from_plugin_definitions(parse(plugin_definitions_string))
+    try:
+        validation_definition = get_validation_definition_from_plugin_definitions(parse(plugin_definitions_string))
+    except ParserError as error:
+        raise ParserError(error.source, error.errors) from None
+    else:
+        return validation_definition
 
 
 def get_validation_definition_from_plugin_definitions(validator_definitions: list[Definition]) -> Definition:
     """
     Find the Definition associated with the specific validator plugin.
 
     Args:
```

## aac/plugins/validators/_validator_result.py

```diff
@@ -29,12 +29,11 @@
 
     def get_messages_as_string(self) -> str:
         """Get all of the validator result messages as a single string."""
 
         def format_message(finding: ValidatorFinding) -> str:
             loc = finding.location
             return (
-                f"\nValidation finding from '{loc.validation_name}' of level {finding.severity.name} in {loc.source.uri}. "
-                f"Message:\n {finding.message}"
+                f"\nValidation {finding.severity.name} from '{loc.validation_name}' in {loc.source.uri}. {finding.message}"
             )
 
         return "\n".join([format_message(finding) for finding in self.findings.get_all_findings()])
```

## aac/plugins/validators/defined_references/_validate_references.py

```diff
@@ -4,15 +4,16 @@
 from aac.lang.definitions.lexeme import Lexeme
 from aac.lang.definitions.source_location import SourceLocation
 from aac.lang.definitions.structure import get_substructures_by_type
 from aac.lang.language_context import LanguageContext
 from aac.plugins.validators import ValidatorFindings, ValidatorResult
 
 
-PLUGIN_NAME = "Type references exist"
+PLUGIN_NAME = "Validate type references"
+VALIDATION_NAME = "Type references exist"
 
 
 def validate_references(
     definition_under_test: Definition,
     target_schema_definition: Definition,
     language_context: LanguageContext,
     *validation_args,
@@ -51,15 +52,17 @@
             else:
                 missing_field_in_dictionary = f"Missing field 'type' in validation content dictionary: {dict_to_validate}"
                 logging.debug(missing_field_in_dictionary)
                 name_lexeme = definition_under_test.get_lexeme_with_value(definition_under_test.name)
 
                 if not name_lexeme:
                     name_lexeme, *_ = definition_under_test.lexemes
-                    name_lexeme = name_lexeme or Lexeme(SourceLocation(0, 0, 0, 0), definition_under_test.source.uri, definition_under_test.name)
+                    name_lexeme = name_lexeme or Lexeme(
+                        SourceLocation(0, 0, 0, 0), definition_under_test.source.uri, definition_under_test.name
+                    )
                     logging.error(f"Definition '{definition_under_test.name}' is missing its name lexeme.")
 
                 findings.add_error_finding(definition_under_test, missing_field_in_dictionary, PLUGIN_NAME, name_lexeme)
 
     dicts_to_test = get_substructures_by_type(definition_under_test, target_schema_definition, language_context)
     list(map(validate_dict, dicts_to_test))
```

## aac/plugins/validators/defined_references/defined_references.yaml

```diff
@@ -1,33 +1,39 @@
+plugin:
+  name: Validate type references
+  description: An AaC plugin that enables validating the types of references.
+  definitionValidations:
+    - name: Type references exist
+---
 validation:
   name: Type references exist
-  description: Verify that references to definitions and models are defined
+  description: Verify that references to definitions and models are defined.
   behavior:
-    - name: Verify that referenced definitions are defined
-      type: request-response
+    - name: Verify that referenced definitions are defined.
+      type: REQUEST_RESPONSE
       description:
       input:
         - name: input
           type: ValidatorInput
       output:
         - name: results
           type: ValidatorOutput
       acceptance:
-        - scenario: Successfully validate definition references
+        - scenario: Successfully validate definition references.
           given:
             - The ValidatorInput content consists of valid AaC definitions.
             - The ValidatorInput contains some AaC definitions that reference other definitions.
           when:
-            - The input is validated
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput does not indicate any errors
-            - The ValidatorOutput does not indicate any warnings
-            - The ValidatorOutput indicates the validator plugin under test is valid
-        - scenario: Fail to validate definition references
+            - The ValidatorOutput does not indicate any errors.
+            - The ValidatorOutput does not indicate any warnings.
+            - The ValidatorOutput indicates the validator plugin under test is valid.
+        - scenario: Fail to validate definition references.
           given:
             - The ValidatorInput content consists of otherwise valid AaC definitions.
             - The ValidatorInput contains at least one AaC definitions that references a definition that does not exist.
           when:
-            - The ValidatorInput is validated
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput has errors
-            - The ValidatorOutput errors indicate that there is no corresponding definition with the same name
+            - The ValidatorOutput has errors.
+            - The ValidatorOutput errors indicate that there is no corresponding definition with the same name.
```

## aac/plugins/validators/exclusive_fields/__init__.py

```diff
@@ -1,14 +1,14 @@
 """Validation plugin that ensures that only one of the fields identified via arguments is defined."""
 
 from aac.plugins import hookimpl
 from aac.plugins.plugin import Plugin
 from aac.plugins._common import get_plugin_definitions_from_yaml
 from aac.plugins.validators._common import get_plugin_validations_from_definitions
-from aac.plugins.validators.exclusive_fields._exclusive_fields import PLUGIN_NAME, validate_exclusive_fields
+from aac.plugins.validators.exclusive_fields._validate_exclusive_fields import PLUGIN_NAME, validate_exclusive_fields
 
 
 @hookimpl
 def get_plugin() -> Plugin:
     """
     Returns information about the plugin.
```

## aac/plugins/validators/exclusive_fields/exclusive_fields.yaml

```diff
@@ -1,46 +1,55 @@
+plugin:
+  name: Validate mutually exlusive fields
+  description: |
+    An AaC plugin that enables validating the presence of only one of a number
+    of mutually exclusive fields on a definition.
+  definitionValidations:
+    - name: Mutually exclusive fields
+---
 validation:
   name: Mutually exclusive fields
   description: |
     Verify that only one of the fields are defined at any time.
 
-    Exclusive fields are defined by declaring the exclusive field names as validation arguments.
+    Exclusive fields are defined by declaring the exclusive field names as
+    validation arguments.
   behavior:
     - name: Verify mutually exclusive fields
-      type: request-response
+      type: REQUEST_RESPONSE
       description:
       input:
         - name: input
           type: ValidatorInput
       output:
         - name: results
           type: ValidatorOutput
       acceptance:
-        - scenario: Successfully validate one exclusive field
+        - scenario: Successfully validate one exclusive field.
           given:
             - The ValidatorInput content consists of valid AaC definitions.
             - The ValidatorInput contains some AaC definitions with only one of the mutually exclusive fields defined.
           when:
-            - The input is validation
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput does not indicate any errors
-            - The ValidatorOutput does not indicate any warnings
-            - The ValidatorOutput indicates the validator plugin under test is valid
-        - scenario: Successfully validate zero exclusive fields
+            - The ValidatorOutput does not indicate any errors.
+            - The ValidatorOutput does not indicate any warnings.
+            - The ValidatorOutput indicates the validator plugin under test is valid.
+        - scenario: Successfully validate zero exclusive fields.
           given:
             - The ValidatorInput content consists of valid AaC definitions.
             - The ValidatorInput contains some AaC definitions with none of the mutually exclusive fields defined.
           when:
-            - The input is validation
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput does not indicate any errors
-            - The ValidatorOutput does not indicate any warnings
-            - The ValidatorOutput indicates the validator plugin under test is valid
-        - scenario: Fail to validate multiple exclusive fields
+            - The ValidatorOutput does not indicate any errors.
+            - The ValidatorOutput does not indicate any warnings.
+            - The ValidatorOutput indicates the validator plugin under test is valid.
+        - scenario: Fail to validate multiple exclusive fields.
           given:
             - The ValidatorInput content consists of otherwise valid AaC definitions.
             - The ValidatorInput contains some AaC definitions with more than one of the mutually exclusive fields defined.
           when:
-            - The ValidatorInput is validated
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput has errors
-            - The ValidatorOutput errors indicate that mutually exclusive fields are simultaneously defined.
+            - The ValidatorOutput has errors.
+            - The ValidatorOutput errors indicate that mutually exclusive fields are simultaneously defined.
```

## aac/plugins/validators/reference_fields/_validate_reference_fields.py

```diff
@@ -3,15 +3,16 @@
 from aac.lang.definitions.definition import Definition
 from aac.lang.definitions.references import is_reference_format_valid
 from aac.lang.definitions.structure import get_substructures_by_type
 from aac.lang.language_context import LanguageContext
 from aac.plugins.validators import ValidatorFindings, ValidatorResult
 
 
-PLUGIN_NAME = "Reference format valid"
+PLUGIN_NAME = "Validate query reference format"
+VALIDATION_NAME = "Reference format valid"
 
 
 def validate_reference_fields(
     definition_under_test: Definition,
     target_schema_definition: Definition,
     language_context: LanguageContext,
     *validation_args,
@@ -54,16 +55,16 @@
                 reference_field_name_lexeme = definition_under_test.get_lexeme_with_value(reference_field_name)
                 findings.add_error_finding(
                     definition_under_test, missing_reference_field, PLUGIN_NAME, reference_field_name_lexeme
                 )
                 logging.debug(missing_reference_field)
 
             # field must be contain a parsable reference value
-            elif not is_reference_format_valid(field_value)[0]:
-                invalid_reference_format = f"Reference field '{reference_field_name}' is not properly formatted: {field_value} - {is_reference_format_valid(field_value)[1]}"
+            elif not is_reference_format_valid(field_value):
+                invalid_reference_format = f"Reference field '{reference_field_name}' is not properly formatted: {field_value}"
                 reference_field_name_lexeme = definition_under_test.get_lexeme_with_value(reference_field_name)
                 findings.add_error_finding(
                     definition_under_test, invalid_reference_format, PLUGIN_NAME, reference_field_name_lexeme
                 )
                 logging.debug(invalid_reference_format)
 
     dicts_to_test = get_substructures_by_type(definition_under_test, target_schema_definition, language_context)
```

## aac/plugins/validators/reference_fields/reference_fields.yaml

```diff
@@ -1,33 +1,40 @@
+plugin:
+  name: Validate query reference format
+  description: |
+    An AaC plugin that enables validating the format of a query reference.
+  definitionValidations:
+    - name: Reference format valid
+---
 validation:
   name: Reference format valid
-  description: Verifies every field declared as reference is properly formatted for processing
+  description: Verify that every field declared as reference is properly formatted for processing.
   behavior:
-    - name: Verify that reference fields properly formatted.
-      type: request-response
+    - name: Verify that reference fields are properly formatted.
+      type: REQUEST_RESPONSE
       description:
       input:
         - name: input
           type: ValidatorInput
       output:
         - name: results
           type: ValidatorOutput
       acceptance:
-        - scenario: Successfully Validate a definition's reference fields
+        - scenario: Successfully validate a definition's reference fields.
           given:
             - The ValidatorInput content consists of valid AaC definitions.
             - The ValidatorInput contains some AaC fields that reference other definitions.
           when:
-            - The input is validation
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput does not indicate any errors
-            - The ValidatorOutput does not indicate any warnings
-            - The ValidatorOutput indicates the definition under test is valid
-        - scenario: Fail to validate a definition's reference fields
+            - The ValidatorOutput does not indicate any errors.
+            - The ValidatorOutput does not indicate any warnings.
+            - The ValidatorOutput indicates the definition under test is valid.
+        - scenario: Fail to validate a definition's reference fields.
           given:
             - The ValidatorInput content consists of otherwise valid AaC definitions.
             - The ValidatorInput contains at least one reference field that is incorrectly formatted.
           when:
-            - The ValidatorInput is validated
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput has errors
-            - The ValidatorOutput errors indicate that there are incorrectly formatted reference fields
+            - The ValidatorOutput has errors.
+            - The ValidatorOutput errors indicate that there are incorrectly formatted reference fields.
```

## aac/plugins/validators/reference_targets/_validate_reference_targets.py

```diff
@@ -1,17 +1,19 @@
 import logging
 
+from aac.lang.constants import DEFINITION_FIELD_FIELDS, DEFINITION_FIELD_NAME, DEFINITION_FIELD_TYPE, PRIMITIVE_TYPE_REFERENCE
 from aac.lang.definitions.definition import Definition
 from aac.lang.definitions.references import get_reference_target_definitions, is_reference_format_valid
 from aac.lang.definitions.structure import get_substructures_by_type
 from aac.lang.language_context import LanguageContext
 from aac.plugins.validators import FindingLocation, ValidatorFindings, ValidatorResult
 
 
-PLUGIN_NAME = "Reference target valid"
+PLUGIN_NAME = "Validate query reference targets"
+VALIDATION_NAME = "Reference target valid"
 
 
 def validate_reference_targets(
     definition_under_test: Definition,
     target_schema_definition: Definition,
     language_context: LanguageContext,
     *validation_args,
@@ -27,24 +29,24 @@
 
     Returns:
         A ValidatorResult containing any applicable error messages.
     """
     findings = ValidatorFindings()
 
     reference_field_names = validation_args
-    schema_defined_fields_as_list = target_schema_definition.get_top_level_fields().get("fields") or []
-    schema_defined_fields_as_dict = {field.get("name"): field for field in schema_defined_fields_as_list}
+    schema_defined_fields_as_list = target_schema_definition.get_top_level_fields().get(DEFINITION_FIELD_FIELDS) or []
+    schema_defined_fields_as_dict = {field.get(DEFINITION_FIELD_NAME): field for field in schema_defined_fields_as_list}
 
     def validate_dict(dict_to_validate: dict) -> None:
         for reference_field_name in reference_field_names:
             field_value = dict_to_validate.get(reference_field_name)
-            field_type = schema_defined_fields_as_dict.get(reference_field_name, {}).get("type")
+            field_type = schema_defined_fields_as_dict.get(reference_field_name, {}).get(DEFINITION_FIELD_TYPE)
 
             # field type must be reference
-            if field_type != "reference":
+            if field_type != PRIMITIVE_TYPE_REFERENCE:
                 non_reference_field = f"Reference format validation cannot be performed on non-reference field '{reference_field_name}'.  Type is '{field_type}'"
                 reference_field_name_lexeme = definition_under_test.get_lexeme_with_value(reference_field_name)
                 findings.add_error_finding(
                     definition_under_test, non_reference_field, PLUGIN_NAME, reference_field_name_lexeme
                 )
                 logging.debug(non_reference_field)
 
@@ -54,16 +56,16 @@
                 reference_field_name_lexeme = definition_under_test.get_lexeme_with_value(reference_field_name)
                 findings.add_error_finding(
                     definition_under_test, missing_reference_field, PLUGIN_NAME, reference_field_name_lexeme
                 )
                 logging.debug(missing_reference_field)
 
             # field must be contain a parsable reference value
-            elif not is_reference_format_valid(field_value)[0]:
-                invalid_reference_format = f"Reference field '{reference_field_name}' is not properly formatted: {field_value} - {is_reference_format_valid(field_value)[1]}"
+            elif not is_reference_format_valid(field_value):
+                invalid_reference_format = f"Reference field '{reference_field_name}' is not properly formatted: {field_value}"
                 reference_field_name_lexeme = definition_under_test.get_lexeme_with_value(reference_field_name)
                 findings.add_error_finding(
                     definition_under_test, invalid_reference_format, PLUGIN_NAME, reference_field_name_lexeme
                 )
                 logging.debug(invalid_reference_format)
 
             # field must reference an existing target
```

## aac/plugins/validators/reference_targets/reference_targets.yaml

```diff
@@ -1,33 +1,41 @@
+plugin:
+  name: Validate query reference targets
+  description: An AaC plugin that enables validating query reference targets.
+  definitionValidations:
+    - name: Reference target valid
+---
 validation:
   name: Reference target valid
-  description: Verifies every field declared as reference are valid and reference an existing model element
+  description: |
+    Verify every field declared as a reference is valid and reference an
+    existing model element.
   behavior:
-    - name: Reference target valid
-      type: request-response
+    - name: Reference target is valid.
+      type: REQUEST_RESPONSE
       description:
       input:
         - name: input
           type: ValidatorInput
       output:
         - name: results
           type: ValidatorOutput
       acceptance:
-        - scenario: Successfully Validate a definition's reference field targets
+        - scenario: Successfully validate a definition's reference field targets.
           given:
             - The ValidatorInput content consists of valid AaC definitions.
             - The ValidatorInput contains some AaC fields that reference other existing definitions.
           when:
-            - The input is validation
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput does not indicate any errors
-            - The ValidatorOutput does not indicate any warnings
-            - The ValidatorOutput indicates the validator plugin under test is valid
-        - scenario: Fail to validate a definition's reference field targets
+            - The ValidatorOutput does not indicate any errors.
+            - The ValidatorOutput does not indicate any warnings.
+            - The ValidatorOutput indicates the validator plugin under test is valid.
+        - scenario: Fail to validate a definition's reference field targets.
           given:
             - The ValidatorInput content consists of otherwise valid AaC definitions.
             - The ValidatorInput contains at least one reference field that references a non-existent target.
           when:
-            - The ValidatorInput is validated
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput has errors
-            - The ValidatorOutput errors indicate that there are reference field targets
+            - The ValidatorOutput has errors.
+            - The ValidatorOutput errors indicate that there are reference field targets.
```

## aac/plugins/validators/required_fields/__init__.py

```diff
@@ -1,15 +1,20 @@
 """Validation plugin to ensure that each definition has all required fields populated."""
 
+from aac.lang.constants import DEFINITION_FIELD_ARGUMENTS, DEFINITION_FIELD_NAME
 from aac.lang.definitions.definition import Definition
 from aac.plugins import hookimpl
 from aac.plugins.plugin import Plugin
 from aac.plugins._common import get_plugin_definitions_from_yaml
 from aac.plugins.validators._common import get_plugin_validations_from_definitions
-from aac.plugins.validators.required_fields._validate_required_fields import PLUGIN_NAME, validate_required_fields
+from aac.plugins.validators.required_fields._validate_required_fields import (
+    PLUGIN_NAME,
+    VALIDATION_NAME,
+    validate_required_fields,
+)
 
 
 @hookimpl
 def get_plugin() -> Plugin:
     """
     Returns information about the plugin.
 
@@ -36,9 +41,9 @@
 
     Args:
         definition (Definition): The definition to search through
 
     Returns:
         The list of field names declared as required fields in the definition.
     """
-    required_validation = [v for v in definition.get_validations() or [] if v.get("name") == PLUGIN_NAME]
-    return len(required_validation) == 1 and required_validation[0].get("arguments") or []
+    required_validation = [v for v in definition.get_validations() or [] if v.get(DEFINITION_FIELD_NAME) == VALIDATION_NAME]
+    return len(required_validation) == 1 and required_validation[0].get(DEFINITION_FIELD_ARGUMENTS) or []
```

## aac/plugins/validators/required_fields/_validate_required_fields.py

```diff
@@ -4,15 +4,16 @@
 from aac.lang.definitions.definition import Definition
 from aac.lang.definitions.structure import get_substructures_by_type
 from aac.lang.definitions.type import is_array_type
 from aac.lang.language_context import LanguageContext
 from aac.plugins.validators import ValidatorFindings, ValidatorResult
 
 
-PLUGIN_NAME = "Required fields are present"
+PLUGIN_NAME = "Validate required fields"
+VALIDATION_NAME = "Required fields are present"
 
 
 def validate_required_fields(
     definition_under_test: Definition,
     target_schema_definition: Definition,
     language_context: LanguageContext,
     *validation_args,
```

## aac/plugins/validators/required_fields/required_fields.yaml

```diff
@@ -1,33 +1,39 @@
+plugin:
+  name: Validate required fields
+  description: An AaC plugin that enables validating all required fields are present in a definition.
+  definitionValidations:
+    - name: Required fields are present
+---
 validation:
   name: Required fields are present
-  description: Verifies every field declared as required is present and populated
+  description: Verify every field declared as required is present and populated.
   behavior:
     - name: Verify that definition fields marked as required are populated.
-      type: request-response
+      type: REQUEST_RESPONSE
       input:
         - name: input
           type: ValidatorInput
       output:
         - name: results
           type: ValidatorOutput
       acceptance:
-        - scenario: Successfully Validate a definition's required fields
+        - scenario: Successfully Validate a definition's required fields.
           given:
             - The ValidatorInput content consists of valid AaC definitions.
             - The ValidatorInput contains some AaC definitions that reference other definitions.
           when:
-            - The input is validation
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput does not indicate any errors
-            - The ValidatorOutput does not indicate any warnings
-            - The ValidatorOutput indicates the validator plugin under test is valid
-        - scenario: Fail to validate a definition's required fields
+            - The ValidatorOutput does not indicate any errors.
+            - The ValidatorOutput does not indicate any warnings.
+            - The ValidatorOutput indicates the validator plugin under test is valid.
+        - scenario: Fail to validate a definition's required fields.
           given:
             - The ValidatorInput content consists of otherwise valid AaC definitions.
             - The ValidatorInput contains at least one field that is required.
             - The ValidatorInput contains at least one required field that is missing.
           when:
-            - The ValidatorInput is validated
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput has errors
-            - The ValidatorOutput errors indicate that there are missing required fields
+            - The ValidatorOutput has errors.
+            - The ValidatorOutput errors indicate that there are missing required fields.
```

## aac/plugins/validators/root_keys/_validate_root_keys.py

```diff
@@ -2,15 +2,16 @@
 
 from aac.lang.definitions.definition import Definition
 from aac.lang.language_context import LanguageContext
 from aac.plugins.validators import ValidatorResult
 from aac.plugins.validators._validator_findings import ValidatorFindings
 
 
-PLUGIN_NAME = "Root key is defined"
+PLUGIN_NAME = "Validate root keys"
+VALIDATION_NAME = "Root key is defined"
 
 
 def validate_root_keys(
     definition_under_test: Definition,
     target_schema_definition: Definition,
     language_context: LanguageContext,
     *validation_args,
```

## aac/plugins/validators/root_keys/root_keys.yaml

```diff
@@ -1,44 +1,51 @@
+plugin:
+  name: Validate root keys
+  description: |
+    An AaC plugin that enables validating that the root key of a definition is
+    defined.
+  definitionValidations:
+    - name: Root key is defined
+---
 validation:
   name: Root key is defined
-  description: Verify that the definition's root key is defined
+  description: Verify that the definition's root key is defined.
   behavior:
-    - name: Verify that the definition's root key is defined
-      type: request-response
-      description:
+    - name: Verify that the definition's root key is defined.
+      type: REQUEST_RESPONSE
       input:
         - name: input
           type: ValidatorInput
       output:
         - name: results
           type: ValidatorOutput
       acceptance:
-        - scenario: Successfully validate definition root key
+        - scenario: Successfully validate definition root key.
           given:
             - The ValidatorInput content consists of valid AaC definitions.
             - The ValidatorInput contains some AaC definition that has a root key defined by the 'root' definition in the core specification.
           when:
-            - The ValidatorInput is validated
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput does not indicate any errors
-            - The ValidatorOutput does not indicate any warnings
-            - The ValidatorOutput indicates the definition under test is valid
-        - scenario: Successfully validate an extended root key
+            - The ValidatorOutput does not indicate any errors.
+            - The ValidatorOutput does not indicate any warnings.
+            - The ValidatorOutput indicates the definition under test is valid.
+        - scenario: Successfully validate an extended root key.
           given:
             - The ValidatorInput content consists of valid AaC definitions.
             - The ValidatorInput content of an extension definition that adds a new root key.
             - The ValidatorInput contains some AaC definition that has a root key that has been added to the 'root' definition in the core specification.
           when:
-            - The ValidatorInput is validated
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput does not indicate any errors
-            - The ValidatorOutput does not indicate any warnings
-            - The ValidatorOutput indicates the definition under test is valid
-        - scenario: Fail to validate definitions that reference keys that are not defined by the 'root' definition
+            - The ValidatorOutput does not indicate any errors.
+            - The ValidatorOutput does not indicate any warnings.
+            - The ValidatorOutput indicates the definition under test is valid.
+        - scenario: Fail to validate definitions that reference keys that are not defined by the 'root' definition.
           given:
             - The ValidatorInput content consists of otherwise valid AaC definitions.
             - The ValidatorInput contains at least one AaC definition that has a root key not defined by the 'root' definition in the core specification.
           when:
-            - The ValidatorInput is validated
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput has errors
+            - The ValidatorOutput has errors.
             - The ValidatorOutput errors indicate that the root key is not defined in the root keys definition.
```

## aac/plugins/validators/subcomponent_type/__init__.py

```diff
@@ -1,14 +1,14 @@
 """Validation plugin to ensure that each model definition has subcomponents of type model."""
 
 from aac.plugins import hookimpl
 from aac.plugins.plugin import Plugin
 from aac.plugins._common import get_plugin_definitions_from_yaml
 from aac.plugins.validators._common import get_plugin_validations_from_definitions
-from aac.plugins.validators.subcomponent_type._subcomponent_type import PLUGIN_NAME, validate_subcomponent_types
+from aac.plugins.validators.subcomponent_type._validate_subcomponent_type import PLUGIN_NAME, validate_subcomponent_types
 
 
 @hookimpl
 def get_plugin() -> Plugin:
     """
     Returns information about the plugin.
```

## aac/plugins/validators/subcomponent_type/subcomponent_type.yaml

```diff
@@ -1,35 +1,43 @@
+plugin:
+  name: Validate model subcomponents
+  description: |
+    An AaC plugin that enables validating subcomponents of a model are models.
+  definitionValidations:
+    - name: Subcomponents are models
+---
 validation:
   name: Subcomponents are models
-  description: Verifies that the type field of every subcomponent refers to a model.
+  description: |
+    Verify that the type field of every subcomponent refers to a model.
   behavior:
     - name: Verify that subcomponents are of the model type.
-      type: request-response
+      type: REQUEST_RESPONSE
       description:
       input:
         - name: input
           type: ValidatorInput
       output:
         - name: results
           type: ValidatorOutput
       acceptance:
-        - scenario: Successfully Validate a model definition's subcomponent types
+        - scenario: Successfully Validate a model definition's subcomponent types.
           given:
             - The ValidatorInput content consists of a model definition.
             - The ValidatorInput contains at least one subcomponent.
             - All subcomponents are model types.
           when:
-            - The ValidatorInput is validated
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput does not indicate any errors
-            - The ValidatorOutput does not indicate any warnings
-            - The ValidatorOutput indicates the definition under test is valid
-        - scenario: Fail to validate a model's subcomponent types
+            - The ValidatorOutput does not indicate any errors.
+            - The ValidatorOutput does not indicate any warnings.
+            - The ValidatorOutput indicates the definition under test is valid.
+        - scenario: Fail to validate a model's subcomponent types.
           given:
             - The ValidatorInput content consists of a model definition.
             - The ValidatorInput contains at least one subcomponent.
             - The type of at least one of the subcomponents is not model.
           when:
-            - The ValidatorInput is validated
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput has errors
+            - The ValidatorOutput has errors.
             - The ValidatorOutput errors indicate that the subcomponent(s) are not models.
```

## aac/plugins/validators/unique_names/__init__.py

```diff
@@ -1,14 +1,14 @@
 """Validation plugin to ensure that all Definitions have unique names."""
 
 from aac.plugins import hookimpl
 from aac.plugins.plugin import Plugin
 from aac.plugins._common import get_plugin_definitions_from_yaml
 from aac.plugins.validators._common import get_plugin_validations_from_definitions
-from aac.plugins.validators.unique_names._unique_names import PLUGIN_NAME, validate_unique_names
+from aac.plugins.validators.unique_names._validate_unique_names import PLUGIN_NAME, validate_unique_names
 
 
 @hookimpl
 def get_plugin() -> Plugin:
     """
     Returns information about the plugin.
```

## aac/plugins/validators/unique_names/unique_names.yaml

```diff
@@ -1,32 +1,38 @@
+plugin:
+  name: Validate names are not duplicated
+  description: An AaC plugin that enables validating the uniqueness of definition names.
+  definitionValidations:
+    - name: Unique definition names
+---
 validation:
   name: Unique definition names
-  description: Verifies that all Definitions have unique names.
+  description: Verify that all Definitions have unique names.
   behavior:
     - name: Verify that Definitions have unique names.
-      type: request-response
+      type: REQUEST_RESPONSE
       input:
         - name: definitions
           type: ValidatorInput
       output:
         - name: results
           type: ValidatorOutput
       acceptance:
         - scenario: Successfully validate a collection of definitions in which no definition name is duplicated.
           given:
             - The ValidatorInput, definitions, contains a collection of Definitions.
             - All of the Definition names are unique in the collection of Definitions.
           when:
-            - The "Unique definition names" validator plugin is executed.
+            - The validator plugin is executed.
           then:
             - The ValidatorOutput does not indicate any errors.
-            - The ValidatorOutput does not indicate any warnings
+            - The ValidatorOutput does not indicate any warnings.
             - The ValidatorOutput indicates the ValidatorInput under test is valid.
         - scenario: Fail to validate a collection of definitions with duplicated names.
           given:
             - The ValidatorInput, definitions, contains a collection of Definitions.
             - There are at least two Definitions in the collection with the same name.
           when:
-            - The "Unique definition names" validator plugin is executed.
+            - The validator plugin is executed.
           then:
             - The ValidatorOutput has errors.
             - The ValidatorOutput errors indicate that there are at least two Definitions with the same name.
```

## aac/plugins/validators/validator_implementation/__init__.py

```diff
@@ -1,14 +1,17 @@
 """Validation plugin to ensure that each validation definition has a corresponding validation implementation."""
 
 from aac.plugins import hookimpl
 from aac.plugins.plugin import Plugin
 from aac.plugins._common import get_plugin_definitions_from_yaml
 from aac.plugins.validators._common import get_plugin_validations_from_definitions
-from aac.plugins.validators.validator_implementation._validator_implementation import PLUGIN_NAME, validate_validator_implementations
+from aac.plugins.validators.validator_implementation._validate_validator_implementation import (
+    PLUGIN_NAME,
+    validate_validator_implementations,
+)
 
 
 @hookimpl
 def get_plugin() -> Plugin:
     """
     Returns information about the plugin.
```

## aac/plugins/validators/validator_implementation/validator_implementation.yaml

```diff
@@ -1,33 +1,41 @@
+plugin:
+  name: Validate implementations for validators
+  description: An AaC plugin that ensures an implementation exists for all validators.
+  definitionValidations:
+    - name: Validation definition has an implementation
+---
 validation:
   name: Validation definition has an implementation
-  description: Verifies that every validation definition has a corresponding python plugin implementation
+  description: |
+    Verify that every validation definition has a corresponding python plugin
+    implementation.
   behavior:
-    - name: Verify validation definition and implementation
-      type: request-response
+    - name: Verify validation definition and implementation.
+      type: REQUEST_RESPONSE
       description:
       input:
         - name: input
           type: ValidatorInput
       output:
         - name: results
           type: ValidatorOutput
       acceptance:
-        - scenario: Successfully Validate a Validator Plugin
+        - scenario: Successfully validate a validator plugin.
           given:
             - The validation plugin has a valid `validation` definition.
             - The validation definition has a corresponding python implementation.
           when:
-            - The validator plugin is tested
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput does not indicate any errors
-            - The ValidatorOutput does not indicate any warnings
-            - The ValidatorOutput indicates the validator plugin under test is valid
-        - scenario: Fail to Validate a Validator Plugin with Missing Python Implementation
+            - The ValidatorOutput does not indicate any errors.
+            - The ValidatorOutput does not indicate any warnings.
+            - The ValidatorOutput indicates the validator plugin under test is valid.
+        - scenario: Fail to validate a validator plugin with missing python implementation.
           given:
             - The validation plugin has a valid `validation` definition.
             - The validation does not have definition has a corresponding python implementation.
           when:
-            - The validator plugin is tested
+            - The validator plugin is executed.
           then:
-            - The ValidatorOutput has errors
-            - The ValidatorOutput errors indicate that there is no corresponding python implementation
+            - The ValidatorOutput has errors.
+            - The ValidatorOutput errors indicate that there is no corresponding python implementation.
```

## aac/spec/core.py

```diff
@@ -1,14 +1,17 @@
 """Functions to allow interacting with the core AaC spec."""
+import copy
 
+from aac.lang.constants import DEFINITION_FIELD_FIELDS, DEFINITION_NAME_ROOT, ROOT_KEY_SCHEMA
 from aac.lang.definitions.collections import get_definition_by_name
 from aac.lang.definitions.definition import Definition
 from aac.lang.definitions.search import search_definition
 from aac.package_resources import get_resource_file_contents, get_resource_file_path
 from aac.io.parser import parse
+from aac.io.parser._parser_error import ParserError
 
 PRIMITIVES: list[str] = []
 ROOT_NAMES: list[str] = []
 AAC_CORE_SPEC_DEFINITIONS: list[Definition] = []
 CORE_SPEC_FILE_NAME = "spec.yaml"
 
 
@@ -19,22 +22,27 @@
     The AaC model specification is
     defined as an AaC model and is needed for model validation.
 
     Returns:
         Returns a list of parsed definitions that compose the core
         AaC specification.
     """
+
     def set_files_to_not_user_editable(definition):
         definition.source.is_user_editable = False
 
     global AAC_CORE_SPEC_DEFINITIONS
     if not len(AAC_CORE_SPEC_DEFINITIONS) > 0:
         core_spec_as_yaml = get_aac_spec_as_yaml()
-        AAC_CORE_SPEC_DEFINITIONS = parse(core_spec_as_yaml, _get_aac_spec_file_path())
-        list(map(set_files_to_not_user_editable, AAC_CORE_SPEC_DEFINITIONS))
+        try:
+            AAC_CORE_SPEC_DEFINITIONS = parse(core_spec_as_yaml, _get_aac_spec_file_path())
+        except ParserError as error:
+            raise ParserError(error.source, error.errors) from None
+        else:
+            list(map(set_files_to_not_user_editable, AAC_CORE_SPEC_DEFINITIONS))
 
     return AAC_CORE_SPEC_DEFINITIONS
 
 
 def get_aac_spec_as_yaml() -> str:
     """Get the base AaC spec in YAML.
 
@@ -63,15 +71,15 @@
     """
 
     global PRIMITIVES
 
     if len(PRIMITIVES) == 0 or reload:
         aac_definitions = get_aac_spec()
         primitives_definition = get_definition_by_name("Primitives", aac_definitions)
-        PRIMITIVES = search_definition(primitives_definition, ["enum", "values"])
+        PRIMITIVES = copy.deepcopy(search_definition(primitives_definition, ["enum", "values"]))
 
     return PRIMITIVES
 
 
 def get_root_keys(reload: bool = False) -> list[str]:
     """Gets the list of root names as defined in the AaC DSL specification.
 
@@ -99,15 +107,15 @@
             Default is False.
 
     Returns:
         A list of dictionaries representing the root keys and their contextual information.
     """
 
     aac_definitions = get_aac_spec()
-    root_definition = get_definition_by_name("root", aac_definitions)
+    root_definition = get_definition_by_name(DEFINITION_NAME_ROOT, aac_definitions)
 
-    return search_definition(root_definition, ["schema", "fields"])
+    return search_definition(root_definition, [ROOT_KEY_SCHEMA, DEFINITION_FIELD_FIELDS])
 
 
 def _get_aac_spec_file_path() -> str:
     """Get the path for the spec file in the AaC package on the filesystem."""
     return get_resource_file_path(__package__, CORE_SPEC_FILE_NAME)
```

## aac/spec/spec.yaml

```diff
@@ -1,77 +1,101 @@
 schema:
-  name: root
+  name: Root
   description: |
     root is a special case representing the root of the architecture model and
     not explicitly included in a model file
   fields:
     - name: import
-      type: string[]
+      type: Import
       description: |
-        A list of references to other models composing the current model.
-
-        Component model definitions must be visible from the current model's
-        scope.
+        A definition that represents the list of imported files containing
+        externally-defined definitions that are referenced in the current file.
     - name: enum
-      type: enum
+      type: Enum
       description: |
         A definition that represents an enumerated type of value.
 
         An example of when to use an 'enum' is when you want to provide several
         different options for a single value.
     - name: schema
-      type: schema
+      type: Schema
       description: |
         A definition that defines the schema/structure of definitions.
 
         A 'schema' definition can alternatively be thought as a defining the
         data structure of a definition.
-    - name: map
-      type: Map
-      description: |
-        A definition that represents a key-value pair. Used to define Maps
-        and the types for the keys and values.
-
-        An example use of Map would be to declare a key-value data structure
-        with keys of type A and values of type B.
     - name: model
-      type: model
+      type: Model
       description: |
         A definition that represents a system and/or component model.
 
         An example of when to use a 'model' is when you want to define the
         behavior for some component of the system.
     - name: usecase
-      type: usecase
+      type: Usecase
       description: |
         A definition that represents a usecase for the system.
 
         An example of when to use a 'usecase' is when you want to define how the
         system might be used in a particular instance.
     - name: ext
-      type: extension
+      type: Extension
       description: |
         A meta definition used for adding information to another definition.
 
         An example of when to use an 'ext' is when you wish to add extra
         information to a model that isn't included in the core specification or
         the specification of any plugins you may have installed.
 
         You can extend any 'enum' and 'schema' definition.
+    - name: command_group
+      type: CommandGroup
+      description: |
+        A reference to a command group under which one, or more, plugins can
+        nest related commands.
+
+        CommandGroups are referenced by name.
+    - name: plugin
+      type: Plugin
+      description: |
+        A reference to a plugin. Plugins can provide any extra functionality
+        desired on top of AaC-modeled systems from document generation to code
+        generation and everything in between.
+
+        Plugins are referenced by name.
     - name: validation
       type: Validation
       description: |
-        A reference to a validation plugin. Validation plugins provide verification and validation
-        for the definition to which they are attached and any uses of that definition, depending
-        on the validation plugins referenced by it.
+        A reference to a validation plugin. Validation plugins provide
+        verification and validation for the definition to which they are
+        attached and any uses of that definition, depending on the validation
+        plugins referenced by it.
 
         Validators are referenced by name.
+    - name: spec
+      type: Specification
+      description: |
+        A requirement specification definition to capture desired behavior or attributes of the system being modeled.
+
+        Within many contexts requirements remain the central element of any Model-Based System Engineering solution.
+        AaC supports the definition, derivation, and trace of requirements throughout the model using the spec type and
+        associated reference capabilities.
+---
+schema:
+  name: Import
+  fields:
+    - name: files
+      type: file[]
+  validation:
+    - name: Required fields are present
+      arguments:
+        - files
 ---
 schema:
-  name: enum
+  name: Enum
   fields:
     - name: name
       type: string
       description: |
         The name of the enumeration.
     - name: values
       type: string[]
@@ -80,22 +104,22 @@
   validation:
     - name: Required fields are present
       arguments:
         - name
         - values
 ---
 schema:
-  name: extension
+  name: Extension
   fields:
     - name: name
       type: string
       description: |
         The name of the extension.
     - name: type
-      type: string
+      type: reference
       description: |
         The name of the 'schema' or 'enum' definition that this definition is
         extending.
     - name: enumExt
       type: EnumExtension
       description: |
         If extending an 'enum' definition, this represents a list of the items
@@ -110,17 +134,14 @@
         If extending an 'schema' definition, this represents a list of the items
         to add to the 'schema's 'fields' property.
 
         Note: Only one of 'enumExt' and 'schemaExt' are valid per extension.
 
         See also, 'SchemaExtension'
   validation:
-    - name: Type references exist
-      arguments:
-        - type
     - name: Mutually exclusive fields
       arguments:
         - schemaExt
         - enumExt
     - name: Required fields are present
       arguments:
         - name
@@ -178,25 +199,19 @@
         - description
         - behavior
 ---
 schema:
   name: ValidationReference
   fields:
     - name: name
-      type: string
-      description: |
-        The name of the validation definition.
+      type: reference
+      description: The name of the validation definition.
     - name: arguments
       type: string[]
-      description: |
-        A list of arguments to pass to the validator.
-  validation:
-    - name: Required fields are present
-      arguments:
-        - name
+      description: A list of arguments to pass to the validator.
 ---
 schema:
   name: ValidatorInput
   fields:
     - name: name
       type: string
       description: |
@@ -243,18 +258,19 @@
         - scenario
         - when
         - then
 ---
 enum:
   name: BehaviorType
   values:
-    - pub-sub
-    - request-response
-    - startup
-    - timer
+    - PUB_SUB
+    - REQUEST_RESPONSE
+    - STARTUP
+    - TIMER
+    - LOGGING
 ---
 enum:
   name: Primitives
   values:
     - string
     - int
     - number
@@ -291,32 +307,36 @@
         - name
         - type
     - name: Type references exist
       arguments:
         - type
 ---
 schema:
-  name: schema
+  name: Schema
   fields:
     - name: name
       type: string
       description: |
         The name of the schema definition.
     - name: inherits
-      type: DefinitionReference[]
+      type: reference[]
       description: |
         A list of Schema definition names that this definition inherits from.
     - name: fields
       type: Field[]
       description: |
         A list of fields that make up the definition.
     - name: validation
       type: ValidationReference[]
       description: |
         References and additional arguments for validations to apply to the definition.
+    - name: requirements
+      type: RequirementReference
+      description: |
+        A list of requirements that define the characteristics to be satisfied by the schema.
   validation:
     - name: Root key is defined
     - name: Required fields are present
       arguments:
         - name
         - fields
     - name: Unique definition names
@@ -353,22 +373,26 @@
         The list of all the fields that are outputs to the component when the
         behavior is performed.
     - name: acceptance
       type: Scenario[]
       description: |
         A list of scenarios that define the acceptance criteria to signify that
         the system is behaving as expected.
+    - name: requirements
+      type: RequirementReference
+      description: |
+        A list of allocated requirements defining the expected behavior to be provided.
   validation:
     - name: Required fields are present
       arguments:
         - name
         - type
 ---
 schema:
-  name: model
+  name: Model
   fields:
     - name: name
       type: string
       description: |
         The name of the model.
     - name: description
       type: string
@@ -386,22 +410,26 @@
     - name: state
       type: Field[]
       description: |
         A list of data items representing internal state of the modeled entity.
         State is visible within the model but is not visible to other models.
         State may be visible between multiple instances of the modeled entity to
         support horizontal scaling.
+    - name: requirements
+      type: RequirementReference
+      description: |
+        A reference to requirements relevant to the modeled item.
   validation:
     - name: Subcomponents are models
     - name: Required fields are present
       arguments:
         - name
 ---
 schema:
-  name: usecase
+  name: Usecase
   fields:
     - name: name
       type: string
       description: |
         The name of the use case.
     - name: description
       type: string
@@ -476,51 +504,204 @@
   validation:
     - name: Required fields are present
       arguments:
         - condition
         - steps
 ---
 schema:
-  name: Map
-  description: Defines a map/key-value pair data structure, and the typing.
+  name: CommandGroup
   fields:
     - name: name
       type: string
-      description: The name of the Map type
-    - name: key_type
+      description: The name of the command group.
+    - name: display
       type: string
-      description: The key type for elements in the map.
-    - name: value_type
+      description: |
+        The display name of the command group for use in user interfaces. If not
+        provided, 'name' will be used.
+    - name: helpText
       type: string
-      description: The value type for elements in the map.
+      description: |
+        The text that will be displayed as help text when displaying command
+        group usage.
   validation:
     - name: Required fields are present
       arguments:
         - name
-        - key_type
-        - value_type
+        - helpText
 ---
 schema:
-  name: KeyValuePair
-  description: Defines a key-value pair, use in list to create key-value pairs in AaC.
+  name: PluginCommand
   fields:
-    - name: key
+    - name: name
       type: string
-      description: The key map entry.
-    - name: value
+      description: The name of the command.
+    - name: display
+      type: string
+      description: |
+        The display name of the command for use in user interfaces. If not
+        provided, 'name' will be used.
+    - name: group
+      type: reference
+      description: The command group under which to place this command.
+    - name: helpText
       type: string
-      description: The value map entry.
+      description: |
+        A description that will be displayed as help text when displaying
+        command usage.
+    - name: input
+      type: Field[]
+      description: |
+        The list of all the fields that are inputs to the component when the
+        command is executed.
+    - name: output
+      type: Field[]
+      description: |
+        The list of all the fields that are outputs from the component when the
+        command is executed.
+    - name: acceptance
+      type: Scenario[]
+      description: |
+        A list of scenarios that define the acceptance criteria to signify that
+        the command is behaving as expected.
   validation:
     - name: Required fields are present
       arguments:
-        - key
-        - value
+        - name
+        - helpText
+        - acceptance
 ---
 schema:
-  name: DefinitionReference
+  name: Plugin
   fields:
     - name: name
       type: string
+    - name: description
+      type: string
+    - name: commands
+      type: PluginCommand[]
+    - name: definitionSources
+      type: file[]
+    - name: definitionValidations
+      type: ValidationReference[]
+    - name: primitiveValidations
+      type: ValidationReference[]
   validation:
-    - name: Type references exist
+    - name: Required fields are present
+      arguments:
+        - name
+        - description
+---
+command_group:
+  name: Generation
+  display: gen
+  helpText: Commands used for generating artifacts.
+---
+command_group:
+  name: Management
+  display: mgmt
+  helpText: Commands that enable management of AaC data.
+---
+command_group:
+  name: Internal
+  display: internal
+  helpText: Internal commands not intended for use by end-users or non-AaC developers.
+---
+command_group:
+  name: Backend
+  display: backend
+  helpText: Commands that enable a client/server style workflow.
+---
+command_group:
+  name: Query
+  display: show
+  helpText: Commands whose purpose is to show specific information.
+---
+schema:
+  name: Specification
+  fields:
+    - name: name
+      type: string
+    - name: description
+      type: string
+    - name: sections
+      type: SpecSection[]
+    - name: requirements
+      type: Requirement[]
+  required:
+    - name
+  validation:
+    - name: Required fields are present
+      arguments:
+        - name
+---
+schema:
+  name: SpecSection
+  fields:
+    - name: name
+      type: string
+    - name: description
+      type: string
+    - name: requirements
+      type: Requirement[]
+  required:
+    - name
+  validation:
+    - name: Required fields are present
+      arguments:
+        - name
+---
+schema:
+  name: Requirement
+  fields:
+    - name: id
+      type: string
+    - name: shall
+      type: string
+    - name: parent
+      type: RequirementReference
+    - name: child
+      type: RequirementReference
+    - name: attributes
+      type: RequirementAttribute[]
+  required:
+    - id
+    - shall
+  validation:
+    - name: Required fields are present
+      arguments:
+        - id
+        - shall
+    - name: Requirement ID is unique
+      arguments:
+        - id
+---
+schema:
+  name: RequirementAttribute
+  fields:
+    - name: name
+      type: string
+    - name: value
+      type: string
+  required:
+    - name
+    - value
+  validation:
+    - name: Required fields are present
+      arguments:
+        - name
+        - value
+---
+schema:
+  name: RequirementReference
+  fields:
+    - name: ids
+      type: string[]
+  required:
+    - ids
+  validation:
+    - name: Required fields are present
+      arguments:
+        - ids
+    - name: Referenced IDs exist
       arguments:
-        - name
+        - ids
```

## aac/validate/_validate.py

```diff
@@ -1,12 +1,13 @@
 import logging
 from contextlib import contextmanager
 from typing import Generator, Any, Optional
 
 from aac.io.parser import parse
+from aac.io.parser._parser_error import ParserError
 from aac.lang.active_context_lifecycle_manager import get_active_context
 from aac.lang.constants import (
     DEFINITION_FIELD_NAME,
     DEFINITION_FIELD_ARGUMENTS,
     DEFINITION_FIELD_FIELDS,
     DEFINITION_FIELD_TYPE,
 )
@@ -58,15 +59,20 @@
 
     Args:
         source (str): The source of the YAML representation of the model.
 
     Yields:
         A ValidationResults:py:class:`aac.validate.ValidationResult` indicating the result.
     """
-    yield _with_validation(parse(source), get_active_context())
+    try:
+        validation_result = _with_validation(parse(source), get_active_context())
+    except ParserError as error:
+        raise ParserError(error.source, error.errors) from None
+    else:
+        yield validation_result
 
 
 def _with_validation(
     user_definitions: list[Definition], language_context: LanguageContext, validate_context: bool = True
 ) -> ValidatorResult:
     try:
         result = _validate_definitions(user_definitions, language_context, validate_context)
@@ -82,14 +88,25 @@
 def _validate_definitions(
     definitions: list[Definition], language_context: LanguageContext, validate_context: bool
 ) -> ValidatorResult:
     validation_context = language_context.copy()
 
     for definition in definitions:
         existing_definition = validation_context.get_definition_by_uid(definition.uid)
+        if not existing_definition:
+            possible_match = validation_context.get_definition_by_name(definition.name)
+
+            # If the definition source, structure, and name match go ahead and assume it's the same definition.
+            if (
+                possible_match
+                and possible_match.source.uri == definition.source.uri
+                and possible_match.structure == definition.structure
+            ):
+                existing_definition = possible_match
+                definition.uid = existing_definition.uid
 
         if existing_definition:
             validation_context.update_definition_in_context(definition)
         else:
             validation_context.add_definition_to_context(definition)
 
     validator_plugins = validation_context.get_definition_validations()
@@ -151,15 +168,17 @@
 
     for validation in defined_validations:
         if validation.get(DEFINITION_FIELD_NAME) == validator_plugin.name:
             validation_args = validation.get(DEFINITION_FIELD_ARGUMENTS) or []
 
     validator_result = None
     try:
-        validator_result = validator_plugin.validation_function(definition, target_schema_definition, language_context, *validation_args)
+        validator_result = validator_plugin.validation_function(
+            definition, target_schema_definition, language_context, *validation_args
+        )
     except Exception as exception:
         exception_message = f"Validator '{validator_plugin.name}' failed with an exception: {exception}"
         finding_location = FindingLocation(validator_plugin.name, definition.source, 0, 0, 0, 0)
         exception_finding = ValidatorFinding(definition, FindingSeverity.ERROR, exception_message, finding_location)
         validator_result = ValidatorResult([definition], ValidatorFindings(findings=[exception_finding]))
 
     return validator_result
@@ -213,15 +232,15 @@
     ]
 
     validator_finding = None
 
     if validators:
         validator, *_ = validators
         try:
-            validator_finding = validator.validation_function(source_def, field_value)
+            validator_finding = validator.validation_function(source_def, field_value, language_context)
         except Exception as exception:
             exception_message = f"Validator '{validator.name}' failed with an exception: {exception}"
             finding_location = FindingLocation(validator.name, source_def.source, 0, 0, 0, 0)
             validator_finding = ValidatorFinding(source_def, FindingSeverity.ERROR, exception_message, finding_location)
     else:
         logging.info(f"No primitive type validation for '{field_type}'")
```

## Comparing `aac/plugins/first_party/specifications/globally_unique_id.py` & `aac/plugins/validators/unique_requirement_ids/_validate_unique_requirement_ids.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,85 @@
 """AaC validator implementation module for specification global req id uniqueness."""
 from typing import Tuple, Set, Dict
 
+from aac.lang.constants import ROOT_KEY_SPECIFICATION
 from aac.lang.definitions.definition import Definition
 from aac.lang.language_context import LanguageContext
 from aac.lang.definitions.structure import get_substructures_by_type
 from aac.plugins.validators import ValidatorFindings, ValidatorResult
 
 
-UNIQUE_REQ_ID_VALIDATOR_NAME = "Requirement id is unique"
+PLUGIN_NAME = "Validate requirement IDs are not duplicated"
+VALIDATION_NAME = "Requirement ID is unique"
 
 # this has to be global so that it persists across validator invocations on each definition
 ERROR_MSGS = set()
 
 
 def validate_unique_ids(
     definition_under_test: Definition,
     target_schema_definition: Definition,
     language_context: LanguageContext,
     *validation_args,
 ) -> ValidatorResult:
     """
-    Validates that the id of a Requirement is globally unique within the context.
+    Validate that the ID of a Requirement is globally unique within the context.
 
     Args:
         definition_under_test (Definition): The definition that's being validated.
         target_schema_definition (Definition): A definition with applicable validation.
         language_context (LanguageContext): The language context.
-        *validation_args: The names of the required fields.
 
     Returns:
         A ValidatorResult containing any applicable error messages.
     """
     findings = ValidatorFindings()
 
     # this test must be performed globally
     global_ids: Dict[str, Definition] = {}
-    spec_roots = language_context.get_definitions_by_root_key("spec")
+    spec_roots = language_context.get_definitions_by_root_key(ROOT_KEY_SPECIFICATION)
     for spec in spec_roots:
         unique_ids, duplicate_ids = _test_spec_ids(spec, target_schema_definition, language_context)
         if len(duplicate_ids) > 0:
             for id in duplicate_ids:
-                if spec.get_lexeme_with_value(id):  # have to do this because you sometimes get duplicate ids form imported specs
+                if spec.get_lexeme_with_value(id):
                     findings.add_error_finding(
-                        spec, f"{id} is not a unique requirement id within spec {spec.name}", UNIQUE_REQ_ID_VALIDATOR_NAME, spec.get_lexeme_with_value(id)
+                        spec,
+                        f"{id} is not a unique requirement id within spec {spec.name}",
+                        VALIDATION_NAME,
+                        spec.get_lexeme_with_value(id),
                     )
         for id in unique_ids:
             if id in global_ids:
                 # found a cross definition duplicate
                 msg = f"{id} is not a unique requirement across specs '{spec.name}' and '{global_ids[id].name}'"
                 if msg not in ERROR_MSGS:  # if we don't do this check we'll get the same findings multiple times
                     ERROR_MSGS.add(msg)
                     # issue two findings, one for each file
-                    findings.add_error_finding(spec, msg, UNIQUE_REQ_ID_VALIDATOR_NAME, spec.get_lexeme_with_value(id))
-                    findings.add_error_finding(global_ids[id], msg, UNIQUE_REQ_ID_VALIDATOR_NAME, global_ids[id].get_lexeme_with_value(id))
+                    findings.add_error_finding(spec, msg, VALIDATION_NAME, spec.get_lexeme_with_value(id))
+                    findings.add_error_finding(global_ids[id], msg, VALIDATION_NAME, global_ids[id].get_lexeme_with_value(id))
             else:
                 global_ids[id] = spec
 
     return ValidatorResult([definition_under_test], findings)
 
 
-def _test_spec_ids(spec_definition: Definition, requirement_definition: Definition, language_context: LanguageContext) -> Tuple[Set, Set]:
+def _test_spec_ids(
+    spec_definition: Definition, requirement_definition: Definition, language_context: LanguageContext
+) -> Tuple[Set, Set]:
     """
-    Searches a given spec definition for duplicate ids.
+    Search a given spec definition for duplicate IDs.
 
     Args:
         spec_definition (Definition): The definition that's being validated.
-        requirements_definition (Definition): A definition for the Requirement type.
+        requirement_definition (Definition): A definition for the Requirement type.
         language_context (LanguageContext): The language context.
 
     Returns:
-        A set of discovered local requirement ids and a set of duplicate ids within the definition.
+        A set of discovered local requirement IDs and a set of duplicate IDs within the definition.
     """
     local_ids = set()
     duplicate_ids = set()
 
     for req_dict in get_substructures_by_type(spec_definition, requirement_definition, language_context):
         id = req_dict["id"]
         if id in local_ids:
```

## Comparing `aac/plugins/first_party/specifications/referenced_ids_exist.py` & `aac/plugins/validators/requirement_references/_validate_requirement_references.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""AaC validator implementation module for specification req reference ids."""
 from typing import Set, Dict
 
 from aac.lang.definitions.definition import Definition
 from aac.lang.language_context import LanguageContext
 from aac.lang.definitions.structure import get_substructures_by_type
 from aac.plugins.validators import ValidatorFindings, ValidatorResult
 
 
-SPEC_REF_ID_VALIDATOR_NAME = "Referenced IDs exist"
+PLUGIN_NAME = "Validate referenced IDs"
+VALIDATION_NAME = "Referenced IDs exist"
 
 ALL_REQ_IDS: Set[str] = set()
 
 SPEC_REF_ERRORS: Dict[str, str] = {}
 
 
 def validate_referenced_ids(
@@ -42,15 +42,15 @@
                 if id not in ALL_REQ_IDS:
                     err_msg = f"Referenced requirement '{id}' is not defined"
                     if err_msg in SPEC_REF_ERRORS.keys() and SPEC_REF_ERRORS[err_msg] == definition_under_test.source.uri:
                         pass  # this just prevents duplicate errors for the user
                     else:
                         SPEC_REF_ERRORS[err_msg] = definition_under_test.source.uri
                         findings.add_error_finding(
-                            definition_under_test, err_msg, SPEC_REF_ID_VALIDATOR_NAME, definition_under_test.get_lexeme_with_value(id)
+                            definition_under_test, err_msg, VALIDATION_NAME, definition_under_test.get_lexeme_with_value(id)
                         )
 
     return ValidatorResult([definition_under_test], findings)
 
 
 def _get_all_requirement_ids(target_schema_definition, language_context):
     if len(ALL_REQ_IDS) == 0:  # don't repeat this for every validator invocation
```

## Comparing `aac/plugins/validators/exclusive_fields/_exclusive_fields.py` & `aac/plugins/validators/exclusive_fields/_validate_exclusive_fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from aac.lang.definitions.definition import Definition
 from aac.lang.definitions.structure import get_substructures_by_type
 from aac.lang.language_context import LanguageContext
 from aac.plugins.validators import ValidatorFindings, ValidatorResult
 
 
-PLUGIN_NAME = "Mutually exclusive fields"
+PLUGIN_NAME = "Validate mutually exlusive fields"
+VALIDATION_NAME = "Mutually exclusive fields"
 
 
 def validate_exclusive_fields(
     definition_under_test: Definition,
     target_schema_definition: Definition,
     language_context: LanguageContext,
     *validation_args,
```

## Comparing `aac/plugins/validators/subcomponent_type/_subcomponent_type.py` & `aac/plugins/validators/subcomponent_type/_validate_subcomponent_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from aac.lang.definitions.definition import Definition
 from aac.lang.definitions.structure import get_substructures_by_type
 from aac.lang.language_context import LanguageContext
 from aac.plugins.validators import ValidatorFindings, ValidatorResult
 
 
-PLUGIN_NAME = "Subcomponents are models"
+PLUGIN_NAME = "Validate model subcomponents"
+VALIDATION_NAME = "Subcomponents are models"
 
 
 def validate_subcomponent_types(
     definition_under_test: Definition,
     target_schema_definition: Definition,
     language_context: LanguageContext,
     *validation_args,
```

## Comparing `aac/plugins/validators/unique_names/_unique_names.py` & `aac/plugins/validators/unique_names/_validate_unique_names.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 from os import linesep
-from aac.lang.constants import DEFINITION_FIELD_NAME
 
+from aac.lang.constants import DEFINITION_FIELD_NAME
 from aac.lang.definitions.definition import Definition
 from aac.lang.language_context import LanguageContext
 from aac.plugins.validators._validator_result import ValidatorFindings, ValidatorResult
 
 
-PLUGIN_NAME = "Unique definition names"
+PLUGIN_NAME = "Validate names are not duplicated"
+VALIDATION_NAME = "Unique definition names"
 
 
 def validate_unique_names(
     definition_under_test: Definition,
     target_schema_definition: Definition,
     language_context: LanguageContext,
     *validation_args,
```

## Comparing `aac/plugins/validators/validator_implementation/_validator_implementation.py` & `aac/plugins/validators/validator_implementation/_validate_validator_implementation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging
 
+from aac.lang.constants import DEFINITION_FIELD_NAME
 from aac.lang.definitions.definition import Definition
 from aac.lang.definitions.structure import get_substructures_by_type
 from aac.lang.language_context import LanguageContext
 from aac.plugins.validators import ValidatorFindings, ValidatorResult
 
 
-PLUGIN_NAME = "Validation definition has an implementation"
+PLUGIN_NAME = "Validate implementations for validators"
+VALIDATION_NAME = "Validation definition has an implementation"
 
 
 def validate_validator_implementations(
     definition_under_test: Definition,
     target_schema_definition: Definition,
     language_context: LanguageContext,
     *validation_args,
@@ -25,28 +27,25 @@
 
     Returns:
         A ValidatorResult containing any applicable error messages.
     """
     findings = ValidatorFindings()
 
     def validate_dict(dict_to_validate: dict) -> None:
-        validator_implementations = language_context.get_definition_validations()
-        validation_name = dict_to_validate.get("name")
-        validation_plugins = [plugin for plugin in validator_implementations if plugin.name == validation_name]
-
-        if not validation_plugins:
-            registered_plugin_names = [plugin.name for plugin in validator_implementations]
-            registered_plugin_names = f"Validation '{validation_name}' did not have a corresponding implementation. Registered plugin names: {registered_plugin_names}"
-            validation_name_lexeme = definition_under_test.get_lexeme_with_value(validation_name)
-            findings.add_error_finding(target_schema_definition, registered_plugin_names, PLUGIN_NAME, validation_name_lexeme)
-            logging.debug(registered_plugin_names)
-        elif validation_plugins and not len(validation_plugins) == 1:
-            registered_plugin_names = [plugin.name for plugin in validator_implementations]
-            registered_plugin_names = f"Validation '{validation_name}' returned multiple corresponding implementations. Matching plugins: {validation_plugins}"
+        validation_name = dict_to_validate.get(DEFINITION_FIELD_NAME, "")
+        active_validations = {
+            validation.name: validation
+            for validation in language_context.get_primitive_validations() + language_context.get_definition_validations()
+        }
+
+        if validation_name in active_validations and active_validations.get(validation_name).validation_function is None:
+            no_implementation_error_message = f"Validation '{validation_name}' did not have a corresponding implementation."
             validation_name_lexeme = definition_under_test.get_lexeme_with_value(validation_name)
-            findings.add_error_finding(target_schema_definition, registered_plugin_names, PLUGIN_NAME, validation_name_lexeme)
-            logging.debug(registered_plugin_names)
+            findings.add_error_finding(
+                target_schema_definition, no_implementation_error_message, PLUGIN_NAME, validation_name_lexeme
+            )
+            logging.debug(no_implementation_error_message)
 
     dicts_to_test = get_substructures_by_type(definition_under_test, target_schema_definition, language_context)
     list(map(validate_dict, dicts_to_test))
 
     return ValidatorResult([definition_under_test], findings)
```

## Comparing `aac-0.1.9.dist-info/METADATA` & `aac-0.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,97 +1,98 @@
 Metadata-Version: 2.1
 Name: aac
-Version: 0.1.9
+Version: 0.2.0
 Summary: A distinctly different take on Model-Based System Engineering (MBSE) that allows a system modeller to define a system in simple yaml. 
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: MBSE
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
-Requires-Dist: attrs (>=22.1)
-Requires-Dist: pyrsistent (>=0.19)
-Requires-Dist: PyYAML (>=6.0)
-Requires-Dist: six (>=1.16)
-Requires-Dist: click (>=8.1)
-Requires-Dist: pathspec (>=0.10)
-Requires-Dist: regex (>=2022.10.31)
-Requires-Dist: typing-extensions (>=4.4)
-Requires-Dist: pluggy (>=1.0)
-Requires-Dist: Jinja2 (>=3.1)
-Requires-Dist: MarkupSafe (>=2.1)
-Requires-Dist: pygls (==0.13.1)
-Requires-Dist: fastapi (>=0.86)
-Requires-Dist: starlette (>=0.20.4)
-Requires-Dist: anyio (<5,>=3.6.0)
-Requires-Dist: sniffio (>=1.3)
-Requires-Dist: uvicorn (>=0.19.0)
-Requires-Dist: requests (>=2.28.0)
+Requires-Dist: attrs (~=22.2.0)
+Requires-Dist: pyrsistent (~=0.19.3)
+Requires-Dist: PyYAML (~=6.0.0)
+Requires-Dist: types-PyYAML (~=6.0.12.2)
+Requires-Dist: six (~=1.16.0)
+Requires-Dist: click (~=8.1.3)
+Requires-Dist: pathspec (~=0.10.3)
+Requires-Dist: regex (~=2022.10.31)
+Requires-Dist: typing-extensions (~=4.4.0)
+Requires-Dist: pluggy (~=1.0.0)
+Requires-Dist: Jinja2 (~=3.1.2)
+Requires-Dist: MarkupSafe (~=2.1.1)
+Requires-Dist: pygls (~=0.13.1)
+Requires-Dist: fastapi (~=0.89.0)
+Requires-Dist: starlette (>=0.22.0)
+Requires-Dist: anyio (<5,~=3.6.2)
+Requires-Dist: sniffio (~=1.3.0)
+Requires-Dist: uvicorn (~=0.20.0)
+Requires-Dist: requests (>=2.28.1)
 Provides-Extra: all
 Requires-Dist: tox (>=3.24) ; extra == 'all'
 Requires-Dist: nose2 (>=0.10.0) ; extra == 'all'
 Requires-Dist: coverage (>=6.0) ; extra == 'all'
 Requires-Dist: flake8 (>=4.0) ; extra == 'all'
 Requires-Dist: flake8-docstrings (>=1.6.0) ; extra == 'all'
 Requires-Dist: flake8-fixme (>=1.1.1) ; extra == 'all'
 Requires-Dist: flake8-eradicate (>=1.2.0) ; extra == 'all'
 Requires-Dist: flake8-assertive (>=1.3.0) ; extra == 'all'
 Requires-Dist: eradicate (<3.0,>=2.0) ; extra == 'all'
 Requires-Dist: httpx (>=0.23.0) ; extra == 'all'
-Requires-Dist: wheel (==0.37.0) ; extra == 'all'
+Requires-Dist: wheel (~=0.40.0) ; extra == 'all'
 Requires-Dist: pip-tools (>=6.9.0) ; extra == 'all'
 Requires-Dist: tomli (<2.0.0) ; extra == 'all'
 Requires-Dist: black (==22.3.0) ; extra == 'all'
 Requires-Dist: platformdirs (>=2.4) ; extra == 'all'
 Requires-Dist: mccabe (==0.6.1) ; extra == 'all'
-Requires-Dist: mypy-extensions (==0.4.3) ; extra == 'all'
+Requires-Dist: mypy (~=1.1.0) ; extra == 'all'
+Requires-Dist: mypy-extensions (~=1.0.0) ; extra == 'all'
 Requires-Dist: pycodestyle (>=2.8.0) ; extra == 'all'
 Requires-Dist: pyflakes (>=2.4) ; extra == 'all'
 Requires-Dist: build (==0.7.0) ; extra == 'all'
 Requires-Dist: twine (==3.4.2) ; extra == 'all'
 Requires-Dist: Sphinx (==4.2.0) ; extra == 'all'
 Requires-Dist: sphinxcontrib-applehelp (==1.0.2) ; extra == 'all'
 Requires-Dist: sphinxcontrib-devhelp (==1.0.2) ; extra == 'all'
 Requires-Dist: sphinxcontrib-htmlhelp (==2.0.0) ; extra == 'all'
 Requires-Dist: sphinxcontrib-jsmath (==1.0.1) ; extra == 'all'
 Requires-Dist: sphinxcontrib-qthelp (==1.0.3) ; extra == 'all'
 Requires-Dist: sphinxcontrib-serializinghtml (==1.1.5) ; extra == 'all'
 Requires-Dist: furo (==2021.10.9) ; extra == 'all'
 Requires-Dist: pipdeptree (>=2.2.0) ; extra == 'all'
 Requires-Dist: Pygments (>=2.5.1) ; extra == 'all'
-Requires-Dist: mypy (>=0.961) ; extra == 'all'
 Requires-Dist: types-PyYAML (>=6.0.9) ; extra == 'all'
 Requires-Dist: requests (>=2.27.0) ; extra == 'all'
 Provides-Extra: dev
-Requires-Dist: wheel (==0.37.0) ; extra == 'dev'
+Requires-Dist: wheel (~=0.40.0) ; extra == 'dev'
 Requires-Dist: pip-tools (>=6.9.0) ; extra == 'dev'
 Requires-Dist: tomli (<2.0.0) ; extra == 'dev'
 Requires-Dist: black (==22.3.0) ; extra == 'dev'
 Requires-Dist: platformdirs (>=2.4) ; extra == 'dev'
 Requires-Dist: coverage (>=6.0) ; extra == 'dev'
 Requires-Dist: mccabe (==0.6.1) ; extra == 'dev'
-Requires-Dist: mypy-extensions (==0.4.3) ; extra == 'dev'
+Requires-Dist: mypy (~=1.1.0) ; extra == 'dev'
+Requires-Dist: mypy-extensions (~=1.0.0) ; extra == 'dev'
 Requires-Dist: pycodestyle (>=2.8.0) ; extra == 'dev'
 Requires-Dist: pyflakes (>=2.4) ; extra == 'dev'
 Requires-Dist: build (==0.7.0) ; extra == 'dev'
 Requires-Dist: twine (==3.4.2) ; extra == 'dev'
 Requires-Dist: Sphinx (==4.2.0) ; extra == 'dev'
 Requires-Dist: sphinxcontrib-applehelp (==1.0.2) ; extra == 'dev'
 Requires-Dist: sphinxcontrib-devhelp (==1.0.2) ; extra == 'dev'
 Requires-Dist: sphinxcontrib-htmlhelp (==2.0.0) ; extra == 'dev'
 Requires-Dist: sphinxcontrib-jsmath (==1.0.1) ; extra == 'dev'
 Requires-Dist: sphinxcontrib-qthelp (==1.0.3) ; extra == 'dev'
 Requires-Dist: sphinxcontrib-serializinghtml (==1.1.5) ; extra == 'dev'
 Requires-Dist: furo (==2021.10.9) ; extra == 'dev'
 Requires-Dist: pipdeptree (>=2.2.0) ; extra == 'dev'
 Requires-Dist: Pygments (>=2.5.1) ; extra == 'dev'
-Requires-Dist: mypy (>=0.961) ; extra == 'dev'
 Requires-Dist: types-PyYAML (>=6.0.9) ; extra == 'dev'
 Requires-Dist: requests (>=2.27.0) ; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: tox (>=3.24) ; extra == 'test'
 Requires-Dist: nose2 (>=0.10.0) ; extra == 'test'
 Requires-Dist: coverage (>=6.0) ; extra == 'test'
 Requires-Dist: flake8 (>=4.0) ; extra == 'test'
@@ -209,51 +210,53 @@
 - ext: Allows you to easily extend the AaC DSL itself and tailor it to your needs.
 
 Although you can use the yaml trick above when modelling your system, it would be better to keep things more
 structured and organized.  To help with this AaC allows you to define each item you model in a separate file and
 then import it as needed.  To do this just put an **import** at the root of your model file.
 
 Here's an example of the EchoService broken into two files:
-- Message.yaml
-    ```yaml
-    schema:
-    name: Message
-    fields:
+*Message.yaml*
+```yaml
+schema:
+  name: Message
+  fields:
     - name: body
-        type: string
+      type: string
     - name: sender
-        type: string
-    ```
-- EchoService.yaml
-    ```yaml
-    import:
+      type: string
+```
+*EchoService.yaml*
+```yaml
+import:
+  files:
     - ./Message.yaml
-    model:
-    name: EchoService
-    description: This is a message mirror.
-    behavior:
-        - name: echo
-        type: request-response
-        description: This is the one thing it does.
-        input:
-            - name: inbound
-            type: Message
-        output:
-            - name: outbound
-            type: Message
-        acceptance:
-            - scenario: onReceive
-            given:
-            - The EchoService is running.
-            when:
-                - The user sends a message to EchoService.
-            then:
-                - The user receives the same message from EchoService.
+---
+model:
+  name: EchoService
+  description: This is a message mirror.
+  behavior:
+    - name: echo
+      type: request-response
+      description: This is the one thing it does.
+      input:
+        - name: inbound
+          type: Message
+      output:
+        - name: outbound
+          type: Message
+      acceptance:
+        - scenario: onReceive
+          given:
+          - The EchoService is running.
+          when:
+          - The user sends a message to EchoService.
+          then:
+          - The user receives the same message from EchoService.
+```
 
-    ```
 Ok, so that's interesting, but what can you do with the AaC model once you've built it?
 AaC is designed and built on years of experimentation, experience, and learning.  But this version
 is a brand new implementation rewritten entirely in Python in an attempt to make AaC more user friendly
 to both the casual user and the power user. Right now AaC doesn't have a lot of additional features.
 But new plugins are being created to deliver more functionality.  Over time there will be plugins
 available to use the AaC model to auto-generate content for reviews, documentation, and even system
 development and deployment.
@@ -293,7 +296,8 @@
     - Run '''aac plugin-behavior-name model_file''' to see your plugin in action.
 1) If you wish you can now package and publish your plugin to PyPI for other AaC users to download and use.
     - From your plugin directory run '''python -m build'''
     - From your plugin directory run '''python -m twine upload dist/*'''
 
 We're also actively working on other functionality so keep an eye out for new updates.
 
+
```

## Comparing `aac-0.1.9.dist-info/RECORD` & `aac-0.2.0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,202 +1,217 @@
-aac/__init__.py,sha256=UzUak1OjlXXnrbIspNYGb9NO4yzllWumrQLIj6TvIFs,695
-aac/__main__.py,sha256=SLqUkmPrf-B24xN6h62f-3P6YnKDrf4X26xOzSdOOIo,177
+aac/__init__.py,sha256=iJGGBGGHB4Wr5CZNVVJXSxF5tKXkZLJu-v2mCAb7ZFw,681
+aac/__main__.py,sha256=1FbYh29S3YnkKu0B34sZJqB7taUtJ2dP5VuPeYMgk5g,175
 aac/package_resources.py,sha256=jorW4ZtikiybXyGYV1-w73K6nM3ou0DntHp5cj6URpU,972
 aac/cli/__init__.py,sha256=doEp70zA135B6FRhavoHmNjAwRu-dllKCMNR86rnUqI,57
 aac/cli/aac_command.py,sha256=ijsb7TImUJlrV6oLRJ_wPn8aFI_yPrTkeaNXGpudhGU,2096
-aac/cli/execute.py,sha256=O3p05p-SMBPjqX5uDeqfnomtvAye-7wrDenSvOLc5uY,2584
+aac/cli/execute.py,sha256=ogmLDYDBxqCCV2a9LBRUrVgAPsIDitljPdRexlFXDCw,2743
 aac/cli/builtin_commands/__init__.py,sha256=NI-h2FJ2v795YF06doIg6oFLhJnfTu8zPIoREF_wa3Q,54
 aac/cli/builtin_commands/validate/__init__.py,sha256=BJ2C8ImK-U3WVIZ8DC1J-zXL9ZplijAoJTGZhC3-QMs,1207
-aac/cli/builtin_commands/validate/validate.yaml,sha256=yFRe97bdG-VdAEAJgqQAJTVPX_GBoygfF-ovyS1dPlc,1476
-aac/cli/builtin_commands/validate/validate_impl.py,sha256=Lb0q-doNx2aQ320x29JPWESOOLciToMq9tYuM850u_8,2710
+aac/cli/builtin_commands/validate/validate.yaml,sha256=fAUz6LYC-6Aosek4dk-qVTjf4B2cTwnn7WWiHVoAaBQ,1470
+aac/cli/builtin_commands/validate/validate_impl.py,sha256=B2yZFlFoFErvjrcN57TO4MtBfPd-e2f_5c_7-e4JCYI,3110
 aac/cli/builtin_commands/version/__init__.py,sha256=wcaYAiCQ__Dsfw1G0rfPpoEO89pQcT38WW48FvpW4Hk,795
-aac/cli/builtin_commands/version/version.yaml,sha256=FE6qMm8hEnu25N1ocH_GqZW5fHCtZFgemwPiUHjc7OU,431
-aac/cli/builtin_commands/version/version_impl.py,sha256=Xt3wFU-atninB-pbV8AvyIvJUS937Hd5aARCaB33WDw,428
+aac/cli/builtin_commands/version/version.yaml,sha256=-tUCW26h_tkgEqM3yRobzYKtTEEjSOXbtxcnucZVpZY,435
+aac/cli/builtin_commands/version/version_impl.py,sha256=W7RlpGxl3TLh_p3VxvBeIX6PtAr0ouwA1LJDoHXj8u4,428
 aac/io/__init__.py,sha256=ILCEL2vx9GQXwSkVxomrSuVopHmMSLCzGcZqlQ9fyHg,66
 aac/io/constants.py,sha256=U1AEnVw3cfZFHs3MKloLJtaC0BssIa8afN8j70-Vw0g,253
 aac/io/paths.py,sha256=M-82oL8jeqSMRbZ0TeyWoAY4NojCuHn-FOpO0jc02O0,2507
 aac/io/writer.py,sha256=MV47rdgUFcBplsJbD9Kqtfki5sxcJiAeyXDeTbYN50k,2275
 aac/io/files/__init__.py,sha256=kOJIWgpdjujZd9lkx3Us1w0_4Fq30zCS2Y9uiGi5rGk,63
-aac/io/files/aac_file.py,sha256=Oc01aM2t2AumfYa6Jr9XFHlPCvndvayV179H6SPOPds,913
-aac/io/files/find.py,sha256=DiBYqVHjcP4XnR4R_a6sUTZfbiftNH2fXa-mj6jMtog,1626
-aac/io/parser/__init__.py,sha256=h1_h05zfqhraMdUcEGeZkYBqzLIXWAiqd-EsQCPk7xo,210
-aac/io/parser/_parse_source.py,sha256=t0NyfHHQHHJOfKkmJmHTF3as9g0RM-Crq_r6G4uZj5c,10005
-aac/io/parser/_parser_error.py,sha256=drZZP1S7xopeHg_gnOURTFn8v7lU-_5fmppha2tgtds,416
+aac/io/files/aac_file.py,sha256=3CbUbkS-zbJQVKLdikawYXbdVCJMPtt4r6i0V1_0euA,925
+aac/io/files/find.py,sha256=uy45_vUzUNEzP5Bc3jinRspwOBZh4sVbpQ34gi2wC0E,1628
+aac/io/parser/__init__.py,sha256=4UTu1lA9HqWIG9_nd4cwo5M6ffe8phyKYU3y2v9UzsM,427
+aac/io/parser/_cache.py,sha256=JHiOvXxG-60ujn3Ff-kzos0B0lOi--4lS4IDK1L0cks,4849
+aac/io/parser/_cache_manager.py,sha256=7S4cyEMVSPp2Yce-E003t3Vpks8mdrwX9uhDESXDpug,534
+aac/io/parser/_parse_source.py,sha256=uBpI4mDSzhXB02KAZsop2eMwC3-fwFKkhdqLINGWkN4,7610
+aac/io/parser/_parser_error.py,sha256=Y-NVlfI4_CfqYktvUXZIRFdm5Ar7Nd7iQBNCQ-AYPyQ,415
+aac/io/parser/_yaml.py,sha256=iSUKlymSDITHJxeyUZicUiQ-toYqBr-PrRLT1bU25H4,4629
 aac/lang/__init__.py,sha256=IWgyG5kI7CavzTM0gP6LTKNN-EFxRc5jc88b5XJMCF8,52
-aac/lang/active_context_lifecycle_manager.py,sha256=Rt4LGMbsZIgYiwq8rZUJTxRfKvHwC9OuWlFPi28hD98,1628
-aac/lang/constants.py,sha256=55HpptJ1FEjhwFOC6mgI5sCLyjH16aICL0zbGo5IrMc,1415
-aac/lang/hierarchy.py,sha256=AUHMctLg4dJvCIlg4cy5uZpQTwV7cCIm4Qcx-bNYzFU,3000
-aac/lang/language_context.py,sha256=cxZc0u7xXmHSlGfXgI6zVh6RTsxSUKawhcev9HXCBHY,29109
+aac/lang/active_context_lifecycle_manager.py,sha256=VscSVW2bFK3_Pc5K9Gop5UTR-TgvQwKZNNWexmjTMXI,1603
+aac/lang/constants.py,sha256=ZqlyJY10kpoc_4ZdlSGEBsq1p46H_8mgFTa9eZzRM4I,3210
+aac/lang/hierarchy.py,sha256=NxS8kBN6F1-_TL3XBaoBU3tjcWq_usIXlUvQtCmsI2s,4139
+aac/lang/language_context.py,sha256=cVDOka1ywLFU5UVzqSYaxjVTID18VGDYJeIAqyTqiCw,30160
 aac/lang/language_error.py,sha256=fxUkAd4wNfl2sGegf8dHmonviieYR12RwDakgu56X7Q,230
 aac/lang/definitions/__init__.py,sha256=LwpFYMWB-ueS1WVe7MImJ2s0QMqVerFocpXvphQ1c38,85
 aac/lang/definitions/collections.py,sha256=tqhQOvD2SNtlSJ2E_tA_oK39GuHUFG3d8-b4UK2JPPg,3777
-aac/lang/definitions/definition.py,sha256=T7mBC5yWx77U4SX6tlZAJ8ce2xL-hfxr1cFxK0zZXDQ,7729
-aac/lang/definitions/extensions.py,sha256=sbJ-WqhrdvS_EEYG6CeWYMq_sxa2i1eUg1nuZ045A1E,9139
+aac/lang/definitions/definition.py,sha256=DY691_lquOKxiDnS-39k-49UfNhKGzWjFCnaKKa-PaY,9179
+aac/lang/definitions/extensions.py,sha256=xXLk435AMI7YCBZcFccIn35jDxs2QSDPjmLevNTjhac,11643
 aac/lang/definitions/inheritance.py,sha256=MgtDRpYmOpg1VohXDZIUM72u7uaJZ7DeiS1VYi5OpMU,3136
 aac/lang/definitions/json_schema.py,sha256=1jStAh9Qj9faapM73wQ5FL2Lh3ISzkOb4eHIYt8fWYI,7104
 aac/lang/definitions/lexeme.py,sha256=xwYO3ASJcjyKvI9AkB18r7YVO-U2Jvv1BMYvRuY9ZpA,1025
-aac/lang/definitions/references.py,sha256=PX7tDi-9Odxh8Y1Nmvmrj_v_Zzq94snSzUgXLrrc0p8,10713
-aac/lang/definitions/schema.py,sha256=7bFElYkoUlanjTlWWGjE3OIL1pz94Oda4s9HY4ZKECE,4479
+aac/lang/definitions/metadata_structure.py,sha256=8nuYEGOt3ZgklGyS3zvUVi9XnbTvAoJXIqE8YIdsFe4,3921
+aac/lang/definitions/references.py,sha256=YZJK2TWIU-NfQNWjTUaYVa0hyq21DPi2LcilGfNn63Q,9943
+aac/lang/definitions/schema.py,sha256=UQSjNKfSeMH_iH73W48MdWY9eqpBImzQM0ps2ali9uY,7827
 aac/lang/definitions/search.py,sha256=ciJgI3BrVcVQ012FLGCeJkrMimPKP7N0aj5X_6tqyFM,5149
 aac/lang/definitions/source_location.py,sha256=fZj9jj9rp7iFj7J5B_6CMCYlvReyxL1bpOuWNJsYMtQ,1193
+aac/lang/definitions/structural_node.py,sha256=pQ77khyM8X3Pqv1pdt2AykrZ5ydJzgyVL2IWtjrGgVs,3495
 aac/lang/definitions/structure.py,sha256=jo4oo4asmu4c6tP0ISho00RMJ2b20lEsUBCRZfgHWS4,5891
 aac/lang/definitions/type.py,sha256=42c7Xc7P_uOgQnDviYJlgfvtMhsOevoie8Z7us7fmXc,401
 aac/persistence/__init__.py,sha256=Hni7xJ9Y4obdQLT5SziHyiC_WHQoSyYVPAw8Ei6_3Jc,198
 aac/persistence/state_file_error.py,sha256=kNfN8D61w3IBMZA07i2Ra3UAxzeZAI3AauxacGIE_uo,154
 aac/plugins/__init__.py,sha256=B8m8wu0L5t8GzT9yBQlV0tsK08-aTK6rqCZfqPM9vWY,695
-aac/plugins/_common.py,sha256=mk9hrrWHPsnsNiqOOzm3yWDmYI-J4gW6SRtbQs6aXMk,511
+aac/plugins/_common.py,sha256=p2xsTrehRM4RCF2HB3ZZnryN5b8P9cDTotoMLPtUBr8,704
 aac/plugins/hookspecs.py,sha256=UZdxAzrr1If3-_q_CxUn_vq9jYv7YhePIAn2QYvc3-s,323
-aac/plugins/plugin.py,sha256=mcy0SI3_muSHGbywFGGzhRNUg-9lD1IAhFYMahKmne8,4437
+aac/plugins/plugin.py,sha256=P4Ky4lgAt5Zru7utAqi_SwKTYBIo9Ap2qmbwjckVHjQ,4627
 aac/plugins/plugin_execution.py,sha256=Gg0YtimVT8mN4f6r7xgP22BTibL4Y92tSNV3Ug_8YqY,5296
-aac/plugins/plugin_manager.py,sha256=QeUWBZGp-kjJzSezSyRavSeX_55XJLJjGTDnHsl5pcE,2459
+aac/plugins/plugin_manager.py,sha256=4-FBDS6Fn6NfCZSP2AH2HDW2DfdT3OuXta_1w4BPFJY,2864
 aac/plugins/contributions/__init__.py,sha256=FtBuI_lqCh1NLbUdAjqNiYHaoTwGgkYCAZ9HcNlas1E,68
 aac/plugins/contributions/contribution_points.py,sha256=xDquexyxwW3iOqhv0BryBu1Wlgu_GbFifOwxXjveDDg,9885
 aac/plugins/contributions/plugin_contribution.py,sha256=5u5qBqoncibSwsPMJEfTOw7qUOuTSOuV6fB5k-PaVTs,1150
 aac/plugins/contributions/contribution_types/__init__.py,sha256=gqzjSVppqCn5FuF653u1xBRHeFm4lXxwQ5iCEmbp714,524
 aac/plugins/contributions/contribution_types/contribution_type.py,sha256=YRcvlC2BNcHL8SayVOVGOgZ1jmRMHswv3AGDTyhF72Q,353
-aac/plugins/contributions/contribution_types/definition_validation_contribution.py,sha256=soVF6LVD9UURscdyvBUarpIWrfpB-L-uIIFoIivazqo,957
-aac/plugins/contributions/contribution_types/primitive_validation_contribution.py,sha256=aPK89QyI0GEMhSNR6NcXQAdYeTq9wXK5PVvj3KSCcvA,859
+aac/plugins/contributions/contribution_types/definition_validation_contribution.py,sha256=GGsqpGfJBfrGOotOxksZ1uhymeRH8V3CL1KEpCSAQTc,1118
+aac/plugins/contributions/contribution_types/primitive_validation_contribution.py,sha256=-bNJTkoOLfyOAIXlg_Bi6rJqcRHWM5KJHncjmlVGrCM,1022
 aac/plugins/first_party/__init__.py,sha256=OLaKTA4dS84z8Dg_rnR9a-R576kmWSqLRJufJrPbvp4,69
+aac/plugins/first_party/active_context/__init__.py,sha256=ksCkoZ26bJ6s56ubpk2fYe8TCPCIwwzV3x-DEoJ25TU,2514
+aac/plugins/first_party/active_context/active_context.yaml,sha256=yhlYYbiaICXvRov-95pwoCjqzGZzL7sfJHbEru1AKT0,6501
+aac/plugins/first_party/active_context/active_context_impl.py,sha256=0xeNCeN5tAeDJClvG3Q96cmNLTdnmeVOOk6Cxs4IBOQ,3947
 aac/plugins/first_party/gen_design_doc/__init__.py,sha256=pnDINlzhrUDGAgYzoHadG2AyCXGko4J3PA1cogR4pZI,1520
-aac/plugins/first_party/gen_design_doc/gen_design_doc.yaml,sha256=Qa8kALzF-p0-JOKv6Ra8vNffkUHhsJaM1ftGioIyrow,1312
-aac/plugins/first_party/gen_design_doc/gen_design_doc_impl.py,sha256=jn1UQh8qz_dVDqI8AjFkUT26Lk0-iMk8TFER4M2-_4o,4290
+aac/plugins/first_party/gen_design_doc/gen_design_doc.yaml,sha256=dR864B6L6Fowd30KtapCe8FaUX9R01LFOsVKSd9yVFs,1284
+aac/plugins/first_party/gen_design_doc/gen_design_doc_impl.py,sha256=iYB7YlBIJn_spZxWcHPGzeok8ouicN0bH7m4nEme_iY,4429
 aac/plugins/first_party/gen_design_doc/templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aac/plugins/first_party/gen_design_doc/templates/datum.md.jinja2,sha256=RTNJudVSOuaydiWj_AqcxAiKMtKXDUkJZTMYA5LDF5g,257
-aac/plugins/first_party/gen_design_doc/templates/macros.jinja2,sha256=GI-RFzMLLbV0Kq6FHI0xtpcEEhA-uNHzPjWomoDnPQQ,262
-aac/plugins/first_party/gen_design_doc/templates/model.md.jinja2,sha256=TxeieOkZqzZiLPH41Q51h0MXOW05NKcFfjWP0f_qKPc,995
-aac/plugins/first_party/gen_design_doc/templates/system-design-doc.md.jinja2,sha256=tKPoirGTK_Rmc-0IbuVu5x1YhFLIwNrX1sT9NlQyozU,340
-aac/plugins/first_party/gen_design_doc/templates/usecase.md.jinja2,sha256=AD7Z6z8hrE_x-uHjzYCQawfaK-OFXI7OSp2p2xSE8u4,434
-aac/plugins/first_party/gen_gherkin_behaviors/__init__.py,sha256=nnx2McyEGOOjXi07VPyAKzluihB8WkxN8FFwqckFNvc,1769
+aac/plugins/first_party/gen_design_doc/templates/datum.md.jinja2,sha256=cPHiWBPaOeyMQaAHbKYOjeZdStnNn5b1jW8QpaIHceQ,254
+aac/plugins/first_party/gen_design_doc/templates/macros.jinja2,sha256=dOA9tpjJeQBH-3OPSvcl56r0J3o1FxUhmjOrl0r-dEg,260
+aac/plugins/first_party/gen_design_doc/templates/model.md.jinja2,sha256=Mh-UfTBkr9Lh3kXjBHoQzy9meIGWOPcJm3ZkY-tuu7A,988
+aac/plugins/first_party/gen_design_doc/templates/system-design-doc.md.jinja2,sha256=97UgO_3SqHI1IXt_4wqLkz7qntPaKuCFF2sbfmUhdAg,334
+aac/plugins/first_party/gen_design_doc/templates/usecase.md.jinja2,sha256=98ldTdWKGfqzV8NqTmCeZKfKFw4RgCQurUbkH5dYQYg,430
+aac/plugins/first_party/gen_gherkin_behaviors/__init__.py,sha256=BWAIctH-AvGa2bskExoPF0eiXH4s0IVXrFk27kJXNfc,1760
 aac/plugins/first_party/gen_gherkin_behaviors/behavior.feature.jinja2,sha256=mxN9P_kvMXlSYKlGYX7_RKamTuc30Q2uwF4yj80BTaU,639
-aac/plugins/first_party/gen_gherkin_behaviors/gen_gherkin_behaviors.yaml,sha256=KFLGptkyilm6rJOmkGXBXqGAnA-JSAbPnQWWNWuiszA,1181
-aac/plugins/first_party/gen_gherkin_behaviors/gen_gherkin_behaviors_impl.py,sha256=BI51Vn6juQUzHj-hAhpGf1soUnHJI7yYRAtdWbBoGOg,6986
+aac/plugins/first_party/gen_gherkin_behaviors/gen_gherkin_behaviors.yaml,sha256=eMsC2NkdNJMDqCcwc6oaaO_ceyu-CJCtxW3BR9mDxWg,1156
+aac/plugins/first_party/gen_gherkin_behaviors/gen_gherkin_behaviors_impl.py,sha256=zL-ZqagYkhokeoN01LZGnCeIMyzsEUEvZOxSzx1JVXE,7000
 aac/plugins/first_party/gen_json/__init__.py,sha256=ZwLc3W3DNokSFySFnVHrzxvK5XM-r9dk4XLFIsjD4GI,1470
-aac/plugins/first_party/gen_json/gen_json.yaml,sha256=F7DvJQwDyL0jWkb_EGkbpqUTSyY3qxLIgr6E786XRDM,950
-aac/plugins/first_party/gen_json/gen_json_impl.py,sha256=q1ttl2UR0j-sya288oJnvyaiY4S9Dl5lSeu2ZXgbHJE,1987
+aac/plugins/first_party/gen_json/gen_json.yaml,sha256=itU96uADIWdlRjC0LS_2Aa5vq1Djqm-xz6CTGQ3H6xw,997
+aac/plugins/first_party/gen_json/gen_json_impl.py,sha256=OU8avk2TkMYEDcf_yt6xgpkxoxTYeus70khNxgLpWyM,2006
 aac/plugins/first_party/gen_plant_uml/__init__.py,sha256=zxSNkJqniWX7yhBGRND8tWMP8RM4u9kNkyAv8bdGero,2763
-aac/plugins/first_party/gen_plant_uml/gen_plant_uml.yaml,sha256=QbVkAgScmlM3unH9343fhINUeyqSo1rzsXSM6oCzfvQ,4050
-aac/plugins/first_party/gen_plant_uml/gen_plant_uml_impl.py,sha256=q6UH4A2q7-Ptls-wJZSt3T-DDu6EPVO_M19_YZOa_p0,12544
+aac/plugins/first_party/gen_plant_uml/gen_plant_uml.yaml,sha256=XIJSEru3JxVDvZRkksqtP9xwb4NSHn2bduIUbBKkXS0,4334
+aac/plugins/first_party/gen_plant_uml/gen_plant_uml_impl.py,sha256=DvI5pCxVbXiGGw2h3eQQs1U16nWj-aBWGKQH2upbMiY,12572
 aac/plugins/first_party/gen_plant_uml/templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aac/plugins/first_party/gen_plant_uml/templates/component/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aac/plugins/first_party/gen_plant_uml/templates/component/component_diagram.puml.jinja2,sha256=R0OGXfZ9ddINv22TzEO06XM_Z6wKBcaWcDknAGk8rH8,960
 aac/plugins/first_party/gen_plant_uml/templates/object/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aac/plugins/first_party/gen_plant_uml/templates/object/object_diagram.puml.jinja2,sha256=oILUCRacFEs-zf3wAdAEnzqARAmDTIcAv3Vo4ixfueI,258
+aac/plugins/first_party/gen_plant_uml/templates/object/object_diagram.puml.jinja2,sha256=5-VL_q4L2cMaU1DS6TqGWDQfW6326MsjMVYvkdD0TdM,255
 aac/plugins/first_party/gen_plant_uml/templates/sequence/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aac/plugins/first_party/gen_plant_uml/templates/sequence/sequence_diagram.puml.jinja2,sha256=ay98zeixQNefjsRsHzVwsPkHr3ph-vJQQP9erSk6FZY,300
+aac/plugins/first_party/gen_plant_uml/templates/sequence/sequence_diagram.puml.jinja2,sha256=KSPP8rwluWyAMHbeJya7GA72rhnmepzLowQmNkct3ZA,297
 aac/plugins/first_party/gen_plugin/GeneratePluginException.py,sha256=SbiJ_bV4dZFbwuboYGZw9dxRfuHzBtwXdcXPYobcJqU,204
-aac/plugins/first_party/gen_plugin/__init__.py,sha256=uAWTThmQmsBfDn0PZ-8r4NsRM8iNuLsiHolfUS7h8tM,1441
-aac/plugins/first_party/gen_plugin/gen_plugin.yaml,sha256=lb2O027trVrPBICDKDJi_VheXkdwSv-d4zQ7j5ppZ60,1841
-aac/plugins/first_party/gen_plugin/gen_plugin_impl.py,sha256=4fbC01AkKcFL73DwebK6khA1KcDtf4gVvfFFEUv9Dlo,15242
+aac/plugins/first_party/gen_plugin/__init__.py,sha256=gPs-GUIgLcnbMj_7aHE56kUkPKQs0eP4g7CGLgID4Vk,1442
+aac/plugins/first_party/gen_plugin/gen_plugin.yaml,sha256=8p8KSC9GZ0jZUBvYVyGUrhW26QbpXVouYHkTZ50DfZM,1780
+aac/plugins/first_party/gen_plugin/gen_plugin_impl.py,sha256=EQqgVNLWQM1xHiQoTkHIxOG-AuZppHNkIePm-pAVIC0,17121
 aac/plugins/first_party/gen_plugin/templates/__init__.py,sha256=RAp2ZUFhJakZktpR1RhPEtLWRiOVmrl9i3ubtjue-OM,170
 aac/plugins/first_party/gen_plugin/templates/first_party/__init__.py,sha256=RAp2ZUFhJakZktpR1RhPEtLWRiOVmrl9i3ubtjue-OM,170
-aac/plugins/first_party/gen_plugin/templates/first_party/__init__.py.jinja2,sha256=O3in4nnIpQKsMKliiEahBTn9UeW2b846Zyj91JrZZPc,2750
-aac/plugins/first_party/gen_plugin/templates/first_party/plugin_impl.py.jinja2,sha256=vd04lCkJyYDL171QFzivbGoBiz_WegTWjftHcYt6KFM,1827
-aac/plugins/first_party/gen_plugin/templates/first_party/test_plugin_impl.py.jinja2,sha256=FdEClX7p_qQrt7KQ7qBp9h020UmaKnK2wpxRMhXRFVA,1017
-aac/plugins/first_party/gen_plugin/templates/third_party/README.md.jinja2,sha256=FoZ1ykYlkvkBccG2swQAA_MX3yMRhxexP2ErZa3taeo,966
+aac/plugins/first_party/gen_plugin/templates/first_party/__init__.py.jinja2,sha256=spUQ0pDJdkSCHdAQliE0JjPXyCw3iLxq6qZm1OXp7MI,2700
+aac/plugins/first_party/gen_plugin/templates/first_party/plugin_impl.py.jinja2,sha256=X9XPEs-pQR0zkkh_xOfpDp70yRthjdymugvqA26wTTE,1821
+aac/plugins/first_party/gen_plugin/templates/first_party/test_plugin_impl.py.jinja2,sha256=cAijrgg9DvMiAIoHFVY3TgfCWC0LJaQz7Xjq4LXE_GA,1036
+aac/plugins/first_party/gen_plugin/templates/third_party/README.md.jinja2,sha256=zC5BHuifWu-E72-LjA9freCTskcx-fR2Ii4o0rv0bJ4,931
 aac/plugins/first_party/gen_plugin/templates/third_party/__init__.py,sha256=RAp2ZUFhJakZktpR1RhPEtLWRiOVmrl9i3ubtjue-OM,170
-aac/plugins/first_party/gen_plugin/templates/third_party/__init__.py.jinja2,sha256=cpIthVGbDLkfngMnL3wQ0KkAdH594EitPQ0G_gYk7oE,2734
-aac/plugins/first_party/gen_plugin/templates/third_party/plugin_impl.py.jinja2,sha256=o_gKxBq8jX1jBRKsZVi7moV0DZxxobR5j4_ge4nsmtM,1704
-aac/plugins/first_party/gen_plugin/templates/third_party/setup.py.jinja2,sha256=5xiFBVhFvm-X6qPyObiC1rkCzbBx_TNrkvxQ7yhokJs,935
-aac/plugins/first_party/gen_plugin/templates/third_party/test_plugin_impl.py.jinja2,sha256=G3A4QtkfAntn1ITakHpulYRnGu7RxVQeKdtTgPt-lcs,942
+aac/plugins/first_party/gen_plugin/templates/third_party/__init__.py.jinja2,sha256=knwhivCHGIDl3MsP_V44bMYvYBTmjSj9kiWylNHuscM,2685
+aac/plugins/first_party/gen_plugin/templates/third_party/plugin_impl.py.jinja2,sha256=udAAW23_NTL4pPNCdHvhwRVedrF4pvz_1Zd6HGrg19Y,1698
+aac/plugins/first_party/gen_plugin/templates/third_party/setup.py.jinja2,sha256=xNssWA7MJfzcE3IkpFj-FGwW-BKegVtvoa2M1_xbpak,954
+aac/plugins/first_party/gen_plugin/templates/third_party/test_plugin_impl.py.jinja2,sha256=TYMfK8GSkstF0UmlJbhP95RieTshRDqGIJ2GimIuY44,961
 aac/plugins/first_party/gen_plugin/templates/third_party/tox.ini.jinja2,sha256=PruP8cw-FdJNQXn3LbSWqWmOsR-1dHFhIhkGWwdWWHU,761
 aac/plugins/first_party/gen_protobuf/__init__.py,sha256=5jBeQJoHKx_Zw8FQRZcHM1_8ahQTLtSNAzn-unHtKSY,1462
-aac/plugins/first_party/gen_protobuf/gen_protobuf.yaml,sha256=cSlkmmSLU2nrcLtevUeTFq6wUL7EuLQCOBdcktyNHcg,1679
-aac/plugins/first_party/gen_protobuf/gen_protobuf_impl.py,sha256=KpUd_SvYm7tXV_KcSHJnDN5e3og5wHe2_u-fcWADoms,19204
+aac/plugins/first_party/gen_protobuf/gen_protobuf.yaml,sha256=QP-VW7EK2vDSjb0zCNKOxQ1e3Px42d7KNL5WagaGhk8,2632
+aac/plugins/first_party/gen_protobuf/gen_protobuf_impl.py,sha256=DDMzciel9wjJL0NM4Mk9gMNeiO0R1BI5RbDRqVNGbxQ,19919
 aac/plugins/first_party/gen_protobuf/message.proto.jinja2,sha256=7VlxT4i26QiLoD6D6txIOvJoYjhh60dFrIEl-fAR2fc,1006
 aac/plugins/first_party/help_dump/__init__.py,sha256=8VhGeV-jXImSvyeaZg1PRpZdi-yfxYsgHpEGbfKAObo,811
-aac/plugins/first_party/help_dump/help-dump.yaml,sha256=vZFE-py2w7rsKq6nkn-QkSDtV9PV8PyG4E5528isS70,956
-aac/plugins/first_party/help_dump/help_dump_impl.py,sha256=kthh6gsxzB9_k9TaF3ct6fnfp2BzOXqWFi_LobfrIIk,957
+aac/plugins/first_party/help_dump/help-dump.yaml,sha256=GlFJL2fj_jj6ARj0CLDwWYVqx2KJG0FNJWVtinIrksI,906
+aac/plugins/first_party/help_dump/help_dump_impl.py,sha256=pjW8-dMfhqMYD4aibD7ZUd8gvT2VPE-abPPDbF92Wro,965
 aac/plugins/first_party/lsp_server/__init__.py,sha256=as1BThgbkmvcQOB13XtZkRdhrLi1ShZxKs2cz10NUr4,1403
 aac/plugins/first_party/lsp_server/conversion_helpers.py,sha256=w8lBh4TOMzf7j0Iit87XiZ5-yfczEH8lYgsFpFcv9Kc,1227
-aac/plugins/first_party/lsp_server/language_server.py,sha256=JRlLekxzGbAELIGhUn_6dWseHpdfAUeNPceho09f_Bw,11826
-aac/plugins/first_party/lsp_server/lsp-server.yaml,sha256=XKtR8dxRUfM4v67z5_C50IHUlYDt7Np_l-LXTPxB_1E,1414
+aac/plugins/first_party/lsp_server/language_server.py,sha256=W6MzrwcLgL97d0p9gVinhJZe3uz--oXh0Zxe9EWRPaU,11791
+aac/plugins/first_party/lsp_server/lsp-server.yaml,sha256=zocsTLdvaTnLSeP2lly_NAOwHjg1XkfEc1Ekxbjxj3A,1481
 aac/plugins/first_party/lsp_server/managed_workspace_file.py,sha256=s7lIy77kWXFDEzRBYGWTLo_oUNZ6D2UtImtx8eZwZms,593
-aac/plugins/first_party/lsp_server/start_lsp_server_impl.py,sha256=x4bVdBPAgTB2ux70o7oghP0LdXFACBfW8klZneD467o,1194
+aac/plugins/first_party/lsp_server/start_lsp_server_impl.py,sha256=v_KVqA5Z2MgN2PP2aPFlXzOtUT31YUA2pGNlTUTnMUE,1197
 aac/plugins/first_party/lsp_server/providers/__init__.py,sha256=CU3NxNAU6EYZEQb2vOjdzf_2rb0PBmzQLqZr6_LhN_k,64
-aac/plugins/first_party/lsp_server/providers/code_completion_provider.py,sha256=MvHcO2YzD96y_V0I2qq9wR_tPju7NC8blgLt3TYvLhs,4214
-aac/plugins/first_party/lsp_server/providers/find_references_provider.py,sha256=Ovv50lHkCxUecIwY1IdVZAWftdo3VMGZqfAfYUWyDaA,5804
-aac/plugins/first_party/lsp_server/providers/goto_definition_provider.py,sha256=xPjG3jEn9einjlP-WCcaKM14AtlYAvPTGI_0B0Y4tP8,7384
-aac/plugins/first_party/lsp_server/providers/hover_provider.py,sha256=11llkV35BdoUBxqYg9kbnC0Bhnbh0RhcjMiqdJpvLP0,1375
+aac/plugins/first_party/lsp_server/providers/code_completion_provider.py,sha256=zuSnyPcTH2FRjRO2MO4BSE9PLRj42dy6jhcg-JiH9Ak,4430
+aac/plugins/first_party/lsp_server/providers/document_link_provider.py,sha256=rgSdaUWsRcqYyxWQKPtsHntgPALCd6aUy9QWn4eXayE,2593
+aac/plugins/first_party/lsp_server/providers/find_references_provider.py,sha256=QVwNpgCc8KK_1mZuYsVegElHh7laaXQx_h9SUUtpDOM,5799
+aac/plugins/first_party/lsp_server/providers/goto_definition_provider.py,sha256=5ft4Pe6hb-GFXRQJaVmeZA8I9rvbfL8d2Jg1htMdBTg,7275
+aac/plugins/first_party/lsp_server/providers/hover_provider.py,sha256=7mQFcZTZRJ7f2n8snD9w0xEFDIJ-WtUK68BqkEeK4Ew,1523
 aac/plugins/first_party/lsp_server/providers/locations.py,sha256=ncMNXxM-e-hGAK_fwaVQ6dT0904VfewrpKq934Mvz5g,580
-aac/plugins/first_party/lsp_server/providers/lsp_provider.py,sha256=XrEqk4F7cipjNne3neV63PGYGw8tMMbKaSewRjfYxHM,491
+aac/plugins/first_party/lsp_server/providers/lsp_provider.py,sha256=Z86Ptqw9lY33ktbRhadnrPNjKPmQevQxdb6vw8-wcKY,467
 aac/plugins/first_party/lsp_server/providers/prepare_rename_provider.py,sha256=baMeiRpCXwO6ETLmsoFnpBAKsVyPy1gmetZy7bBNDDY,1461
-aac/plugins/first_party/lsp_server/providers/publish_diagnostics_provider.py,sha256=7kVOkeCtgZ2ahrVimTUaGgKovETosKZ7gqCkm4RS6OM,2838
-aac/plugins/first_party/lsp_server/providers/rename_provider.py,sha256=ecyjCUqVBbhaCDBOd8vfFp7n5qQB3lUNB1SYkfetTHc,6411
-aac/plugins/first_party/lsp_server/providers/semantic_tokens_provider.py,sha256=ZvNkjmq6Xq5E8USz01ZaMk3WZKf9RrsfFxW43R3qTso,7107
-aac/plugins/first_party/lsp_server/providers/symbols.py,sha256=en6xhcRqMgr5ARbZA8elA_N1Pl31j3LvW5z8uMa1cYE,3381
-aac/plugins/first_party/material_model/__init__.py,sha256=h3jOW0uEPxgqDkZ-vRcfA6zdAnRmJcqM_3deR-FRhDA,673
-aac/plugins/first_party/material_model/material_model.yaml,sha256=IjZXbWspd_VOjtd_GHFg2Uasw5kZR91Yj5O7LbsIhf0,4710
-aac/plugins/first_party/material_model/material_model_impl.py,sha256=9-hpgxviqB_6d3ay9fYxjEv8R2MuF3G-y0AqNfXRqcU,102
+aac/plugins/first_party/lsp_server/providers/publish_diagnostics_provider.py,sha256=Ymtkrb_Szwbz0xlh8bL1JNTMJHoIC0o9hVBUBT8R7lc,3712
+aac/plugins/first_party/lsp_server/providers/rename_provider.py,sha256=yEVhA4I7Ph3punDtG-YUgKJXiBqB46pMJjrYo--clo0,8796
+aac/plugins/first_party/lsp_server/providers/semantic_tokens_provider.py,sha256=lR4G9gJLlvctkfK4uQ-SEP66LSnorYzRkYEkRG2nSMw,6989
+aac/plugins/first_party/lsp_server/providers/symbols.py,sha256=azulLyk4Kj0v7cVTIc70Xcte0FU8IoJ-mP1d508oqdI,3589
 aac/plugins/first_party/plugin_management/__init__.py,sha256=92tqWgrPi6H4Qt7xWeyKaQf7HyoLZHB6pFLjWwMej-g,2220
-aac/plugins/first_party/plugin_management/plugin-management.yaml,sha256=zT5Q6ivPbKvEkBgprbwkZVzHSvHozqinaTR5p3xLo20,5264
-aac/plugins/first_party/plugin_management/plugin_management_impl.py,sha256=DABcSgg-kfagDTRGA_nPxBw2SuarQ_5GYTT1rnwrZ08,4411
-aac/plugins/first_party/primitive_type_check/__init__.py,sha256=62uLLQa24h_P8xCw3J3P69OpDixq_78BXrKX8pRbU_A,786
-aac/plugins/first_party/primitive_type_check/primitive_type_check.yaml,sha256=OaduQl3hUktHLaeP6oV7gOMQiQUHh0WV0mSi6EXSbLQ,2256
-aac/plugins/first_party/primitive_type_check/validators/__init__.py,sha256=RyNbxrdraK3LTY2206uUg4jW9INTtooR3C4K2js778Y,911
-aac/plugins/first_party/primitive_type_check/validators/bool_validator.py,sha256=nWQqbIUhD8fZya-wiCauxbk8PjBWbPbmwgEX-Z3zXyQ,1819
-aac/plugins/first_party/primitive_type_check/validators/int_validator.py,sha256=iCvCGC5QGttP7mQDwknIcEOfRRxqMSPw4XenOZ5-UrU,2226
+aac/plugins/first_party/plugin_management/plugin-management.yaml,sha256=wVTrVZKMy7YgIctMVauvyTsg1POiIDHwfT_AhC2-gPQ,4969
+aac/plugins/first_party/plugin_management/plugin_management_impl.py,sha256=ZO5-eFu09sZM3jbxCckeCsbYX6E7IAQnpbC2flUe3-A,4411
+aac/plugins/first_party/primitive_type_check/__init__.py,sha256=sUPZqCJyvZSewIQBJ_XGE3S8uLxPWLRkv_r1IT_YhyU,1138
+aac/plugins/first_party/primitive_type_check/primitive_type_check.yaml,sha256=Avsb3wH_Vp1P4frKJbr0KMh502Xc9djB3QtqEnsmVk8,16042
+aac/plugins/first_party/primitive_type_check/validators/__init__.py,sha256=_vxaZUWgbI6sxKXqUmHVgr_FTImb5Dfzj783ct41a0M,932
+aac/plugins/first_party/primitive_type_check/validators/bool_validator.py,sha256=2iaYlE-pzSlb9WLdzeazNwX6YOMIo25JUvLT9UQxkqs,1933
+aac/plugins/first_party/primitive_type_check/validators/date_validator.py,sha256=cPndlOP0hhuaE1kOoPMItbNvpBMIlE2ydDUrUwQOeCY,1974
+aac/plugins/first_party/primitive_type_check/validators/file_validator.py,sha256=2Hhr0ouOkwkuW-KuqDkyeUpQ9iGis8Uq7uZzUlMvXow,2156
+aac/plugins/first_party/primitive_type_check/validators/int_validator.py,sha256=25vsSOhzgt4FfW_LivUFILU0LCdhmwWx61nUKjbT2P0,2326
+aac/plugins/first_party/primitive_type_check/validators/num_validator.py,sha256=Tct4VmOeqU3eUMjjhmb4vwqwY14M3PK1qsurS3CZIR0,1955
+aac/plugins/first_party/primitive_type_check/validators/reference_validator.py,sha256=S26uP184B97Zjc45TxUMdi5027qf6XqYonnhdPS4m08,1800
+aac/plugins/first_party/primitive_type_check/validators/string_validator.py,sha256=tyHpyzMAaVkfVN-YsQLXFfnlIuNWjc3U0AlHPhcygMw,1852
 aac/plugins/first_party/print_spec/__init__.py,sha256=8cfItdvlXbrXzQvF5QgG_dKFgpEAWaXyqTAXqzSFzM8,1017
-aac/plugins/first_party/print_spec/print-spec.yaml,sha256=JtScObWU8p2bVzAGd8znz26uPAHSydXT6H-3EPG5vro,898
-aac/plugins/first_party/print_spec/print_spec_impl.py,sha256=lCOn03Cvie1ETe1lzAg83WvX7XP3GZw1PoJSXQfW39c,957
-aac/plugins/first_party/rest_api/__init__.py,sha256=iPo1HDpd9-b4JsXGJfDVDGLMOnYxGQuDVD5xMVCqZBI,1667
-aac/plugins/first_party/rest_api/aac_rest_api_impl.py,sha256=Uh44fXfb1-eHi4lNCTvFd730w5YAncMphNp4P-YGers,2138
-aac/plugins/first_party/rest_api/aac_rest_app.py,sha256=bgm2ud9Qnsyh9AE1ZaL2tfFRTvmi_bT3FFGcTk1OITs,13921
-aac/plugins/first_party/rest_api/rest_api.yaml,sha256=T_a2m00zjtDkDK7X9CJyMWmRqNIxVnW39ZD1ICNqlmc,1947
+aac/plugins/first_party/print_spec/print-spec.yaml,sha256=CYmmKC_QY8FYQQa9eOREdzhC_8HGzOWCRgn8Qbhc0bk,899
+aac/plugins/first_party/print_spec/print_spec_impl.py,sha256=-T7BhoeUtQuH3ffcmA9rYE_3M7JPphdYeM3xMl8uT6g,967
+aac/plugins/first_party/rest_api/__init__.py,sha256=mW2F7gy4_6uHe0z0sXA04YkaZ8OZNdevpVa8fzrucvs,1662
+aac/plugins/first_party/rest_api/aac_rest_api_impl.py,sha256=z-JnBkSwzXTiQMfe8V2gp57xw4F4qbTOS_kbtDj1p0I,2135
+aac/plugins/first_party/rest_api/aac_rest_app.py,sha256=i6Hj2lwRLfxjb_v1yOkrPTLSQCVHgRxjSFsAPbJ3e0M,16354
+aac/plugins/first_party/rest_api/rest_api.yaml,sha256=qa_a1EaiErbAugwJ8NsNz4PYJUOUkQPlXXCUHNDhb7g,1973
 aac/plugins/first_party/rest_api/models/__init__.py,sha256=A77lrsYjeoZcpyX7zKb-rRTEeXb0zcyW8hZJU7t6CLw,52
 aac/plugins/first_party/rest_api/models/command_model.py,sha256=c7h3ZGnXfVGO8Vq_Kk1wmkOqmY2MnD1L_LDnNKYbTyQ,1563
 aac/plugins/first_party/rest_api/models/definition_model.py,sha256=O0bG7DSweCBeodADQT5zBe4b4IvfBfSY1Fab3LsDEWc,1347
 aac/plugins/first_party/rest_api/models/file_model.py,sha256=P6GpNdHnQrg46BSO4S1Es5Zf7_gcLPMgaSuGbp8Hra8,1480
-aac/plugins/first_party/specifications/__init__.py,sha256=dTIOSYy95EmEDOrsiEJ3P50t6PFdnEI7BsL1GsNlWE0,2891
-aac/plugins/first_party/specifications/globally_unique_id.py,sha256=uPe2oElEOyk98waU0YoyvzSE_ExuUaSPUpQU43Zox4g,3684
-aac/plugins/first_party/specifications/referenced_ids_exist.py,sha256=CD7Dwlr3CjZYDbJe_1GNCy7CCJmXL0j2hI1FCp9o6nM,2757
-aac/plugins/first_party/specifications/specifications.yaml,sha256=_SNbkDcCR5EGWVzP9ny9xFv0DiyeQoD87mpofh7hw-A,6167
-aac/plugins/first_party/specifications/specifications_impl.py,sha256=YD9bUiCBMk0XfC-QaHK0dq0HD4fnFc3NlmF8ZP1k3AA,3688
-aac/plugins/validators/__init__.py,sha256=alJRjkl4UDZCdUVWQZk0PHCCg0SVPhnqzuFO6xDjftU,663
-aac/plugins/validators/_common.py,sha256=uHDwDgpiJP74vY4AuLZcJgAlvKdVdZy7bbhWBjMftRs,2077
+aac/plugins/first_party/specifications/__init__.py,sha256=jSGNbQ3IcoCGQH20zl8K55aS5_z646Qd9c9_WkLJv7s,1544
+aac/plugins/first_party/specifications/specifications.yaml,sha256=zjUTsRVjE0UfvMUwuc4Gip3z7XCB9rh60jeyKuQmBio,994
+aac/plugins/first_party/specifications/specifications_impl.py,sha256=VrPU-lcWHiClzoayhyl8JBzUTL3zpLqLQv4_lYSsbpc,3697
+aac/plugins/validators/__init__.py,sha256=rEQ2PedVsE6gwORYAIeHwZJo3qmkIK5JlSNKvzfYvrI,812
+aac/plugins/validators/_common.py,sha256=heIMVu8o4igM-re3NvxXQJsubM8LlCWxfSHN74dpRNQ,2302
 aac/plugins/validators/_finding_location.py,sha256=_ViWWoNqkOzU0FNWErRZoV5Sq0hWiTwbkD_cAK-5wDo,2538
 aac/plugins/validators/_validator_finding.py,sha256=eV6E_5E4VRK6GpFeTCV7N4RGgGAHA9vbgD-Gbvmgor8,1564
 aac/plugins/validators/_validator_findings.py,sha256=SicrukKNIYCi7zJ9U6ZBgrf0c8jt46pBo66dde-JAx0,2902
-aac/plugins/validators/_validator_result.py,sha256=auONV2IgBp2HUdHiyORfJP53AqvnO_Zfg4k_kpKky7k,1749
+aac/plugins/validators/_validator_result.py,sha256=Zk1p3uGKs7yCz0m5ijc_49EM1H2vTUZLTM-2AbyeiTQ,1701
 aac/plugins/validators/defined_references/__init__.py,sha256=lrvAKvCzbMEWWssiiaeL6Z4LGHdty062JcR8oO3Mt1g,1060
-aac/plugins/validators/defined_references/_validate_references.py,sha256=j5JVFh_jmauRdxmTV8AwYdql5-rDSXDx4VxWCVdJXZQ,3262
-aac/plugins/validators/defined_references/defined_references.yaml,sha256=uEYfx1ydzFedsAfUu5qHJs58n4Mdi_SSduv0PN6MsS4,1443
-aac/plugins/validators/exclusive_fields/__init__.py,sha256=i1j2lkrrJDqyGw9IkFEQM43glIksM8uxiUkMLuSlf4s,1054
-aac/plugins/validators/exclusive_fields/_exclusive_fields.py,sha256=5OeLVUnCIB176T3uux_Mc09asxdFpX4Vr7lBUnn9wR4,1968
-aac/plugins/validators/exclusive_fields/exclusive_fields.yaml,sha256=_ExGrKLlCQPjLhHF8gBO3jTWVsucdbnrGXOs8Ztq1v8,2117
+aac/plugins/validators/defined_references/_validate_references.py,sha256=c6OXBBufxD9xVsecTOh-RjxpusgPXWKpIk4RlFNnfCc,3353
+aac/plugins/validators/defined_references/defined_references.yaml,sha256=G3VAUe-4G8P9jpYNRhznCHJVuABXy7ptdspL8iBlTDY,1648
+aac/plugins/validators/exclusive_fields/__init__.py,sha256=WhVqO13IUtakV14zM_Q9nhhPS66r7QwRZC2YgehYx1E,1063
+aac/plugins/validators/exclusive_fields/_validate_exclusive_fields.py,sha256=-evrlLpl23OVA8g-Q2NkQQDKJiCZjHTi5swOVkr3ic8,2022
+aac/plugins/validators/exclusive_fields/exclusive_fields.yaml,sha256=7N-5YyQhwPFUeAiWEWnMYETIf_LeEd3sCFrmR9TZsnk,2417
 aac/plugins/validators/reference_fields/__init__.py,sha256=jVX5jMhBfvkIcB1dNESMuhmSpQY144mzcXdhtHoeD70,1051
-aac/plugins/validators/reference_fields/_validate_reference_fields.py,sha256=jRrbepX6CMCJe7eP6jxOCE_st6yd5rG6zhiJa8YAPnE,3596
-aac/plugins/validators/reference_fields/reference_fields.yaml,sha256=9tLt1ngHaI5BWcQ1cH3v4pMM1m8YJM0vsAhH3Hqbx30,1450
+aac/plugins/validators/reference_fields/_validate_reference_fields.py,sha256=hvHTKgvIUF8m6QSL2AoO1OllPrPubqf-HOTwH0p8JqM,3599
+aac/plugins/validators/reference_fields/reference_fields.yaml,sha256=GNbbLMzxW5ACZpc62_5WDtYlEUYmxUItqKGZYw6QWFo,1681
 aac/plugins/validators/reference_targets/__init__.py,sha256=BD5K5ntJKJLoPDBTxL1Tg9HN6uf17JrY2owOvRKbWgs,1056
-aac/plugins/validators/reference_targets/_validate_reference_targets.py,sha256=S1MmONVuAHYRIjhlFuK0OfjZfHeOcjzOmEOD1YiedGE,4423
-aac/plugins/validators/reference_targets/reference_targets.yaml,sha256=nP6IBWieye_miZKBJLYm70cxTItiPhMEqpK7b0jxEcg,1459
-aac/plugins/validators/required_fields/__init__.py,sha256=-Ocx0MRKfDckjHOmAJgt2rdG7AtQMW_pPpN43Zp1_XI,1638
-aac/plugins/validators/required_fields/_validate_required_fields.py,sha256=vT_n0lsh5Hp4GMk_qNe0CsqzUV0Spj-zgPzYmj1iwi4,3327
-aac/plugins/validators/required_fields/required_fields.yaml,sha256=KqL9B_QEwnRCBImszyt6_7odOgQIvAbaZRH_ohoELtw,1496
+aac/plugins/validators/reference_targets/_validate_reference_targets.py,sha256=4xwv4D8n5UrrNTWAqcI-4d1fj97KEm041es6F7V3_6A,4612
+aac/plugins/validators/reference_targets/reference_targets.yaml,sha256=5mAA2e1CzGZboG-dCTiIu_ylR2T9WJOWtAxJHpwwGXU,1683
+aac/plugins/validators/required_fields/__init__.py,sha256=y-h8qafS1v_7lnd5HdQu7ss_hZ0wHsOT1RNfsInvEtE,1787
+aac/plugins/validators/required_fields/_validate_required_fields.py,sha256=oWpqutFKYN7vov2ZOZF0vM-0sMyDH04GoqvQ34QnNDs,3372
+aac/plugins/validators/required_fields/required_fields.yaml,sha256=D3FTETNtfqhaY_gcnrNXA7oWgYKXopP0hKy213Qa18Y,1726
+aac/plugins/validators/requirement_references/__init__.py,sha256=noDeg0jum1lUhVkjDSJuc75SufnLZShfVSvELDtNNw0,1049
+aac/plugins/validators/requirement_references/_validate_requirement_references.py,sha256=Ls5S03m31Zuyc-o79C17uZOPm08o5vzrM90gauFvcdo,2696
+aac/plugins/validators/requirement_references/requirement_references.yaml,sha256=u7BSGNPw5sGv60bFlNSzdEDJIj3k7a67qX0UnUDvuZQ,1644
 aac/plugins/validators/root_keys/__init__.py,sha256=ShBblVggn18L8ONXdjNSvStUE0o6OTGjYCbAN2Nzp2A,1012
-aac/plugins/validators/root_keys/_validate_root_keys.py,sha256=WrUsFQirpz3sHc3PzEr6TFHrNTQPHTyxNo70Lk-8YHQ,1601
-aac/plugins/validators/root_keys/root_keys.yaml,sha256=5N4724Nvu8Xs2BOofwkXo3a0qV9c-s4pGMn9BpF-JIg,2257
-aac/plugins/validators/subcomponent_type/__init__.py,sha256=g61p2AIDpR0TiNc-qDDgmIQtsPhwcVqGHyq8OQDN3gw,1053
-aac/plugins/validators/subcomponent_type/_subcomponent_type.py,sha256=NTj_-3qb14pTmyVesk8cef_-Uscl9pxwayzU1XKlGdI,2979
-aac/plugins/validators/subcomponent_type/subcomponent_type.yaml,sha256=M1V-NVCD8RKh71hMhy41SlMM4il_5_eg3d8j3Wlxnjg,1493
-aac/plugins/validators/unique_names/__init__.py,sha256=0pc26PFMWdGybIvUIfAtnro74qLAgC-OC6Osi0VilmU,1006
-aac/plugins/validators/unique_names/_unique_names.py,sha256=f5NDizheJSdFms65oaYCXXfu1xbm2MGqkCMYjaSOpdE,2311
-aac/plugins/validators/unique_names/unique_names.yaml,sha256=Xg-yLCGv2PA34g-Cr5KfwS5wa6P31hnkexQhO3JV7nU,1524
-aac/plugins/validators/validator_implementation/__init__.py,sha256=3AiW-N0jwNitMrO3BLuRYoYW5Qj7vl4OqFMFixRS1D0,1107
-aac/plugins/validators/validator_implementation/_validator_implementation.py,sha256=mzrG5wyNPXv1PLkvnK5iL-qIrAX2h7vDaN01z6XEEwY,2775
-aac/plugins/validators/validator_implementation/validator_implementation.yaml,sha256=w2UhcTEPhyQMLbal7IzD5n6DmrwhNxOrnCi9NDaBnCo,1470
+aac/plugins/validators/root_keys/_validate_root_keys.py,sha256=2lGpEDR_s9GKV-GHxwOBQ4lpp2s0xCGybe5AbmAluww,1640
+aac/plugins/validators/root_keys/root_keys.yaml,sha256=pBh_fZMUkxQtIHLwdwS8C900hvdRWKtoz6HLleKXlyg,2461
+aac/plugins/validators/subcomponent_type/__init__.py,sha256=KZ6XuNu81AKfYvYrE1tZ_SgKDodolTbHe3DN4MBgOXw,1062
+aac/plugins/validators/subcomponent_type/_validate_subcomponent_type.py,sha256=Y67akbMXvm-skQZNEWLp1xX0BZHVUBIuOG3RW_8q3jU,3028
+aac/plugins/validators/subcomponent_type/subcomponent_type.yaml,sha256=wvIBtFvcSZA6KBMC4rBhnRF2LHVMXPDqceC2cPAh59s,1714
+aac/plugins/validators/unique_names/__init__.py,sha256=5cbWEQMKb4546aE_J06WNKsQNjdfE01HHEPE4r-l2VU,1015
+aac/plugins/validators/unique_names/_validate_unique_names.py,sha256=bUspqkuoVnq3Yf0gnopHgj9b8Y2gCffn3VV-Rlq3F28,2365
+aac/plugins/validators/unique_names/unique_names.yaml,sha256=IeTdU-usAlhEJHTl-X_Qzflc5msllSE4qUydeSD93cI,1675
+aac/plugins/validators/unique_requirement_ids/__init__.py,sha256=7ylTfYdKaXOm7kXsJstbgTDR-KzaiXO9jHSQV2mk3Dg,1049
+aac/plugins/validators/unique_requirement_ids/_validate_unique_requirement_ids.py,sha256=I6i3iNNAghgNJ7SH4N8UFR1EYL-DQ_m7A-AQLuc2nY4,3698
+aac/plugins/validators/unique_requirement_ids/unique_requirement_ids.yaml,sha256=-hpx5oZ7nuuGZE-s5Dk0aVWOFsohwfeW7VldQW4CIj4,1689
+aac/plugins/validators/validator_implementation/__init__.py,sha256=tykmf4GPr99QyEFpVxpcUnmnMu_-VI8KdUg5r8qb74Q,1129
+aac/plugins/validators/validator_implementation/_validate_validator_implementation.py,sha256=9jaw-5ydQZfWCcQr77xrVAtH4XDUCvM5bQ6Zkgt90Vs,2317
+aac/plugins/validators/validator_implementation/validator_implementation.yaml,sha256=ZoXQ4oOV4kpYLd-TUr6BQOwpafFMd6LqE7mAfaa19ag,1722
 aac/serialization/__init__.py,sha256=D7X8SF-q8A9sHoUgIp1TiS0FxCMVMmCO8oucooHoEeM,246
 aac/serialization/aac_command_encoder.py,sha256=FSDWW3_VWyODXr3wk4-Yq3CUtmidGKLcS7FMPrsjsIM,1076
 aac/spec/__init__.py,sha256=iDhmFu_ZRDVW8Mj4HFA8NEhIkUAV9NBJLvinckdnVqg,317
-aac/spec/core.py,sha256=GRHohDHQMusznfFQqXAh8Kq0WCZoCfrMUQJ9oK3Vn5Y,3790
-aac/spec/spec.yaml,sha256=i_pGah2kzhjKk_yClIC-7SVxtlIBV-n0wHbs3eargHY,14319
+aac/spec/core.py,sha256=JLGJOG5zoB8LrXcqQGwKin_5u4FGBdqQUWs94oM8VwY,4140
+aac/spec/spec.yaml,sha256=o9Ufc2jxhTO1Ro6lpqwG6-GQjMd7U1pe_BVeZlMo6Wc,18876
 aac/templates/__init__.py,sha256=rHx3LezGq79lpCUjronIx0C22Dd95ExxeQl8v0Aok_0,190
 aac/templates/engine.py,sha256=YOpkz06bKyqbFoARLB8B1z2zfWlBj7fmIbdgIyd2FnA,6327
 aac/templates/error.py,sha256=fmZpuXNLfq2uqjTrolvxKkS8Cf37CqBrn0f09gQuXCY,379
 aac/validate/__init__.py,sha256=I-k_-_FLX8D88H69EnCEq_80DY8QWc6u7zwqmtyO5GA,532
 aac/validate/_collect_validators.py,sha256=a24vBF6aBY5gyhCfRsTUWLioDx6t21AVKfNh4mhhMEM,3995
-aac/validate/_validate.py,sha256=yDnFXDF18NHkJpvS0OpaPEcOpF7rNZTsN0rnI1qs0hA,10478
+aac/validate/_validate.py,sha256=d3XwgihSqwRCU_w2tWjB1q9exKfNMtgr-IgM0PG7dSw,11286
 aac/validate/_validation_error.py,sha256=pNLC7scBvNfWCbGUZsqiuIfsRVZUD7yJOXJsDNM6nzI,214
-aac-0.1.9.dist-info/METADATA,sha256=XLXtpyGzGfhk1-GKOpnMJWvU4kIBGowSUfAELmk_B14,15083
-aac-0.1.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-aac-0.1.9.dist-info/entry_points.txt,sha256=FDaq5Vh3wL3K1byO7ho0LtiRpHg9vrr9mW0xECkmWxc,45
-aac-0.1.9.dist-info/top_level.txt,sha256=xOCuEGfR7nNuBR15J9eDu3CwMr8Rb2GEVL9HEilW1c4,4
-aac-0.1.9.dist-info/RECORD,,
+aac-0.2.0.dist-info/METADATA,sha256=T_XGUsdI6jpsqqf3qOXWc0SOJo4rAlKO1PkE4Xvh8lA,15070
+aac-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aac-0.2.0.dist-info/entry_points.txt,sha256=FDaq5Vh3wL3K1byO7ho0LtiRpHg9vrr9mW0xECkmWxc,45
+aac-0.2.0.dist-info/top_level.txt,sha256=xOCuEGfR7nNuBR15J9eDu3CwMr8Rb2GEVL9HEilW1c4,4
+aac-0.2.0.dist-info/RECORD,,
```

