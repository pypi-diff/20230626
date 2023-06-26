# Comparing `tmp/compliance-trestle-2.1.1.tar.gz` & `tmp/compliance-trestle-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compliance-trestle-2.1.1.tar", last modified: Fri May 12 18:07:56 2023, max compression
+gzip compressed data, was "compliance-trestle-2.2.0.tar", last modified: Mon Jun 26 21:32:06 2023, max compression
```

## Comparing `compliance-trestle-2.1.1.tar` & `compliance-trestle-2.2.0.tar`

### file list

```diff
@@ -1,1624 +1,1637 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.674946 compliance-trestle-2.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.470946 compliance-trestle-2.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.470946 compliance-trestle-2.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.github/ISSUE_TEMPLATE/new_collaborator.md
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.github/ISSUE_TEMPLATE/proposed_change.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.470946 compliance-trestle-2.1.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.github/PULL_REQUEST_TEMPLATE/develop.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.github/PULL_REQUEST_TEMPLATE/hotfix.md
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.github/PULL_REQUEST_TEMPLATE/other.md
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.github/PULL_REQUEST_TEMPLATE/release.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.github/dco.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.470946 compliance-trestle-2.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.github/workflows/conventional-pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.github/workflows/python-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.pylintrc_tests
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/.yapf-config
--rw-r--r--   0 runner    (1001) docker     (123)    90087 2023-05-12 18:07:54.000000 compliance-trestle-2.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/DCO1.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/MAINTAINERS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-12 18:07:56.674946 compliance-trestle-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.474946 compliance-trestle-2.1.1/compliance_trestle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-12 18:07:56.000000 compliance-trestle-2.1.1/compliance_trestle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    97038 2023-05-12 18:07:56.000000 compliance-trestle-2.1.1/compliance_trestle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:07:56.000000 compliance-trestle-2.1.1/compliance_trestle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 18:07:56.000000 compliance-trestle-2.1.1/compliance_trestle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-12 18:07:56.000000 compliance-trestle-2.1.1/compliance_trestle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 18:07:56.000000 compliance-trestle-2.1.1/compliance_trestle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.474946 compliance-trestle-2.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.498946 compliance-trestle-2.1.1/docs/api_reference/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.cli.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.common.common_types.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.common.const.md
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.common.err.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.common.file_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.common.list_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.common.load_validate.md
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.common.log.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.common.model_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.common.str_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.common.trash.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.common.type_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.all_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.base_model.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.catalog.catalog_api.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.catalog.catalog_interface.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.catalog.catalog_merger.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.catalog.catalog_reader.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.catalog.catalog_writer.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.catalog_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.add.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.assemble.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.author.catalog.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.author.command.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.author.common.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.author.component.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.author.consts.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.author.docs.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.author.folders.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.author.headers.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.author.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.author.profile.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.author.ssp.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.author.versioning.template_versioning.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.command_docs.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.common.cmd_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.common.return_codes.md
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.create.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.describe.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.href.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.import_.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.init.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.merge.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.partial_object_validate.md
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.remove.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.replicate.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.split.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.task.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.validate.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.commands.version.md
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.control_context.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.control_interface.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.control_reader.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.control_writer.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.docs_control_writer.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.draw_io.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.duplicates_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.generators.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.generic_oscal.md
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.links_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.markdown.base_markdown_node.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.markdown.control_markdown_node.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.markdown.docs_markdown_node.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.markdown.markdown_api.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.markdown.markdown_const.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.markdown.markdown_processor.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.markdown.markdown_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.markdown.md_writer.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.models.actions.md
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.models.elements.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.models.file_content_type.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.models.interfaces.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.models.plans.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.object_factory.md
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.parser.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.pipeline.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.profile_resolver.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.refs_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.remote.cache.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.repository.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.resolver.merge.md
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.resolver.modify.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.resolver.prune.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.rule_parameters_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.ssp_io.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.trestle_base_model.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.core.validator_factory.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.oscal.assessment_plan.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.oscal.assessment_results.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.oscal.catalog.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.oscal.common.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.oscal.component.md
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.oscal.poam.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.oscal.profile.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.oscal.ssp.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.tasks.base_task.md
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.tasks.cis_xlsx_to_oscal_catalog.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.tasks.csv_to_oscal_cd.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.tasks.ocp4_cis_profile_to_oscal_catalog.md
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.tasks.ocp4_cis_profile_to_oscal_cd.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.tasks.oscal_profile_to_osco_profile.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.tasks.osco_result_to_oscal_ar.md
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.tasks.tanium_result_to_oscal_ar.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.tasks.transform.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.tasks.xccdf_result_to_oscal_ar.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.tasks.xlsx_helper.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.tasks.xlsx_to_oscal_cd.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.tasks.xlsx_to_oscal_profile.md
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.transforms.implementations.osco.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.transforms.implementations.tanium.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.transforms.implementations.xccdf.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.transforms.results.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.transforms.transformer_factory.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.transforms.transformer_helper.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/api_reference/trestle.transforms.transformer_singleton.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.502946 compliance-trestle-2.1.1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   161907 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/assets/Canonical_trestle_auditree_workflows.png
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/assets/README
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/assets/canonical_trestle_auditree_workflows.drawio
--rw-r--r--   0 runner    (1001) docker     (123)   329379 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/assets/drawio_data_menu.png
--rw-r--r--   0 runner    (1001) docker     (123)   264094 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/assets/drawio_editing_data.png
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/assets/sample_ssp.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    44185 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/assets/template_versioning.png
--rw-r--r--   0 runner    (1001) docker     (123)    58223 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/cli.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.502946 compliance-trestle-2.1.1/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/contributing/DCO.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/contributing/mkdocs_contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/contributing/plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/contributing/trestle_oscal_object_model.md
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/contributing/website.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.502946 compliance-trestle-2.1.1/docs/css/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/demonstrations-content.md
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/errors.md
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/maintainers.md
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/mkdocs_code_of_conduct.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.502946 compliance-trestle-2.1.1/docs/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/plugins/compliance-trestle-fedramp.md
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/python_trestle_setup.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.502946 compliance-trestle-2.1.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)   146161 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.png
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/reference/third-party-result-schema-SCC.md
--rw-r--r--   0 runner    (1001) docker     (123)    26836 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/trestle_author.md
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/trestle_author_jinja.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.502946 compliance-trestle-2.1.1/docs/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.502946 compliance-trestle-2.1.1/docs/tutorials/continuous-compliance/
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/continuous-compliance/ContinuousCompliance.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    25984 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/continuous-compliance/ContinuousCompliance.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/continuous-compliance/continuous-compliance.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.506946 compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.png
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/profile_does.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    37208 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/profile_does.png
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.png
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    67327 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.png
--rw-r--r--   0 runner    (1001) docker     (123)    74265 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/ssp_profile_catalog_authoring.md
--rw-r--r--   0 runner    (1001) docker     (123)    23090 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/ssp_profile_options.docx
--rw-r--r--   0 runner    (1001) docker     (123)    44581 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/trestle_ssp_author_options.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.506946 compliance-trestle-2.1.1/docs/tutorials/task.csv-to-oscal-cd/
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.csv-to-oscal-cd/component-definition.json
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.csv-to-oscal-cd/demo-csv-to-oscal-cd.config
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.csv-to-oscal-cd/ocp4-sample-input.csv
--rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.csv-to-oscal-cd/transformation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.506946 compliance-trestle-2.1.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/demo-ocp4-cis-profile-to-oscal-catalog.config
--rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/transformation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.506946 compliance-trestle-2.1.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/demo-ocp4-cis-profile-to-oscal-cd.config
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/enabled_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/selected_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/transformation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.506946 compliance-trestle-2.1.1/docs/tutorials/task.tanium-result-to-oscal-ar/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.tanium-result-to-oscal-ar/800px-Australia_scarsdale_nimons_bridge.copyright-info.txt
--rw-r--r--   0 runner    (1001) docker     (123)   111352 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.tanium-result-to-oscal-ar/800px-Australia_scarsdale_nimons_bridge.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.tanium-result-to-oscal-ar/transformation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.506946 compliance-trestle-2.1.1/docs/tutorials/task.transformer-construction/
--rw-r--r--   0 runner    (1001) docker     (123)    56735 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.transformer-construction/assessment-results-nist.png
--rw-r--r--   0 runner    (1001) docker     (123)   100092 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.transformer-construction/assessment-results.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    43615 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.transformer-construction/assessment-results.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.transformer-construction/transformer-construction.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    28213 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.transformer-construction/transformer-construction.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/task.transformer-construction/transformer-construction.md
--rw-r--r--   0 runner    (1001) docker     (123)    27754 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/docs/tutorials/trestle_sample_workflow.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.506946 compliance-trestle-2.1.1/internal_spec_documents/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/internal_spec_documents/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/internal_spec_documents/caching_spec.md
--rw-r--r--   0 runner    (1001) docker     (123)    30894 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/internal_spec_documents/trestle-spec.md
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/internal_spec_documents/trestle-task-spec.md
--rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.510946 compliance-trestle-2.1.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/cleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.510946 compliance-trestle-2.1.1/scripts/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/experiments/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/experiments/json_serialize_ben.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/experiments/profile_json_seriallze_ben.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/experiments/profile_tanium_ben.sh
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/experiments/profiling_tools_setup_OSX.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/experiments/tanium_ben.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/flatten_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/gen_oscal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/have_files_changed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/order_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    35528 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/oscal_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/schema_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/simplify_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/simplify_retain_ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/tanium_transform_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/update_uuids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/utf8me.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/scripts/website_automation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-12 18:07:56.674946 compliance-trestle-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/sonar-project.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.510946 compliance-trestle-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.466946 compliance-trestle-2.1.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.510946 compliance-trestle-2.1.1/tests/data/author/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.446946 compliance-trestle-2.1.1/tests/data/author/0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.510946 compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/not_mxfile.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_extra_fields_compressed.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_missing_fields_compressed.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_metadata_compressed.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_metadata_uncompressed.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_bad_internal_structure.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_compressed.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed_mangled.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/two_tabs_metadata_compressed.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_bad_md.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_compressed.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.514946 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_1_md_format/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_1_md_format/bad_instance_bold_heading.md
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_1_md_format/bad_instance_heading_wrong_type.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_1_md_format/bad_instance_missing_heading.md
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_1_md_format/bad_instance_no_header.md
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_1_md_format/bad_instance_reordered.md
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_1_md_format/bad_instance_yaml_header_change.md
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_1_md_format/correct_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_1_md_format/correct_instance_extra_features.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_1_md_format/template.md
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_1_md_format/yaml_header_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.514946 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_2_md_with_md_header/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_2_md_with_md_header/bad_heading_content_changed_header.md
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_2_md_with_md_header/bad_heading_content_extra_lines.md
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_2_md_with_md_header/instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_2_md_with_md_header/template.md
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_2_md_with_md_header/wrong_heading_title.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.514946 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_3_md_hand_edited/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_000.md
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_001.md
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_002.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_3_md_hand_edited/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.514946 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_format_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_bold_heading.md
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_heading_wrong_type.md
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_missing_heading.md
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_reordered.md
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_yaml_header_change.md
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_format_extras/correct_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_format_extras/correct_instance_extra_features.md
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_format_extras/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.514946 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_substitutions/bad_added_header.md
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_substitutions/bad_modified_header_deep.md
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_substitutions/correct_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_substitutions/correct_instance_empty_subs.md
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_substitutions/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.518946 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_5_md_ignored/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_5_md_ignored/__ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_5_md_ignored/_ignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_5_md_ignored/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_5_md_ignored/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_5_md_ignored/correct_instance.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.518946 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/correct_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/0.0.1/test_5_md_ignored/template.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/bad_md_header.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.518946 compliance-trestle-2.1.1/tests/data/author/controls/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/controls/control_no_labels.md
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/controls/control_some_labels.md
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/controls/control_with_bad_component.md
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/controls/control_with_bad_system_comp.md
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/controls/control_with_components.md
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/controls/control_with_components_and_param_template.md
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/controls/control_with_components_and_params.md
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/controls/control_with_double_comp.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.450946 compliance-trestle-2.1.1/tests/data/author/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.518946 compliance-trestle-2.1.1/tests/data/author/docs/candidate_invalid_readme/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/docs/candidate_invalid_readme/correct_instance_extra_features.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/docs/candidate_invalid_readme/not_valid.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/docs/candidate_invalid_readme/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.518946 compliance-trestle-2.1.1/tests/data/author/docs/candidate_valid_readme/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/docs/candidate_valid_readme/correct_instance_extra_features.md
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/docs/candidate_valid_readme/correct_instance_extra_features_2.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/docs/candidate_valid_readme/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.518946 compliance-trestle-2.1.1/tests/data/author/docs/template_folder_invalid/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/docs/template_folder_invalid/extra_file.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/docs/template_folder_invalid/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/docs/template_folder_invalid/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.518946 compliance-trestle-2.1.1/tests/data/author/docs/template_folder_valid_with_readme/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/docs/template_folder_valid_with_readme/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/docs/template_folder_valid_with_readme/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.518946 compliance-trestle-2.1.1/tests/data/author/governed_folders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_folder_is_a_file
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.518946 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_bad_content/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_bad_content/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_bad_content/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.518946 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_missing/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_missing/architecture.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.518946 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_mixed_name/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_mixed_name/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_mixed_name/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.518946 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_no_header/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_no_header/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_no_header/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.518946 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_no_header/subdir/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_no_header/subdir/architecture.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.522946 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_renamed/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_renamed/architecture_really_bad.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_renamed/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.522946 compliance-trestle-2.1.1/tests/data/author/governed_folders/folder_with_bad_drawio/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/folder_with_bad_drawio/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/folder_with_bad_drawio/diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/folder_with_bad_drawio/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.522946 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.522946 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_limits_of_changes/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_limits_of_changes/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_limits_of_changes/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.522946 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_with_readme/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_with_readme/.hidden_test
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_with_readme/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_with_readme/network.md
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_with_readme/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.522946 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_with_version/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_with_version/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_with_version/diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_with_version/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.522946 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/__ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/_ignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/_ignore_not_instance.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/diagram.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.522946 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore_not_instance.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/architecture.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.522946 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/_ignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.522946 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_folder/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_folder/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_folder/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_folder_with_drawio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_folder_with_drawio/.hidden_does_not_affect
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_folder_with_drawio/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_folder_with_drawio/diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_folder_with_drawio/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_folder_with_version/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_folder_with_version/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_folder_with_version/diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_folder_with_version/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_with_readme/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_with_readme/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_with_readme/network.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/template_with_readme/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/governed_folders/utf16test_bad/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/utf16test_bad/sample.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/governed_folders/utf16test_good/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/governed_folders/utf16test_good/sample.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.454946 compliance-trestle-2.1.1/tests/data/author/headers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/bad_templates_drawio/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/bad_templates_drawio/template.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/bad_templates_drawio/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/bad_templates_md/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/bad_templates_md/template.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/bad_templates_md/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/bad_templates_wrong_names/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/bad_templates_wrong_names/templatesss.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/bad_templates_wrong_names/templatessss.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/empty_headers/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/empty_headers/a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/empty_headers/b copy.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/empty_headers/b.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_drawio/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_drawio/a_file.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_drawio/whos_is_this.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_drawio_bad_file/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_drawio_bad_file/a_markdown_file.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_drawio_bad_file/another_file.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_md/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_md/my_drawio.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_md/my_md.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_md_bad_file/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_md_bad_file/a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_md_bad_file/b.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.450946 compliance-trestle-2.1.1/tests/data/author/headers/global/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/global/good/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/good/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.450946 compliance-trestle-2.1.1/tests/data/author/headers/global/good/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/global/good/catalogs/my_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/good/catalogs/my_catalog/catalogs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/global/good/sample_indexable_1/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/good/sample_indexable_1/sample.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/global/good/sample_indexable_2/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/good/sample_indexable_2/sample.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/good/unindexed.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_exceptions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_exceptions/bad_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_exceptions/bad_sample/bad_sample.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.450946 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_exceptions/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.526946 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_exceptions/catalogs/my_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_exceptions/catalogs/my_catalog/catalogs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.530946 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_1/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_1/sample.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.530946 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_2/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_2/sample.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_exceptions/unindexed.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.530946 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_nested_exceptions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.450946 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_nested_exceptions/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.530946 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_nested_exceptions/catalogs/my_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_nested_exceptions/catalogs/my_catalog/catalogs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.530946 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_nested_exceptions/nested/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.530946 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_nested_exceptions/nested/bad/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_nested_exceptions/nested/bad/bad_sample.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.530946 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_nested_exceptions/nested/good/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_nested_exceptions/nested/good/sample.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_nested_exceptions/nested/sample.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.530946 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_nested_exceptions/sample_indexable_1/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_nested_exceptions/sample_indexable_1/sample.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/global/pass_with_nested_exceptions/unindexed.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.530946 compliance-trestle-2.1.1/tests/data/author/headers/good_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/good_templates/template.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/good_templates/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.530946 compliance-trestle-2.1.1/tests/data/author/headers/good_templates_wo_drawio/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/good_templates_wo_drawio/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.530946 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/__ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/_ignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/_ignore_not_instance.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/correct_a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/correct_b.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/correct_instance.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.530946 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/deep/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/deep/_ignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/deep/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/deep/_ignore_not_instance.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/deep/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/deep/correct_instance.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.530946 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/deep/even_deeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/deep/even_deeper/_ignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/deep/even_deeper/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/deep/even_deeper/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/deep/even_deeper/correct_a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/deep/even_deeper/correct_instance.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.530946 compliance-trestle-2.1.1/tests/data/author/headers/meets_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/meets_templates/a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/meets_templates/b.md
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/meets_templates/d.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.534946 compliance-trestle-2.1.1/tests/data/author/headers/passes_with_extraneous_files/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/passes_with_extraneous_files/a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/passes_with_extraneous_files/b.md
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/passes_with_extraneous_files/d.drawio
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/passes_with_extraneous_files/irrelevant.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.534946 compliance-trestle-2.1.1/tests/data/author/headers/recursive_pass/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/recursive_pass/a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/recursive_pass/b copy.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/recursive_pass/b.md
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/recursive_pass/d.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.534946 compliance-trestle-2.1.1/tests/data/author/headers/recursive_pass/some_depth/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/recursive_pass/some_depth/a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/recursive_pass/some_depth/b copy.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/recursive_pass/some_depth/b.md
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/headers/recursive_pass/some_depth/d.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.534946 compliance-trestle-2.1.1/tests/data/author/ssp/
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/ssp/ssp_example.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.534946 compliance-trestle-2.1.1/tests/data/author/utf16test/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/utf16test/sample_okay.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/utf16test/sample_utf16.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.534946 compliance-trestle-2.1.1/tests/data/author/versions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.534946 compliance-trestle-2.1.1/tests/data/author/versions/1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/versions/1.0.0/bad_template_wrong_folder.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/versions/1.0.0/good_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.534946 compliance-trestle-2.1.1/tests/data/author/versions/1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/versions/1.1.0/bad_instance_mismatched_versions.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/versions/1.1.0/bad_template_mismatched_versions.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/versions/1.1.0/good_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/versions/1.1.0/good_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/versions/bad_template_with_version_outside_structure.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/author/versions/good_instance_with_version_outside_structure.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.534946 compliance-trestle-2.1.1/tests/data/csv/
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/csv/bp.sample.v2.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.454946 compliance-trestle-2.1.1/tests/data/csv/component-definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.534946 compliance-trestle-2.1.1/tests/data/csv/component-definitions/bp/
--rw-r--r--   0 runner    (1001) docker     (123)    42744 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/csv/component-definitions/bp/component-definition.json
--rw-r--r--   0 runner    (1001) docker     (123)    54973 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/csv/ocp4-user.v2.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.534946 compliance-trestle-2.1.1/tests/data/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja/lookup_table.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja/profile_to_docs.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja/profile_to_docs_invalid.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja/profile_to_docs_only_some_sections.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja/profile_to_docs_with_group_title.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja/profile_to_docs_with_subparts.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja/ssp_template.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja/ssp_template_no_input_profile_ssp.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja/sub_content.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja/sub_content_with_subs.md
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja/use_lookup_table.md.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.538946 compliance-trestle-2.1.1/tests/data/jinja_cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_cmd/empty_test.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_cmd/number_captions_data.md
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_cmd/number_captions_expected_output.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.538946 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/MDDatestamp_default.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/MDDatestamp_format.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/MDDatestamp_invalid.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/MDDatestamp_newline.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/MDSection_include_nested.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/MDSection_include_nested.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/MDSection_include_top_level.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/MDSection_include_top_level.md
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/MDSection_include_top_level_adjusted.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/MDSection_include_top_level_adjusted.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/env_include.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/env_include.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/env_include_adjusted.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/env_include_adjusted.md
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/env_nested_c_c.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/env_nested_c_c.md
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/env_nested_c_c_double.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/env_nested_c_c_double.md
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/env_nested_c_n.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/env_nested_c_n.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/nested_c.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/nested_n.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/jinja_markdown_include/test_markdown.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.546946 compliance-trestle-2.1.1/tests/data/json/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/bad_simple.json
--rw-r--r--   0 runner    (1001) docker     (123)    21655 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/comp_def.json
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/comp_def_a.json
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/comp_def_b.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/comp_def_readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/comp_prof.json
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/comp_prof_aa.json
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/comp_prof_ab.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/comp_prof_ba.json
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/comp_prof_bad.json
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/comp_prof_bb.json
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/good_simple.json
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/minimal_catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/minimal_catalog_bad_oscal_version.json
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/minimal_catalog_extra_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/minimal_catalog_missing_roles.json
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/minimal_catalog_missing_uuid.json
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/minimal_catalog_no_responsible-parties.json
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/minimal_catalog_roles.json
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/minimal_catalog_roles_double.json
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/minimal_catalog_roles_double_rp.json
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/minimal_catalog_with_groups.json
--rw-r--r--   0 runner    (1001) docker     (123)    16376 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/nist_tutorial_catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/nist_tutorial_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/profile_bad_control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/profile_missing_position.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/profile_with_alter_props.json
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/profile_with_alter_subparts.json
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/profile_with_incorrect_alter.json
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/pull_nist_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/simple_catalog_no_parts.json
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/simple_mapping.json
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/simple_test_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/simple_test_profile_no_params.json
--rw-r--r--   0 runner    (1001) docker     (123)   221136 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/simplified_nist_catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/simplified_nist_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/test_profile_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/test_profile_b.json
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/test_profile_c.json
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/test_profile_d.json
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/test_profile_e.json
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/test_profile_f.json
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/json/test_profile_g.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.546946 compliance-trestle-2.1.1/tests/data/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/markdown/valid_complex_md.md
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/markdown/valid_levels_no_text.md
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/markdown/valid_levels_no_text_increased_level.md
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/markdown/valid_no_headers.md
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/markdown/valid_no_lvl1_headers.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.546946 compliance-trestle-2.1.1/tests/data/ocp4-cis/
--rw-r--r--   0 runner    (1001) docker     (123)    23806 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/ocp4-cis/catalog.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.546946 compliance-trestle-2.1.1/tests/data/split_merge/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.546946 compliance-trestle-2.1.1/tests/data/split_merge/.trestle/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/.trestle/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.550946 compliance-trestle-2.1.1/tests/data/split_merge/load_distributed/
--rw-r--r--   0 runner    (1001) docker     (123)  3169371 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/load_distributed/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/load_distributed/groups.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.554946 compliance-trestle-2.1.1/tests/data/split_merge/step0-merged_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.454946 compliance-trestle-2.1.1/tests/data/split_merge/step0-merged_catalog/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.554946 compliance-trestle-2.1.1/tests/data/split_merge/step0-merged_catalog/catalogs/mycatalog/
--rw-r--r--   0 runner    (1001) docker     (123)  4498050 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step0-merged_catalog/catalogs/mycatalog/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step0-merged_catalog/next_step.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.558946 compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.454946 compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.558946 compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.562946 compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/back-matter.json
--rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/groups.json
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/next_step.sh
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/previous_step.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.562946 compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.454946 compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.562946 compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.566946 compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/back-matter.json
--rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/groups.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.566946 compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/parties.json
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/responsible-parties.json
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/roles.json
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/next_step.sh
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/previous_step.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.566946 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.454946 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.566946 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.570946 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/back-matter.json
--rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/groups.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.570946 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/parties.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.570946 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties/00000__responsible-party.json
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties/00001__responsible-party.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.570946 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles/00000__role.json
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles/00001__role.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles.json
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/next_step.sh
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/previous_step.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.570946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.454946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.570946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.574946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/back-matter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.574946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.454946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.578946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    48380 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    54960 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    70506 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    26470 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00014__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    30598 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00015__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    22931 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00016__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00017__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00018__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    18970 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00019__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00020__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00021__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00022__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00023__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00024__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.454946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.578946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    18701 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.582946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    18060 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    15966 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00014__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00015__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.582946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    24785 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.582946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    27281 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    15190 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    34660 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    28847 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.586946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    29166 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    14993 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13963 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    21335 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.586946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    29620 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    51627 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.586946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    38793 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.590946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.590946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    18885 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.594946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    24929 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00014__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00015__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00016__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00017__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00018__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00019__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00020__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00021__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00022__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.594946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    22272 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.598946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00014__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00015__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00016__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00017__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00018__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00019__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00020__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00021__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00022__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00023__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00024__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00025__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00026__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00027__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00028__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00029__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00030__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00031__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.598946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.598946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.602946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    30706 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.602946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    42212 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)   101326 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    25087 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    34032 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    32683 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00014__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00015__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    37819 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00016__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00017__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00018__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00019__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00020__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00021__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00022__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.610946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    72606 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00014__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00015__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00016__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00017__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00018__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00019__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00020__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00021__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00022__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00023__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00024__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00025__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00026__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00027__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00028__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00029__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00030__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00031__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00032__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00033__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00034__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00035__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00036__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00037__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00038__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00039__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00040__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00041__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00042__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00043__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00044__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00045__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00046__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00047__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00048__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00049__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00050__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.614946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    26554 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    67388 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    36771 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00014__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00015__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00016__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00017__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00018__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00019__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00020__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00021__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00022__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.614946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.614946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/parties.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.614946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/responsible-parties/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/responsible-parties/00000__responsible-party.json
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/responsible-parties/00001__responsible-party.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.614946 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/roles/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/roles/00000__role.json
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/roles/00001__role.json
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/next_step.sh
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/previous_step.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/spread-sheet/
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/spread-sheet/bad_parameter_name_and_description.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/spread-sheet/duplicate_column_heading.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/spread-sheet/embedded_blank_in_goal_name_id.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/spread-sheet/embedded_blank_in_parameter_name.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/spread-sheet/embedded_blank_in_rule_name_id.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/spread-sheet/good.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/spread-sheet/good_with_blank_rows.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/spread-sheet/missing_column_heading.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/spread-sheet/missing_control_id.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/spread-sheet/missing_resource_title.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/spread-sheet/missing_rule_name_id.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.466946 compliance-trestle-2.1.1/tests/data/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/cis-xlsx-to-oscal-catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_RedHat_OpenShift_Container_Platform_Benchmark_v1.2.0-2.snippet.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_Red_Hat_Enterprise_Linux_8_Benchmark_v2.0.0.snippet.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/cis-xlsx-to-oscal-catalog/test-cis-xlsx-to-oscal-catalog.ocp.config
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/cis-xlsx-to-oscal-catalog/test-cis-xlsx-to-oscal-catalog.rhel.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/csv-to-oscal-cd/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/csv-to-oscal-cd/test-csv-to-oscal-cd-bp.config
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/csv-to-oscal-cd/test-csv-to-oscal-cd.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input/cis.profile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input-bogus/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input-bogus/cis.profile
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/test-ocp4-cis-profile-to-oscal-catalog.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.458946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.462946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_cni_conf/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_cni_conf/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_apiserver/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_controller_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_controller_manager/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_cni_conf/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_cni_conf/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_apiserver/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_controller_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_controller_manager/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_apiserver/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_controller_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_controller_manager/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_memory_available/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_memory_available/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_nodefs_available/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_nodefs_available/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules2.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules3.json
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/rule2var.json
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/output/
--rw-r--r--   0 runner    (1001) docker     (123)    20254 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/output/component-definition.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.462946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.462946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.618946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis-node.profile
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis.profile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.622946 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test.profile
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test2.profile
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test3.profile
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd.config
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd2.config
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd3.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.622946 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.622946 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-no.json
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-yes.json
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-no.json
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-yes.json
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.2.0-parms-no.json
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-1.0.0-parms-yes.json
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-no.json
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-yes.json
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-scc.json
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.39-parms-no.config
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.39-parms-yes.config
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.40-parms-no.config
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.40-parms-yes.config
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.2.0-parms-no.config
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-1.0.0-parms-yes.config
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-bogus.config
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-no-input-file.config
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-no-output-dir.config
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-no-overwrite.config
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-parms-no.config
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-parms-yes.config
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-scc.config
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-set.config
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.462946 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.622946 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.622946 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-no/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-no/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.622946 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-yes/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-yes/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.622946 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-no/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-no/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.622946 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-yes/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-yes/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.622946 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.2.0-parms-no/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.2.0-parms-no/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.626946 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-1.0.0-parms-yes/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-1.0.0-parms-yes/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.626946 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-no/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-no/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.626946 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-yes/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-yes/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.626946 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-scc/
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-scc/tailored-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.622946 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output-set/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output-set/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.626946 compliance-trestle-2.1.1/tests/data/tasks/osco/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.626946 compliance-trestle-2.1.1/tests/data/tasks/osco/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/input/ignore.me
--rw-r--r--   0 runner    (1001) docker     (123)    52753 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/input/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.626946 compliance-trestle-2.1.1/tests/data/tasks/osco/input-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    52859 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/input-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.626946 compliance-trestle-2.1.1/tests/data/tasks/osco/input-bad-yaml/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/input-bad-yaml/bad.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.626946 compliance-trestle-2.1.1/tests/data/tasks/osco/input-compressed/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/input-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.626946 compliance-trestle-2.1.1/tests/data/tasks/osco/input-configmaps/
--rw-r--r--   0 runner    (1001) docker     (123)   608191 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/input-configmaps/configmaps.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.626946 compliance-trestle-2.1.1/tests/data/tasks/osco/input-fetcher/
--rw-r--r--   0 runner    (1001) docker     (123)   105678 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/input-fetcher/cluster_resource.json
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_resources.json
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.626946 compliance-trestle-2.1.1/tests/data/tasks/osco/input-xml-ocp4/
--rw-r--r--   0 runner    (1001) docker     (123)    78761 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/input-xml-ocp4/ocp4-check-result.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.626946 compliance-trestle-2.1.1/tests/data/tasks/osco/input-xml-rhel7/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/input-xml-rhel7/rhel7-check-result.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.630946 compliance-trestle-2.1.1/tests/data/tasks/osco/output/
--rw-r--r--   0 runner    (1001) docker     (123)   155263 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.630946 compliance-trestle-2.1.1/tests/data/tasks/osco/output-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)   155462 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.630946 compliance-trestle-2.1.1/tests/data/tasks/osco/output-compressed/
--rw-r--r--   0 runner    (1001) docker     (123)   155263 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.630946 compliance-trestle-2.1.1/tests/data/tasks/osco/output-configmaps/
--rw-r--r--   0 runner    (1001) docker     (123)  1870504 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/output-configmaps/configmaps.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.630946 compliance-trestle-2.1.1/tests/data/tasks/osco/output-fetcher/
--rw-r--r--   0 runner    (1001) docker     (123)   366829 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/output-fetcher/cluster_resource.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/output-fetcher/cluster_resource_no_data.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/output-fetcher/cluster_resource_no_kind0.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/output-fetcher/cluster_resource_no_kind1.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/output-fetcher/cluster_resource_no_resources.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/output-fetcher/cluster_resource_no_results.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.630946 compliance-trestle-2.1.1/tests/data/tasks/osco/output-xml-ocp4/
--rw-r--r--   0 runner    (1001) docker     (123)   273677 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/output-xml-ocp4/ocp4-check-result.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.634946 compliance-trestle-2.1.1/tests/data/tasks/osco/output-xml-rhel7/
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/output-xml-rhel7/rhel7-check-result.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar-1.3.5.config
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar-bad-yaml.config
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar-compressed.config
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar-configmaps.config
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar-fetcher.config
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar-xml-ocp4.config
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar-xml-rhel7.config
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.634946 compliance-trestle-2.1.1/tests/data/tasks/tanium/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/tanium/demo-tanium-result-to-oscal-ar.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.634946 compliance-trestle-2.1.1/tests/data/tasks/tanium/input/
--rw-r--r--   0 runner    (1001) docker     (123)   314329 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/tanium/input/Tanium.comply-results-json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.634946 compliance-trestle-2.1.1/tests/data/tasks/tanium/input-bad/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/tanium/input-bad/Tanium.comply-results-bad
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.634946 compliance-trestle-2.1.1/tests/data/tasks/tanium/input-doc/
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/tanium/input-doc/Tanium.doc-json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.634946 compliance-trestle-2.1.1/tests/data/tasks/tanium/output/
--rw-r--r--   0 runner    (1001) docker     (123)  1997259 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/tanium/output/Tanium.oscal.2020.json
--rw-r--r--   0 runner    (1001) docker     (123)  1997259 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/tanium/output/Tanium.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.638946 compliance-trestle-2.1.1/tests/data/tasks/xccdf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.638946 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output/
--rw-r--r--   0 runner    (1001) docker     (123)   157229 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.638946 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)   157432 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.638946 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-compressed/
--rw-r--r--   0 runner    (1001) docker     (123)   157229 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.638946 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-configmaps/
--rw-r--r--   0 runner    (1001) docker     (123)  1891646 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-configmaps/configmaps.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.642946 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-fetcher/
--rw-r--r--   0 runner    (1001) docker     (123)   371515 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-fetcher/cluster_resource.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_data.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_kind0.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_kind1.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_resources.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_results.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.642946 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-xml-ocp4/
--rw-r--r--   0 runner    (1001) docker     (123)   276795 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-xml-ocp4/ocp4-check-result.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.642946 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-xml-rhel7/
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-xml-rhel7/rhel7-check-result.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-1.3.5.config
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-bad-yaml.config
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-compressed.config
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-configmaps.config
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-fetcher.config
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-xml-ocp4.config
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-xml-rhel7.config
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.642946 compliance-trestle-2.1.1/tests/data/tasks/xlsx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.642946 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output/
--rw-r--r--   0 runner    (1001) docker     (123)    67226 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output/component-definition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output/profile.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.642946 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-by-check/
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-by-check/profile.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.642946 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-by-control/
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-by-control/profile.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.642946 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-by-rule/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-by-rule/profile.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.642946 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-filtered/
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-filtered/profile.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.642946 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-missing-control-id/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-missing-control-id/profile.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.642946 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-missing-rule-name-id/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-missing-rule-name-id/profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xlsx/test-xlsx-to-oscal-cd.config
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/tasks/xlsx/test-xlsx-to-oscal-profile.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.646946 compliance-trestle-2.1.1/tests/data/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)    99263 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/yaml/bad_component_dup_uuid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    99257 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/yaml/bad_component_no_tz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/yaml/bad_simple.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    99263 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/yaml/good_component.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    99263 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/yaml/good_component_diff_tz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/yaml/good_simple.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/data/yaml/header_with_metadata.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.646946 compliance-trestle-2.1.1/tests/functionality/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/functionality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/functionality/chevron_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/functionality/example_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/functionality/pathlib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.646946 compliance-trestle-2.1.1/tests/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/manual_tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/manual_tests/split_test_1.sh
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/manual_tests/split_test_issue_630.sh
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/manual_tests/split_validate_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1362 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/manual_tests/test_binary.sh
--rw-r--r--   0 runner    (1001) docker     (123)    25661 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.646946 compliance-trestle-2.1.1/tests/trestle/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/cli_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.646946 compliance-trestle-2.1.1/tests/trestle/core/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/base_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.650946 compliance-trestle-2.1.1/tests/trestle/core/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/add_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/assemble_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.650946 compliance-trestle-2.1.1/tests/trestle/core/commands/author/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/author/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/author/catalog_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/author/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/author/component_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    29859 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/author/docs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24635 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/author/folders_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20612 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/author/headers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12791 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/author/jinja_cmd_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    44627 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/author/profile_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    29613 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/author/ssp_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.650946 compliance-trestle-2.1.1/tests/trestle/core/commands/author/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/author/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/author/versioning/template_versioning_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/cmd_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/create_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/describe_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/href_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/import__test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/init_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/merge_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/partial_object_validate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/remove_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/replicate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/split_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/task_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18571 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/validate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/commands/version_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/control_io_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/draw_io_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/err_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/jinja_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.650946 compliance-trestle-2.1.1/tests/trestle/core/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/markdown/markdown_node_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17571 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/markdown/markdown_validator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.654946 compliance-trestle-2.1.1/tests/trestle/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/models/create_path_action_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/models/element_path_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/models/element_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/models/file_content_type_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/models/interfaces_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/models/plans_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/models/remove_action_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/models/remove_path_action_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/models/update_action_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/models/write_action_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/models/write_file_action_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21160 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/profile_resolver_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.654946 compliance-trestle-2.1.1/tests/trestle/core/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15089 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/remote/cache_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/repository_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/ssp_io_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/core/validator_helper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.654946 compliance-trestle-2.1.1/tests/trestle/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/parsing/parsing_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.654946 compliance-trestle-2.1.1/tests/trestle/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/tasks/base_task_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/tasks/cis_xlsx_to_oscal_catalog_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    46119 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/tasks/csv_to_oscal_cd_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/tasks/ocp4_cis_profile_to_oscal_catalog_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/tasks/ocp4_cis_profile_to_oscal_cd_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/tasks/oscal_profile_to_osco_profile_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/tasks/osco_result_to_oscal_ar_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15849 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/tasks/tanium_result_to_oscal_ar_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/tasks/transform_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/tasks/xccdf_result_to_oscal_ar_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/tasks/xlsx_to_oscal_cd_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/tasks/xlsx_to_oscal_profile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.654946 compliance-trestle-2.1.1/tests/trestle/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/transforms/transformer_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/transforms/transformer_helper_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.654946 compliance-trestle-2.1.1/tests/trestle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29420 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/utils/fs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/utils/list_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/utils/load_distributed_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/utils/md_writer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/tests/trestle/utils/trash_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.658946 compliance-trestle-2.1.1/trestle/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-12 18:07:54.000000 compliance-trestle-2.1.1/trestle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.658946 compliance-trestle-2.1.1/trestle/common/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/common/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16924 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/common/err.py
--rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/common/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/common/list_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/common/load_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/common/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    44383 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/common/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/common/str_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/common/trash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/common/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.662946 compliance-trestle-2.1.1/trestle/core/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/all_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.662946 compliance-trestle-2.1.1/trestle/core/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/catalog/catalog_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42306 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/catalog/catalog_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/catalog/catalog_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/catalog/catalog_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    22324 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/catalog/catalog_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/catalog_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.662946 compliance-trestle-2.1.1/trestle/core/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/assemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.666946 compliance-trestle-2.1.1/trestle/core/commands/author/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/author/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/author/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/author/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/author/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16138 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/author/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/author/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/author/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/author/folders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/author/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14168 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/author/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)    24848 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/author/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    41371 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/author/ssp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.666946 compliance-trestle-2.1.1/trestle/core/commands/author/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/author/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/author/versioning/template_versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/command_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.666946 compliance-trestle-2.1.1/trestle/core/commands/common/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/common/cmd_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/common/return_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/describe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/href.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/partial_object_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/replicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    22026 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/split.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/control_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    49620 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/control_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    23766 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/control_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    28904 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/control_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/docs_control_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/draw_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/duplicates_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    20080 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/generic_oscal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/links_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.666946 compliance-trestle-2.1.1/trestle/core/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/markdown/base_markdown_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    28079 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/markdown/control_markdown_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/markdown/docs_markdown_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/markdown/markdown_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/markdown/markdown_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/markdown/markdown_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/markdown/markdown_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/markdown/md_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.666946 compliance-trestle-2.1.1/trestle/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16242 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/models/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25162 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/models/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/models/file_content_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/models/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/models/plans.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/profile_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/refs_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.670946 compliance-trestle-2.1.1/trestle/core/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20205 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/remote/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16329 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.670946 compliance-trestle-2.1.1/trestle/core/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/resolver/_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/resolver/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    16076 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/resolver/modify.py
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/resolver/prune.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/rule_parameters_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/ssp_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/trestle_base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/core/validator_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.670946 compliance-trestle-2.1.1/trestle/oscal/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/oscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26369 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/oscal/assessment_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    35188 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/oscal/assessment_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/oscal/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    80055 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/oscal/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/oscal/component.py
--rw-r--r--   0 runner    (1001) docker     (123)    26943 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/oscal/poam.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/oscal/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/oscal/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37519 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/oscal/ssp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.670946 compliance-trestle-2.1.1/trestle/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/resources/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.670946 compliance-trestle-2.1.1/trestle/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/resources/templates/FedRAMP_control_header_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/resources/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/resources/templates/template.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/resources/templates/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.674946 compliance-trestle-2.1.1/trestle/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/tasks/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    18021 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/tasks/cis_xlsx_to_oscal_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    63140 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/tasks/csv_to_oscal_cd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/tasks/ocp4_cis_profile_to_oscal_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    25634 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/tasks/ocp4_cis_profile_to_oscal_cd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/tasks/oscal_profile_to_osco_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/tasks/osco_result_to_oscal_ar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/tasks/tanium_result_to_oscal_ar.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/tasks/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/tasks/xccdf_result_to_oscal_ar.py
--rw-r--r--   0 runner    (1001) docker     (123)    23198 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/tasks/xlsx_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17402 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/tasks/xlsx_to_oscal_cd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/tasks/xlsx_to_oscal_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.674946 compliance-trestle-2.1.1/trestle/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:07:56.674946 compliance-trestle-2.1.1/trestle/transforms/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/transforms/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28870 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/transforms/implementations/osco.py
--rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/transforms/implementations/tanium.py
--rw-r--r--   0 runner    (1001) docker     (123)    23496 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/transforms/implementations/xccdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/transforms/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/transforms/transformer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/transforms/transformer_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-12 18:05:01.000000 compliance-trestle-2.1.1/trestle/transforms/transformer_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.585586 compliance-trestle-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.265584 compliance-trestle-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.265584 compliance-trestle-2.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/ISSUE_TEMPLATE/new_collaborator.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/ISSUE_TEMPLATE/proposed_change.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.265584 compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE/develop.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE/hotfix.md
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE/other.md
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE/release.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/dco.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.269584 compliance-trestle-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/workflows/conventional-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/workflows/python-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.pylintrc_tests
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.yapf-config
+-rw-r--r--   0 runner    (1001) docker     (123)    92397 2023-06-26 21:32:03.000000 compliance-trestle-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/DCO1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-06-26 21:32:06.585586 compliance-trestle-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.269584 compliance-trestle-2.2.0/compliance_trestle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-06-26 21:32:06.000000 compliance-trestle-2.2.0/compliance_trestle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    97672 2023-06-26 21:32:06.000000 compliance-trestle-2.2.0/compliance_trestle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:32:06.000000 compliance-trestle-2.2.0/compliance_trestle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:32:06.000000 compliance-trestle-2.2.0/compliance_trestle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-26 21:32:06.000000 compliance-trestle-2.2.0/compliance_trestle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 21:32:06.000000 compliance-trestle-2.2.0/compliance_trestle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.269584 compliance-trestle-2.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.289584 compliance-trestle-2.2.0/docs/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.common_types.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.const.md
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.err.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.file_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.list_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.load_validate.md
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.log.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.model_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.str_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.trash.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.type_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.all_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.base_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.catalog.catalog_api.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.catalog.catalog_interface.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.catalog.catalog_merger.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.catalog.catalog_reader.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.catalog.catalog_writer.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.catalog_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.add.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.assemble.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.catalog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.command.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.common.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.component.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.consts.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.docs.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.folders.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.headers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.profile.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.ssp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.versioning.template_versioning.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.command_docs.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.common.cmd_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.common.return_codes.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.create.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.describe.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.href.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.import_.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.init.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.merge.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.partial_object_validate.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.remove.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.replicate.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.split.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.task.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.validate.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.version.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.control_context.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.control_interface.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.control_reader.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.control_writer.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.docs_control_writer.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.draw_io.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.duplicates_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.generators.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.generic_oscal.md
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.links_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.base_markdown_node.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.control_markdown_node.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.docs_markdown_node.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.markdown_api.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.markdown_const.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.markdown_processor.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.markdown_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.md_writer.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.models.actions.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.models.elements.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.models.file_content_type.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.models.interfaces.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.models.plans.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.object_factory.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.parser.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.profile_resolver.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.refs_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.remote.cache.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.repository.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.resolver.merge.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.resolver.modify.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.resolver.prune.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.rule_parameters_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.ssp_io.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.trestle_base_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.validator_factory.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.assessment_plan.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.assessment_results.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.catalog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.common.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.component.md
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.poam.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.profile.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.ssp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.base_task.md
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.cis_xlsx_to_oscal_catalog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.csv_to_oscal_cd.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.ocp4_cis_profile_to_oscal_catalog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.ocp4_cis_profile_to_oscal_cd.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.oscal_catalog_to_csv.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.oscal_profile_to_osco_profile.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.osco_result_to_oscal_ar.md
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.tanium_result_to_oscal_ar.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.transform.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.xccdf_result_to_oscal_ar.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.xlsx_helper.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.xlsx_to_oscal_cd.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.xlsx_to_oscal_profile.md
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.transforms.implementations.osco.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.transforms.implementations.tanium.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.transforms.implementations.xccdf.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.transforms.results.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.transforms.transformer_factory.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.transforms.transformer_helper.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.transforms.transformer_singleton.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.289584 compliance-trestle-2.2.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   161907 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/assets/Canonical_trestle_auditree_workflows.png
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/assets/README
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/assets/canonical_trestle_auditree_workflows.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)   329379 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/assets/drawio_data_menu.png
+-rw-r--r--   0 runner    (1001) docker     (123)   264094 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/assets/drawio_editing_data.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/assets/sample_ssp.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    44185 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/assets/template_versioning.png
+-rw-r--r--   0 runner    (1001) docker     (123)    58223 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/cli.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.289584 compliance-trestle-2.2.0/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/contributing/DCO.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/contributing/mkdocs_contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/contributing/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/contributing/trestle_oscal_object_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/contributing/website.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.289584 compliance-trestle-2.2.0/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/demonstrations-content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/errors.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/maintainers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/mkdocs_code_of_conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.289584 compliance-trestle-2.2.0/docs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/plugins/compliance-trestle-fedramp.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/python_trestle_setup.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.293584 compliance-trestle-2.2.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)   146161 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/reference/third-party-result-schema-SCC.md
+-rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/trestle_author.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/trestle_author_jinja.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.293584 compliance-trestle-2.2.0/docs/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.293584 compliance-trestle-2.2.0/docs/tutorials/continuous-compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/continuous-compliance/ContinuousCompliance.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    25984 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/continuous-compliance/ContinuousCompliance.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/continuous-compliance/continuous-compliance.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.293584 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/profile_does.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    37208 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/profile_does.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    67327 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76787 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/ssp_profile_catalog_authoring.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/ssp_profile_options.docx
+-rw-r--r--   0 runner    (1001) docker     (123)    75117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/trestle_ssp_author_options.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.293584 compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/component-definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/demo-csv-to-oscal-cd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/ocp4-sample-input.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/transformation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.297584 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/demo-ocp4-cis-profile-to-oscal-catalog.config
+-rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/transformation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.297584 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/demo-ocp4-cis-profile-to-oscal-cd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/enabled_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/selected_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/transformation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.297584 compliance-trestle-2.2.0/docs/tutorials/task.tanium-result-to-oscal-ar/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.tanium-result-to-oscal-ar/800px-Australia_scarsdale_nimons_bridge.copyright-info.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   111352 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.tanium-result-to-oscal-ar/800px-Australia_scarsdale_nimons_bridge.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.tanium-result-to-oscal-ar/transformation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.297584 compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/
+-rw-r--r--   0 runner    (1001) docker     (123)    56735 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/assessment-results-nist.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100092 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/assessment-results.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    43615 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/assessment-results.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/transformer-construction.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    28213 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/transformer-construction.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/transformer-construction.md
+-rw-r--r--   0 runner    (1001) docker     (123)    27754 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/trestle_sample_workflow.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.297584 compliance-trestle-2.2.0/internal_spec_documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/internal_spec_documents/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/internal_spec_documents/caching_spec.md
+-rw-r--r--   0 runner    (1001) docker     (123)    30894 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/internal_spec_documents/trestle-spec.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/internal_spec_documents/trestle-task-spec.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.301584 compliance-trestle-2.2.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.301584 compliance-trestle-2.2.0/scripts/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/experiments/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/experiments/json_serialize_ben.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/experiments/profile_json_seriallze_ben.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/experiments/profile_tanium_ben.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/experiments/profiling_tools_setup_OSX.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/experiments/tanium_ben.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/flatten_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/gen_oscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/have_files_changed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/order_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35528 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/oscal_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/schema_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/simplify_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/simplify_retain_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/tanium_transform_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/update_uuids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/utf8me.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/website_automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-26 21:32:06.585586 compliance-trestle-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/sonar-project.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.301584 compliance-trestle-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.261583 compliance-trestle-2.2.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.301584 compliance-trestle-2.2.0/tests/data/author/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.237583 compliance-trestle-2.2.0/tests/data/author/0.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.305584 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/not_mxfile.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_extra_fields_compressed.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_missing_fields_compressed.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_metadata_compressed.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_metadata_uncompressed.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_bad_internal_structure.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_compressed.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed_mangled.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/two_tabs_metadata_compressed.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_bad_md.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_compressed.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.305584 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/bad_instance_bold_heading.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/bad_instance_heading_wrong_type.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/bad_instance_missing_heading.md
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/bad_instance_no_header.md
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/bad_instance_reordered.md
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/bad_instance_yaml_header_change.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/correct_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/correct_instance_extra_features.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/template.md
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/yaml_header_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.305584 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_2_md_with_md_header/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_2_md_with_md_header/bad_heading_content_changed_header.md
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_2_md_with_md_header/bad_heading_content_extra_lines.md
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_2_md_with_md_header/instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_2_md_with_md_header/template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_2_md_with_md_header/wrong_heading_title.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.305584 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_000.md
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_001.md
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_002.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.309584 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_bold_heading.md
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_heading_wrong_type.md
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_missing_heading.md
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_reordered.md
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_yaml_header_change.md
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/correct_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/correct_instance_extra_features.md
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.309584 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_substitutions/bad_added_header.md
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_substitutions/bad_modified_header_deep.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_substitutions/correct_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_substitutions/correct_instance_empty_subs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_substitutions/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.309584 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/__ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/correct_instance.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.309584 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/correct_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/template.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/bad_md_header.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.309584 compliance-trestle-2.2.0/tests/data/author/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_no_labels.md
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_some_labels.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_with_bad_component.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_with_bad_system_comp.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_with_components.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_with_components_and_param_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_with_components_and_params.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_with_double_comp.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.237583 compliance-trestle-2.2.0/tests/data/author/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/docs/candidate_invalid_readme/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/candidate_invalid_readme/correct_instance_extra_features.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/candidate_invalid_readme/not_valid.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/candidate_invalid_readme/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/docs/candidate_valid_readme/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/candidate_valid_readme/correct_instance_extra_features.md
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/candidate_valid_readme/correct_instance_extra_features_2.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/candidate_valid_readme/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/docs/template_folder_invalid/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/template_folder_invalid/extra_file.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/template_folder_invalid/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/template_folder_invalid/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/docs/template_folder_valid_with_readme/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/template_folder_valid_with_readme/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/template_folder_valid_with_readme/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_folder_is_a_file
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_bad_content/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_bad_content/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_bad_content/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_missing/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_missing/architecture.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_mixed_name/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_mixed_name/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_mixed_name/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_no_header/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_no_header/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_no_header/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_no_header/subdir/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_no_header/subdir/architecture.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_renamed/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_renamed/architecture_really_bad.md
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_renamed/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/folder_with_bad_drawio/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/folder_with_bad_drawio/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/folder_with_bad_drawio/diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/folder_with_bad_drawio/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.317584 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_limits_of_changes/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_limits_of_changes/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_limits_of_changes/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.317584 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_readme/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_readme/.hidden_test
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_readme/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_readme/network.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_readme/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.317584 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_version/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_version/diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_version/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.317584 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/__ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/_ignore_not_instance.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/diagram.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.317584 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore_not_instance.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/architecture.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.317584 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.317584 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_drawio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_drawio/.hidden_does_not_affect
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_drawio/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_drawio/diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_drawio/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_version/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_version/diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_version/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_with_readme/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_with_readme/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_with_readme/network.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_with_readme/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/governed_folders/utf16test_bad/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/utf16test_bad/sample.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/governed_folders/utf16test_good/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/utf16test_good/sample.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.241583 compliance-trestle-2.2.0/tests/data/author/headers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_drawio/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_drawio/template.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_drawio/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_md/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_md/template.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_md/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_wrong_names/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_wrong_names/templatesss.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_wrong_names/templatessss.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/headers/empty_headers/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/empty_headers/a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/empty_headers/b copy.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/empty_headers/b.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio/a_file.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio/whos_is_this.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio_bad_file/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio_bad_file/a_markdown_file.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio_bad_file/another_file.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md/my_drawio.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md/my_md.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md_bad_file/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md_bad_file/a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md_bad_file/b.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.241583 compliance-trestle-2.2.0/tests/data/author/headers/global/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/good/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/good/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.241583 compliance-trestle-2.2.0/tests/data/author/headers/global/good/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/good/catalogs/my_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/good/catalogs/my_catalog/catalogs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/good/sample_indexable_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/good/sample_indexable_1/sample.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/good/sample_indexable_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/good/sample_indexable_2/sample.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/good/unindexed.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/bad_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/bad_sample/bad_sample.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.241583 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/catalogs/my_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/catalogs/my_catalog/catalogs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_1/sample.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_2/sample.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/unindexed.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.241583 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/catalogs/my_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/catalogs/my_catalog/catalogs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/nested/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/nested/bad/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/nested/bad/bad_sample.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/nested/good/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/nested/good/sample.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/nested/sample.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/sample_indexable_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/sample_indexable_1/sample.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/unindexed.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/good_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/good_templates/template.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/good_templates/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/good_templates_wo_drawio/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/good_templates_wo_drawio/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/__ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/_ignore_not_instance.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/correct_a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/correct_b.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/correct_instance.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/_ignore_not_instance.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/correct_instance.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/even_deeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/even_deeper/_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/even_deeper/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/even_deeper/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/even_deeper/correct_a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/even_deeper/correct_instance.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/headers/meets_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/meets_templates/a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/meets_templates/b.md
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/meets_templates/d.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/headers/passes_with_extraneous_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/passes_with_extraneous_files/a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/passes_with_extraneous_files/b.md
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/passes_with_extraneous_files/d.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/passes_with_extraneous_files/irrelevant.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/b copy.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/b.md
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/d.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/some_depth/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/some_depth/a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/some_depth/b copy.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/some_depth/b.md
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/some_depth/d.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/ssp/
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/ssp/ssp_example.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.333584 compliance-trestle-2.2.0/tests/data/author/utf16test/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/utf16test/sample_okay.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/utf16test/sample_utf16.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.333584 compliance-trestle-2.2.0/tests/data/author/versions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.333584 compliance-trestle-2.2.0/tests/data/author/versions/1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/1.0.0/bad_template_wrong_folder.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/1.0.0/good_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.333584 compliance-trestle-2.2.0/tests/data/author/versions/1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/1.1.0/bad_instance_mismatched_versions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/1.1.0/bad_template_mismatched_versions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/1.1.0/good_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/1.1.0/good_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/bad_template_with_version_outside_structure.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/good_instance_with_version_outside_structure.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.333584 compliance-trestle-2.2.0/tests/data/csv/
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/csv/bp.sample.v2.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.245583 compliance-trestle-2.2.0/tests/data/csv/component-definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.333584 compliance-trestle-2.2.0/tests/data/csv/component-definitions/bp/
+-rw-r--r--   0 runner    (1001) docker     (123)    42744 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/csv/component-definitions/bp/component-definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54973 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/csv/ocp4-user.v2.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.333584 compliance-trestle-2.2.0/tests/data/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/lookup_table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/profile_to_docs.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/profile_to_docs_invalid.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/profile_to_docs_no_part_prose.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/profile_to_docs_only_some_sections.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/profile_to_docs_with_group_title.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/profile_to_docs_with_subparts.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/ssp_template.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/ssp_template_no_input_profile_ssp.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/sub_content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/sub_content_with_subs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/use_lookup_table.md.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.337584 compliance-trestle-2.2.0/tests/data/jinja_cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_cmd/empty_test.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_cmd/number_captions_data.md
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_cmd/number_captions_expected_output.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.337584 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDDatestamp_default.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDDatestamp_format.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDDatestamp_invalid.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDDatestamp_newline.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDSection_include_nested.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDSection_include_nested.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDSection_include_top_level.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDSection_include_top_level.md
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDSection_include_top_level_adjusted.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDSection_include_top_level_adjusted.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_include.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_include.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_include_adjusted.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_include_adjusted.md
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_nested_c_c.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_nested_c_c.md
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_nested_c_c_double.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_nested_c_c_double.md
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_nested_c_n.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_nested_c_n.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/nested_c.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/nested_n.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/test_markdown.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.345584 compliance-trestle-2.2.0/tests/data/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/bad_simple.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21655 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_def.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_def_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_def_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_def_readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_prof.json
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_prof_aa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_prof_ab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_prof_ba.json
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_prof_bad.json
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_prof_bb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_prof_part_none.json
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/good_simple.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/leveraged_ssp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/leveraged_ssp_readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_bad_oscal_version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_extra_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_missing_roles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_missing_uuid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_no_responsible-parties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_roles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_roles_double.json
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_roles_double_rp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_with_groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16376 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/nist_tutorial_catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/nist_tutorial_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/profile_bad_control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/profile_missing_position.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/profile_with_alter_props.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/profile_with_alter_subparts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/profile_with_incorrect_alter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/pull_nist_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simple_catalog_no_parts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simple_mapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simple_test_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simple_test_profile_less.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simple_test_profile_more.json
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simple_test_profile_no_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simple_test_profile_single.json
+-rw-r--r--   0 runner    (1001) docker     (123)   221136 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simplified_nist_catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simplified_nist_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/test_profile_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/test_profile_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/test_profile_c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/test_profile_d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/test_profile_e.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/test_profile_f.json
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/test_profile_g.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.345584 compliance-trestle-2.2.0/tests/data/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/markdown/valid_complex_md.md
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/markdown/valid_levels_no_text.md
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/markdown/valid_levels_no_text_increased_level.md
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/markdown/valid_no_headers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/markdown/valid_no_lvl1_headers.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.345584 compliance-trestle-2.2.0/tests/data/ocp4-cis/
+-rw-r--r--   0 runner    (1001) docker     (123)    23806 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/ocp4-cis/catalog.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.349584 compliance-trestle-2.2.0/tests/data/split_merge/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.349584 compliance-trestle-2.2.0/tests/data/split_merge/.trestle/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/.trestle/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.353584 compliance-trestle-2.2.0/tests/data/split_merge/load_distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)  3169371 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/load_distributed/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/load_distributed/groups.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.357584 compliance-trestle-2.2.0/tests/data/split_merge/step0-merged_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.245583 compliance-trestle-2.2.0/tests/data/split_merge/step0-merged_catalog/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.357584 compliance-trestle-2.2.0/tests/data/split_merge/step0-merged_catalog/catalogs/mycatalog/
+-rw-r--r--   0 runner    (1001) docker     (123)  4498050 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step0-merged_catalog/catalogs/mycatalog/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step0-merged_catalog/next_step.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.361584 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.245583 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.361584 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.369584 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/back-matter.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/next_step.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/previous_step.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.369584 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.245583 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.369584 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.373584 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/back-matter.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/groups.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.373584 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/parties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/responsible-parties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/roles.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/next_step.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/previous_step.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.373584 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.245583 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.373584 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.377585 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/back-matter.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/groups.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.381585 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/parties.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.381585 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties/00000__responsible-party.json
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties/00001__responsible-party.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.381585 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles/00000__role.json
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles/00001__role.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/next_step.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/previous_step.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.381585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.245583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.381585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.381585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/back-matter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.385584 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.389585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48380 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54960 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    70506 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26470 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00014__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30598 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00015__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22931 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00016__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00017__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00018__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18970 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00019__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00020__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00021__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00022__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00023__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00024__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.389585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18701 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.393585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18060 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15966 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00014__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00015__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.393585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24785 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.397585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27281 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15190 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34660 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28847 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.397585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29166 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14993 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13963 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21335 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.401585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29620 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    51627 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.401585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38793 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.405585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.405585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18885 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.413585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24929 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00014__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00015__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00016__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00017__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00018__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00019__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00020__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00021__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00022__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.413585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22272 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.421585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00014__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00015__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00016__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00017__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00018__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00019__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00020__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00021__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00022__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00023__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00024__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00025__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00026__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00027__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00028__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00029__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00030__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00031__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.425585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.425585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.429585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30706 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.433585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42212 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)   101326 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25087 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34032 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32683 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00014__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00015__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37819 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00016__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00017__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00018__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00019__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00020__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00021__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00022__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.449585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    72606 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00014__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00015__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00016__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00017__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00018__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00019__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00020__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00021__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00022__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00023__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00024__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00025__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00026__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00027__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00028__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00029__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00030__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00031__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00032__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00033__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00034__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00035__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00036__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00037__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00038__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00039__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00040__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00041__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00042__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00043__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00044__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00045__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00046__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00047__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00048__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00049__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00050__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.453585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26554 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    67388 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36771 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00014__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00015__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00016__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00017__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00018__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00019__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00020__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00021__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00022__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.457585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.457585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/parties.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.457585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/responsible-parties/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/responsible-parties/00000__responsible-party.json
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/responsible-parties/00001__responsible-party.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.457585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/roles/00000__role.json
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/roles/00001__role.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/next_step.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/previous_step.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.461585 compliance-trestle-2.2.0/tests/data/spread-sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/bad_parameter_name_and_description.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/duplicate_column_heading.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/embedded_blank_in_goal_name_id.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/embedded_blank_in_parameter_name.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/embedded_blank_in_rule_name_id.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/good.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/good_with_blank_rows.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/missing_column_heading.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/missing_control_id.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/missing_resource_title.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/missing_rule_name_id.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.257583 compliance-trestle-2.2.0/tests/data/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.461585 compliance-trestle-2.2.0/tests/data/tasks/cis-xlsx-to-oscal-catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_RedHat_OpenShift_Container_Platform_Benchmark_v1.2.0-2.snippet.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_Red_Hat_Enterprise_Linux_8_Benchmark_v2.0.0.snippet.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/cis-xlsx-to-oscal-catalog/test-cis-xlsx-to-oscal-catalog.ocp.config
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/cis-xlsx-to-oscal-catalog/test-cis-xlsx-to-oscal-catalog.rhel.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.461585 compliance-trestle-2.2.0/tests/data/tasks/csv-to-oscal-cd/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/csv-to-oscal-cd/test-csv-to-oscal-cd-bp.config
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/csv-to-oscal-cd/test-csv-to-oscal-cd.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.461585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input/cis.profile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input-bogus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input-bogus/cis.profile
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/test-ocp4-cis-profile-to-oscal-catalog.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.253584 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.253584 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_cni_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_cni_conf/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_apiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_apiserver/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_controller_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_controller_manager/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_cni_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_cni_conf/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_apiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_apiserver/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_controller_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_controller_manager/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_apiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_apiserver/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_controller_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_controller_manager/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_memory_available/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_memory_available/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_nodefs_available/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_nodefs_available/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.469585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/rule2var.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.469585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/output/
+-rw-r--r--   0 runner    (1001) docker     (123)    20254 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/output/component-definition.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.253584 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.253584 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.469585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis-node.profile
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis.profile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.469585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test.profile
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test2.profile
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test3.profile
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd3.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.469585 compliance-trestle-2.2.0/tests/data/tasks/oscal-catalog-to-csv/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-catalog-to-csv/test-oscal-catalog-to-csv-rev-5-by-control.config
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-catalog-to-csv/test-oscal-catalog-to-csv-rev-5-by-statement.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.473585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-no.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-yes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-no.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-yes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.2.0-parms-no.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-1.0.0-parms-yes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-no.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-yes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-scc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.39-parms-no.config
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.39-parms-yes.config
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.40-parms-no.config
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.40-parms-yes.config
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.2.0-parms-no.config
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-1.0.0-parms-yes.config
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-bogus.config
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-no-input-file.config
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-no-output-dir.config
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-no-overwrite.config
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-parms-no.config
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-parms-yes.config
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-scc.config
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-set.config
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.257583 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-no/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-no/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-yes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-yes/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-no/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-no/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-yes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-yes/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.2.0-parms-no/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.2.0-parms-no/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-1.0.0-parms-yes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-1.0.0-parms-yes/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-no/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-no/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-yes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-yes/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.481585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-scc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-scc/tailored-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output-set/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output-set/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.481585 compliance-trestle-2.2.0/tests/data/tasks/osco/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.481585 compliance-trestle-2.2.0/tests/data/tasks/osco/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input/ignore.me
+-rw-r--r--   0 runner    (1001) docker     (123)    52753 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.481585 compliance-trestle-2.2.0/tests/data/tasks/osco/input-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    52859 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.481585 compliance-trestle-2.2.0/tests/data/tasks/osco/input-bad-yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-bad-yaml/bad.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.481585 compliance-trestle-2.2.0/tests/data/tasks/osco/input-compressed/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.485585 compliance-trestle-2.2.0/tests/data/tasks/osco/input-configmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)   608191 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-configmaps/configmaps.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.485585 compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/
+-rw-r--r--   0 runner    (1001) docker     (123)   105678 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_resources.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.485585 compliance-trestle-2.2.0/tests/data/tasks/osco/input-xml-ocp4/
+-rw-r--r--   0 runner    (1001) docker     (123)    78761 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-xml-ocp4/ocp4-check-result.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.485585 compliance-trestle-2.2.0/tests/data/tasks/osco/input-xml-rhel7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-xml-rhel7/rhel7-check-result.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.485585 compliance-trestle-2.2.0/tests/data/tasks/osco/output/
+-rw-r--r--   0 runner    (1001) docker     (123)   155263 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.485585 compliance-trestle-2.2.0/tests/data/tasks/osco/output-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)   155462 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.489585 compliance-trestle-2.2.0/tests/data/tasks/osco/output-compressed/
+-rw-r--r--   0 runner    (1001) docker     (123)   155263 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.489585 compliance-trestle-2.2.0/tests/data/tasks/osco/output-configmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)  1870504 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-configmaps/configmaps.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.493585 compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/
+-rw-r--r--   0 runner    (1001) docker     (123)   366829 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/cluster_resource.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/cluster_resource_no_data.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/cluster_resource_no_kind0.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/cluster_resource_no_kind1.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/cluster_resource_no_resources.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/cluster_resource_no_results.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.493585 compliance-trestle-2.2.0/tests/data/tasks/osco/output-xml-ocp4/
+-rw-r--r--   0 runner    (1001) docker     (123)   273677 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-xml-ocp4/ocp4-check-result.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.493585 compliance-trestle-2.2.0/tests/data/tasks/osco/output-xml-rhel7/
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-xml-rhel7/rhel7-check-result.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar-1.3.5.config
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar-bad-yaml.config
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar-compressed.config
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar-configmaps.config
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar-fetcher.config
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar-xml-ocp4.config
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar-xml-rhel7.config
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.493585 compliance-trestle-2.2.0/tests/data/tasks/tanium/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/tanium/demo-tanium-result-to-oscal-ar.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.493585 compliance-trestle-2.2.0/tests/data/tasks/tanium/input/
+-rw-r--r--   0 runner    (1001) docker     (123)   314329 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/tanium/input/Tanium.comply-results-json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.493585 compliance-trestle-2.2.0/tests/data/tasks/tanium/input-bad/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/tanium/input-bad/Tanium.comply-results-bad
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.493585 compliance-trestle-2.2.0/tests/data/tasks/tanium/input-doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/tanium/input-doc/Tanium.doc-json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.497585 compliance-trestle-2.2.0/tests/data/tasks/tanium/output/
+-rw-r--r--   0 runner    (1001) docker     (123)  1997259 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/tanium/output/Tanium.oscal.2020.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1997259 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/tanium/output/Tanium.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.501586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.501586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output/
+-rw-r--r--   0 runner    (1001) docker     (123)   157229 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.505586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)   157432 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.505586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-compressed/
+-rw-r--r--   0 runner    (1001) docker     (123)   157229 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.505586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-configmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)  1891646 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-configmaps/configmaps.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/
+-rw-r--r--   0 runner    (1001) docker     (123)   371515 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/cluster_resource.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_data.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_kind0.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_kind1.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_resources.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_results.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-xml-ocp4/
+-rw-r--r--   0 runner    (1001) docker     (123)   276795 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-xml-ocp4/ocp4-check-result.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-xml-rhel7/
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-xml-rhel7/rhel7-check-result.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-1.3.5.config
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-bad-yaml.config
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-compressed.config
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-configmaps.config
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-fetcher.config
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-xml-ocp4.config
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-xml-rhel7.config
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output/
+-rw-r--r--   0 runner    (1001) docker     (123)    67226 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output/component-definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output/profile.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-check/
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-check/profile.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-control/
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-control/profile.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-rule/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-rule/profile.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-filtered/
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-filtered/profile.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.513586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-missing-control-id/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-missing-control-id/profile.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.513586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-missing-rule-name-id/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-missing-rule-name-id/profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/test-xlsx-to-oscal-cd.config
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/test-xlsx-to-oscal-profile.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.513586 compliance-trestle-2.2.0/tests/data/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)    99263 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/yaml/bad_component_dup_uuid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    99257 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/yaml/bad_component_no_tz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/yaml/bad_simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    99263 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/yaml/good_component.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    99263 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/yaml/good_component_diff_tz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/yaml/good_simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/yaml/header_with_metadata.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.513586 compliance-trestle-2.2.0/tests/functionality/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/functionality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/functionality/chevron_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/functionality/example_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/functionality/pathlib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.517586 compliance-trestle-2.2.0/tests/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/manual_tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/manual_tests/split_test_1.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/manual_tests/split_test_issue_630.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/manual_tests/split_validate_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1362 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/manual_tests/test_binary.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    26384 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.517586 compliance-trestle-2.2.0/tests/trestle/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.521586 compliance-trestle-2.2.0/tests/trestle/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/base_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.525586 compliance-trestle-2.2.0/tests/trestle/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/add_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/assemble_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.529586 compliance-trestle-2.2.0/tests/trestle/core/commands/author/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/catalog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29859 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/docs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24635 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/folders_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20612 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/headers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/jinja_cmd_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/profile_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32856 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/ssp_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.529586 compliance-trestle-2.2.0/tests/trestle/core/commands/author/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/versioning/template_versioning_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/cmd_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/create_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/describe_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/href_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/import__test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/init_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/merge_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/partial_object_validate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/remove_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/replicate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/split_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/task_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18571 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/validate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/version_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/control_io_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/draw_io_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/err_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/jinja_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.529586 compliance-trestle-2.2.0/tests/trestle/core/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/markdown/markdown_node_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17571 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/markdown/markdown_validator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.533586 compliance-trestle-2.2.0/tests/trestle/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/create_path_action_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/element_path_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/element_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/file_content_type_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/interfaces_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/plans_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/remove_action_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/remove_path_action_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/update_action_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/write_action_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/write_file_action_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21160 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/profile_resolver_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.533586 compliance-trestle-2.2.0/tests/trestle/core/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15089 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/remote/cache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/repository_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/ssp_io_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/validator_helper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.533586 compliance-trestle-2.2.0/tests/trestle/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/parsing/parsing_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.537586 compliance-trestle-2.2.0/tests/trestle/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/base_task_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/cis_xlsx_to_oscal_catalog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46119 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/csv_to_oscal_cd_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/ocp4_cis_profile_to_oscal_catalog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/ocp4_cis_profile_to_oscal_cd_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/oscal_catalog_to_csv_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/oscal_profile_to_osco_profile_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/osco_result_to_oscal_ar_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15849 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/tanium_result_to_oscal_ar_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/transform_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/xccdf_result_to_oscal_ar_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/xlsx_to_oscal_cd_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/xlsx_to_oscal_profile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.537586 compliance-trestle-2.2.0/tests/trestle/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/transforms/transformer_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/transforms/transformer_helper_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.541586 compliance-trestle-2.2.0/tests/trestle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29420 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/utils/fs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/utils/list_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/utils/load_distributed_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/utils/md_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/utils/trash_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.541586 compliance-trestle-2.2.0/trestle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-26 21:32:03.000000 compliance-trestle-2.2.0/trestle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.545586 compliance-trestle-2.2.0/trestle/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17322 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/err.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/list_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/load_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44383 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/str_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/trash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.553586 compliance-trestle-2.2.0/trestle/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/all_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.557586 compliance-trestle-2.2.0/trestle/core/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/catalog/catalog_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42306 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/catalog/catalog_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/catalog/catalog_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/catalog/catalog_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22324 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/catalog/catalog_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/catalog_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.561586 compliance-trestle-2.2.0/trestle/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/assemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.565586 compliance-trestle-2.2.0/trestle/core/commands/author/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16138 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14168 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33967 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43643 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/ssp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.565586 compliance-trestle-2.2.0/trestle/core/commands/author/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/versioning/template_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/command_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.565586 compliance-trestle-2.2.0/trestle/core/commands/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/common/cmd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/common/return_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/describe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/href.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/partial_object_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/replicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22026 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/control_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49620 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/control_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23766 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/control_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28904 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/control_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/docs_control_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/draw_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/duplicates_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20080 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/generic_oscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/links_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.569586 compliance-trestle-2.2.0/trestle/core/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/base_markdown_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28075 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/control_markdown_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/docs_markdown_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/markdown_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/markdown_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/markdown_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/markdown_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/md_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.569586 compliance-trestle-2.2.0/trestle/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16242 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/models/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25162 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/models/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/models/file_content_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/models/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/models/plans.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/profile_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/refs_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.569586 compliance-trestle-2.2.0/trestle/core/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/remote/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16329 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.573586 compliance-trestle-2.2.0/trestle/core/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/resolver/_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/resolver/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16076 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/resolver/modify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/resolver/prune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/rule_parameters_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/ssp_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/trestle_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/validator_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.577586 compliance-trestle-2.2.0/trestle/oscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26369 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/assessment_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35188 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/assessment_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80055 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26943 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/poam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37519 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/ssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.577586 compliance-trestle-2.2.0/trestle/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/resources/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.577586 compliance-trestle-2.2.0/trestle/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/resources/templates/FedRAMP_control_header_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/resources/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/resources/templates/template.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/resources/templates/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.581586 compliance-trestle-2.2.0/trestle/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/cis_xlsx_to_oscal_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63140 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/csv_to_oscal_cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/ocp4_cis_profile_to_oscal_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25634 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/ocp4_cis_profile_to_oscal_cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/oscal_catalog_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/oscal_profile_to_osco_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/osco_result_to_oscal_ar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/tanium_result_to_oscal_ar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/xccdf_result_to_oscal_ar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23198 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/xlsx_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17402 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/xlsx_to_oscal_cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/xlsx_to_oscal_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.581586 compliance-trestle-2.2.0/trestle/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.585586 compliance-trestle-2.2.0/trestle/transforms/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28870 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/implementations/osco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/implementations/tanium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23496 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/implementations/xccdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/transformer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/transformer_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/transformer_singleton.py
```

### Comparing `compliance-trestle-2.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `compliance-trestle-2.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/.github/PULL_REQUEST_TEMPLATE/develop.md` & `compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE/develop.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/.github/PULL_REQUEST_TEMPLATE/release.md` & `compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE/release.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/.github/PULL_REQUEST_TEMPLATE.md` & `compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/.github/workflows/codeql-analysis.yml` & `compliance-trestle-2.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/.github/workflows/conventional-pr.yml` & `compliance-trestle-2.2.0/.github/workflows/conventional-pr.yml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/.github/workflows/python-push.yml` & `compliance-trestle-2.2.0/.github/workflows/python-push.yml`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,27 @@
         include:
         - os: ubuntu-latest
           path: ~/.cache/pip
         - os: macos-latest
           path: ~/Library/Caches/pip
         - os: windows-latest
           path: ~\AppData\Local\pip\Cache
-        python-version: [3.7, 3.8, 3.9]
+        # optional 3.7 test
+        - os: ubuntu-latest
+          path: ~/.cache/pip
+          python-version: 3.7
+        # optional 3.7 test
+        - os: macos-latest
+          path: ~/Library/Caches/pip
+          python-version: 3.7.16
+        # optional 3.7 test
+        - os: windows-latest
+          path: ~\AppData\Local\pip\Cache
+          python-version: 3.7
+        python-version: [3.8, 3.9]
 
     steps:
     - name: Don't mess with  line endings
       run: |
         git config --global core.autocrlf false
     - uses: actions/checkout@v2
       with:
```

### Comparing `compliance-trestle-2.1.1/.github/workflows/python-test.yml` & `compliance-trestle-2.2.0/.github/workflows/python-test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -88,22 +88,35 @@
 
   test:
     # This test
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
+        python-version: [3.8, 3.9]
         include:
         - os: ubuntu-latest
           path: ~/.cache/pip
         - os: macos-latest
           path: ~/Library/Caches/pip
         - os: windows-latest
           path: ~\AppData\Local\pip\Cache
-        python-version: [3.7, 3.8, 3.9]
+        # optional 3.7 test
+        - os: ubuntu-latest
+          path: ~/.cache/pip
+          python-version: 3.7
+        # optional 3.7 test
+        - os: macos-latest
+          path: ~/Library/Caches/pip
+          python-version: 3.7.16
+        # optional 3.7 test
+        - os: windows-latest
+          path: ~\AppData\Local\pip\Cache
+          python-version: 3.7
+          
     steps:
     - name: Don't mess with line endings
       run: |
         git config --global core.autocrlf false
     - uses: actions/checkout@v2
       with:
         fetch-depth: 0
@@ -118,24 +131,24 @@
         key: ${{ matrix.os }}-${{ matrix.python-version }}-pip-${{ hashFiles('setup.cfg') }}
         restore-keys: |
          ${{ matrix.os }}-${{ matrix.python-version }}-pip-
     - name: Install build tools
       run: |
         make develop
     - name: Pytest Fast
-      if: ${{ !(matrix.os == 'ubuntu-latest' && matrix.python-version == '3.7') }}
+      if: ${{ !(matrix.os == 'ubuntu-latest' && matrix.python-version == '3.8') }}
       run: |
         make test
     - name: Pytest Cov
-      if: ${{ matrix.os == 'ubuntu-latest' && matrix.python-version == '3.7' }}
+      if: ${{ matrix.os == 'ubuntu-latest' && matrix.python-version == '3.8' }}
       run: |
         make test-cov
 
     - name: Upload artifact
-      if: ${{ matrix.os == 'ubuntu-latest' && matrix.python-version == '3.7' }}
+      if: ${{ matrix.os == 'ubuntu-latest' && matrix.python-version == '3.8' }}
       uses: actions/upload-artifact@v2
       with:
         name: coverage
         path: coverage.xml
 
   sonar:
     if: ${{ github.event.pull_request.base.repo.url == github.event.pull_request.head.repo.url }}
@@ -150,15 +163,15 @@
         git config --global core.autocrlf false
     - uses: actions/checkout@v2
       with:
         submodules: true
     - name: Set up Python
       uses: actions/setup-python@v2
       with:
-        python-version: 3.7
+        python-version: 3.8
     - uses: actions/cache@v2
       with:
         path: ~/.cache/pip
         key: ubuntu-latest-3.9-pip-${{ hashFiles('setup.cfg') }}
         restore-keys: |
           ubuntu-latest-3.9-pip-
     - name: Install build tools
@@ -174,15 +187,15 @@
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}  # Needed to get PR information, if any
         SONAR_TOKEN: ${{ secrets.SONAR_TOKEN }}
       with:
         args: >
           -Dsonar.python.coverage.reportPaths=coverage.xml
           -Dsonar.tests=tests/
           -Dsonar.sources=trestle/ 
-          -Dsonar.python.version=3.7
+          -Dsonar.python.version=3.8
           -Dsonar.projectKey=compliance-trestle
           -Dsonar.organization=compliance-trestle
           -Dsonar.cpd.exclusions=trestle/oscal/*.py
     - name: SonarQube Quality Gate check
       uses: sonarsource/sonarqube-quality-gate-action@master
       # Force to fail step after specific time
       timeout-minutes: 5
```

### Comparing `compliance-trestle-2.1.1/.gitignore` & `compliance-trestle-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/.pre-commit-config.yaml` & `compliance-trestle-2.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/CHANGELOG.md` & `compliance-trestle-2.2.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,34 @@
 # Compliance-trestle changelog
 
 
 <!--next-version-placeholder-->
 
+## v2.2.0 (2023-06-26)
+
+### Feature
+
+* Add profile-inherit command ([#1392](https://github.com/IBM/compliance-trestle/issues/1392)) ([`3bd53ff`](https://github.com/IBM/compliance-trestle/commit/3bd53ff370cece77fc78082dbc04304af12c6647))
+* Oscal-catalog-to-csv ([#1396](https://github.com/IBM/compliance-trestle/issues/1396)) ([`5f59a7f`](https://github.com/IBM/compliance-trestle/commit/5f59a7fc7cf8b88a9f77ba4554dd493acff67114))
+* Adds control origination to ssp-filter ([#1375](https://github.com/IBM/compliance-trestle/issues/1375)) ([`509afa7`](https://github.com/IBM/compliance-trestle/commit/509afa7df124f8a6c3516ad06db256777baaef98))
+
+### Fix
+
+* Drop python 3.7 support as required  ([`cf4160b`](https://github.com/IBM/compliance-trestle/commit/cf4160bc25336cb9362150906a8aaeda308c4134))
+* Change the community call to use bluejeans events ([#1400](https://github.com/IBM/compliance-trestle/issues/1400)) ([`9380cc8`](https://github.com/IBM/compliance-trestle/commit/9380cc813f8b044640fecb4ee302207d3c66d29a))
+* Python 3.7.17 issue ([#1408](https://github.com/IBM/compliance-trestle/issues/1408)) ([`6849c3b`](https://github.com/IBM/compliance-trestle/commit/6849c3b01d0adfd1261b9929a7d5c1866dd38973))
+* Log warning for duplicate part ids when writing markdown from json ([#1395](https://github.com/IBM/compliance-trestle/issues/1395)) ([`760dd4b`](https://github.com/IBM/compliance-trestle/commit/760dd4b4dd6ac405df3db0c2d39d9973ab61a0f4))
+* Use empty string if prose in part is None while writing to markdown ([#1390](https://github.com/IBM/compliance-trestle/issues/1390)) ([`5427fbb`](https://github.com/IBM/compliance-trestle/commit/5427fbb445e9a54a2ede1caa7e15c15b8977dd10))
+* Some tests failing on linux ([#1387](https://github.com/IBM/compliance-trestle/issues/1387)) ([`f0ffdec`](https://github.com/IBM/compliance-trestle/commit/f0ffdecb963d7cd341b6b40be3a02efd3e76748d))
+* Update readme with webex details ([#1383](https://github.com/IBM/compliance-trestle/issues/1383)) ([`4263f1a`](https://github.com/IBM/compliance-trestle/commit/4263f1a72fa9a3ebea01b3b5c301cf89a962bf9c))
+
+### Documentation
+
+* Update maintainers list ([#1394](https://github.com/IBM/compliance-trestle/issues/1394)) ([`c53faa4`](https://github.com/IBM/compliance-trestle/commit/c53faa40ce23a5ad5476cbb6e2c3d32a8e6818dc))
+
 ## v2.1.1 (2023-05-12)
 ### Fix
 * Change lint title action ([#1352](https://github.com/IBM/compliance-trestle/issues/1352)) ([`5444206`](https://github.com/IBM/compliance-trestle/commit/5444206f8b8c8e6904ec180472c569e246255975))
 * Docs for task xlsx-result-to-oscal-ar replacing "osco" ([#1369](https://github.com/IBM/compliance-trestle/issues/1369)) ([`850ed0a`](https://github.com/IBM/compliance-trestle/commit/850ed0a99e0298496b0df1e91c22bd80c290b6e1))
 * Ssp response missing status and rules ([#1358](https://github.com/IBM/compliance-trestle/issues/1358)) ([`43daf5f`](https://github.com/IBM/compliance-trestle/commit/43daf5f9fca2495c1dbb8fa2ea39cb7184a9e191))
 * Xccdf to oscal-ar ([#1336](https://github.com/IBM/compliance-trestle/issues/1336)) ([`7305883`](https://github.com/IBM/compliance-trestle/commit/730588327ea54a5fc7a5d1f597a3ffeee92e0e48))
 * Handle tabs in statement prose and parts ([#1359](https://github.com/IBM/compliance-trestle/issues/1359)) ([`c34dbea`](https://github.com/IBM/compliance-trestle/commit/c34dbeaa7dd75cd614393c57cba97fa9e5c8d699))
```

### Comparing `compliance-trestle-2.1.1/CODE_OF_CONDUCT.md` & `compliance-trestle-2.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/CONTRIBUTING.md` & `compliance-trestle-2.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/DCO1.1.txt` & `compliance-trestle-2.2.0/DCO1.1.txt`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/LICENSE` & `compliance-trestle-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/MAINTAINERS.md` & `compliance-trestle-2.2.0/MAINTAINERS.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 Trestle was designed and open sourced by a team based at [IBM Research](https://www.research.ibm.com/) and others around the world.  The list includes:
 
-Christopher Butler - [butler54](https://github.com/butler54)
-
-Bruno Marques - [brunomarq](https://github.com/brunomarq)
+Alejandro Jose Leiva Palomo [AleJo2995](https://github.com/AleJo2995)
 
-Lenin Mehedy - [leninmehedy](https://github.com/leninmehedy)
+Christopher Butler [butler54](https://github.com/butler54)
 
-Simon Metson - [drsm79](https://github.com/drsm79)
+Lou Degenaro [degenaro](https://github.com/degenaro)
 
-Frank Suits - [fsuits](https://github.com/fsuits)
+Frank Suits [fsuits](https://github.com/fsuits)
 
-Jeff Tan - [jeffdmgit](https://github.com/jeffdmgit)
+Jennifer Power [jpower432](https://github.com/jpower432)
 
-Nebula Alam - [aNebula](https://github.com/aNebula)
+Manjiree Gadgil [mrgadgil](https://github.com/mrgadgil)
 
 Vikas Agarwal [vikas-agarwal76](https://github.com/vikas-agarwal76)
-
-Lou Degenaro [degenaro](https://github.com/degenaro)
-
-Ekaterina Nikonova [enikonovad](https://github.com/enikonovad)
-
-Alejandro Jose Leiva Palomo [AleJo2995](https://github.com/AleJo2995)
```

### Comparing `compliance-trestle-2.1.1/Makefile` & `compliance-trestle-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/PKG-INFO` & `compliance-trestle-2.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: compliance-trestle
-Version: 2.1.1
-Summary: Tools to manage & autogenerate python objects representing the OSCAL layers/models
-Home-page: https://ibm.github.io/compliance-trestle
-Author: IBM
-Author-email: avikas@in.ibm.com
-License: Apache Software License v2
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Compliance-trestle (also known as `trestle`)
 
 ![[OS Compatibility](#prerequisites)](https://img.shields.io/badge/platform-osx%20%7C%20linux%20%7C%20windows-orange.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/compliance-trestle)
 ![[Pre-commit](https://github.com/pre-commit/pre-commit)](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
 ![[Code Coverage](https://sonarcloud.io/dashboard?id=compliance-trestle)](https://sonarcloud.io/api/project_badges/measure?project=compliance-trestle&metric=coverage)
 ![[Quality gate](https://sonarcloud.io/dashboard?id=compliance-trestle)](https://sonarcloud.io/api/project_badges/measure?project=compliance-trestle&metric=alert_status)
@@ -107,31 +84,41 @@
 ## Development status
 
 Compliance trestle is currently stable and is based on NIST OSCAL version 1.0.4, with active development continuing.
 
 ## Community call
 
 We would like to share development in progress for compliance trestle, coming soon and get feedback from community on what features would they like to see in compliance trestle.\
-The community call will happen every 2 week(s) on Tuesday at 10am EST.\
+The community call will happen every 2 week(s) on Tuesday at 10.00am EST.\
 Meeting information:
 
 ```
+You have been invited to Attend at the following event :
 Compliance Trestle Community Call
-Hosted by MANJIREE GADGIL
+Every 2nd week on Tuesday; from June 27th, 2023 at 10:00 am EST for 0.5 hour
+
+To join, select from the following options: 
+
+1) Web Browser
+    a) https://primetime.bluejeans.com/a2m/live-event/dcwuavtj
+
+2) Laptop paired with room system (Best Experience)
+    a) Dial: meet@bjn.vc or 104.238.247.247 in the room system.
+    b) Go to https://primetime.bluejeans.com/a2m/live-event/dcwuavtj/room-system/
+    c) Enter the pairing code displayed on your room system's screen into your browser.
+
+3) Room System
+    a) Dial: meet@bjn.vc or 104.238.247.247 in the room system.
+    b) Enter Meeting ID : 499830564  and Passcode :  8231
+
+4) Joining via a mobile device?
+    a) Open this link : https://primetime.bluejeans.com/a2m/live-event/dcwuavtj 
+    b) Download the app if you don’t have it already 
+    c) Enter event ID : dcwuavtj
 
-https://ibm.webex.com/ibm/j.php?MTID=m46740e85f87f290d0848c6941c489b0a
-Tuesday, May 16, 2023 10:30 AM | 30 minutes | (UTC-04:00) Eastern Time (US & Canada)
-Occurs every 2 week(s) on Tuesday effective 5/16/2023 from 10:30 AM to 11:00 AM, (UTC-04:00) Eastern Time (US & Canada)
-
-Join by phone
-1-844-531-0958 United States Toll Free
-1-669-234-1178 United States Toll
-1-669-234-1178 United States Toll
-Host access code 979 191 85
-Attendee access code 979 379 85
 ```
 
 ## Contributing to Trestle
 
 Our project welcomes external contributions. Please consult [contributing](https://ibm.github.io/compliance-trestle/contributing/mkdocs_contributing/) to get started.
 
 ## License & Authors
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `compliance-trestle-2.1.1/README.md` & `compliance-trestle-2.2.0/docs/index.md`

 * *Files 11% similar despite different names*

```diff
@@ -65,60 +65,28 @@
 Future roadmap anticipates that support for xml [import](https://github.com/IBM/compliance-trestle/issues/177) and [upstream references](https://github.com/IBM/compliance-trestle/issues/178) will be enabled. However, it is expected
 that full support will remain only for `json` and  `yaml`.
 
 Users needing to import XML OSCAL artifacts are recommended to look at NIST's XML to json conversion page [here](https://github.com/usnistgov/OSCAL/tree/master/json#oscal-xml-to-json-converters).
 
 ## Python codebase, easy installation via pip
 
-Trestle runs on almost all Python platforms (e.g. Linux, Mac, Windows), is available on PyPi and can be easily installed via pip. It is under active development and new releases are made available regularly.\
-To install run: `pip install compliance-trestle`\
-See [Install trestle in a python virtual environment](https://ibm.github.io/compliance-trestle/python_trestle_setup/) for the full installation guide.
-
-## Complete documentation and tutorials
-
-Complete documentation, tutorials, and background on compliance can be found [here](https://ibm.github.io/compliance-trestle).
-
-## Demos
-
-A collection of demos utilizing trestle can be found in the related project [compliance-trestle-demos](https://github.com/IBM/compliance-trestle-demos).
+Trestle runs on most all python platforms (e.g. Linux, Mac, Windows) and is available on PyPi so it is easily installed via pip.  It is under active development and new releases are made available regularly.
 
 ## Development status
 
 Compliance trestle is currently stable and is based on NIST OSCAL version 1.0.4, with active development continuing.
 
-## Community call
-
-We would like to share development in progress for compliance trestle, coming soon and get feedback from community on what features would they like to see in compliance trestle.\
-The community call will happen every 2 week(s) on Tuesday at 10am EST.\
-Meeting information:
-
-```
-Compliance Trestle Community Call
-Hosted by MANJIREE GADGIL
-
-https://ibm.webex.com/ibm/j.php?MTID=m46740e85f87f290d0848c6941c489b0a
-Tuesday, May 16, 2023 10:30 AM | 30 minutes | (UTC-04:00) Eastern Time (US & Canada)
-Occurs every 2 week(s) on Tuesday effective 5/16/2023 from 10:30 AM to 11:00 AM, (UTC-04:00) Eastern Time (US & Canada)
-
-Join by phone
-1-844-531-0958 United States Toll Free
-1-669-234-1178 United States Toll
-1-669-234-1178 United States Toll
-Host access code 979 191 85
-Attendee access code 979 379 85
-```
-
 ## Contributing to Trestle
 
-Our project welcomes external contributions. Please consult [contributing](https://ibm.github.io/compliance-trestle/contributing/mkdocs_contributing/) to get started.
+Our project welcomes external contributions. Please consult [contributing](contributing/mkdocs_contributing/) to get started.
 
 ## License & Authors
 
-If you would like to see the detailed LICENSE click [here](LICENSE).
-Consult [contributors](https://github.com/IBM/compliance-trestle/graphs/contributors) for a list of authors and [maintainers](MAINTAINERS.md) for the core team.
+If you would like to see the detailed LICENSE click [here](license/).
+Consult [contributors](https://github.com/IBM/compliance-trestle/graphs/contributors) for a list of authors and [maintainers](maintainers/) for the core team.
 
 ```text
 # Copyright (c) 2020 IBM Corp. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
```

### Comparing `compliance-trestle-2.1.1/compliance_trestle.egg-info/PKG-INFO` & `compliance-trestle-2.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compliance-trestle
-Version: 2.1.1
+Version: 2.2.0
 Summary: Tools to manage & autogenerate python objects representing the OSCAL layers/models
 Home-page: https://ibm.github.io/compliance-trestle
 Author: IBM
 Author-email: avikas@in.ibm.com
 License: Apache Software License v2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -107,31 +107,41 @@
 ## Development status
 
 Compliance trestle is currently stable and is based on NIST OSCAL version 1.0.4, with active development continuing.
 
 ## Community call
 
 We would like to share development in progress for compliance trestle, coming soon and get feedback from community on what features would they like to see in compliance trestle.\
-The community call will happen every 2 week(s) on Tuesday at 10am EST.\
+The community call will happen every 2 week(s) on Tuesday at 10.00am EST.\
 Meeting information:
 
 ```
+You have been invited to Attend at the following event :
 Compliance Trestle Community Call
-Hosted by MANJIREE GADGIL
+Every 2nd week on Tuesday; from June 27th, 2023 at 10:00 am EST for 0.5 hour
+
+To join, select from the following options: 
+
+1) Web Browser
+    a) https://primetime.bluejeans.com/a2m/live-event/dcwuavtj
+
+2) Laptop paired with room system (Best Experience)
+    a) Dial: meet@bjn.vc or 104.238.247.247 in the room system.
+    b) Go to https://primetime.bluejeans.com/a2m/live-event/dcwuavtj/room-system/
+    c) Enter the pairing code displayed on your room system's screen into your browser.
+
+3) Room System
+    a) Dial: meet@bjn.vc or 104.238.247.247 in the room system.
+    b) Enter Meeting ID : 499830564  and Passcode :  8231
+
+4) Joining via a mobile device?
+    a) Open this link : https://primetime.bluejeans.com/a2m/live-event/dcwuavtj 
+    b) Download the app if you don’t have it already 
+    c) Enter event ID : dcwuavtj
 
-https://ibm.webex.com/ibm/j.php?MTID=m46740e85f87f290d0848c6941c489b0a
-Tuesday, May 16, 2023 10:30 AM | 30 minutes | (UTC-04:00) Eastern Time (US & Canada)
-Occurs every 2 week(s) on Tuesday effective 5/16/2023 from 10:30 AM to 11:00 AM, (UTC-04:00) Eastern Time (US & Canada)
-
-Join by phone
-1-844-531-0958 United States Toll Free
-1-669-234-1178 United States Toll
-1-669-234-1178 United States Toll
-Host access code 979 191 85
-Attendee access code 979 379 85
 ```
 
 ## Contributing to Trestle
 
 Our project welcomes external contributions. Please consult [contributing](https://ibm.github.io/compliance-trestle/contributing/mkdocs_contributing/) to get started.
 
 ## License & Authors
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `compliance-trestle-2.1.1/compliance_trestle.egg-info/SOURCES.txt` & `compliance-trestle-2.2.0/compliance_trestle.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -145,14 +145,15 @@
 docs/api_reference/trestle.oscal.profile.md
 docs/api_reference/trestle.oscal.ssp.md
 docs/api_reference/trestle.tasks.base_task.md
 docs/api_reference/trestle.tasks.cis_xlsx_to_oscal_catalog.md
 docs/api_reference/trestle.tasks.csv_to_oscal_cd.md
 docs/api_reference/trestle.tasks.ocp4_cis_profile_to_oscal_catalog.md
 docs/api_reference/trestle.tasks.ocp4_cis_profile_to_oscal_cd.md
+docs/api_reference/trestle.tasks.oscal_catalog_to_csv.md
 docs/api_reference/trestle.tasks.oscal_profile_to_osco_profile.md
 docs/api_reference/trestle.tasks.osco_result_to_oscal_ar.md
 docs/api_reference/trestle.tasks.tanium_result_to_oscal_ar.md
 docs/api_reference/trestle.tasks.transform.md
 docs/api_reference/trestle.tasks.xccdf_result_to_oscal_ar.md
 docs/api_reference/trestle.tasks.xlsx_helper.md
 docs/api_reference/trestle.tasks.xlsx_to_oscal_cd.md
@@ -454,14 +455,15 @@
 tests/data/author/versions/1.1.0/good_template.md
 tests/data/csv/bp.sample.v2.csv
 tests/data/csv/ocp4-user.v2.csv
 tests/data/csv/component-definitions/bp/component-definition.json
 tests/data/jinja/lookup_table.yaml
 tests/data/jinja/profile_to_docs.md.jinja
 tests/data/jinja/profile_to_docs_invalid.md.jinja
+tests/data/jinja/profile_to_docs_no_part_prose.md.jinja
 tests/data/jinja/profile_to_docs_only_some_sections.md.jinja
 tests/data/jinja/profile_to_docs_with_group_title.md.jinja
 tests/data/jinja/profile_to_docs_with_subparts.md.jinja
 tests/data/jinja/ssp_template.md.jinja
 tests/data/jinja/ssp_template_no_input_profile_ssp.md.jinja
 tests/data/jinja/sub_content.md
 tests/data/jinja/sub_content_with_subs.md
@@ -499,15 +501,18 @@
 tests/data/json/comp_def_readme.md
 tests/data/json/comp_prof.json
 tests/data/json/comp_prof_aa.json
 tests/data/json/comp_prof_ab.json
 tests/data/json/comp_prof_ba.json
 tests/data/json/comp_prof_bad.json
 tests/data/json/comp_prof_bb.json
+tests/data/json/comp_prof_part_none.json
 tests/data/json/good_simple.json
+tests/data/json/leveraged_ssp.json
+tests/data/json/leveraged_ssp_readme.md
 tests/data/json/minimal_catalog.json
 tests/data/json/minimal_catalog_bad_oscal_version.json
 tests/data/json/minimal_catalog_extra_fields.json
 tests/data/json/minimal_catalog_missing_roles.json
 tests/data/json/minimal_catalog_missing_uuid.json
 tests/data/json/minimal_catalog_no_responsible-parties.json
 tests/data/json/minimal_catalog_roles.json
@@ -521,15 +526,18 @@
 tests/data/json/profile_with_alter_props.json
 tests/data/json/profile_with_alter_subparts.json
 tests/data/json/profile_with_incorrect_alter.json
 tests/data/json/pull_nist_profile.json
 tests/data/json/simple_catalog_no_parts.json
 tests/data/json/simple_mapping.json
 tests/data/json/simple_test_profile.json
+tests/data/json/simple_test_profile_less.json
+tests/data/json/simple_test_profile_more.json
 tests/data/json/simple_test_profile_no_params.json
+tests/data/json/simple_test_profile_single.json
 tests/data/json/simplified_nist_catalog.json
 tests/data/json/simplified_nist_profile.json
 tests/data/json/test_profile_a.json
 tests/data/json/test_profile_b.json
 tests/data/json/test_profile_c.json
 tests/data/json/test_profile_d.json
 tests/data/json/test_profile_e.json
@@ -968,14 +976,16 @@
 tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules2.json
 tests/data/tasks/ocp4-cis-profile-to-oscal-cd/output/component-definition.json
 tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis-node.profile
 tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis.profile
 tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test.profile
 tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test2.profile
 tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test3.profile
+tests/data/tasks/oscal-catalog-to-csv/test-oscal-catalog-to-csv-rev-5-by-control.config
+tests/data/tasks/oscal-catalog-to-csv/test-oscal-catalog-to-csv-rev-5-by-statement.config
 tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.39-parms-no.config
 tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.39-parms-yes.config
 tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.40-parms-no.config
 tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.40-parms-yes.config
 tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.2.0-parms-no.config
 tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-1.0.0-parms-yes.config
 tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-bogus.config
@@ -1161,14 +1171,15 @@
 tests/trestle/parsing/parsing_test.py
 tests/trestle/tasks/__init__.py
 tests/trestle/tasks/base_task_test.py
 tests/trestle/tasks/cis_xlsx_to_oscal_catalog_test.py
 tests/trestle/tasks/csv_to_oscal_cd_test.py
 tests/trestle/tasks/ocp4_cis_profile_to_oscal_catalog_test.py
 tests/trestle/tasks/ocp4_cis_profile_to_oscal_cd_test.py
+tests/trestle/tasks/oscal_catalog_to_csv_test.py
 tests/trestle/tasks/oscal_profile_to_osco_profile_test.py
 tests/trestle/tasks/osco_result_to_oscal_ar_test.py
 tests/trestle/tasks/tanium_result_to_oscal_ar_test.py
 tests/trestle/tasks/transform_test.py
 tests/trestle/tasks/xccdf_result_to_oscal_ar_test.py
 tests/trestle/tasks/xlsx_to_oscal_cd_test.py
 tests/trestle/tasks/xlsx_to_oscal_profile_test.py
@@ -1306,14 +1317,15 @@
 trestle/resources/templates/template.md
 trestle/tasks/__init__.py
 trestle/tasks/base_task.py
 trestle/tasks/cis_xlsx_to_oscal_catalog.py
 trestle/tasks/csv_to_oscal_cd.py
 trestle/tasks/ocp4_cis_profile_to_oscal_catalog.py
 trestle/tasks/ocp4_cis_profile_to_oscal_cd.py
+trestle/tasks/oscal_catalog_to_csv.py
 trestle/tasks/oscal_profile_to_osco_profile.py
 trestle/tasks/osco_result_to_oscal_ar.py
 trestle/tasks/tanium_result_to_oscal_ar.py
 trestle/tasks/transform.py
 trestle/tasks/xccdf_result_to_oscal_ar.py
 trestle/tasks/xlsx_helper.py
 trestle/tasks/xlsx_to_oscal_cd.py
```

### Comparing `compliance-trestle-2.1.1/compliance_trestle.egg-info/requires.txt` & `compliance-trestle-2.2.0/compliance_trestle.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/assets/Canonical_trestle_auditree_workflows.png` & `compliance-trestle-2.2.0/docs/assets/Canonical_trestle_auditree_workflows.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/assets/canonical_trestle_auditree_workflows.drawio` & `compliance-trestle-2.2.0/docs/assets/canonical_trestle_auditree_workflows.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/assets/drawio_data_menu.png` & `compliance-trestle-2.2.0/docs/assets/drawio_data_menu.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/assets/drawio_editing_data.png` & `compliance-trestle-2.2.0/docs/assets/drawio_editing_data.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/assets/sample_ssp.md.jinja` & `compliance-trestle-2.2.0/docs/assets/sample_ssp.md.jinja`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/assets/template_versioning.png` & `compliance-trestle-2.2.0/docs/assets/template_versioning.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/cli.md` & `compliance-trestle-2.2.0/docs/cli.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/contributing/DCO.md` & `compliance-trestle-2.2.0/docs/contributing/DCO.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/contributing/plugins.md` & `compliance-trestle-2.2.0/docs/contributing/plugins.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/contributing/trestle_oscal_object_model.md` & `compliance-trestle-2.2.0/docs/contributing/trestle_oscal_object_model.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/contributing/website.md` & `compliance-trestle-2.2.0/docs/contributing/website.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/css/mkdocstrings.css` & `compliance-trestle-2.2.0/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/demonstrations-content.md` & `compliance-trestle-2.2.0/docs/demonstrations-content.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/license.md` & `compliance-trestle-2.2.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/plugins/compliance-trestle-fedramp.md` & `compliance-trestle-2.2.0/docs/plugins/compliance-trestle-fedramp.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/python_trestle_setup.md` & `compliance-trestle-2.2.0/docs/python_trestle_setup.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.png` & `compliance-trestle-2.2.0/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.xlsx` & `compliance-trestle-2.2.0/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/reference/third-party-result-schema-SCC.md` & `compliance-trestle-2.2.0/docs/reference/third-party-result-schema-SCC.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/trestle_author.md` & `compliance-trestle-2.2.0/docs/trestle_author.md`

 * *Files 2% similar despite different names*

```diff
@@ -587,14 +587,29 @@
 
 2. To assemble markdowns to a JSON profile
 
 > trestle author profile-assemble
 
 The `profile` author commands allow you to edit additions made by a profile to its imported controls that end up in the final resolved profile catalog.  Only the additions may be edited or added to the generated markdown control files - and those additions can then be assembled into a new version of the original profile, with those additions.  For more details on its usage please see [the profile authoring tutorial](https://ibm.github.io/compliance-trestle/tutorials/ssp_profile_catalog_authoring/ssp_profile_catalog_authoring).
 
+### Profile generation with inheritance
+
+CLI evocation:
+
+> trestle author profile-inherit
+
+The `profile-inherit` sub-command takes a given parent profile and filters its imported controls based inherited controls from a given SSP.
+
+The leveraged SSP is evaluated based on whether provided and responsibility statements for all `by-component` fields are set for each applicable control, as well as the implementation status.
+All components must have exported provided statements, no exported responsibility statements, and an implementation status of `implemented` in order for a control to be filtered from the output profile (i.e. controls delta profile).
+
+As with the other related author commands, if an existing destination file already exists, it is not updated if no changes would be made.
+
+For more details on its usage please see [the ssp-filter tutorial](https://ibm.github.io/compliance-trestle/tutorials/ssp_profile_catalog_authoring/ssp_profile_catalog_authoring).
+
 ### SSP authoring
 
 CLI evocation:
 
 1. To generate markdowns for editing SSP
 
 > trestle author ssp-generate
@@ -609,22 +624,24 @@
 
 ### SSP Content Filtering
 
 CLI evocation:
 
 > trestle author ssp-filter
 
-The `ssp-filter` sub-command takes a given SSP and filters its contents based on a given profile, list of components, and/or control implementation status.
+The `ssp-filter` sub-command takes a given SSP and filters its contents based on a given profile, list of components, control implementation status and/or control origination.
 
 If filtering by profile, the SSP is assumed to contain a superset of controls needed by the profile, and the filter operation generates a new SSP with just the controls needed by that profile.  If the profile references a control not in the SSP, the routine fails with an error.
 
-If filtering by components, a colon-delimited list of components should be provided, with `This system` as the default name for the overall required component for the entire system.  Case and spaces are ignored in the component names, so the names could be specified as `--components "this system: my component"`.  The resulting, filtered ssp will have updated implementated requirements with filtered by_components on each requirement, and filtered by_components on each statement.
+If filtering by components, a colon-delimited list of components should be provided, with `This system` as the default name for the overall required component for the entire system.  Case and spaces are ignored in the component names, so the names could be specified as `--components "this system: my component"`.  The resulting, filtered ssp will have updated implemented requirements with filtered by_components on each requirement, and filtered by_components on each statement.
+
+If filtering by control implementation status, a comma-delimited list of implementation status values should be provided. These values must comply with the OSCAL SSP format references's allowed values, which are as follows: implemented, partial, planned, alternative, and not-applicable.
 
-If filtering by control implementation status, a comma-demilited list of implementation status values should be provided. These values must comply with the OSCAL SSP format references's allowed values, which are as follows: implemented, partial, planned, alternative, and not-applicable.
+If filtering by control origination, a comma-delimited list of control origination values should be provided. These values must comply with the OSCAL SSP format references's allowed values for the control origination property, which are as follows: system-specific, inherited, organization, customer-configured, and customer-provided.
 
-You may filter by a combination of a profile, list of component names, and implementation statuses.
+You may filter by a combination of a profile, list of component names, implementation statuses, and control origination values.
 
 As with the other related author commands, if an existing destination file already exists, it is not updated if no changes would be made.
 
 For more details on its usage please see [the ssp-filter tutorial](https://ibm.github.io/compliance-trestle/tutorials/ssp_profile_catalog_authoring/ssp_profile_catalog_authoring).
 
 </details>
```

### Comparing `compliance-trestle-2.1.1/docs/trestle_author_jinja.md` & `compliance-trestle-2.2.0/docs/trestle_author_jinja.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/continuous-compliance/ContinuousCompliance.drawio` & `compliance-trestle-2.2.0/docs/tutorials/continuous-compliance/ContinuousCompliance.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/continuous-compliance/ContinuousCompliance.jpg` & `compliance-trestle-2.2.0/docs/tutorials/continuous-compliance/ContinuousCompliance.jpg`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/continuous-compliance/continuous-compliance.md` & `compliance-trestle-2.2.0/docs/tutorials/continuous-compliance/continuous-compliance.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.drawio` & `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.png` & `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/profile_does.drawio` & `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/profile_does.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/profile_does.png` & `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/profile_does.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.drawio` & `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.png` & `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.drawio` & `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.png` & `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.drawio` & `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.png` & `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/ssp_profile_catalog_authoring/ssp_profile_catalog_authoring.md` & `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/ssp_profile_catalog_authoring.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 <summary>The author commands</summary>
 
 The author commands are:
 
 1. `catalog-generate` converts a control Catalog to individual controls in markdown format for addition or editing of guidance prose and parameters, with parameters stored in a yaml header at the top of the markdown file.  `catalog-assemble` then gathers the prose and parameters and updates the controls in the Catalog to make a new OSCAL Catalog.
 1. `profile-generate` takes a given Profile and converts the controls represented by its resolved profile catalog to individual controls in markdown format, with sections corresponding to the content that the Profile adds to the Catalog, along with both the current values of parameters in the resolved profile catalog - and the values that are being modified by the given profile's SetParameters.  The user may edit the content or add more, and `profile-assemble` then gathers the updated content and creates a new OSCAL Profile that includes those changes.
 1. `profile-resolve` is special as an authoring tool because it does not involve markdown and instead it simply creates a JSON resolved profile catalog from a specified JSON profile in the trestle directory.  There are options to specify whether or not parameters get replace in the control prose or not, along with any special brackets that might be desired to indicate the parameters embedded in the prose.
+1. `profile-inherit` takes a given parent profile and filters its contents based on the inherited controls included in a given ssp to be include in the final profile.
 1. `component-generate` takes a given ComponentDefinition file and represents all the controls in markdown in separate directories for each Component in the file.  This allows editing of the prose on a per-component basis.  `component-assemble` then assembles the markdown for all controls in all component directories into a new, or the same, ComponentDefinition file.
 1. `ssp-generate` takes a given Profile and an optional list of component-definitions, and represents the individual controls as markdown files with sections that prompt for prose regarding the implementation response for items in the statement of the control, with separate response sections for each component.  `ssp-assemble` then gathers the response sections and creates an OSCAL System Security Plan comprising the resolved profile catalog and the implementation responses for each component.  The list of component-definitions is optional, but without them the SSP will only have one component: `This System`.  Rules, parameters and status associated with the implemented requirements are stored in the SetParameters and Properties of the components in the component definitions and represented in the markdown, allowing changes to be made to the parameter values and status.  These edits are then included in the assembled SSP.  Note that the rules themselves may not be edited and strictly correspond to what is in the component definitions.
 1. `ssp-filter` takes a given ssp and filters its contents based on the controls included in a provided profile, or in a list of components to be included in the final ssp.
 
 In summary, the `catalog` tools allow conversion of a Catalog to markdown for editing - and back again to a Catalog.  The `profile` tools similarly convert a Profile's resolved profile catalog to markdown and allow conversion to a new Profile with modified additions that get applied in resolving the profile catalog.  `component` tools perform similarly for ComponentDefinitions.  Finally, the `ssp` tools allow the addition of implementation prose to the markdown of a system security plan, which is then assembled into a JSON SSP on a by-component basis.
 
 Note that the original ssp implementation in trestle created SSP's by adding prose directly to the SSP markdown on a per-component basis, and there was no connection with separate ComponentDefinition JSON files.  This is now changed so that control responses can be added to the ComponentDefinition and then merged to create the SSP markdown.  In addition, rules and status are captured in the component definition as properties that propogate via markdown into the assembled SSP.  The OSCAL schema doesn't include a form of implementation status for components in the component definition, which is why trestle embeds the status value in the properties.  Similarly, rules and rule parameter values are not currently part of the schema, so they are also embedded in properties.
@@ -520,14 +521,59 @@
 
 Similar options apply to the `jinja` authoring commands.
 
 </details>
 
 <details markdown>
 
+<summary>trestle author profile-inherit</summary>
+
+The `trestle author profile-inherit` command is different from the `generate/assemble` commands because it doesn't involve markdown and instead
+it takes an parent profile and ssp and creates child profile in `JSON` format.
+
+When utilizing a process with leveraged authorizations, use the command `trestle author profile-inherit` to create a profile with initial content using a parent profile and SSP with inheritable controls. The provided and responsibility statements for all `by-component` fields, as well as the implementation status, will be used to evaluate the leveraged SSP.
+To be filtered from the output profile (i.e. controls delta profile), all components must have exported provided statements, no exported responsibility statements, and an implementation status of `implemented`.
+
+The filter command is invoked as:
+
+`trestle author profile-inherit --profile my_parent --ssp my_leveraged_ssp --output controls_delta_profile`
+
+Both the parent profile and the SSP must be present in the trestle workspace. This command produces a new workspace profile that imports the parent profile and filters the inherited controls from the SSP using the `exclude-controls` and `include-controls` fields in the profile import.
+
+<details markdown>
+
+<summary>Example imports generated from profile-inherit</summary>
+
+```json
+  "imports": [
+      {
+        "href": "trestle://profiles/controls_delta/profile.json",
+        "include-controls": [
+          {
+            "with-ids": [
+              "ac-2"
+            ]
+          }
+        ],
+        "exclude-controls": [
+          {
+            "with-ids": [
+              "ac-1"
+            ]
+          }
+        ]
+      }
+    ]
+```
+
+</details>
+</details>
+
+<details markdown>
+
 <summary>trestle author component-generate and component-assemble</summary>
 
 The `trestle author component-generate` command takes a JSON ComponentDefinition file and creates markdown for its controls in separate directories for each of the DefinedComponents in the file.  This allows specifying the implementation response and status for each component separately in separate markdown files for a control.  In addition, the markdown captures Rules in the control that specify descriptions and parameter values that apply to the expected responses.
 
 The command has few options compared to other author commands and only requires specifying `--name` and `--output` for the ComponentDefinition and output markdown directory, respectively.
 
 Here is an example of the generated markdown for the component `OSCO` in the ComponentDefinition file.  Note that this file will be under the subdirectory `OSCO/source_name` of the specified output directory - and any other DefinedComponents will have corresponding subdirectories level with the `OSCO` one.  Here `source_name` refers to the name of the profile or catalog in the ComponentDefinition that is the source for this control.  The control markdown files are written into directories split by both component name and source name.  If the source refers to a general uri and not a named profile or catalog in the trestle directory, then names such as `source_001` and `source_002` are assigned.  The actual source title can be found in the yaml header of any of the control markdown files.
@@ -1006,21 +1052,21 @@
 
 </details>
 
 <details markdown>
 
 <summary>trestle author ssp-filter</summary>
 
-Once you have an SSP in the trestle directory you can filter its contents with a profile, list of components, or list of implementation status values by using the command `trestle author ssp-filter`.  The SSP is assumed to contain a superset of the controls needed by the profile if a profile is specified, and the filter operation will generate a new SSP with only those controls needed by the profile.  If a list of component names is provided, only the specified components will appear in the system implementation of the ssp. If a list of implementation statuses is provided, controls with implementations including those statuses will appear in the control implementation of the ssp.
+Once you have an SSP in the trestle directory you can filter its contents with a profile, list of components, list of implementation statuses, or list control origination values by using the command `trestle author ssp-filter`.  The SSP is assumed to contain a superset of the controls needed by the profile if a profile is specified, and the filter operation will generate a new SSP with only those controls needed by the profile.  If a list of component names is provided, only the specified components will appear in the system implementation of the ssp. If a list of implementation statuses is provided, controls with implementations including those statuses will appear in the control implementation of the ssp. Similarly, if a list of control origination values is provided, implemented requirements with a control origination property value included in the provided values will appear in the control implementation of the ssp.
 
 The filter command is invoked as:
 
-`trestle author ssp-filter --name my_ssp --profile my_profile --components comp_a:comp_b --implementation-status "planned,partial" --output my_culled_ssp`
+`trestle author ssp-filter --name my_ssp --profile my_profile --components comp_a:comp_b --implementation-status "planned,partial" --control-origination "customer-configured" --output my_culled_ssp`
 
-The SSP must be present in the trestle workspace and, if filtering by profile, that profile must also be in the trestle workspace. This command will generate a new SSP in the workspace. If the profile makes reference to a control not in the SSP then the routine will fail with an error message.  Similarly, if one of the components is not present in the ssp the routine will also fail. The implementation statuses must be one of the allowed values as defined in the OSCAL SSP JSON format reference. Those include the following: implemented, partial, planned, alternative, and not-applicable. If an invalid value is provided, an error is returned.
+The SSP must be present in the trestle workspace and, if filtering by profile, that profile must also be in the trestle workspace. This command will generate a new SSP in the workspace. If the profile makes reference to a control not in the SSP then the routine will fail with an error message.  Similarly, if one of the components is not present in the ssp the routine will also fail. The implementation statuses must be one of the allowed values as defined in the OSCAL SSP JSON format reference. Those include the following: implemented, partial, planned, alternative, and not-applicable. If an invalid value is provided, an error is returned. The control origination values also must be one of the allowed values as defined in the OSCAL SSP JSON format reference. Those include the following: system-specific, inherited, customer-configured, customer-provided, and organization. If an invalid value is provided, an error is returned.
 
 </details>
 
 <details markdown>
 
 <summary>Summary of options used by the catalog, profile, component and ssp authoring tools.</summary>
```

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.csv-to-oscal-cd/component-definition.json` & `compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/component-definition.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.csv-to-oscal-cd/ocp4-sample-input.csv` & `compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/ocp4-sample-input.csv`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.csv-to-oscal-cd/transformation.md` & `compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/transformation.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/transformation.md` & `compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/transformation.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/demo-ocp4-cis-profile-to-oscal-cd.config` & `compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/demo-ocp4-cis-profile-to-oscal-cd.config`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/enabled_rules.json` & `compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/enabled_rules.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/transformation.md` & `compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/transformation.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.tanium-result-to-oscal-ar/800px-Australia_scarsdale_nimons_bridge.jpg` & `compliance-trestle-2.2.0/docs/tutorials/task.tanium-result-to-oscal-ar/800px-Australia_scarsdale_nimons_bridge.jpg`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.tanium-result-to-oscal-ar/transformation.md` & `compliance-trestle-2.2.0/docs/tutorials/task.tanium-result-to-oscal-ar/transformation.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.transformer-construction/assessment-results-nist.png` & `compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/assessment-results-nist.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.transformer-construction/assessment-results.drawio` & `compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/assessment-results.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.transformer-construction/assessment-results.jpg` & `compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/assessment-results.jpg`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.transformer-construction/transformer-construction.drawio` & `compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/transformer-construction.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.transformer-construction/transformer-construction.jpg` & `compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/transformer-construction.jpg`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/task.transformer-construction/transformer-construction.md` & `compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/transformer-construction.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/docs/tutorials/trestle_sample_workflow.md` & `compliance-trestle-2.2.0/docs/tutorials/trestle_sample_workflow.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/internal_spec_documents/caching_spec.md` & `compliance-trestle-2.2.0/internal_spec_documents/caching_spec.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/internal_spec_documents/trestle-spec.md` & `compliance-trestle-2.2.0/internal_spec_documents/trestle-spec.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/internal_spec_documents/trestle-task-spec.md` & `compliance-trestle-2.2.0/internal_spec_documents/trestle-task-spec.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/mkdocs.yml` & `compliance-trestle-2.2.0/mkdocs.yml`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,15 @@
       - ssp: api_reference/trestle.oscal.ssp.md
     - tasks:
       - base_task: api_reference/trestle.tasks.base_task.md
       - cis_xlsx_to_oscal_catalog: api_reference/trestle.tasks.cis_xlsx_to_oscal_catalog.md
       - csv_to_oscal_cd: api_reference/trestle.tasks.csv_to_oscal_cd.md
       - ocp4_cis_profile_to_oscal_catalog: api_reference/trestle.tasks.ocp4_cis_profile_to_oscal_catalog.md
       - ocp4_cis_profile_to_oscal_cd: api_reference/trestle.tasks.ocp4_cis_profile_to_oscal_cd.md
+      - oscal_catalog_to_csv: api_reference/trestle.tasks.oscal_catalog_to_csv.md
       - oscal_profile_to_osco_profile: api_reference/trestle.tasks.oscal_profile_to_osco_profile.md
       - osco_result_to_oscal_ar: api_reference/trestle.tasks.osco_result_to_oscal_ar.md
       - tanium_result_to_oscal_ar: api_reference/trestle.tasks.tanium_result_to_oscal_ar.md
       - transform: api_reference/trestle.tasks.transform.md
       - xccdf_result_to_oscal_ar: api_reference/trestle.tasks.xccdf_result_to_oscal_ar.md
       - xlsx_helper: api_reference/trestle.tasks.xlsx_helper.md
       - xlsx_to_oscal_cd: api_reference/trestle.tasks.xlsx_to_oscal_cd.md
```

### Comparing `compliance-trestle-2.1.1/scripts/cleanup.py` & `compliance-trestle-2.2.0/scripts/cleanup.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/experiments/README.md` & `compliance-trestle-2.2.0/scripts/experiments/README.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/experiments/json_serialize_ben.py` & `compliance-trestle-2.2.0/scripts/experiments/json_serialize_ben.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/experiments/tanium_ben.py` & `compliance-trestle-2.2.0/scripts/experiments/tanium_ben.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/flatten_schema.py` & `compliance-trestle-2.2.0/scripts/flatten_schema.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/gen_oscal.py` & `compliance-trestle-2.2.0/scripts/gen_oscal.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/have_files_changed.py` & `compliance-trestle-2.2.0/scripts/have_files_changed.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/order_classes.py` & `compliance-trestle-2.2.0/scripts/order_classes.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/oscal_normalize.py` & `compliance-trestle-2.2.0/scripts/oscal_normalize.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/schema_integrity.py` & `compliance-trestle-2.2.0/scripts/schema_integrity.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/simplify_catalog.py` & `compliance-trestle-2.2.0/scripts/simplify_catalog.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/simplify_retain_ac.py` & `compliance-trestle-2.2.0/scripts/simplify_retain_ac.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/tanium_transform_script.py` & `compliance-trestle-2.2.0/scripts/tanium_transform_script.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/update_uuids.py` & `compliance-trestle-2.2.0/scripts/update_uuids.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/utf8me.py` & `compliance-trestle-2.2.0/scripts/utf8me.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/scripts/website_automation.py` & `compliance-trestle-2.2.0/scripts/website_automation.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/setup.cfg` & `compliance-trestle-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/setup.py` & `compliance-trestle-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/__init__.py` & `compliance-trestle-2.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/conftest.py` & `compliance-trestle-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_extra_fields_compressed.drawio` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_extra_fields_compressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_missing_fields_compressed.drawio` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_missing_fields_compressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_metadata_compressed.drawio` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_metadata_compressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_metadata_uncompressed.drawio` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_metadata_uncompressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_bad_internal_structure.drawio` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_bad_internal_structure.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_compressed.drawio` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_compressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed.drawio` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed_mangled.drawio` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed_mangled.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/two_tabs_metadata_compressed.drawio` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/two_tabs_metadata_compressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_bad_md.drawio` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_bad_md.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_compressed.drawio` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_compressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/test_2_md_with_md_header/template.md` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/test_2_md_with_md_header/template.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_000.md` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_000.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_001.md` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_001.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_002.md` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_002.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/test_3_md_hand_edited/template.md` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/template.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/0.0.1/test_4_md_format_extras/correct_instance_extra_features.md` & `compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/correct_instance_extra_features.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/controls/control_with_bad_component.md` & `compliance-trestle-2.2.0/tests/data/author/controls/control_with_bad_component.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/controls/control_with_bad_system_comp.md` & `compliance-trestle-2.2.0/tests/data/author/controls/control_with_bad_system_comp.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/controls/control_with_components.md` & `compliance-trestle-2.2.0/tests/data/author/controls/control_with_components.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/controls/control_with_components_and_param_template.md` & `compliance-trestle-2.2.0/tests/data/author/controls/control_with_components_and_param_template.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/controls/control_with_components_and_params.md` & `compliance-trestle-2.2.0/tests/data/author/controls/control_with_components_and_params.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/controls/control_with_double_comp.md` & `compliance-trestle-2.2.0/tests/data/author/controls/control_with_double_comp.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_bad_content/network.md` & `compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_bad_content/network.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_mixed_name/architecture.md` & `compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_mixed_name/architecture.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/governed_folders/bad_instance_renamed/network.md` & `compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_renamed/network.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/governed_folders/folder_with_bad_drawio/diagram.drawio` & `compliance-trestle-2.2.0/tests/data/author/governed_folders/folder_with_bad_drawio/diagram.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance/network.md` & `compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance/network.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_limits_of_changes/network.md` & `compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_limits_of_changes/network.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_with_readme/network.md` & `compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_readme/network.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/governed_folders/good_instance_with_version/diagram.drawio` & `compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_version/diagram.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/diagram.drawio` & `compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/diagram.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/diagram.drawio` & `compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/diagram.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/governed_folders/template_folder_with_drawio/diagram.drawio` & `compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_drawio/diagram.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/governed_folders/template_folder_with_version/diagram.drawio` & `compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_version/diagram.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/bad_templates_drawio/template.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_drawio/template.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/bad_templates_md/template.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_md/template.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/bad_templates_wrong_names/templatesss.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_wrong_names/templatesss.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/empty_headers/a.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/empty_headers/a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_drawio/whos_is_this.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio/whos_is_this.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_drawio_bad_file/a_markdown_file.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio_bad_file/a_markdown_file.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_md/my_drawio.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md/my_drawio.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/fails_validation_md_bad_file/a.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md_bad_file/a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/good_templates/template.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/good_templates/template.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/correct_a.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/correct_a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/correct_b.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/correct_b.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/ignored_files/deep/even_deeper/correct_a.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/even_deeper/correct_a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/meets_templates/a.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/meets_templates/a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/meets_templates/d.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/meets_templates/d.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/passes_with_extraneous_files/a.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/passes_with_extraneous_files/a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/passes_with_extraneous_files/d.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/passes_with_extraneous_files/d.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/recursive_pass/a.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/recursive_pass/d.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/d.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/recursive_pass/some_depth/a.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/some_depth/a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/headers/recursive_pass/some_depth/d.drawio` & `compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/some_depth/d.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/author/ssp/ssp_example.json` & `compliance-trestle-2.2.0/tests/data/author/ssp/ssp_example.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/csv/bp.sample.v2.csv` & `compliance-trestle-2.2.0/tests/data/csv/bp.sample.v2.csv`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/csv/component-definitions/bp/component-definition.json` & `compliance-trestle-2.2.0/tests/data/csv/component-definitions/bp/component-definition.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/csv/ocp4-user.v2.csv` & `compliance-trestle-2.2.0/tests/data/csv/ocp4-user.v2.csv`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/jinja/ssp_template.md.jinja` & `compliance-trestle-2.2.0/tests/data/jinja/ssp_template.md.jinja`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/jinja_markdown_include/env_nested_c_c_double.md` & `compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_nested_c_c_double.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/comp_def.json` & `compliance-trestle-2.2.0/tests/data/json/comp_def.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/comp_def_a.json` & `compliance-trestle-2.2.0/tests/data/json/comp_def_a.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/comp_def_b.json` & `compliance-trestle-2.2.0/tests/data/json/comp_def_b.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999799061213992%*

 * *Differences: {"'component-definition'": "{'components': {0: {'control-implementations': {0: "*

 * *                           "{'implemented-requirements': {0: {'props': {insert: [(2, "*

 * *                           "OrderedDict([('name', 'control-origination'), ('value', "*

 * *                           "'system-specific')])), (3, OrderedDict([('name', "*

 * *                           "'control-origination'), ('value', 'customer-configured')]))]}}}}}}, 1: "*

 * *                           "{'control-implementations': {0: {'implemented-requ […]*

```diff
@@ -13,14 +13,22 @@
                                     {
                                         "name": "Rule_Id",
                                         "value": "top_shared_rule_1"
                                     },
                                     {
                                         "name": "implementation-status",
                                         "value": "implemented"
+                                    },
+                                    {
+                                        "name": "control-origination",
+                                        "value": "system-specific"
+                                    },
+                                    {
+                                        "name": "control-origination",
+                                        "value": "customer-configured"
                                     }
                                 ],
                                 "responsible-roles": [
                                     {
                                         "party-uuids": [
                                             "ce1f379a-fcdd-485a-a7b7-6f02c0763dd2"
                                         ],
@@ -161,14 +169,18 @@
                                     {
                                         "name": "Rule_Id",
                                         "value": "rule_1"
                                     },
                                     {
                                         "name": "implementation-status",
                                         "value": "implemented"
+                                    },
+                                    {
+                                        "name": "control-origination",
+                                        "value": "system-specific"
                                     }
                                 ],
                                 "responsible-roles": [
                                     {
                                         "party-uuids": [
                                             "ce1f379a-fcdd-485a-a7b7-6f02c0763dd2"
                                         ],
```

### Comparing `compliance-trestle-2.1.1/tests/data/json/comp_def_readme.md` & `compliance-trestle-2.2.0/tests/data/json/comp_def_readme.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/comp_prof.json` & `compliance-trestle-2.2.0/tests/data/json/comp_prof.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/comp_prof_aa.json` & `compliance-trestle-2.2.0/tests/data/json/comp_prof_aa.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/comp_prof_ab.json` & `compliance-trestle-2.2.0/tests/data/json/comp_prof_ab.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/comp_prof_ba.json` & `compliance-trestle-2.2.0/tests/data/json/comp_prof_ba.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/comp_prof_bad.json` & `compliance-trestle-2.2.0/tests/data/json/comp_prof_bad.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/comp_prof_bb.json` & `compliance-trestle-2.2.0/tests/data/json/comp_prof_bb.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/minimal_catalog.json` & `compliance-trestle-2.2.0/tests/data/json/minimal_catalog.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/minimal_catalog_bad_oscal_version.json` & `compliance-trestle-2.2.0/tests/data/json/minimal_catalog_bad_oscal_version.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/minimal_catalog_extra_fields.json` & `compliance-trestle-2.2.0/tests/data/json/minimal_catalog_extra_fields.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/minimal_catalog_roles.json` & `compliance-trestle-2.2.0/tests/data/json/minimal_catalog_roles.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/minimal_catalog_roles_double.json` & `compliance-trestle-2.2.0/tests/data/json/minimal_catalog_roles_double.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/minimal_catalog_roles_double_rp.json` & `compliance-trestle-2.2.0/tests/data/json/minimal_catalog_roles_double_rp.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/minimal_catalog_with_groups.json` & `compliance-trestle-2.2.0/tests/data/json/minimal_catalog_with_groups.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/nist_tutorial_catalog.json` & `compliance-trestle-2.2.0/tests/data/json/nist_tutorial_catalog.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/nist_tutorial_profile.json` & `compliance-trestle-2.2.0/tests/data/json/nist_tutorial_profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/profile_bad_control.json` & `compliance-trestle-2.2.0/tests/data/json/profile_bad_control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/profile_missing_position.json` & `compliance-trestle-2.2.0/tests/data/json/profile_missing_position.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/profile_with_alter_props.json` & `compliance-trestle-2.2.0/tests/data/json/profile_with_alter_props.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/profile_with_alter_subparts.json` & `compliance-trestle-2.2.0/tests/data/json/profile_with_alter_subparts.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/profile_with_incorrect_alter.json` & `compliance-trestle-2.2.0/tests/data/json/profile_with_incorrect_alter.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/pull_nist_profile.json` & `compliance-trestle-2.2.0/tests/data/json/pull_nist_profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/simple_catalog_no_parts.json` & `compliance-trestle-2.2.0/tests/data/json/simple_catalog_no_parts.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/simple_mapping.json` & `compliance-trestle-2.2.0/tests/data/json/simple_mapping.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/simple_test_profile.json` & `compliance-trestle-2.2.0/tests/data/json/simple_test_profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/simple_test_profile_no_params.json` & `compliance-trestle-2.2.0/tests/data/json/simple_test_profile_no_params.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/simplified_nist_catalog.json` & `compliance-trestle-2.2.0/tests/data/json/simplified_nist_catalog.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/simplified_nist_profile.json` & `compliance-trestle-2.2.0/tests/data/json/simplified_nist_profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/test_profile_a.json` & `compliance-trestle-2.2.0/tests/data/json/test_profile_a.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/test_profile_b.json` & `compliance-trestle-2.2.0/tests/data/json/test_profile_b.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/test_profile_c.json` & `compliance-trestle-2.2.0/tests/data/json/test_profile_c.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/test_profile_d.json` & `compliance-trestle-2.2.0/tests/data/json/test_profile_d.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/test_profile_e.json` & `compliance-trestle-2.2.0/tests/data/json/test_profile_e.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/test_profile_f.json` & `compliance-trestle-2.2.0/tests/data/json/test_profile_f.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/json/test_profile_g.json` & `compliance-trestle-2.2.0/tests/data/json/test_profile_g.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/markdown/valid_complex_md.md` & `compliance-trestle-2.2.0/tests/data/markdown/valid_complex_md.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/markdown/valid_no_headers.md` & `compliance-trestle-2.2.0/tests/data/markdown/valid_no_headers.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/markdown/valid_no_lvl1_headers.md` & `compliance-trestle-2.2.0/tests/data/markdown/valid_no_lvl1_headers.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/ocp4-cis/catalog.json` & `compliance-trestle-2.2.0/tests/data/ocp4-cis/catalog.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/.trestle/config.ini` & `compliance-trestle-2.2.0/tests/data/split_merge/.trestle/config.ini`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/README.md` & `compliance-trestle-2.2.0/tests/data/split_merge/README.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/load_distributed/catalog.json` & `compliance-trestle-2.2.0/tests/data/split_merge/load_distributed/catalog.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/load_distributed/groups.json` & `compliance-trestle-2.2.0/tests/data/split_merge/load_distributed/groups.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step0-merged_catalog/catalogs/mycatalog/catalog.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step0-merged_catalog/catalogs/mycatalog/catalog.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step0-merged_catalog/next_step.sh` & `compliance-trestle-2.2.0/tests/data/split_merge/step0-merged_catalog/next_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/back-matter.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/back-matter.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/groups.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/groups.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/metadata.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/metadata.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/next_step.sh` & `compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/next_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step1-split_root_elements/previous_step.sh` & `compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/previous_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/back-matter.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/back-matter.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/groups.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/groups.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/parties.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/parties.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/next_step.sh` & `compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/next_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step2-split_metadata_elements/previous_step.sh` & `compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/previous_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/back-matter.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/back-matter.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/groups.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/groups.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/parties.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/parties.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/next_step.sh` & `compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/next_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/previous_step.sh` & `compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/previous_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/back-matter.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/back-matter.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00009__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00010__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00011__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00012__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00013__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00014__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00014__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00015__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00015__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00016__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00016__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00017__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00017__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00018__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00018__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00019__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00019__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00020__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00020__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00021__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00021__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00022__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00022__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00023__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00023__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00024__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00024__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00009__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00010__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00011__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00012__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00013__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00014__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00014__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00015__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00015__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00009__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00010__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00011__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00012__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00013__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00009__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00010__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00011__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00012__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00009__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00010__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00011__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00009__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00009__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00010__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00011__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00012__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00013__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00014__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00014__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00015__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00015__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00016__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00016__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00017__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00017__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00018__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00018__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00019__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00019__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00020__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00020__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00021__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00021__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00022__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00022__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00009__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00010__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00009__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00010__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00011__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00012__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00013__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00014__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00014__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00015__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00015__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00016__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00016__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00017__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00017__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00018__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00018__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00019__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00019__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00020__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00020__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00021__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00021__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00022__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00022__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00023__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00023__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00024__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00024__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00025__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00025__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00026__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00026__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00027__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00027__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00028__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00028__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00029__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00029__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00030__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00030__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00031__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00031__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00009__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00009__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00010__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00011__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00012__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00013__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00014__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00014__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00015__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00015__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00016__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00016__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00017__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00017__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00018__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00018__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00019__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00019__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00020__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00020__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00021__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00021__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00022__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00022__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00009__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00010__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00011__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00012__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00013__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00014__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00014__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00015__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00015__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00016__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00016__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00017__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00017__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00018__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00018__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00019__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00019__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00020__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00020__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00021__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00021__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00022__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00022__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00023__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00023__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00024__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00024__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00025__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00025__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00026__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00026__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00027__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00027__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00028__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00028__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00029__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00029__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00030__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00030__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00031__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00031__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00032__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00032__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00033__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00033__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00034__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00034__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00035__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00035__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00036__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00036__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00037__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00037__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00038__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00038__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00039__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00039__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00040__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00040__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00041__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00041__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00042__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00042__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00043__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00043__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00044__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00044__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00045__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00045__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00046__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00046__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00047__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00047__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00048__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00048__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00049__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00049__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00050__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00050__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00009__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00010__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00011__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00012__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00013__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00014__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00014__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00015__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00015__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00016__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00016__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00017__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00017__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00018__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00018__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00019__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00019__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00020__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00020__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00021__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00021__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00022__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00022__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00000__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00001__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00002__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00003__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00004__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00005__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00006__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00007__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00008__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00009__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00010__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00011__control.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/parties.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/parties.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata.json` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/split_merge/step4_split_groups_array/previous_step.sh` & `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/previous_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/spread-sheet/bad_parameter_name_and_description.xlsx` & `compliance-trestle-2.2.0/tests/data/spread-sheet/bad_parameter_name_and_description.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/spread-sheet/duplicate_column_heading.xlsx` & `compliance-trestle-2.2.0/tests/data/spread-sheet/duplicate_column_heading.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/spread-sheet/embedded_blank_in_goal_name_id.xlsx` & `compliance-trestle-2.2.0/tests/data/spread-sheet/embedded_blank_in_goal_name_id.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/spread-sheet/embedded_blank_in_parameter_name.xlsx` & `compliance-trestle-2.2.0/tests/data/spread-sheet/embedded_blank_in_parameter_name.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/spread-sheet/embedded_blank_in_rule_name_id.xlsx` & `compliance-trestle-2.2.0/tests/data/spread-sheet/embedded_blank_in_rule_name_id.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/spread-sheet/good.xlsx` & `compliance-trestle-2.2.0/tests/data/spread-sheet/good.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/spread-sheet/good_with_blank_rows.xlsx` & `compliance-trestle-2.2.0/tests/data/spread-sheet/good_with_blank_rows.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/spread-sheet/missing_column_heading.xlsx` & `compliance-trestle-2.2.0/tests/data/spread-sheet/missing_column_heading.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/spread-sheet/missing_control_id.xlsx` & `compliance-trestle-2.2.0/tests/data/spread-sheet/missing_control_id.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/spread-sheet/missing_resource_title.xlsx` & `compliance-trestle-2.2.0/tests/data/spread-sheet/missing_resource_title.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/spread-sheet/missing_rule_name_id.xlsx` & `compliance-trestle-2.2.0/tests/data/spread-sheet/missing_rule_name_id.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_RedHat_OpenShift_Container_Platform_Benchmark_v1.2.0-2.snippet.xlsx` & `compliance-trestle-2.2.0/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_RedHat_OpenShift_Container_Platform_Benchmark_v1.2.0-2.snippet.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_Red_Hat_Enterprise_Linux_8_Benchmark_v2.0.0.snippet.xlsx` & `compliance-trestle-2.2.0/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_Red_Hat_Enterprise_Linux_8_Benchmark_v2.0.0.snippet.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input/cis.profile` & `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input/cis.profile`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input-bogus/cis.profile` & `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input-bogus/cis.profile`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules.json` & `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules2.json` & `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules2.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/rule2var.json` & `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/rule2var.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules.json` & `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules2.json` & `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules2.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/output/component-definition.json` & `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/output/component-definition.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis-node.profile` & `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis-node.profile`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis.profile` & `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis.profile`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test2.profile` & `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test2.profile`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd.config` & `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd.config`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd2.config` & `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd2.config`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd3.config` & `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd3.config`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-no.json` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-no.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-yes.json` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-yes.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-no.json` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-no.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-yes.json` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-yes.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.2.0-parms-no.json` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.2.0-parms-no.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-1.0.0-parms-yes.json` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-1.0.0-parms-yes.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-no.json` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-no.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-yes.json` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-yes.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-scc.json` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-scc.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile.json` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-no/osco-profile.yaml` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-no/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-yes/osco-profile.yaml` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-yes/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-no/osco-profile.yaml` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-no/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-yes/osco-profile.yaml` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-yes/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.2.0-parms-no/osco-profile.yaml` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.2.0-parms-no/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-1.0.0-parms-yes/osco-profile.yaml` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-1.0.0-parms-yes/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-no/osco-profile.yaml` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-no/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-yes/osco-profile.yaml` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-yes/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-scc/tailored-profile.yaml` & `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-scc/tailored-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/input/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml` & `compliance-trestle-2.2.0/tests/data/tasks/osco/input/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/input-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml` & `compliance-trestle-2.2.0/tests/data/tasks/osco/input-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/input-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.yaml` & `compliance-trestle-2.2.0/tests/data/tasks/osco/input-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/input-configmaps/configmaps.yaml` & `compliance-trestle-2.2.0/tests/data/tasks/osco/input-configmaps/configmaps.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/input-fetcher/cluster_resource.json` & `compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_data.json` & `compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_data.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind0.json` & `compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind0.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind1.json` & `compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind1.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_resources.json` & `compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_resources.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_results.json` & `compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_results.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/input-xml-ocp4/ocp4-check-result.xml` & `compliance-trestle-2.2.0/tests/data/tasks/osco/input-xml-ocp4/ocp4-check-result.xml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/input-xml-rhel7/rhel7-check-result.xml` & `compliance-trestle-2.2.0/tests/data/tasks/osco/input-xml-rhel7/rhel7-check-result.xml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/osco/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/osco/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/osco/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/output-configmaps/configmaps.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/osco/output-configmaps/configmaps.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/output-fetcher/cluster_resource.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/cluster_resource.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/output-xml-ocp4/ocp4-check-result.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/osco/output-xml-ocp4/ocp4-check-result.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/osco/output-xml-rhel7/rhel7-check-result.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/osco/output-xml-rhel7/rhel7-check-result.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/tanium/input/Tanium.comply-results-json` & `compliance-trestle-2.2.0/tests/data/tasks/tanium/input/Tanium.comply-results-json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/tanium/input-doc/Tanium.doc-json` & `compliance-trestle-2.2.0/tests/data/tasks/tanium/input-doc/Tanium.doc-json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/tanium/output/Tanium.oscal.2020.json` & `compliance-trestle-2.2.0/tests/data/tasks/tanium/output/Tanium.oscal.2020.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/tanium/output/Tanium.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/tanium/output/Tanium.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xccdf/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/xccdf/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-configmaps/configmaps.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-configmaps/configmaps.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-fetcher/cluster_resource.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/cluster_resource.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-xml-ocp4/ocp4-check-result.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-xml-ocp4/ocp4-check-result.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xccdf/output-xml-rhel7/rhel7-check-result.oscal.json` & `compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-xml-rhel7/rhel7-check-result.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xlsx/output/component-definition.json` & `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output/component-definition.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xlsx/output/profile.json` & `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-by-check/profile.json` & `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-check/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-by-control/profile.json` & `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-control/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-by-rule/profile.json` & `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-rule/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-filtered/profile.json` & `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-filtered/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-missing-control-id/profile.json` & `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-missing-control-id/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xlsx/output-missing-rule-name-id/profile.json` & `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-missing-rule-name-id/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/tasks/xlsx/test-xlsx-to-oscal-cd.config` & `compliance-trestle-2.2.0/tests/data/tasks/xlsx/test-xlsx-to-oscal-cd.config`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/yaml/bad_component_dup_uuid.yaml` & `compliance-trestle-2.2.0/tests/data/yaml/bad_component_dup_uuid.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/yaml/bad_component_no_tz.yaml` & `compliance-trestle-2.2.0/tests/data/yaml/bad_component_no_tz.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/yaml/good_component.yaml` & `compliance-trestle-2.2.0/tests/data/yaml/good_component.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/yaml/good_component_diff_tz.yaml` & `compliance-trestle-2.2.0/tests/data/yaml/good_component_diff_tz.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/data/yaml/header_with_metadata.yaml` & `compliance-trestle-2.2.0/tests/data/yaml/header_with_metadata.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/functionality/__init__.py` & `compliance-trestle-2.2.0/tests/functionality/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/functionality/chevron_test.py` & `compliance-trestle-2.2.0/tests/functionality/chevron_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/functionality/example_test.py` & `compliance-trestle-2.2.0/tests/functionality/example_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/functionality/pathlib_test.py` & `compliance-trestle-2.2.0/tests/functionality/pathlib_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/manual_tests/split_test_1.sh` & `compliance-trestle-2.2.0/tests/manual_tests/split_test_1.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/manual_tests/split_test_issue_630.sh` & `compliance-trestle-2.2.0/tests/manual_tests/split_test_issue_630.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/manual_tests/split_validate_test.sh` & `compliance-trestle-2.2.0/tests/manual_tests/split_validate_test.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/manual_tests/test_binary.sh` & `compliance-trestle-2.2.0/tests/manual_tests/test_binary.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/test_utils.py` & `compliance-trestle-2.2.0/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from trestle.core.commands.import_ import ImportCmd
 from trestle.core.models.file_content_type import FileContentType
 from trestle.core.repository import Repository
 from trestle.oscal import catalog as cat
 from trestle.oscal import common
 from trestle.oscal import component as comp
 from trestle.oscal import profile as prof
+from trestle.oscal import ssp
 
 if file_utils.is_windows():  # pragma: no cover
     import win32api
     import win32con
 
 logger = logging.getLogger(__name__)
 
@@ -402,14 +403,36 @@
         repo.load_and_import_model(cat_path, cat_name)
         new_href = f'trestle://catalogs/{cat_name}/catalog.json'
     else:
         new_href = str(cat_path.resolve())
     assert HrefCmd.change_import_href(trestle_root, main_profile_name, new_href, 0) == 0
 
 
+def setup_for_inherit(
+    tmp_trestle_dir: pathlib.Path, prof_name: str, output_name: str, ssp_name: str
+) -> argparse.Namespace:
+    """Create the ssp and parent profile for inherit commands."""
+    load_from_json(tmp_trestle_dir, 'simplified_nist_catalog', 'nist_cat', cat.Catalog)
+    if prof_name:
+        load_from_json(tmp_trestle_dir, prof_name, prof_name, prof.Profile)
+    if ssp_name:
+        load_from_json(tmp_trestle_dir, ssp_name, ssp_name, ssp.SystemSecurityPlan)
+
+    args = argparse.Namespace(
+        trestle_root=tmp_trestle_dir,
+        profile=prof_name,
+        output=output_name,
+        ssp=ssp_name,
+        version=None,
+        verbose=0,
+    )
+
+    return args
+
+
 def load_from_json(
     tmp_trestle_dir: pathlib.Path, file_prefix: str, model_name: str, model_type: OscalBaseModel
 ) -> None:
     """Load model from JSON test dir."""
     src_path = JSON_TEST_DATA_PATH / f'{file_prefix}.json'
     dst_path = ModelUtils.get_model_path_for_name_and_class(
         tmp_trestle_dir, model_name, model_type, FileContentType.JSON
```

### Comparing `compliance-trestle-2.1.1/tests/trestle/__init__.py` & `compliance-trestle-2.2.0/tests/trestle/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/cli_test.py` & `compliance-trestle-2.2.0/tests/trestle/cli_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/__init__.py` & `compliance-trestle-2.2.0/tests/trestle/core/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/base_model_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/base_model_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/__init__.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/add_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/add_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/assemble_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/assemble_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/author/__init__.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/author/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/author/catalog_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/author/catalog_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -689,15 +689,15 @@
 
 
 """
 
     file_utils.insert_text_in_file(md_path, '## Control Statement', control_statement_prose_with_parts)
 
     catalog_assemble = 'trestle author catalog-assemble -o my_catalog -m md_catalog'
-    test_utils.execute_command_and_assert(catalog_assemble, 1, monkeypatch)
+    test_utils.execute_command_and_assert(catalog_assemble, 0, monkeypatch)
 
     _, error = capsys.readouterr()
     assert 'Duplicate part id ac-2_smt.a' in error
 
 
 def test_catalog_tab_in_statement(tmp_trestle_dir: pathlib.Path, monkeypatch: MonkeyPatch, capsys) -> None:
     """Test catalog-assemble with tab characters in control statement and parts."""
```

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/author/command_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/author/command_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,42 +18,44 @@
 import sys
 
 from _pytest.monkeypatch import MonkeyPatch
 
 import pytest
 
 import trestle.cli
+from trestle.core.commands.common.return_codes import CmdReturnCodes
 
 
 def test_governed_docs_cli(tmp_trestle_dir: pathlib.Path, monkeypatch: MonkeyPatch) -> None:
     """Test happy path of md governed-docs subcommand."""
     command = 'trestle author docs'
     monkeypatch.setattr(sys, 'argv', command.split())
     with pytest.raises(SystemExit) as wrapped_error:
         trestle.cli.run()
         # FIXME: Needs to be changed once implemented.
     assert wrapped_error.type == SystemExit
-    assert wrapped_error.value.code == 2
+    assert wrapped_error.value.code == CmdReturnCodes.INCORRECT_ARGS.value
 
 
 def test_governed_folders_cli(tmp_trestle_dir: pathlib.Path, monkeypatch: MonkeyPatch) -> None:
     """Test happy path of author governed-folders subcommand."""
     command = 'trestle author folders'
     monkeypatch.setattr(sys, 'argv', command.split())
     with pytest.raises(SystemExit) as wrapped_error:
         trestle.cli.run()
         # FIXME: Needs to be changed once implemented.
     assert wrapped_error.type == SystemExit
-    assert wrapped_error.value.code == 2
+    assert wrapped_error.value.code == CmdReturnCodes.INCORRECT_ARGS.value
 
 
 @pytest.mark.parametrize(
     'command_string', [('trestle author docs setup -tn test'), ('trestle author folders setup -tn test')]
 )
 def test_failure_not_trestle(command_string, tmp_path: pathlib.Path, monkeypatch: MonkeyPatch) -> None:
     """Test for failure based on not in trestle directory."""
     monkeypatch.setattr(sys, 'argv', command_string.split())
+    monkeypatch.chdir(tmp_path)
     with pytest.raises(SystemExit) as wrapped_error:
         trestle.cli.run()
         # FIXME: Needs to be changed once implemented.
     assert wrapped_error.type == SystemExit
-    assert wrapped_error.value.code == 5
+    assert wrapped_error.value.code == CmdReturnCodes.TRESTLE_ROOT_ERROR.value
```

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/author/component_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/author/component_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/author/docs_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/author/docs_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/author/folders_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/author/folders_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/author/headers_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/author/headers_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/author/jinja_cmd_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/author/jinja_cmd_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,22 @@
 from tests.test_utils import execute_command_and_assert, setup_for_ssp
 
 from trestle.core.commands.author.jinja import _number_captions
 from trestle.core.commands.author.ssp import SSPGenerate
 from trestle.core.markdown.docs_markdown_node import DocsMarkdownNode
 
 
-def setup_ssp(testdata_dir: pathlib.Path, tmp_trestle_dir: pathlib.Path, monkeypatch: MonkeyPatch):
+def setup_ssp(
+    testdata_dir: pathlib.Path,
+    tmp_trestle_dir: pathlib.Path,
+    monkeypatch: MonkeyPatch,
+    profile_name: str = 'comp_prof'
+):
     """Prepare repository for docs generation."""
-    args, _ = setup_for_ssp(tmp_trestle_dir, 'comp_prof', 'my_ssp')
+    args, _ = setup_for_ssp(tmp_trestle_dir, profile_name, 'my_ssp')
     ssp_cmd = SSPGenerate()
     assert ssp_cmd._run(args) == 0
 
     command_ssp_gen = f'trestle author ssp-assemble -m my_ssp -o ssp_json -cd {args.compdefs}'
     execute_command_and_assert(command_ssp_gen, 0, monkeypatch)
 
     for file_name in os.listdir(testdata_dir / 'jinja'):
@@ -147,14 +152,27 @@
                 node3 = tree.get_node_for_key('## Implementation Guidance')
                 assert node3
 
                 node4 = tree.get_node_for_key('# AC-1 - Policy and Procedures')
                 assert node4.get_node_for_key('## Implementation Guidance')
 
 
+def test_jinja_profile_docs_no_part_prose(
+    testdata_dir: pathlib.Path, tmp_trestle_dir: pathlib.Path, monkeypatch: MonkeyPatch
+) -> None:
+    """Test Jinja Profile to multiple md files output. Test for if part to add does not have prose at all."""
+    input_template = 'profile_to_docs_no_part_prose.md.jinja'
+    profile_name = 'comp_prof_part_none'
+
+    setup_ssp(testdata_dir, tmp_trestle_dir, monkeypatch, profile_name)
+
+    command_import = f'trestle author jinja -i {input_template} -o controls -p {profile_name} --docs-profile'
+    execute_command_and_assert(command_import, 0, monkeypatch)
+
+
 def test_jinja_profile_docs_with_group_title(
     testdata_dir: pathlib.Path, tmp_trestle_dir: pathlib.Path, monkeypatch: MonkeyPatch
 ) -> None:
     """Test Jinja Profile to multiple md files output with group title."""
     input_template = 'profile_to_docs_with_group_title.md.jinja'
 
     setup_ssp(testdata_dir, tmp_trestle_dir, monkeypatch)
```

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/author/profile_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/author/profile_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import trestle.oscal.profile as prof
 from trestle.cli import Trestle
 from trestle.common import file_utils
 from trestle.common.err import TrestleError
 from trestle.common.list_utils import comma_colon_sep_to_dict, comma_sep_to_list
 from trestle.common.model_utils import ModelUtils
 from trestle.core.catalog.catalog_interface import CatalogInterface
-from trestle.core.commands.author.profile import ProfileAssemble, ProfileGenerate
+from trestle.core.commands.author.profile import ProfileAssemble, ProfileGenerate, ProfileInherit
 from trestle.core.control_interface import ControlInterface
 from trestle.core.markdown.docs_markdown_node import DocsMarkdownNode
 from trestle.core.markdown.markdown_api import MarkdownAPI
 from trestle.core.models.file_content_type import FileContentType
 from trestle.core.profile_resolver import ProfileResolver
 
 # test dicts are of form {'name_exp': [(name, exp_str)...], 'text': prose}
@@ -1012,7 +1012,106 @@
     test_utils.setup_for_multi_profile(tmp_trestle_dir, True, False)
     core_command = 'trestle author profile-resolve -n main_profile -o resolved_catalog -bf (.) '
     test_utils.execute_command_and_assert(core_command + '-sv -sl', 1, monkeypatch)
     test_utils.execute_command_and_assert(core_command + '-sv -lp prefix', 1, monkeypatch)
     test_utils.execute_command_and_assert(core_command + '-lp prefix', 1, monkeypatch)
     test_utils.execute_command_and_assert(core_command + '-vap prefix', 1, monkeypatch)
     test_utils.execute_command_and_assert(core_command + '-sl -vap prefix', 1, monkeypatch)
+
+
+def test_profile_inherit(tmp_trestle_dir: pathlib.Path):
+    """Test profile initialization and seeding for various use cases."""
+    output_profile = 'my_profile'
+    excluded = prof.WithId(__root__='ac-1')
+
+    # Test with a profile and ssp that has all controls with exported information
+    args = test_utils.setup_for_inherit(tmp_trestle_dir, 'simple_test_profile', output_profile, 'leveraged_ssp')
+    prof_inherit = ProfileInherit()
+    assert prof_inherit._run(args) == 0
+
+    result_prof, _ = ModelUtils.load_model_for_class(
+        tmp_trestle_dir,
+        output_profile,
+        prof.Profile,
+        FileContentType.JSON
+    )
+
+    assert result_prof.imports[0].href == 'trestle://profiles/simple_test_profile/profile.json'
+    assert len(result_prof.imports[0].include_controls[0].with_ids) == 2
+    assert len(result_prof.imports[0].exclude_controls[0].with_ids) == 1
+    assert result_prof.imports[0].exclude_controls[0].with_ids[0] == excluded
+
+    # Test with a profile that has more controls than the ssp
+    args = test_utils.setup_for_inherit(tmp_trestle_dir, 'simple_test_profile_more', output_profile, 'leveraged_ssp')
+    prof_inherit = ProfileInherit()
+    assert prof_inherit._run(args) == 0
+
+    result_prof, _ = ModelUtils.load_model_for_class(
+        tmp_trestle_dir,
+        output_profile,
+        prof.Profile,
+        FileContentType.JSON
+    )
+
+    assert result_prof.imports[0].href == 'trestle://profiles/simple_test_profile_more/profile.json'
+    assert len(result_prof.imports[0].include_controls[0].with_ids) == 3
+    assert len(result_prof.imports[0].exclude_controls[0].with_ids) == 1
+    assert result_prof.imports[0].exclude_controls[0].with_ids[0] == excluded
+
+    # Test with a profile that has less controls than the ssp
+    args = test_utils.setup_for_inherit(tmp_trestle_dir, 'simple_test_profile_less', output_profile, 'leveraged_ssp')
+    prof_inherit = ProfileInherit()
+    assert prof_inherit._run(args) == 0
+
+    result_prof, _ = ModelUtils.load_model_for_class(
+        tmp_trestle_dir,
+        output_profile,
+        prof.Profile,
+        FileContentType.JSON
+    )
+
+    assert result_prof.imports[0].href == 'trestle://profiles/simple_test_profile_less/profile.json'
+    assert len(result_prof.imports[0].include_controls[0].with_ids) == 1
+    assert len(result_prof.imports[0].exclude_controls[0].with_ids) == 1
+    assert result_prof.imports[0].exclude_controls[0].with_ids[0] == excluded
+
+    # Test with a profile that has all controls filtered out
+    args = test_utils.setup_for_inherit(tmp_trestle_dir, 'simple_test_profile_single', output_profile, 'leveraged_ssp')
+    prof_inherit = ProfileInherit()
+    assert prof_inherit._run(args) == 0
+
+    result_prof, _ = ModelUtils.load_model_for_class(
+        tmp_trestle_dir,
+        output_profile,
+        prof.Profile,
+        FileContentType.JSON
+    )
+
+    assert result_prof.imports[0].href == 'trestle://profiles/simple_test_profile_single/profile.json'
+    assert len(result_prof.imports[0].include_controls[0].with_ids) == 0
+    assert len(result_prof.imports[0].exclude_controls[0].with_ids) == 1
+    assert result_prof.imports[0].exclude_controls[0].with_ids[0] == excluded
+
+    # Test with version set
+    args = test_utils.setup_for_inherit(tmp_trestle_dir, 'simple_test_profile_less', output_profile, 'leveraged_ssp')
+    prof_inherit = ProfileInherit()
+    args.version = '1.0.0'
+    assert prof_inherit._run(args) == 0
+
+    result_prof, _ = ModelUtils.load_model_for_class(
+        tmp_trestle_dir,
+        output_profile,
+        prof.Profile,
+        FileContentType.JSON
+    )
+
+    assert result_prof.metadata.version == '1.0.0'
+
+    # Force a failure with non-existent profile
+    args.profile = 'bad_prof'
+    prof_inherit = ProfileInherit()
+    assert prof_inherit._run(args) == 1
+
+    # Force a failure with a cyclic dependency
+    args.output = args.profile
+    prof_inherit = ProfileInherit()
+    assert prof_inherit._run(args) == 2
```

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/author/ssp_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/author/ssp_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -482,15 +482,16 @@
         name=ssp_name,
         profile='comp_prof_aa',
         output=filtered_name,
         verbose=0,
         regenerate=False,
         version=None,
         components=None,
-        implementation_status=None
+        implementation_status=None,
+        control_origination=None
     )
     ssp_filter = SSPFilter()
     assert ssp_filter._run(args) == 0
 
     ssp, _ = ModelUtils.load_model_for_class(
         tmp_trestle_dir,
         filtered_name,
@@ -510,15 +511,16 @@
         name=ssp_name,
         profile=None,
         output=filtered_name,
         verbose=0,
         regenerate=True,
         version=None,
         components='comp_aa',
-        implementation_status=None
+        implementation_status=None,
+        control_origination=None
     )
     ssp_filter = SSPFilter()
     assert ssp_filter._run(args) == 0
 
     ssp, _ = ModelUtils.load_model_for_class(
         tmp_trestle_dir,
         filtered_name,
@@ -532,30 +534,32 @@
         name=filtered_name,
         profile=None,
         output=filtered_name,
         verbose=0,
         regenerate=True,
         version=None,
         components='comp_aa',
-        implementation_status=None
+        implementation_status=None,
+        control_origination=None
     )
     ssp_filter = SSPFilter()
     assert ssp_filter._run(args) == 0
 
     # now filter the ssp by multiple implementation statuses
     args = argparse.Namespace(
         trestle_root=tmp_trestle_dir,
         name=ssp_name,
         profile=None,
         output=filtered_name,
         verbose=0,
         regenerate=False,
         version=None,
         components=None,
-        implementation_status='not-applicable,implemented'
+        implementation_status='not-applicable,implemented',
+        control_origination=None
     )
     ssp_filter = SSPFilter()
     assert ssp_filter._run(args) == 0
 
     ssp, _ = ModelUtils.load_model_for_class(
         tmp_trestle_dir,
         filtered_name,
@@ -574,15 +578,16 @@
         name=ssp_name,
         profile=None,
         output=filtered_name,
         verbose=0,
         regenerate=False,
         version=None,
         components=None,
-        implementation_status='not-applicable'
+        implementation_status='not-applicable',
+        control_origination=None
     )
     ssp_filter = SSPFilter()
     assert ssp_filter._run(args) == 0
 
     ssp, _ = ModelUtils.load_model_for_class(
         tmp_trestle_dir,
         filtered_name,
@@ -598,31 +603,36 @@
         trestle_root=tmp_trestle_dir,
         name=ssp_name,
         profile=None,
         output=filtered_name,
         verbose=0,
         regenerate=True,
         version=None,
-        components=None
+        components=None,
+        implementation_status=None,
+        control_origination=None
     )
+
     ssp_filter = SSPFilter()
     assert ssp_filter._run(args) == 1
 
     # now filter the ssp through comp_prof_bad to force error because it references a control not in the ssp
     bad_prof = 'comp_prof_bad'
     test_utils.load_from_json(tmp_trestle_dir, bad_prof, bad_prof, prof.Profile)
     args = argparse.Namespace(
         trestle_root=tmp_trestle_dir,
         name=ssp_name,
         profile=bad_prof,
         output=filtered_name,
         verbose=0,
         regenerate=True,
         version=None,
-        components=None
+        components=None,
+        implementation_status=None,
+        control_origination=None
     )
     ssp_filter = SSPFilter()
     assert ssp_filter._run(args) == 1
 
     # now filter with an invalid implementation status to trigger error
     bad_impl = 'impl_bad'
     args = argparse.Namespace(
@@ -630,15 +640,113 @@
         name=ssp_name,
         profile=None,
         output=filtered_name,
         verbose=0,
         regenerate=True,
         version=None,
         components=None,
-        implementation_status=bad_impl
+        implementation_status=bad_impl,
+        control_origination=None
+    )
+    ssp_filter = SSPFilter()
+    assert ssp_filter._run(args) == 1
+
+
+def test_ssp_filter_control_origination(tmp_trestle_dir: pathlib.Path) -> None:
+    """Test the ssp filter when filtering by control origination."""
+    gen_args, _ = setup_for_ssp(tmp_trestle_dir, prof_name, ssp_name)
+    ssp_gen = SSPGenerate()
+    assert ssp_gen._run(gen_args) == 0
+
+    # create ssp from the markdown
+    ssp_assemble = SSPAssemble()
+    args = argparse.Namespace(
+        trestle_root=tmp_trestle_dir,
+        markdown=ssp_name,
+        output=ssp_name,
+        verbose=0,
+        name=None,
+        version=None,
+        regenerate=False,
+        compdefs=gen_args.compdefs
+    )
+    assert ssp_assemble._run(args) == 0
+
+    ssp: ossp.SystemSecurityPlan
+    ssp, _ = ModelUtils.load_model_for_class(tmp_trestle_dir, ssp_name, ossp.SystemSecurityPlan, FileContentType.JSON)
+
+    assert len(ssp.control_implementation.implemented_requirements) == 8
+
+    filtered_name = 'filtered_ssp'
+
+    # now filter the ssp by multiple control origination values
+    args = argparse.Namespace(
+        trestle_root=tmp_trestle_dir,
+        name=ssp_name,
+        profile=None,
+        output=filtered_name,
+        verbose=0,
+        regenerate=False,
+        version=None,
+        components=None,
+        implementation_status=None,
+        control_origination='customer-configured,system-specific'
+    )
+    ssp_filter = SSPFilter()
+    assert ssp_filter._run(args) == 0
+
+    ssp, _ = ModelUtils.load_model_for_class(
+        tmp_trestle_dir,
+        filtered_name,
+        ossp.SystemSecurityPlan,
+        FileContentType.JSON
+    )
+
+    # confirm the imp_reqs have been culled to two controls
+    assert len(ssp.control_implementation.implemented_requirements) == 2
+
+    # now filter the ssp by a control origination that is unused
+    args = argparse.Namespace(
+        trestle_root=tmp_trestle_dir,
+        name=ssp_name,
+        profile=None,
+        output=filtered_name,
+        verbose=0,
+        regenerate=False,
+        version=None,
+        components=None,
+        implementation_status=None,
+        control_origination='inherited'
+    )
+    ssp_filter = SSPFilter()
+    assert ssp_filter._run(args) == 0
+
+    ssp, _ = ModelUtils.load_model_for_class(
+        tmp_trestle_dir,
+        filtered_name,
+        ossp.SystemSecurityPlan,
+        FileContentType.JSON
+    )
+
+    # confirm the imp_reqs have been culled to zero controls
+    assert len(ssp.control_implementation.implemented_requirements) == 0
+
+    # filter with an invalid control origination to trigger error
+    bad_co = 'co_bad'
+    args = argparse.Namespace(
+        trestle_root=tmp_trestle_dir,
+        name=ssp_name,
+        profile=None,
+        output=filtered_name,
+        verbose=0,
+        regenerate=True,
+        version=None,
+        components=None,
+        implementation_status=None,
+        control_origination=bad_co
     )
     ssp_filter = SSPFilter()
     assert ssp_filter._run(args) == 1
 
 
 def test_ssp_bad_control_id(tmp_trestle_dir: pathlib.Path) -> None:
     """Test ssp gen when profile has bad control id."""
```

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/author/versioning/__init__.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/author/versioning/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/author/versioning/template_versioning_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/author/versioning/template_versioning_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/cmd_utils_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/cmd_utils_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/create_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/create_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/describe_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/describe_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/href_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/href_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from _pytest.monkeypatch import MonkeyPatch
 
 from tests import test_utils
 
 from trestle.cli import Trestle
 from trestle.common.model_utils import ModelUtils
+from trestle.core.commands.common.return_codes import CmdReturnCodes
 from trestle.core.models.file_content_type import FileContentType
 from trestle.oscal import profile
 
 
 def test_href_cmd(
     tmp_path: pathlib.Path, keep_cwd: pathlib.Path, simplified_nist_profile: profile.Profile, monkeypatch: MonkeyPatch
 ) -> None:
@@ -66,31 +67,32 @@
     assert ModelUtils.models_are_equivalent(new_profile, simplified_nist_profile)
 
 
 def test_href_failures(
     tmp_path: pathlib.Path, keep_cwd: pathlib.Path, simplified_nist_profile: profile.Profile, monkeypatch: MonkeyPatch
 ) -> None:
     """Test href failure modes."""
+    cmd_string = 'trestle href -n my_test_model -hr foobar'
+
+    # not in trestle project so fail
+    monkeypatch.setattr(sys, 'argv', cmd_string.split())
+    monkeypatch.chdir(tmp_path)
+    rc = Trestle().run()
+    assert rc == CmdReturnCodes.TRESTLE_ROOT_ERROR.value
+
     # prepare trestle project dir with the file
     models_path, profile_path = test_utils.prepare_trestle_project_dir(
         tmp_path,
         FileContentType.JSON,
         simplified_nist_profile,
         test_utils.PROFILES_DIR)
 
-    cmd_string = 'trestle href -n my_test_model -hr foobar'
-
-    # not in trestle project so fail
-    monkeypatch.setattr(sys, 'argv', cmd_string.split())
-    rc = Trestle().run()
-    assert rc == 5
-
     os.chdir(models_path)
 
     cmd_string = 'trestle href -n my_test_model -hr foobar -i 2'
 
     # add extra import to the profile and ask for import number 2
     simplified_nist_profile.imports.append(simplified_nist_profile.imports[0])
     simplified_nist_profile.oscal_write(profile_path)
     monkeypatch.setattr(sys, 'argv', cmd_string.split())
     rc = Trestle().run()
-    assert rc == 1
+    assert rc == CmdReturnCodes.COMMAND_ERROR.value
```

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/import__test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/import__test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/init_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/init_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/merge_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/merge_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/partial_object_validate_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/partial_object_validate_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/remove_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/remove_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 import pytest
 
 from tests import test_utils
 
 import trestle.common.err as err
 from trestle.cli import Trestle
+from trestle.core.commands.common.return_codes import CmdReturnCodes
 from trestle.core.commands.remove import RemoveCmd
 from trestle.core.models.actions import RemoveAction
 from trestle.core.models.elements import Element, ElementPath
 from trestle.core.models.file_content_type import FileContentType
 from trestle.core.models.plans import Plan
 from trestle.oscal.catalog import Catalog
 
@@ -120,28 +121,28 @@
     else:
         AssertionError()
 
 
 def test_run_failure_switches(tmp_path: pathlib.Path, monkeypatch: MonkeyPatch):
     """Test failure of _run on bad switches for RemoveCmd."""
     # 1. Missing --file argument.
-    testargs = ['trestle', 'remove', '-e', 'catalog.metadata.roles']
+    testargs = ['trestle', 'remove', '-e', 'catalog.metadata.roles', '--trestle-root', str(tmp_path)]
     monkeypatch.setattr(sys, 'argv', testargs)
     with pytest.raises(SystemExit) as e:
         Trestle().run()
     assert e.type == SystemExit
-    assert e.value.code == 2
+    assert e.value.code == CmdReturnCodes.INCORRECT_ARGS.value
 
     # 2. Missing --element argument.
-    testargs = ['trestle', 'remove', '-f', './catalog.json']
+    testargs = ['trestle', 'remove', '-f', './catalog.json', '--trestle-root', str(tmp_path)]
     monkeypatch.setattr(sys, 'argv', testargs)
     with pytest.raises(SystemExit) as e:
         Trestle().run()
     assert e.type == SystemExit
-    assert e.value.code == 2
+    assert e.value.code == CmdReturnCodes.INCORRECT_ARGS.value
 
 
 def test_run_failure_nonexistent_element(
     tmp_path: pathlib.Path, sample_catalog_minimal: Catalog, monkeypatch: MonkeyPatch
 ):
     """Test failure of _run on RemoveCmd in specifying nonexistent element for removal."""
     # Create a temporary catalog file with responsible-parties
@@ -150,42 +151,51 @@
         tmp_path,
         content_type,
         sample_catalog_minimal,
         test_utils.CATALOGS_DIR
     )
 
     # 1. self.remove() fails -- Should happen if wildcard is given, or nonexistent element.
-    testargs = ['trestle', 'remove', '-f', str(catalog_def_file), '-e', 'catalog.blah']
+    testargs = ['trestle', 'remove', '-f', str(catalog_def_file), '-e', 'catalog.blah', '--trestle-root', str(tmp_path)]
     monkeypatch.setattr(sys, 'argv', testargs)
     exitcode = Trestle().run()
-    assert exitcode == 5
+    assert exitcode == CmdReturnCodes.COMMAND_ERROR.value
 
     # 2. Corrupt json file
     source_file_path = pathlib.Path.joinpath(test_utils.JSON_TEST_DATA_PATH, 'bad_simple.json')
     shutil.copyfile(source_file_path, catalog_def_file)
-    testargs = ['trestle', 'remove', '-f', str(catalog_def_file), '-e', 'catalog.metadata.roles']
+    testargs = [
+        'trestle',
+        'remove',
+        '-f',
+        str(catalog_def_file),
+        '-e',
+        'catalog.metadata.roles',
+        '--trestle-root',
+        str(tmp_path)
+    ]
     monkeypatch.setattr(sys, 'argv', testargs)
     exitcode = Trestle().run()
-    assert exitcode == 5
+    assert exitcode == CmdReturnCodes.COMMAND_ERROR.value
 
 
 def test_run_failure_wildcard(tmp_path: pathlib.Path, sample_catalog_minimal: Catalog, monkeypatch: MonkeyPatch):
     """Test failure of _run on RemoveCmd in specifying wildcard in element for removal."""
     # Create a temporary catalog file with responsible-parties
     content_type = FileContentType.JSON
     catalog_def_dir, catalog_def_file = test_utils.prepare_trestle_project_dir(
         tmp_path,
         content_type,
         sample_catalog_minimal,
         test_utils.CATALOGS_DIR
     )
-    testargs = ['trestle', 'remove', '-f', str(catalog_def_file), '-e', 'catalog.*']
+    testargs = ['trestle', 'remove', '-f', str(catalog_def_file), '-e', 'catalog.*', '--trestle-root', str(tmp_path)]
     monkeypatch.setattr(sys, 'argv', testargs)
     exitcode = Trestle().run()
-    assert exitcode == 5
+    assert exitcode == CmdReturnCodes.COMMAND_ERROR.value
 
 
 def test_run_failure_required_element(
     tmp_path: pathlib.Path, keep_cwd: pathlib.Path, sample_catalog_minimal: Catalog, monkeypatch: MonkeyPatch
 ):
     """Test failure of _run on RemoveCmd in specifying a required element for removal."""
     # Create a temporary catalog file with responsible-parties
@@ -194,18 +204,20 @@
         tmp_path,
         content_type,
         sample_catalog_minimal,
         test_utils.CATALOGS_DIR
     )
     # 4. simulate() fails -- Should happen if required element is target for deletion
     monkeypatch.chdir(tmp_path)
-    testargs = ['trestle', 'remove', '-f', str(catalog_def_file), '-e', 'catalog.metadata']
+    testargs = [
+        'trestle', 'remove', '-f', str(catalog_def_file), '-e', 'catalog.metadata', '--trestle-root', str(tmp_path)
+    ]
     monkeypatch.setattr(sys, 'argv', testargs)
     exitcode = Trestle().run()
-    assert exitcode == 1
+    assert exitcode == CmdReturnCodes.COMMAND_ERROR.value
 
 
 def test_run_failure_project_not_found(
     tmp_path: pathlib.Path, sample_catalog_minimal: Catalog, monkeypatch: MonkeyPatch
 ):
     """Test failure of _run on RemoveCmd in specifying file in non-initialized location."""
     # Create a temporary catalog file with responsible-parties
@@ -213,18 +225,18 @@
     catalog_def_dir, catalog_def_file = test_utils.prepare_trestle_project_dir(
         tmp_path,
         content_type,
         sample_catalog_minimal,
         test_utils.CATALOGS_DIR
     )
     # 5. get_contextual_model_type() fails, i.e., "Trestle project not found"
-    testargs = ['trestle', 'remove', '-f', '/dev/null', '-e', 'catalog.metadata']
+    testargs = ['trestle', 'remove', '-f', '/dev/null', '-e', 'catalog.metadata', '--trestle-root', str(tmp_path)]
     monkeypatch.setattr(sys, 'argv', testargs)
     exitcode = Trestle().run()
-    assert exitcode == 5
+    assert exitcode == CmdReturnCodes.COMMAND_ERROR.value
 
 
 def test_run_failure_filenotfounderror(
     tmp_path: pathlib.Path, sample_catalog_minimal: Catalog, monkeypatch: MonkeyPatch
 ):
     """Test failure of _run on RemoveCmd in specifying a nonexistent file."""
     # Create a temporary catalog file with responsible-parties
@@ -234,19 +246,26 @@
         content_type,
         sample_catalog_minimal,
         test_utils.CATALOGS_DIR
     )
     # 6. oscal_read fails because file is not found
     # Must specify catalogs/ location, not catalogs/my_test_model/.
     testargs = [
-        'trestle', 'remove', '-f', re.sub('my_test_model/', '', str(catalog_def_file)), '-e', 'catalog.metadata'
+        'trestle',
+        'remove',
+        '-f',
+        re.sub('my_test_model/', '', str(catalog_def_file)),
+        '-e',
+        'catalog.metadata',
+        '--trestle-root',
+        str(tmp_path)
     ]
     monkeypatch.setattr(sys, 'argv', testargs)
     exitcode = Trestle().run()
-    assert exitcode == 5
+    assert exitcode == CmdReturnCodes.COMMAND_ERROR.value
 
 
 def test_run_failure_plan_execute(
     tmp_path: pathlib.Path,
     keep_cwd: pathlib.Path,
     sample_catalog_minimal: Catalog,
     monkeypatch: MonkeyPatch,
```

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/replicate_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/replicate_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/split_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/split_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/task_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/task_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/validate_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/validate_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/commands/version_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/commands/version_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/control_io_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/control_io_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/draw_io_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/draw_io_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/err_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/err_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/generator_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/generator_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/jinja_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/jinja_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/markdown/__init__.py` & `compliance-trestle-2.2.0/tests/trestle/core/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/markdown/markdown_node_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/markdown/markdown_node_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/markdown/markdown_validator_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/markdown/markdown_validator_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/models/__init__.py` & `compliance-trestle-2.2.0/tests/trestle/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/models/create_path_action_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/models/create_path_action_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/models/element_path_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/models/element_path_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/models/element_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/models/element_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/models/file_content_type_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/models/file_content_type_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/models/interfaces_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/models/interfaces_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/models/plans_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/models/plans_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/models/remove_action_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/models/remove_action_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/models/remove_path_action_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/models/remove_path_action_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/models/update_action_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/models/update_action_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/models/write_action_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/models/write_action_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/models/write_file_action_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/models/write_file_action_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/parser_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/parser_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/profile_resolver_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/profile_resolver_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/remote/__init__.py` & `compliance-trestle-2.2.0/tests/trestle/core/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/remote/cache_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/remote/cache_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/repository_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/repository_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/ssp_io_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/ssp_io_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/utils_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/utils_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/core/validator_helper_test.py` & `compliance-trestle-2.2.0/tests/trestle/core/validator_helper_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/main_test.py` & `compliance-trestle-2.2.0/tests/trestle/main_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/parsing/__init__.py` & `compliance-trestle-2.2.0/tests/trestle/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/parsing/parsing_test.py` & `compliance-trestle-2.2.0/tests/trestle/parsing/parsing_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/tasks/__init__.py` & `compliance-trestle-2.2.0/tests/trestle/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/tasks/base_task_test.py` & `compliance-trestle-2.2.0/tests/trestle/tasks/base_task_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/tasks/cis_xlsx_to_oscal_catalog_test.py` & `compliance-trestle-2.2.0/tests/trestle/tasks/cis_xlsx_to_oscal_catalog_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/tasks/csv_to_oscal_cd_test.py` & `compliance-trestle-2.2.0/tests/trestle/tasks/csv_to_oscal_cd_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/tasks/ocp4_cis_profile_to_oscal_catalog_test.py` & `compliance-trestle-2.2.0/tests/trestle/tasks/ocp4_cis_profile_to_oscal_catalog_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/tasks/ocp4_cis_profile_to_oscal_cd_test.py` & `compliance-trestle-2.2.0/tests/trestle/tasks/ocp4_cis_profile_to_oscal_cd_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/tasks/oscal_profile_to_osco_profile_test.py` & `compliance-trestle-2.2.0/tests/trestle/tasks/oscal_profile_to_osco_profile_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/tasks/osco_result_to_oscal_ar_test.py` & `compliance-trestle-2.2.0/tests/trestle/tasks/osco_result_to_oscal_ar_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/tasks/tanium_result_to_oscal_ar_test.py` & `compliance-trestle-2.2.0/tests/trestle/tasks/tanium_result_to_oscal_ar_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/tasks/transform_test.py` & `compliance-trestle-2.2.0/tests/trestle/tasks/transform_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/tasks/xccdf_result_to_oscal_ar_test.py` & `compliance-trestle-2.2.0/tests/trestle/tasks/xccdf_result_to_oscal_ar_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/tasks/xlsx_to_oscal_cd_test.py` & `compliance-trestle-2.2.0/tests/trestle/tasks/xlsx_to_oscal_cd_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/tasks/xlsx_to_oscal_profile_test.py` & `compliance-trestle-2.2.0/tests/trestle/tasks/xlsx_to_oscal_profile_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/transforms/__init__.py` & `compliance-trestle-2.2.0/tests/trestle/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/transforms/transformer_factory_test.py` & `compliance-trestle-2.2.0/tests/trestle/transforms/transformer_factory_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/transforms/transformer_helper_test.py` & `compliance-trestle-2.2.0/tests/trestle/transforms/transformer_helper_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/utils/__init__.py` & `compliance-trestle-2.2.0/tests/trestle/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/utils/fs_test.py` & `compliance-trestle-2.2.0/tests/trestle/utils/fs_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/utils/list_utils_test.py` & `compliance-trestle-2.2.0/tests/trestle/utils/list_utils_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/utils/load_distributed_test.py` & `compliance-trestle-2.2.0/tests/trestle/utils/load_distributed_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/utils/md_writer_test.py` & `compliance-trestle-2.2.0/tests/trestle/utils/md_writer_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/tests/trestle/utils/trash_test.py` & `compliance-trestle-2.2.0/tests/trestle/utils/trash_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/__init__.py` & `compliance-trestle-2.2.0/trestle/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 Trestle is a tool to which enables the creation and validation of
 documentation artifacts for compliance requirements. It leverages NIST's
 OSCAL (https://pages.nist.gov/OSCAL/documentation/) as a standard data
 format for interchange between tools & people and provides an
 opinionated approach to OSCAL adoption.
 """
 
-__version__ = '2.1.1'
+__version__ = '2.2.0'
```

### Comparing `compliance-trestle-2.1.1/trestle/__main__.py` & `compliance-trestle-2.2.0/trestle/__main__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/cli.py` & `compliance-trestle-2.2.0/trestle/cli.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/common/__init__.py` & `compliance-trestle-2.2.0/trestle/common/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/common/common_types.py` & `compliance-trestle-2.2.0/trestle/common/common_types.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/common/const.py` & `compliance-trestle-2.2.0/trestle/common/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -551,7 +551,19 @@
 VALUE_ASSIGNED_PREFIX = 'value-assigned-prefix'
 
 VALUE_NOT_ASSIGNED_PREFIX = 'value-not-assigned-prefix'
 
 CONTROL_IMPLEMENTATION = 'control-implementation'
 
 IMPLEMENTED_REQUIREMENT = 'implemented-requirement'
+
+# Following 5 are allowed control origination values for
+# SSP -> ControlImplementation -> ImplementedRequirements -> prop[@name='control-origination']/@value
+ORIGINATION_ORGANIZATION = 'organization'
+
+ORIGINATION_SYSTEM_SPECIFIC = 'system-specific'
+
+ORIGINATION_CUSTOMER_CONFIGURED = 'customer-configured'
+
+ORIGINATION_CUSTOMER_PROVIDED = 'customer-provided'
+
+ORIGINATION_INHERITED = 'inherited'
```

### Comparing `compliance-trestle-2.1.1/trestle/common/err.py` & `compliance-trestle-2.2.0/trestle/common/err.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/common/file_utils.py` & `compliance-trestle-2.2.0/trestle/common/file_utils.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/common/list_utils.py` & `compliance-trestle-2.2.0/trestle/common/list_utils.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/common/load_validate.py` & `compliance-trestle-2.2.0/trestle/common/load_validate.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/common/log.py` & `compliance-trestle-2.2.0/trestle/common/log.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/common/model_utils.py` & `compliance-trestle-2.2.0/trestle/common/model_utils.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/common/str_utils.py` & `compliance-trestle-2.2.0/trestle/common/str_utils.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/common/trash.py` & `compliance-trestle-2.2.0/trestle/common/trash.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/common/type_utils.py` & `compliance-trestle-2.2.0/trestle/common/type_utils.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/__init__.py` & `compliance-trestle-2.2.0/trestle/core/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/all_validator.py` & `compliance-trestle-2.2.0/trestle/core/all_validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/base_model.py` & `compliance-trestle-2.2.0/trestle/core/base_model.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/catalog/__init__.py` & `compliance-trestle-2.2.0/trestle/core/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/catalog/catalog_api.py` & `compliance-trestle-2.2.0/trestle/core/catalog/catalog_api.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/catalog/catalog_interface.py` & `compliance-trestle-2.2.0/trestle/core/catalog/catalog_interface.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/catalog/catalog_merger.py` & `compliance-trestle-2.2.0/trestle/core/catalog/catalog_merger.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/catalog/catalog_reader.py` & `compliance-trestle-2.2.0/trestle/core/catalog/catalog_reader.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/catalog/catalog_writer.py` & `compliance-trestle-2.2.0/trestle/core/catalog/catalog_writer.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/catalog_validator.py` & `compliance-trestle-2.2.0/trestle/core/catalog_validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/__init__.py` & `compliance-trestle-2.2.0/trestle/core/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/add.py` & `compliance-trestle-2.2.0/trestle/core/commands/add.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/assemble.py` & `compliance-trestle-2.2.0/trestle/core/commands/assemble.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/author/__init__.py` & `compliance-trestle-2.2.0/trestle/core/commands/author/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/author/catalog.py` & `compliance-trestle-2.2.0/trestle/core/commands/author/catalog.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/author/command.py` & `compliance-trestle-2.2.0/trestle/core/commands/author/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from trestle.core.commands.author.catalog import CatalogAssemble, CatalogGenerate
 from trestle.core.commands.author.component import ComponentAssemble, ComponentGenerate
 from trestle.core.commands.author.docs import Docs
 from trestle.core.commands.author.folders import Folders
 from trestle.core.commands.author.headers import Headers
 from trestle.core.commands.author.jinja import JinjaCmd
-from trestle.core.commands.author.profile import ProfileAssemble, ProfileGenerate, ProfileResolve
+from trestle.core.commands.author.profile import ProfileAssemble, ProfileGenerate, ProfileInherit, ProfileResolve
 from trestle.core.commands.author.ssp import SSPAssemble, SSPFilter, SSPGenerate
 from trestle.core.commands.command_docs import CommandPlusDocs
 
 logger = logging.getLogger(__name__)
 
 
 class AuthorCmd(CommandPlusDocs):
@@ -45,12 +45,13 @@
         ComponentGenerate,
         Docs,
         Folders,
         Headers,
         JinjaCmd,
         ProfileAssemble,
         ProfileGenerate,
+        ProfileInherit,
         ProfileResolve,
         SSPAssemble,
         SSPFilter,
         SSPGenerate
     ]
```

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/author/common.py` & `compliance-trestle-2.2.0/trestle/core/commands/author/common.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/author/component.py` & `compliance-trestle-2.2.0/trestle/core/commands/author/component.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/author/consts.py` & `compliance-trestle-2.2.0/trestle/core/commands/author/consts.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/author/docs.py` & `compliance-trestle-2.2.0/trestle/core/commands/author/docs.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/author/folders.py` & `compliance-trestle-2.2.0/trestle/core/commands/author/folders.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/author/headers.py` & `compliance-trestle-2.2.0/trestle/core/commands/author/headers.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/author/jinja.py` & `compliance-trestle-2.2.0/trestle/core/commands/author/jinja.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/author/profile.py` & `compliance-trestle-2.2.0/trestle/core/commands/author/profile.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,25 +10,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Author commands to generate profile as markdown and assemble to json after edit."""
 
 import argparse
+import copy
 import logging
 import pathlib
 import shutil
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Set
 
 from ruamel.yaml import YAML
 from ruamel.yaml.error import YAMLError
 
 import trestle.common.const as const
 import trestle.common.log as log
+import trestle.core.generators as gens
 import trestle.oscal.profile as prof
+import trestle.oscal.ssp as ssp
 from trestle.common import file_utils
 from trestle.common.err import TrestleError, TrestleNotFoundError, handle_generic_command_exception
 from trestle.common.list_utils import as_filtered_list, as_list, comma_sep_to_list, comma_colon_sep_to_dict, deep_set, none_if_empty  # noqa E501
 from trestle.common.load_validate import load_validate_model_name
 from trestle.common.model_utils import ModelUtils
 from trestle.core.catalog.catalog_api import CatalogAPI
 from trestle.core.commands.author.common import AuthorCommonCommand
@@ -532,7 +535,203 @@
             False,
             value_assigned_prefix,
             value_not_assigned_prefix
         )
         ModelUtils.save_top_level_model(catalog, trestle_root, catalog_name, FileContentType.JSON)
 
         return CmdReturnCodes.SUCCESS.value
+
+
+class ProfileInherit(AuthorCommonCommand):
+    """Generate and populate profile in JSON from a parent profile and leveraged ssp in the trestle workspace."""
+
+    name = 'profile-inherit'
+
+    def _init_arguments(self) -> None:
+        ssp_help_str = 'Name of the leveraged ssp model in the trestle workspace'
+        self.add_argument('-s', '--ssp', help=ssp_help_str, required=True, type=str)
+        profile_help_str = 'Name of the parent profile model in the trestle workspace'
+        self.add_argument('-p', '--profile', help=profile_help_str, required=True, type=str)
+        output_help_str = 'Name of the output generated json Profile'
+        self.add_argument('-o', '--output', help=output_help_str, required=True, type=str)
+        self.add_argument('-vn', '--version', help=const.HELP_VERSION, required=False, type=str)
+
+    def _run(self, args: argparse.Namespace) -> int:
+        try:
+            log.set_log_level_from_args(args)
+            trestle_root: pathlib.Path = args.trestle_root
+
+            if args.profile:
+                if args.profile == args.output:
+                    logger.warning(f'Output profile {args.output} cannot equal parent')
+                    return CmdReturnCodes.INCORRECT_ARGS.value
+
+            return self.initialize_profile(
+                trestle_root=trestle_root,
+                parent_prof_name=args.profile,
+                output_prof_name=args.output,
+                leveraged_ssp_name=args.ssp,
+                version=args.version
+            )
+        except Exception as e:  # pragma: no cover
+            return handle_generic_command_exception(e, logger, 'Profile generation failed')
+
+    @staticmethod
+    def _is_inherited(all_comps: List[ssp.ByComponent]) -> bool:
+        # Fail fast by checking for any non-compliant components.
+        # Must contain provided export statements, no responsibility
+        # statements, and be implemented.
+        for comp in all_comps:
+            if comp.export is None:
+                return False
+
+            if comp.export.responsibilities is not None:
+                return False
+
+            if comp.export.provided is None:
+                return False
+
+            if comp.implementation_status.state != const.STATUS_IMPLEMENTED:
+                return False
+
+        return True
+
+    @staticmethod
+    def update_profile_import(
+        orig_prof_import: prof.Import, leveraged_ssp: ssp.SystemSecurityPlan, catalog_api: CatalogAPI
+    ) -> None:
+        """Add controls to different sections of a profile import based on catalog and leveraged SSP.
+
+        Args:
+            orig_prof_import: The original profile import that will have the control selection updated.
+            leveraged_ssp: SSP input for control filtering
+            catalog_api: Catalog API with access to controls that need to be filtered
+
+        Returns:
+            None
+        """
+        exclude_with_ids: Set[prof.withId] = set()
+        components_by_id: Dict(str, List[ssp.ByComponent]) = {}
+
+        # Create dictionary containing all by-components by control for faster searching
+        for implemented_requirement in leveraged_ssp.control_implementation.implemented_requirements:
+            by_components: List[ssp.ByComponent] = []
+
+            if implemented_requirement.by_components:
+                by_components.extend(implemented_requirement.by_components)
+            if implemented_requirement.statements:
+                for stm in implemented_requirement.statements:
+                    if stm.by_components:
+                        by_components.extend(stm.by_components)
+            components_by_id[implemented_requirement.control_id] = none_if_empty(by_components)
+
+        # Looping by controls in the catalog because the ids in the profile should
+        # be a subset of the catalog and not the ssp controls.
+        catalog_control_ids: Set[str] = set(catalog_api._catalog_interface.get_control_ids())
+        for control_id in catalog_control_ids:
+
+            if control_id not in components_by_id:
+                continue
+
+            by_comps: Optional[List[ssp.ByComponent]] = components_by_id[control_id]
+            if by_comps is not None and ProfileInherit._is_inherited(by_comps):
+                exclude_with_ids.add(control_id)
+
+        include_with_ids: Set[prof.withId] = catalog_control_ids - exclude_with_ids
+
+        orig_prof_import.include_controls = [prof.SelectControlById(with_ids=sorted(include_with_ids))]
+        orig_prof_import.exclude_controls = [prof.SelectControlById(with_ids=sorted(exclude_with_ids))]
+
+    def initialize_profile(
+        self,
+        trestle_root: pathlib.Path,
+        parent_prof_name: str,
+        output_prof_name: str,
+        leveraged_ssp_name: str,
+        version: Optional[str],
+    ) -> int:
+        """Initialize profile with controls from a parent profile, filtering by inherited controls.
+
+        Args:
+            trestle_root: Root directory of the trestle workspace
+            parent_prof_name: Name of the parent profile in the trestle workspace
+            output_prof_name: Name of the output profile json file
+            leveraged_ssp_name: Name of the ssp in the trestle workspace for control filtering
+            version: Optional profile version
+
+        Returns:
+            0 on success, 1 on error
+
+        Notes:
+            The profile model will either be updated or a new json profile created. This will overwrite
+            any import information on an exiting profile, but will preserve control modifications and parameters.
+            Allowing profile updates ensure that SSP export updates can be incorporated into an existing profile. All
+            controls from the original profile will exists and will be grouped by included and excluded controls based
+            on inheritance information.
+        """
+        try:
+            result_profile: prof.Profile
+            existing_profile: Optional[prof.Profile] = None
+
+            existing_profile_path = ModelUtils.get_model_path_for_name_and_class(
+                trestle_root, output_prof_name, prof.Profile
+            )
+
+            # If a profile exists at the output path, use that as a starting point for a new profile.
+            # else create a new sample profile.
+            if existing_profile_path is not None:
+                existing_profile, _ = load_validate_model_name(trestle_root,
+                                                               output_prof_name,
+                                                               prof.Profile,
+                                                               FileContentType.JSON)
+                result_profile = copy.deepcopy(existing_profile)
+            else:
+                result_profile = gens.generate_sample_model(prof.Profile)
+
+            parent_prof_path = ModelUtils.get_model_path_for_name_and_class(
+                trestle_root, parent_prof_name, prof.Profile
+            )
+            if parent_prof_path is None:
+                raise TrestleNotFoundError(
+                    f'Profile {parent_prof_name} does not exist.  An existing profile must be provided.'
+                )
+
+            local_path = f'profiles/{parent_prof_name}/profile.json'
+            profile_import: prof.Import = gens.generate_sample_model(prof.Import)
+            profile_import.href = const.TRESTLE_HREF_HEADING + local_path
+
+            leveraged_ssp: ssp.SystemSecurityPlan
+            try:
+                leveraged_ssp, _ = load_validate_model_name(
+                    trestle_root,
+                    leveraged_ssp_name,
+                    ssp.SystemSecurityPlan,
+                    FileContentType.JSON
+                )
+            except TrestleNotFoundError as e:
+                raise TrestleError(f'SSP {leveraged_ssp_name} not found: {e}')
+
+            prof_resolver = ProfileResolver()
+            catalog = prof_resolver.get_resolved_profile_catalog(
+                trestle_root, parent_prof_path, show_value_warnings=True
+            )
+            catalog_api = CatalogAPI(catalog=catalog)
+
+            # Sort controls based on what controls in the SSP have exported provided information with no
+            # customer responsibility
+            ProfileInherit.update_profile_import(profile_import, leveraged_ssp, catalog_api)
+
+            result_profile.imports[0] = profile_import
+
+            if version:
+                result_profile.metadata.version = version
+
+            if ModelUtils.models_are_equivalent(existing_profile, result_profile):  # type: ignore
+                logger.info('Profile is no different from existing version, so no update.')
+                return CmdReturnCodes.SUCCESS.value
+
+            ModelUtils.update_last_modified(result_profile)  # type: ignore
+            ModelUtils.save_top_level_model(result_profile, trestle_root, output_prof_name, FileContentType.JSON)
+
+        except TrestleError as e:
+            raise TrestleError(f'Error initializing profile {output_prof_name}: {e}')
+        return CmdReturnCodes.SUCCESS.value
```

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/author/ssp.py` & `compliance-trestle-2.2.0/trestle/core/commands/author/ssp.py`

 * *Files 3% similar despite different names*

```diff
@@ -585,15 +585,15 @@
 
 
 class SSPFilter(AuthorCommonCommand):
     """
     Filter the controls in an ssp.
 
     The filtered ssp is based on controls included by the following:
-    profile, components, and/or implementation status.
+    profile, components, implementation status, and/or control origination.
     """
 
     name = 'ssp-filter'
 
     def _init_arguments(self) -> None:
         file_help_str = 'Name of the input ssp'
         self.add_argument('-n', '--name', help=file_help_str, required=True, type=str)
@@ -603,26 +603,29 @@
         self.add_argument('-o', '--output', help=output_help_str, required=True, type=str)
         self.add_argument('-r', '--regenerate', action='store_true', help=const.HELP_REGENERATE)
         self.add_argument('-vn', '--version', help=const.HELP_VERSION, required=False, type=str)
         comp_help_str = 'Colon-delimited list of component names to include in filtered ssp.'
         self.add_argument('-c', '--components', help=comp_help_str, required=False, type=str)
         is_help_str = 'Comma-delimited list of control implementation statuses to include in filtered ssp.'
         self.add_argument('-is', '--implementation-status', help=is_help_str, required=False, type=str)
+        co_help_str = 'Comma-delimited list of control origination values to include in filtered ssp.'
+        self.add_argument('-co', '--control-origination', help=co_help_str, required=False, type=str)
 
     def _run(self, args: argparse.Namespace) -> int:
         try:
             log.set_log_level_from_args(args)
             trestle_root = pathlib.Path(args.trestle_root)
             comp_names: Optional[List[str]] = None
             impl_status_values: Optional[List[str]] = None
+            co_values: Optional[List[str]] = None
 
-            if not (args.components or args.implementation_status or args.profile):
+            if not (args.components or args.implementation_status or args.profile or args.control_origination):
                 logger.warning(
                     'You must specify at least one, or a combination of: profile, list of component names'
-                    ', or list of implementation statuses for ssp-filter.'
+                    ', list of implementation statuses, or list of control origination values for ssp-filter.'
                 )
                 return CmdReturnCodes.COMMAND_ERROR.value
 
             if args.components:
                 comp_names = args.components.split(':')
 
             if args.implementation_status:
@@ -639,53 +642,74 @@
                     if impl_status not in allowed_is_values:
                         logger.warning(
                             f'Provided implementation status "{impl_status}" is invalid.\n'
                             f'Please use the following for ssp-filter: {allowed_is_string}'
                         )
                         return CmdReturnCodes.COMMAND_ERROR.value
 
+            if args.control_origination:
+                co_values = args.control_origination.split(',')
+                allowed_co_values = {
+                    const.ORIGINATION_ORGANIZATION,
+                    const.ORIGINATION_SYSTEM_SPECIFIC,
+                    const.ORIGINATION_INHERITED,
+                    const.ORIGINATION_CUSTOMER_CONFIGURED,
+                    const.ORIGINATION_CUSTOMER_PROVIDED
+                }
+                allowed_co_string = ', '.join(str(item) for item in allowed_co_values)
+                for co in co_values:
+                    if co not in allowed_co_values:
+                        logger.warning(
+                            f'Provided control origination "{co}" is invalid.\n'
+                            f'Please use the following for ssp-filter: {allowed_co_string}'
+                        )
+                        return CmdReturnCodes.COMMAND_ERROR.value
+
             return self.filter_ssp(
                 trestle_root,
                 args.name,
                 args.profile,
                 args.output,
                 args.regenerate,
                 args.version,
                 comp_names,
-                impl_status_values
+                impl_status_values,
+                co_values
             )
         except Exception as e:  # pragma: no cover
             return handle_generic_command_exception(e, logger, 'Error generating the filtered ssp')
 
     def filter_ssp(
         self,
         trestle_root: pathlib.Path,
         ssp_name: str,
         profile_name: str,
         out_name: str,
         regenerate: bool,
         version: Optional[str],
         components: Optional[List[str]] = None,
-        implementation_status: Optional[List[str]] = None
+        implementation_status: Optional[List[str]] = None,
+        control_origination: Optional[List[str]] = None
     ) -> int:
         """
         Filter the ssp and output new ssp.
 
         The filtered ssp is based on controls included by the following:
-        profile, components, and/or implementation status.
+        profile, components, implementation status, and/or control origination.
 
         Args:
             trestle_root: root directory of the trestle workspace
             ssp_name: name of the ssp model
             profile_name: name of the optional profile model used for filtering
             out_name: name of the output ssp model with filtered controls
             regenerate: whether to regenerate the uuid's in the ssp
             version: new version for the model
             components: optional list of component names used for filtering
             implementation_status: optional list of implementation statuses for filtering
+            control_origination: optional list of control origination values for filtering
 
         Returns:
             0 on success, 1 otherwise
         """
         # load the ssp
         ssp: ossp.SystemSecurityPlan
         ssp, _ = load_validate_model_name(trestle_root, ssp_name, ossp.SystemSecurityPlan, FileContentType.JSON)
@@ -794,14 +818,30 @@
                 imp_req.statements = none_if_empty(new_statements)
 
                 if imp_req.by_components is not None or imp_req.statements is not None:
                     new_imp_reqs.append(imp_req)
 
             ssp.control_implementation.implemented_requirements = new_imp_reqs
 
+        # filter implemented requirements by control origination property.
+        # this will remove any implemented requirements without the control origination
+        # property set
+        if control_origination:
+            new_imp_reqs: List[ossp.ImplementedRequirement] = []
+
+            for imp_requirement in ssp.control_implementation.implemented_requirements:
+                if imp_requirement.props:
+                    for prop in imp_requirement.props:
+                        if prop.name == const.CONTROL_ORIGINATION and prop.value in control_origination:
+                            new_imp_reqs.append(imp_requirement)
+                            # only add the imp requirement one time
+                            break
+
+            ssp.control_implementation.implemented_requirements = new_imp_reqs
+
         if version:
             ssp.metadata.version = version
 
         existing_ssp_path = ModelUtils.get_model_path_for_name_and_class(
             trestle_root, out_name, ossp.SystemSecurityPlan
         )
         if existing_ssp_path is not None:
```

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/author/versioning/__init__.py` & `compliance-trestle-2.2.0/trestle/core/commands/author/versioning/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/author/versioning/template_versioning.py` & `compliance-trestle-2.2.0/trestle/core/commands/author/versioning/template_versioning.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/command_docs.py` & `compliance-trestle-2.2.0/trestle/core/commands/command_docs.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/common/__init__.py` & `compliance-trestle-2.2.0/trestle/core/commands/common/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/common/cmd_utils.py` & `compliance-trestle-2.2.0/trestle/core/commands/common/cmd_utils.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/common/return_codes.py` & `compliance-trestle-2.2.0/trestle/core/commands/common/return_codes.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/create.py` & `compliance-trestle-2.2.0/trestle/core/commands/create.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/describe.py` & `compliance-trestle-2.2.0/trestle/core/commands/describe.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/href.py` & `compliance-trestle-2.2.0/trestle/core/commands/href.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/import_.py` & `compliance-trestle-2.2.0/trestle/core/commands/import_.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/init.py` & `compliance-trestle-2.2.0/trestle/core/commands/init.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/merge.py` & `compliance-trestle-2.2.0/trestle/core/commands/merge.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/partial_object_validate.py` & `compliance-trestle-2.2.0/trestle/core/commands/partial_object_validate.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/remove.py` & `compliance-trestle-2.2.0/trestle/core/commands/remove.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/replicate.py` & `compliance-trestle-2.2.0/trestle/core/commands/replicate.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/split.py` & `compliance-trestle-2.2.0/trestle/core/commands/split.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/task.py` & `compliance-trestle-2.2.0/trestle/core/commands/task.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/validate.py` & `compliance-trestle-2.2.0/trestle/core/commands/validate.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/commands/version.py` & `compliance-trestle-2.2.0/trestle/core/commands/version.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/control_context.py` & `compliance-trestle-2.2.0/trestle/core/control_context.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/control_interface.py` & `compliance-trestle-2.2.0/trestle/core/control_interface.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/control_reader.py` & `compliance-trestle-2.2.0/trestle/core/control_reader.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/control_writer.py` & `compliance-trestle-2.2.0/trestle/core/control_writer.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/docs_control_writer.py` & `compliance-trestle-2.2.0/trestle/core/docs_control_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,16 @@
         tag_section_name = section_prefix + f'{section_title}'
         tag_section_name = re.sub(const.MATCH_ALL_EXCEPT_LETTERS_UNDERSCORE_SPACE_REGEX, '', tag_section_name)
         tag_section_name = tag_section_name.replace(' ', '-').replace('_', '-').lower()
         self._md_file.new_header(level=heading_level, title=heading_title, add_new_line_after_header=not tag_pattern)
         if tag_pattern:
             self._md_file.new_line(tag_pattern.replace('[.]', tag_section_name))
             self._md_file.new_paragraph()
-        self._md_file.new_line(part_info.prose)
+        prose = '' if part_info.prose is None else part_info.prose
+        self._md_file.new_line(prose)
         self._md_file.new_paragraph()
 
         for subpart_info in as_list(part_info.parts):
             self._write_part_info(
                 subpart_info, subpart_info.name, tag_pattern, tag_section_name + '-', heading_level + 1
             )
```

### Comparing `compliance-trestle-2.1.1/trestle/core/draw_io.py` & `compliance-trestle-2.2.0/trestle/core/draw_io.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/duplicates_validator.py` & `compliance-trestle-2.2.0/trestle/core/duplicates_validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/generators.py` & `compliance-trestle-2.2.0/trestle/core/generators.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/generic_oscal.py` & `compliance-trestle-2.2.0/trestle/core/generic_oscal.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/jinja.py` & `compliance-trestle-2.2.0/trestle/core/jinja.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/links_validator.py` & `compliance-trestle-2.2.0/trestle/core/links_validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/markdown/__init__.py` & `compliance-trestle-2.2.0/trestle/core/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/markdown/base_markdown_node.py` & `compliance-trestle-2.2.0/trestle/core/markdown/base_markdown_node.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/markdown/control_markdown_node.py` & `compliance-trestle-2.2.0/trestle/core/markdown/control_markdown_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,15 +459,15 @@
                     prev_label = ControlInterface.get_label(parts[-1]) if parts else ''
                     id_text = ControlMarkdownNode._create_next_label(prev_label, indent)
                 id_ = ControlInterface.strip_to_make_ncname(parent_id.rstrip('.') + '.' + id_text.strip('.'))
                 name = const.OBJECTIVE_PART if id_.find('_obj') > 0 else const.ITEM
                 prop = common.Property(name='label', value=id_text)
                 part = common.Part(name=name, id=id_, prose=prose, props=[prop])
                 if id_ in [p.id for p in parts]:
-                    raise TrestleError(
+                    logger.warning(
                         f'Duplicate part id {id_} is found in markdown '
                         f'{tree_context.control_id}. Please correct the part label in line {line}.'
                     )
                 parts.append(part)
                 ii += 1
             elif new_indent > indent:
                 # add new list of parts to last part and continue
```

### Comparing `compliance-trestle-2.1.1/trestle/core/markdown/docs_markdown_node.py` & `compliance-trestle-2.2.0/trestle/core/markdown/docs_markdown_node.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/markdown/markdown_api.py` & `compliance-trestle-2.2.0/trestle/core/markdown/markdown_api.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/markdown/markdown_const.py` & `compliance-trestle-2.2.0/trestle/core/markdown/markdown_const.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/markdown/markdown_processor.py` & `compliance-trestle-2.2.0/trestle/core/markdown/markdown_processor.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/markdown/markdown_validator.py` & `compliance-trestle-2.2.0/trestle/core/markdown/markdown_validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/markdown/md_writer.py` & `compliance-trestle-2.2.0/trestle/core/markdown/md_writer.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/models/__init__.py` & `compliance-trestle-2.2.0/trestle/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/models/actions.py` & `compliance-trestle-2.2.0/trestle/core/models/actions.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/models/elements.py` & `compliance-trestle-2.2.0/trestle/core/models/elements.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/models/file_content_type.py` & `compliance-trestle-2.2.0/trestle/core/models/file_content_type.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/models/interfaces.py` & `compliance-trestle-2.2.0/trestle/core/models/interfaces.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/models/plans.py` & `compliance-trestle-2.2.0/trestle/core/models/plans.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/object_factory.py` & `compliance-trestle-2.2.0/trestle/core/object_factory.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/parser.py` & `compliance-trestle-2.2.0/trestle/core/parser.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/pipeline.py` & `compliance-trestle-2.2.0/trestle/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/profile_resolver.py` & `compliance-trestle-2.2.0/trestle/core/profile_resolver.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/refs_validator.py` & `compliance-trestle-2.2.0/trestle/core/refs_validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/remote/__init__.py` & `compliance-trestle-2.2.0/trestle/core/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/remote/cache.py` & `compliance-trestle-2.2.0/trestle/core/remote/cache.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/repository.py` & `compliance-trestle-2.2.0/trestle/core/repository.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/resolver/__init__.py` & `compliance-trestle-2.2.0/trestle/core/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/resolver/_import.py` & `compliance-trestle-2.2.0/trestle/core/resolver/_import.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/resolver/merge.py` & `compliance-trestle-2.2.0/trestle/core/resolver/merge.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/resolver/modify.py` & `compliance-trestle-2.2.0/trestle/core/resolver/modify.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/resolver/prune.py` & `compliance-trestle-2.2.0/trestle/core/resolver/prune.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/rule_parameters_validator.py` & `compliance-trestle-2.2.0/trestle/core/rule_parameters_validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/ssp_io.py` & `compliance-trestle-2.2.0/trestle/core/ssp_io.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/trestle_base_model.py` & `compliance-trestle-2.2.0/trestle/core/trestle_base_model.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/validator.py` & `compliance-trestle-2.2.0/trestle/core/validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/core/validator_factory.py` & `compliance-trestle-2.2.0/trestle/core/validator_factory.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/oscal/__init__.py` & `compliance-trestle-2.2.0/trestle/oscal/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/oscal/assessment_plan.py` & `compliance-trestle-2.2.0/trestle/oscal/assessment_plan.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/oscal/assessment_results.py` & `compliance-trestle-2.2.0/trestle/oscal/assessment_results.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/oscal/catalog.py` & `compliance-trestle-2.2.0/trestle/oscal/catalog.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/oscal/common.py` & `compliance-trestle-2.2.0/trestle/oscal/common.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/oscal/component.py` & `compliance-trestle-2.2.0/trestle/oscal/component.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/oscal/poam.py` & `compliance-trestle-2.2.0/trestle/oscal/poam.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/oscal/profile.py` & `compliance-trestle-2.2.0/trestle/oscal/profile.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/oscal/ssp.py` & `compliance-trestle-2.2.0/trestle/oscal/ssp.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/resources/__init__.py` & `compliance-trestle-2.2.0/trestle/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/resources/templates/FedRAMP_control_header_template.yaml` & `compliance-trestle-2.2.0/trestle/resources/templates/FedRAMP_control_header_template.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/resources/templates/__init__.py` & `compliance-trestle-2.2.0/trestle/resources/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/resources/templates/template.drawio` & `compliance-trestle-2.2.0/trestle/resources/templates/template.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/tasks/__init__.py` & `compliance-trestle-2.2.0/trestle/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/tasks/base_task.py` & `compliance-trestle-2.2.0/trestle/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/tasks/cis_xlsx_to_oscal_catalog.py` & `compliance-trestle-2.2.0/trestle/tasks/cis_xlsx_to_oscal_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     """
 
     name = 'cis-xlsx-to-oscal-catalog'
     ns = 'https://ibm.github.io/compliance-trestle/schemas/oscal/catalog/cis'
 
     def __init__(self, config_object: Optional[configparser.SectionProxy]) -> None:
         """
-        Initialize trestle task ocp4-cis-profile-to-oscal-catalog.
+        Initialize trestle task.
 
         Args:
             config_object: Config section associated with the task.
         """
         super().__init__(config_object)
 
     def print_info(self) -> None:
```

### Comparing `compliance-trestle-2.1.1/trestle/tasks/csv_to_oscal_cd.py` & `compliance-trestle-2.2.0/trestle/tasks/csv_to_oscal_cd.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/tasks/ocp4_cis_profile_to_oscal_catalog.py` & `compliance-trestle-2.2.0/trestle/tasks/ocp4_cis_profile_to_oscal_catalog.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/tasks/ocp4_cis_profile_to_oscal_cd.py` & `compliance-trestle-2.2.0/trestle/tasks/ocp4_cis_profile_to_oscal_cd.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/tasks/oscal_profile_to_osco_profile.py` & `compliance-trestle-2.2.0/trestle/tasks/oscal_profile_to_osco_profile.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/tasks/osco_result_to_oscal_ar.py` & `compliance-trestle-2.2.0/trestle/tasks/osco_result_to_oscal_ar.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/tasks/tanium_result_to_oscal_ar.py` & `compliance-trestle-2.2.0/trestle/tasks/tanium_result_to_oscal_ar.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/tasks/transform.py` & `compliance-trestle-2.2.0/trestle/tasks/transform.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/tasks/xccdf_result_to_oscal_ar.py` & `compliance-trestle-2.2.0/trestle/tasks/xccdf_result_to_oscal_ar.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/tasks/xlsx_helper.py` & `compliance-trestle-2.2.0/trestle/tasks/xlsx_helper.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/tasks/xlsx_to_oscal_cd.py` & `compliance-trestle-2.2.0/trestle/tasks/xlsx_to_oscal_cd.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/tasks/xlsx_to_oscal_profile.py` & `compliance-trestle-2.2.0/trestle/tasks/xlsx_to_oscal_profile.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/transforms/__init__.py` & `compliance-trestle-2.2.0/trestle/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/transforms/implementations/__init__.py` & `compliance-trestle-2.2.0/trestle/transforms/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/transforms/implementations/osco.py` & `compliance-trestle-2.2.0/trestle/transforms/implementations/osco.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/transforms/implementations/tanium.py` & `compliance-trestle-2.2.0/trestle/transforms/implementations/tanium.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/transforms/implementations/xccdf.py` & `compliance-trestle-2.2.0/trestle/transforms/implementations/xccdf.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/transforms/results.py` & `compliance-trestle-2.2.0/trestle/transforms/results.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/transforms/transformer_factory.py` & `compliance-trestle-2.2.0/trestle/transforms/transformer_factory.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/transforms/transformer_helper.py` & `compliance-trestle-2.2.0/trestle/transforms/transformer_helper.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.1.1/trestle/transforms/transformer_singleton.py` & `compliance-trestle-2.2.0/trestle/transforms/transformer_singleton.py`

 * *Files identical despite different names*

