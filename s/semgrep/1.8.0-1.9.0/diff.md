# Comparing `tmp/semgrep-1.8.0.tar.gz` & `tmp/semgrep-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/semgrep-1.8.0.tar", last modified: Wed Feb  1 02:28:43 2023, max compression
+gzip compressed data, was "dist/semgrep-1.9.0.tar", last modified: Thu Feb  2 00:08:36 2023, max compression
```

## Comparing `semgrep-1.8.0.tar` & `semgrep-1.9.0.tar`

### file list

```diff
@@ -1,129 +1,141 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/
--rw-r--r--   0 root         (0) root         (0)    26526 2023-02-01 02:27:57.000000 semgrep-1.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      155 2023-02-01 02:27:57.000000 semgrep-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13849 2023-02-01 02:28:43.000000 semgrep-1.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-01 02:28:43.000000 semgrep-1.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5649 2023-02-01 02:27:57.000000 semgrep-1.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semdep/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2200 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/find_lockfiles.py
--rw-r--r--   0 root         (0) root         (0)     1362 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/package_restrictions.py
--rw-r--r--   0 root         (0) root         (0)    21662 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/parse_lockfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semdep/parsers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/parsers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2633 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/parsers/gem.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/parsers/go_sum.py
--rw-r--r--   0 root         (0) root         (0)     3220 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/parsers/gradle.py
--rw-r--r--   0 root         (0) root         (0)     3427 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/parsers/package_lock.py
--rw-r--r--   0 root         (0) root         (0)     2321 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/parsers/pipfile.py
--rw-r--r--   0 root         (0) root         (0)     4387 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/parsers/poetry.py
--rw-r--r--   0 root         (0) root         (0)     2767 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/parsers/pom_tree.py
--rw-r--r--   0 root         (0) root         (0)     4876 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/parsers/requirements.py
--rw-r--r--   0 root         (0) root         (0)    10449 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/parsers/util.py
--rw-r--r--   0 root         (0) root         (0)     8327 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semdep/parsers/yarn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep/
--rw-r--r--   0 root         (0) root         (0)       22 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      157 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep/app/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/app/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/app/auth.py
--rw-r--r--   0 root         (0) root         (0)      898 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/app/registry.py
--rw-r--r--   0 root         (0) root         (0)    14354 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/app/scans.py
--rw-r--r--   0 root         (0) root         (0)     6451 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/app/session.py
--rw-r--r--   0 root         (0) root         (0)     5400 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/app/version.py
--rw-r--r--   0 root         (0) root         (0)     8360 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/autofix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep/bin/
--rw-r--r--   0 root         (0) root         (0)       99 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/bin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1672 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/bytesize.py
--rwxr-xr-x   0 root         (0) root         (0)     3072 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19795 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/commands/ci.py
--rw-r--r--   0 root         (0) root         (0)     5218 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/commands/install.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/commands/login.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/commands/lsp.py
--rw-r--r--   0 root         (0) root         (0)     7138 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    32812 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/commands/scan.py
--rw-r--r--   0 root         (0) root         (0)     4338 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/commands/shouldafound.py
--rw-r--r--   0 root         (0) root         (0)     1866 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/commands/wrapper.py
--rw-r--r--   0 root         (0) root         (0)    26837 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/config_resolver.py
--rw-r--r--   0 root         (0) root         (0)     4313 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/constants.py
--rw-r--r--   0 root         (0) root         (0)     8238 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/core_output.py
--rw-r--r--   0 root         (0) root         (0)    40169 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/core_runner.py
--rw-r--r--   0 root         (0) root         (0)     2974 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/default_group.py
--rw-r--r--   0 root         (0) root         (0)     8106 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/dependency_aware_rule.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/dump_ast.py
--rw-r--r--   0 root         (0) root         (0)     4618 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/env.py
--rw-r--r--   0 root         (0) root         (0)    14987 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/error.py
--rw-r--r--   0 root         (0) root         (0)     2543 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/error_handler.py
--rw-r--r--   0 root         (0) root         (0)      317 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/exclude_rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep/external/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/external/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4229 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/external/git_url_parser.py
--rw-r--r--   0 root         (0) root         (0)    14909 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/external/junit_xml.py
--rw-r--r--   0 root         (0) root         (0)    13844 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/external/pymmh3.py
--rw-r--r--   0 root         (0) root         (0)     8134 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/fork_subprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep/formatter/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/formatter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/formatter/base.py
--rw-r--r--   0 root         (0) root         (0)     1491 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/formatter/emacs.py
--rw-r--r--   0 root         (0) root         (0)     4308 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/formatter/gitlab_sast.py
--rw-r--r--   0 root         (0) root         (0)      733 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/formatter/gitlab_secrets.py
--rw-r--r--   0 root         (0) root         (0)     2919 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/formatter/json.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/formatter/junit_xml.py
--rw-r--r--   0 root         (0) root         (0)    16674 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/formatter/sarif.py
--rw-r--r--   0 root         (0) root         (0)    28061 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/formatter/text.py
--rw-r--r--   0 root         (0) root         (0)     1242 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/formatter/vim.py
--rw-r--r--   0 root         (0) root         (0)    13990 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/git.py
--rw-r--r--   0 root         (0) root         (0)    10295 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/ignores.py
--rw-r--r--   0 root         (0) root         (0)    22498 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/join_rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep/lang/
--rw-r--r--   0 root         (0) root         (0)     6384 2023-02-01 02:28:15.000000 semgrep-1.8.0/src/semgrep/lang/lang.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep/lsp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/lsp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11158 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/lsp/config.py
--rw-r--r--   0 root         (0) root         (0)     6539 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/lsp/convert.py
--rw-r--r--   0 root         (0) root         (0)     2722 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/lsp/metrics.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/lsp/run_semgrep.py
--rw-r--r--   0 root         (0) root         (0)    29071 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/lsp/server.py
--rw-r--r--   0 root         (0) root         (0)      287 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/lsp/types.py
--rw-r--r--   0 root         (0) root         (0)    34874 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/meta.py
--rw-r--r--   0 root         (0) root         (0)    14360 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/metrics.py
--rw-r--r--   0 root         (0) root         (0)     5287 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/nosemgrep.py
--rw-r--r--   0 root         (0) root         (0)     1171 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/notifications.py
--rw-r--r--   0 root         (0) root         (0)    19157 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/output.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/output_extra.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/output_from_core.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/parsing_data.py
--rw-r--r--   0 root         (0) root         (0)      492 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/profile_manager.py
--rw-r--r--   0 root         (0) root         (0)     4278 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/profiling.py
--rw-r--r--   0 root         (0) root         (0)     3964 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/project.py
--rw-r--r--   0 root         (0) root         (0)    10159 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/rule.py
--rw-r--r--   0 root         (0) root         (0)    19330 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/rule_lang.py
--rw-r--r--   0 root         (0) root         (0)    18283 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/rule_match.py
--rw-r--r--   0 root         (0) root         (0)     5156 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/semgrep_core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep/semgrep_interfaces/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 02:28:15.000000 semgrep-1.8.0/src/semgrep/semgrep_interfaces/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25907 2023-02-01 02:28:15.000000 semgrep-1.8.0/src/semgrep/semgrep_interfaces/rule_schema_v1.yaml
--rw-r--r--   0 root         (0) root         (0)   110663 2023-02-01 02:28:15.000000 semgrep-1.8.0/src/semgrep/semgrep_interfaces/semgrep_output_v1.py
--rw-r--r--   0 root         (0) root         (0)    19112 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/semgrep_main.py
--rw-r--r--   0 root         (0) root         (0)     3108 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/semgrep_types.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/settings.py
--rw-r--r--   0 root         (0) root         (0)     1175 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/state.py
--rw-r--r--   0 root         (0) root         (0)    28751 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/target_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep/templates/
--rw-r--r--   0 root         (0) root         (0)      211 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/templates/.semgrepignore
--rw-r--r--   0 root         (0) root         (0)     3546 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/terminal.py
--rw-r--r--   0 root         (0) root         (0)    24453 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/test.py
--rw-r--r--   0 root         (0) root         (0)      731 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/types.py
--rw-r--r--   0 root         (0) root         (0)     7666 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/util.py
--rw-r--r--   0 root         (0) root         (0)     1610 2023-02-01 02:27:57.000000 semgrep-1.8.0/src/semgrep/verbose_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13849 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3193 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      332 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-02-01 02:28:43.000000 semgrep-1.8.0/src/semgrep.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)    26526 2023-02-02 00:07:35.000000 semgrep-1.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      155 2023-02-02 00:07:35.000000 semgrep-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13862 2023-02-02 00:08:36.000000 semgrep-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-02 00:08:36.000000 semgrep-1.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5649 2023-02-02 00:07:35.000000 semgrep-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semdep/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semdep/external/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/external/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semdep/external/packaging/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/external/packaging/__about__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/external/packaging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11488 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/external/packaging/_manylinux.py
+-rw-r--r--   0 root         (0) root         (0)     4393 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/external/packaging/_musllinux.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/external/packaging/_structures.py
+-rw-r--r--   0 root         (0) root         (0)    30125 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/external/packaging/specifiers.py
+-rw-r--r--   0 root         (0) root         (0)    15714 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/external/packaging/tags.py
+-rw-r--r--   0 root         (0) root         (0)     4215 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/external/packaging/utils.py
+-rw-r--r--   0 root         (0) root         (0)    14680 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/external/packaging/version.py
+-rw-r--r--   0 root         (0) root         (0)     2200 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/find_lockfiles.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/package_restrictions.py
+-rw-r--r--   0 root         (0) root         (0)    21726 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/parse_lockfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semdep/parsers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/parsers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/parsers/gem.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/parsers/go_sum.py
+-rw-r--r--   0 root         (0) root         (0)     3220 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/parsers/gradle.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/parsers/package_lock.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/parsers/pipfile.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/parsers/poetry.py
+-rw-r--r--   0 root         (0) root         (0)     2767 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/parsers/pom_tree.py
+-rw-r--r--   0 root         (0) root         (0)     4876 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/parsers/requirements.py
+-rw-r--r--   0 root         (0) root         (0)    10449 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/parsers/util.py
+-rw-r--r--   0 root         (0) root         (0)     8327 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semdep/parsers/yarn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      157 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep/app/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/app/auth.py
+-rw-r--r--   0 root         (0) root         (0)      898 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/app/registry.py
+-rw-r--r--   0 root         (0) root         (0)    14354 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/app/scans.py
+-rw-r--r--   0 root         (0) root         (0)     6451 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/app/session.py
+-rw-r--r--   0 root         (0) root         (0)     5400 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/app/version.py
+-rw-r--r--   0 root         (0) root         (0)     8360 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/autofix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep/bin/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/bin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/bytesize.py
+-rwxr-xr-x   0 root         (0) root         (0)     3072 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19929 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/commands/ci.py
+-rw-r--r--   0 root         (0) root         (0)     5218 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/commands/install.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/commands/login.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/commands/lsp.py
+-rw-r--r--   0 root         (0) root         (0)     7138 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    32812 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/commands/scan.py
+-rw-r--r--   0 root         (0) root         (0)     4338 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/commands/shouldafound.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/commands/wrapper.py
+-rw-r--r--   0 root         (0) root         (0)    26837 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/config_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     4313 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/constants.py
+-rw-r--r--   0 root         (0) root         (0)     8238 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/core_output.py
+-rw-r--r--   0 root         (0) root         (0)    40169 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/core_runner.py
+-rw-r--r--   0 root         (0) root         (0)     2974 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/default_group.py
+-rw-r--r--   0 root         (0) root         (0)     8169 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/dependency_aware_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/dump_ast.py
+-rw-r--r--   0 root         (0) root         (0)     4618 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/env.py
+-rw-r--r--   0 root         (0) root         (0)    14987 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/error.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/error_handler.py
+-rw-r--r--   0 root         (0) root         (0)      317 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/exclude_rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep/external/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/external/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4229 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/external/git_url_parser.py
+-rw-r--r--   0 root         (0) root         (0)    14909 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/external/junit_xml.py
+-rw-r--r--   0 root         (0) root         (0)    13844 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/external/pymmh3.py
+-rw-r--r--   0 root         (0) root         (0)     8134 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/fork_subprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep/formatter/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/formatter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/formatter/base.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/formatter/emacs.py
+-rw-r--r--   0 root         (0) root         (0)     4308 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/formatter/gitlab_sast.py
+-rw-r--r--   0 root         (0) root         (0)      733 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/formatter/gitlab_secrets.py
+-rw-r--r--   0 root         (0) root         (0)     2919 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/formatter/json.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/formatter/junit_xml.py
+-rw-r--r--   0 root         (0) root         (0)    16674 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/formatter/sarif.py
+-rw-r--r--   0 root         (0) root         (0)    28061 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/formatter/text.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/formatter/vim.py
+-rw-r--r--   0 root         (0) root         (0)    13990 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/git.py
+-rw-r--r--   0 root         (0) root         (0)    10295 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/ignores.py
+-rw-r--r--   0 root         (0) root         (0)    22498 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/join_rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep/lang/
+-rw-r--r--   0 root         (0) root         (0)     6384 2023-02-02 00:08:03.000000 semgrep-1.9.0/src/semgrep/lang/lang.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep/lsp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/lsp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11158 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/lsp/config.py
+-rw-r--r--   0 root         (0) root         (0)     6539 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/lsp/convert.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/lsp/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/lsp/run_semgrep.py
+-rw-r--r--   0 root         (0) root         (0)    29071 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/lsp/server.py
+-rw-r--r--   0 root         (0) root         (0)      287 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/lsp/types.py
+-rw-r--r--   0 root         (0) root         (0)    35072 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/meta.py
+-rw-r--r--   0 root         (0) root         (0)    14680 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     5287 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/nosemgrep.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/notifications.py
+-rw-r--r--   0 root         (0) root         (0)    19157 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/output.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/output_extra.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/output_from_core.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/parsing_data.py
+-rw-r--r--   0 root         (0) root         (0)      492 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/profile_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4278 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/profiling.py
+-rw-r--r--   0 root         (0) root         (0)     3964 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/project.py
+-rw-r--r--   0 root         (0) root         (0)    10159 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/rule.py
+-rw-r--r--   0 root         (0) root         (0)    19330 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/rule_lang.py
+-rw-r--r--   0 root         (0) root         (0)    18283 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/rule_match.py
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/semgrep_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep/semgrep_interfaces/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-02 00:08:03.000000 semgrep-1.9.0/src/semgrep/semgrep_interfaces/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25907 2023-02-02 00:08:03.000000 semgrep-1.9.0/src/semgrep/semgrep_interfaces/rule_schema_v1.yaml
+-rw-r--r--   0 root         (0) root         (0)   110663 2023-02-02 00:08:03.000000 semgrep-1.9.0/src/semgrep/semgrep_interfaces/semgrep_output_v1.py
+-rw-r--r--   0 root         (0) root         (0)    19275 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/semgrep_main.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/semgrep_types.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/settings.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/state.py
+-rw-r--r--   0 root         (0) root         (0)    28751 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/target_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep/templates/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/templates/.semgrepignore
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/terminal.py
+-rw-r--r--   0 root         (0) root         (0)    24453 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/test.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/types.py
+-rw-r--r--   0 root         (0) root         (0)     7666 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/util.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-02-02 00:07:35.000000 semgrep-1.9.0/src/semgrep/verbose_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13862 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3605 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      332 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-02-02 00:08:36.000000 semgrep-1.9.0/src/semgrep.egg-info/top_level.txt
```

### Comparing `semgrep-1.8.0/LICENSE` & `semgrep-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/PKG-INFO` & `semgrep-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semgrep
-Version: 1.8.0
+Version: 1.9.0
 Summary: Lightweight static analysis for many languages. Find bug variants with patterns that look like source code.
 Home-page: https://github.com/returntocorp/semgrep
 Author: Return To Corporation
 Author-email: support@r2c.dev
 License: UNKNOWN
 Description: </br>
         <p align="center">
@@ -69,15 +69,15 @@
         
         Semgrep is developed and commercially supported by [r2c, a software security company](https://r2c.dev).
         
         ### Language support
         
         <h4 align="center">General availability</h4>
         <p align="center">
-        C# · Go · Java · JavaScript · JSX · JSON · PHP · Python · Ruby · Scala · TypeScript · TSX</br>
+        C# · Go · Java · JavaScript · JSX · JSON · PHP · Python · Ruby · Scala · Terraform · TypeScript · TSX</br>
         </p>
         <h4 align="center">Beta & experimental</h4>
         <p align="center">
         See <a href="https://semgrep.dev/docs/supported-languages/">supported languages</a> for the complete list.
         </p>
         
         ### Getting started
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: semgrep Version: 1.8.0 Summary: Lightweight static
+Metadata-Version: 2.1 Name: semgrep Version: 1.9.0 Summary: Lightweight static
 analysis for many languages. Find bug variants with patterns that look like
 source code. Home-page: https://github.com/returntocorp/semgrep Author: Return
 To Corporation Author-email: support@r2c.dev License: UNKNOWN Description:
                                 [Semgrep_logo]
   **** Code scanning at ludicrous speed.  Find bugs and reachable dependency
                            vulnerabilities in code.
                Enforce your code standards on every commit. ****
@@ -29,15 +29,15 @@
 dependency vulnerabilities. Join hundreds of thousands of other developers and
 security engineers already using Semgrep at companies like GitLab, Dropbox,
 Slack, Figma, Shopify, HashiCorp, Snowflake, and Trail of Bits. Semgrep is
 developed and commercially supported by [r2c, a software security company]
 (https://r2c.dev). ### Language support
                          *** General availability ***
 C# Â· Go Â· Java Â· JavaScript Â· JSX Â· JSON Â· PHP Â· Python Â· Ruby Â· Scala
-                             Â· TypeScript Â· TSX
+                       Â· Terraform Â· TypeScript Â· TSX
                           *** Beta & experimental ***
                 See supported_languages for the complete list.
 ### Getting started To install Semgrep use Homebrew or pip, or run without
 installation via Docker: ```sh # For macOS $ brew install semgrep # For Ubuntu/
 WSL/Linux/macOS $ python3 -m pip install semgrep # To try Semgrep without
 installation run via Docker $ docker run --rm -v "${PWD}:/src" returntocorp/
 semgrep semgrep ``` Once installed, Semgrep can run with single rules or entire
```

### Comparing `semgrep-1.8.0/setup.py` & `semgrep-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     "colorama~=0.4.0",
     "click~=8.1",
     "click-option-group~=0.5",
     "glom~=22.1",
     "requests~=2.22",
     "ruamel.yaml>=0.16.0,<0.18",
     "tqdm~=4.46",
-    "packaging~=21.0",
+    "packaging>=21.0",
     "jsonschema~=4.6",
     "wcmatch~=8.3",
     "peewee~=3.14",
     "defusedxml~=0.7.1",
     "urllib3~=1.26",
     "typing-extensions~=4.2",
     "python-lsp-jsonrpc~=1.0.0",
@@ -136,15 +136,15 @@
     "parsy~=2.0",
 ]
 
 extras_require = {"experiments": ["jsonnet~=0.18"]}
 
 setuptools.setup(
     name="semgrep",
-    version="1.8.0",
+    version="1.9.0",
     author="Return To Corporation",
     author_email="support@r2c.dev",
     description="Lightweight static analysis for many languages. Find bug variants with patterns that look like source code.",
     cmdclass=cmdclass,
     install_requires=install_requires,
     extras_require=extras_require,
     long_description=long_description,
```

### Comparing `semgrep-1.8.0/src/semdep/find_lockfiles.py` & `semgrep-1.9.0/src/semdep/find_lockfiles.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semdep/package_restrictions.py` & `semgrep-1.9.0/src/semdep/package_restrictions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from typing import Iterator
 from typing import List
 from typing import Tuple
 
-import packaging.version
-from packaging.specifiers import SpecifierSet
-
+from semdep.external.packaging.specifiers import InvalidSpecifier  # type: ignore
+from semdep.external.packaging.specifiers import SpecifierSet  # type: ignore
 from semgrep.error import SemgrepError
 from semgrep.semgrep_interfaces.semgrep_output_v1 import DependencyPattern
 from semgrep.semgrep_interfaces.semgrep_output_v1 import FoundDependency
 
 
 def semver_matches(expression: str, actual_version: str) -> bool:
 
     try:
         ss = SpecifierSet(expression)
         matched = len(list(ss.filter([actual_version]))) > 0
         # print(f'does {expression} match {actual_version}?: {matched}')
         return matched
-    except packaging.specifiers.InvalidSpecifier:
+    except InvalidSpecifier:
         raise SemgrepError(
             f"unknown package version comparison expression: {expression}"
         )
 
 
 # compare vulnerable range to version in lockfile
 def dependencies_range_match_any(
```

### Comparing `semgrep-1.8.0/src/semdep/parse_lockfile.py` & `semgrep-1.9.0/src/semdep/parse_lockfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from typing import Generator
 from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import tomli
-from packaging.version import InvalidVersion
-from packaging.version import Version
 
+from semdep.external.packaging.version import InvalidVersion  # type: ignore
+from semdep.external.packaging.version import Version  # type: ignore
 from semgrep.error import SemgrepError
 from semgrep.verbose_logging import getLogger
 
 # NOTE: Defused XML doesn't export types :(
 
 
 logger = getLogger(__name__)
```

### Comparing `semgrep-1.8.0/src/semdep/parsers/gem.py` & `semgrep-1.9.0/src/semdep/parsers/gem.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semdep/parsers/go_sum.py` & `semgrep-1.9.0/src/semdep/parsers/go_sum.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semdep/parsers/gradle.py` & `semgrep-1.9.0/src/semdep/parsers/gradle.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semdep/parsers/package_lock.py` & `semgrep-1.9.0/src/semdep/parsers/package_lock.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semdep/parsers/pipfile.py` & `semgrep-1.9.0/src/semdep/parsers/pipfile.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semdep/parsers/poetry.py` & `semgrep-1.9.0/src/semdep/parsers/poetry.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semdep/parsers/pom_tree.py` & `semgrep-1.9.0/src/semdep/parsers/pom_tree.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semdep/parsers/requirements.py` & `semgrep-1.9.0/src/semdep/parsers/requirements.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semdep/parsers/util.py` & `semgrep-1.9.0/src/semdep/parsers/util.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semdep/parsers/yarn.py` & `semgrep-1.9.0/src/semdep/parsers/yarn.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/app/auth.py` & `semgrep-1.9.0/src/semgrep/app/auth.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/app/registry.py` & `semgrep-1.9.0/src/semgrep/app/registry.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/app/scans.py` & `semgrep-1.9.0/src/semgrep/app/scans.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/app/session.py` & `semgrep-1.9.0/src/semgrep/app/session.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/app/version.py` & `semgrep-1.9.0/src/semgrep/app/version.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/autofix.py` & `semgrep-1.9.0/src/semgrep/autofix.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/bytesize.py` & `semgrep-1.9.0/src/semgrep/bytesize.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/cli.py` & `semgrep-1.9.0/src/semgrep/cli.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/commands/ci.py` & `semgrep-1.9.0/src/semgrep/commands/ci.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,33 +327,36 @@
                 traceback.print_exc()
                 logger.info(f"Could not start scan {e}")
                 sys.exit(FATAL_EXIT_CODE)
 
             assert config  # Config has to be defined here. Helping mypy out
             # Run DeepSemgrep when available but only for full scans
             is_full_scan = metadata.merge_base_ref is None
-            deep = scan_handler.deepsemgrep if scan_handler and is_full_scan else False
+            engine = EngineType.OSS
+            if scan_handler and scan_handler.deepsemgrep:
+                engine = EngineType.INTERFILE if is_full_scan else EngineType.PRO
+
             (semgrep_pro_path, _deep_semgrep_path) = determine_semgrep_pro_path()
 
             # Set a default max_memory for CI runs when DeepSemgrep is on because
             # DeepSemgrep is likely to run out
             if max_memory is None:
-                if deep:
+                if engine is EngineType.INTERFILE:
                     max_memory = DEFAULT_MAX_MEMORY_PRO_CI
                 else:
                     max_memory = 0  # unlimited
             # Same for timeout (Github actions has a 6 hour timeout)
             if interfile_timeout is None:
-                if deep:
+                if engine is EngineType.INTERFILE:
                     interfile_timeout = DEFAULT_PRO_TIMEOUT_CI
                 else:
                     interfile_timeout = 0  # unlimited
-            if deep and not semgrep_pro_path.exists():
+            if engine.is_pro and not semgrep_pro_path.exists():
                 run_install_semgrep_pro()
-            if deep:
+            if engine is EngineType.INTERFILE:
                 # Add the p/deepsemgrep rules
                 # TODO this is a temporary hack!!! In the future,
                 # we will ensure that deepsemgrep rules are in the
                 # default-v1 ruleset. This code should be removed
                 # by Feburary 2023
                 deep_semgrep_rules = Config.from_config_list(["p/deepsemgrep"], None)[
                     0
@@ -382,15 +385,15 @@
                 filtered_rules,
                 profiler,
                 output_extra,
                 shown_severities,
                 lockfile_scan_info,
             ) = semgrep.semgrep_main.main(
                 core_opts_str=core_opts,
-                engine=EngineType.INTERFILE if deep else EngineType.OSS,
+                engine=engine,
                 output_handler=output_handler,
                 target=[os.curdir],  # semgrep ci only scans cwd
                 pattern=None,
                 lang=None,
                 configs=config,
                 no_rewrite_rule_ids=(not rewrite_rule_ids),
                 jobs=jobs,
```

### Comparing `semgrep-1.8.0/src/semgrep/commands/install.py` & `semgrep-1.9.0/src/semgrep/commands/install.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/commands/login.py` & `semgrep-1.9.0/src/semgrep/commands/login.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/commands/lsp.py` & `semgrep-1.9.0/src/semgrep/commands/lsp.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/commands/publish.py` & `semgrep-1.9.0/src/semgrep/commands/publish.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/commands/scan.py` & `semgrep-1.9.0/src/semgrep/commands/scan.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/commands/shouldafound.py` & `semgrep-1.9.0/src/semgrep/commands/shouldafound.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/commands/wrapper.py` & `semgrep-1.9.0/src/semgrep/commands/wrapper.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/config_resolver.py` & `semgrep-1.9.0/src/semgrep/config_resolver.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/constants.py` & `semgrep-1.9.0/src/semgrep/constants.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/core_output.py` & `semgrep-1.9.0/src/semgrep/core_output.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/core_runner.py` & `semgrep-1.9.0/src/semgrep/core_runner.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/default_group.py` & `semgrep-1.9.0/src/semgrep/default_group.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/dependency_aware_rule.py` & `semgrep-1.9.0/src/semgrep/dependency_aware_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 from typing import Callable
 from typing import Dict
 from typing import Iterator
 from typing import List
 from typing import Set
 from typing import Tuple
 
-from packaging.specifiers import InvalidSpecifier
-from packaging.specifiers import SpecifierSet
-
 import semgrep.output_from_core as core
+from semdep.external.packaging.specifiers import InvalidSpecifier  # type: ignore
+from semdep.external.packaging.specifiers import SpecifierSet  # type: ignore
 from semdep.find_lockfiles import find_single_lockfile
 from semdep.package_restrictions import dependencies_range_match_any
 from semgrep.error import SemgrepError
 from semgrep.rule import Rule
 from semgrep.rule_match import RuleMatch
 from semgrep.semgrep_interfaces.semgrep_output_v1 import DependencyMatch
 from semgrep.semgrep_interfaces.semgrep_output_v1 import DependencyPattern
```

### Comparing `semgrep-1.8.0/src/semgrep/dump_ast.py` & `semgrep-1.9.0/src/semgrep/dump_ast.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/env.py` & `semgrep-1.9.0/src/semgrep/env.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/error.py` & `semgrep-1.9.0/src/semgrep/error.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/error_handler.py` & `semgrep-1.9.0/src/semgrep/error_handler.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/external/git_url_parser.py` & `semgrep-1.9.0/src/semgrep/external/git_url_parser.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/external/junit_xml.py` & `semgrep-1.9.0/src/semgrep/external/junit_xml.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/external/pymmh3.py` & `semgrep-1.9.0/src/semgrep/external/pymmh3.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/fork_subprocess.py` & `semgrep-1.9.0/src/semgrep/fork_subprocess.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/formatter/base.py` & `semgrep-1.9.0/src/semgrep/formatter/base.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/formatter/emacs.py` & `semgrep-1.9.0/src/semgrep/formatter/emacs.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/formatter/gitlab_sast.py` & `semgrep-1.9.0/src/semgrep/formatter/gitlab_sast.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/formatter/gitlab_secrets.py` & `semgrep-1.9.0/src/semgrep/formatter/gitlab_secrets.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/formatter/json.py` & `semgrep-1.9.0/src/semgrep/formatter/json.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/formatter/junit_xml.py` & `semgrep-1.9.0/src/semgrep/formatter/junit_xml.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/formatter/sarif.py` & `semgrep-1.9.0/src/semgrep/formatter/sarif.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/formatter/text.py` & `semgrep-1.9.0/src/semgrep/formatter/text.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/formatter/vim.py` & `semgrep-1.9.0/src/semgrep/formatter/vim.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/git.py` & `semgrep-1.9.0/src/semgrep/git.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/ignores.py` & `semgrep-1.9.0/src/semgrep/ignores.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/join_rule.py` & `semgrep-1.9.0/src/semgrep/join_rule.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/lang/lang.json` & `semgrep-1.9.0/src/semgrep/lang/lang.json`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/lsp/config.py` & `semgrep-1.9.0/src/semgrep/lsp/config.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/lsp/convert.py` & `semgrep-1.9.0/src/semgrep/lsp/convert.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/lsp/metrics.py` & `semgrep-1.9.0/src/semgrep/lsp/metrics.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/lsp/run_semgrep.py` & `semgrep-1.9.0/src/semgrep/lsp/run_semgrep.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/lsp/server.py` & `semgrep-1.9.0/src/semgrep/lsp/server.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/meta.py` & `semgrep-1.9.0/src/semgrep/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -759,15 +759,17 @@
 
     @property
     def repo_url(self) -> Optional[str]:
         repo_url = os.getenv("SEMGREP_REPO_URL")
         if repo_url:
             return repo_url
 
-        url = get_url_from_sstp_url(os.getenv("BITBUCKET_GIT_HTTP_ORIGIN"))
+        # Bitbucket Cloud URLs should be in the format: http://bitbucket.org/<workspace>/<repo>
+        # Bitbucker Server URLs should be in the format: https://bitbucket<company>.com/projects/<PROJECT>/repos/<REPO_NAME>
+        url = os.getenv("BITBUCKET_GIT_HTTP_ORIGIN")
         return url if url else super().repo_url
 
     @property
     def branch(self) -> Optional[str]:
         branch = os.getenv("SEMGREP_BRANCH")
         if branch:
             return branch
```

### Comparing `semgrep-1.8.0/src/semgrep/metrics.py` & `semgrep-1.9.0/src/semgrep/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import requests
 from attr import define
 from attr import Factory
 from typing_extensions import LiteralString
 from typing_extensions import TypedDict
 
 from semgrep import __VERSION__
+from semgrep.constants import EngineType
 from semgrep.error import SemgrepError
 from semgrep.parsing_data import ParsingData
 from semgrep.profile_manager import ProfileManager
 from semgrep.profiling import ProfilingData
 from semgrep.rule import Rule
 from semgrep.semgrep_types import Language
 from semgrep.types import FilteredMatches
@@ -96,14 +97,15 @@
 
 
 class ValueRequiredSchema(TypedDict):
     features: Set[str]
 
 
 class ValueSchema(ValueRequiredSchema, total=False):
+    engineRequested: str
     numFindings: int
     numIgnored: int
     ruleHashesWithFindings: Dict[str, int]
 
 
 class FixRateSchema(TypedDict, total=False):
     lowerLimits: Dict[str, int]
@@ -212,14 +214,21 @@
             and metrics_state != legacy_state
         ):
             raise click.BadParameter(
                 "--enable-metrics/--disable-metrics can not be used with either --metrics or SEMGREP_SEND_METRICS"
             )
         self.metrics_state = metrics_state or legacy_state or MetricsState.AUTO
 
+    @suppress_errors
+    def add_engine_type(self, engineType: EngineType) -> None:
+        """
+        Assumes configs is list of arguments passed to semgrep using --config
+        """
+        self.payload["value"]["engineRequested"] = engineType.name
+
     @property
     def is_using_registry(self) -> bool:
         return self._is_using_registry
 
     @is_using_registry.setter
     def is_using_registry(self, value: bool) -> None:
         if self.is_using_registry is False and value is True:
```

### Comparing `semgrep-1.8.0/src/semgrep/nosemgrep.py` & `semgrep-1.9.0/src/semgrep/nosemgrep.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/notifications.py` & `semgrep-1.9.0/src/semgrep/notifications.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/output.py` & `semgrep-1.9.0/src/semgrep/output.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/output_extra.py` & `semgrep-1.9.0/src/semgrep/output_extra.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/parsing_data.py` & `semgrep-1.9.0/src/semgrep/parsing_data.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/profiling.py` & `semgrep-1.9.0/src/semgrep/profiling.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/project.py` & `semgrep-1.9.0/src/semgrep/project.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/rule.py` & `semgrep-1.9.0/src/semgrep/rule.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/rule_lang.py` & `semgrep-1.9.0/src/semgrep/rule_lang.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/rule_match.py` & `semgrep-1.9.0/src/semgrep/rule_match.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/semgrep_core.py` & `semgrep-1.9.0/src/semgrep/semgrep_core.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/semgrep_interfaces/rule_schema_v1.yaml` & `semgrep-1.9.0/src/semgrep/semgrep_interfaces/rule_schema_v1.yaml`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/semgrep_interfaces/semgrep_output_v1.py` & `semgrep-1.9.0/src/semgrep/semgrep_interfaces/semgrep_output_v1.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/semgrep_main.py` & `semgrep-1.9.0/src/semgrep/semgrep_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,21 @@
 
     if exclude_rule is None:
         exclude_rule = []
 
     project_url = get_project_url()
     profiler = ProfileManager()
 
+    # Metrics send part 1: add environment information
+    metrics = get_state().metrics
+    if metrics.is_enabled:
+        metrics.add_project_url(project_url)
+        metrics.add_configs(configs)
+        metrics.add_engine_type(engine)
+
     rule_start_time = time.time()
     configs_obj, config_errors = get_config(
         pattern, lang, configs, replacement=replacement, project_url=project_url
     )
     all_rules = configs_obj.get_rules(no_rewrite_rule_ids)
     profiler.save("config_time", rule_start_time)
 
@@ -492,18 +499,16 @@
         rule_matches_by_rule, keep_ignored=keep_ignored, strict=strict
     )
     profiler.save("ignores_time", ignores_start_time)
     output_handler.handle_semgrep_errors(nosem_errors)
 
     profiler.save("total_time", rule_start_time)
 
-    metrics = get_state().metrics
+    # Metrics send part 2: send results
     if metrics.is_enabled:
-        metrics.add_project_url(project_url)
-        metrics.add_configs(configs)
         metrics.add_rules(filtered_rules, output_extra.profiling_data)
         metrics.add_max_memory_bytes(output_extra.profiling_data)
         metrics.add_targets(output_extra.all_targets, output_extra.profiling_data)
         metrics.add_findings(filtered_matches_by_rule)
         metrics.add_errors(semgrep_errors)
         metrics.add_profiling(profiler)
         metrics.add_parse_rates(output_extra.parsing_data)
```

### Comparing `semgrep-1.8.0/src/semgrep/semgrep_types.py` & `semgrep-1.9.0/src/semgrep/semgrep_types.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/settings.py` & `semgrep-1.9.0/src/semgrep/settings.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/state.py` & `semgrep-1.9.0/src/semgrep/state.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/target_manager.py` & `semgrep-1.9.0/src/semgrep/target_manager.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/terminal.py` & `semgrep-1.9.0/src/semgrep/terminal.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/test.py` & `semgrep-1.9.0/src/semgrep/test.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/types.py` & `semgrep-1.9.0/src/semgrep/types.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/util.py` & `semgrep-1.9.0/src/semgrep/util.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep/verbose_logging.py` & `semgrep-1.9.0/src/semgrep/verbose_logging.py`

 * *Files identical despite different names*

### Comparing `semgrep-1.8.0/src/semgrep.egg-info/PKG-INFO` & `semgrep-1.9.0/src/semgrep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semgrep
-Version: 1.8.0
+Version: 1.9.0
 Summary: Lightweight static analysis for many languages. Find bug variants with patterns that look like source code.
 Home-page: https://github.com/returntocorp/semgrep
 Author: Return To Corporation
 Author-email: support@r2c.dev
 License: UNKNOWN
 Description: </br>
         <p align="center">
@@ -69,15 +69,15 @@
         
         Semgrep is developed and commercially supported by [r2c, a software security company](https://r2c.dev).
         
         ### Language support
         
         <h4 align="center">General availability</h4>
         <p align="center">
-        C# · Go · Java · JavaScript · JSX · JSON · PHP · Python · Ruby · Scala · TypeScript · TSX</br>
+        C# · Go · Java · JavaScript · JSX · JSON · PHP · Python · Ruby · Scala · Terraform · TypeScript · TSX</br>
         </p>
         <h4 align="center">Beta & experimental</h4>
         <p align="center">
         See <a href="https://semgrep.dev/docs/supported-languages/">supported languages</a> for the complete list.
         </p>
         
         ### Getting started
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: semgrep Version: 1.8.0 Summary: Lightweight static
+Metadata-Version: 2.1 Name: semgrep Version: 1.9.0 Summary: Lightweight static
 analysis for many languages. Find bug variants with patterns that look like
 source code. Home-page: https://github.com/returntocorp/semgrep Author: Return
 To Corporation Author-email: support@r2c.dev License: UNKNOWN Description:
                                 [Semgrep_logo]
   **** Code scanning at ludicrous speed.  Find bugs and reachable dependency
                            vulnerabilities in code.
                Enforce your code standards on every commit. ****
@@ -29,15 +29,15 @@
 dependency vulnerabilities. Join hundreds of thousands of other developers and
 security engineers already using Semgrep at companies like GitLab, Dropbox,
 Slack, Figma, Shopify, HashiCorp, Snowflake, and Trail of Bits. Semgrep is
 developed and commercially supported by [r2c, a software security company]
 (https://r2c.dev). ### Language support
                          *** General availability ***
 C# Â· Go Â· Java Â· JavaScript Â· JSX Â· JSON Â· PHP Â· Python Â· Ruby Â· Scala
-                             Â· TypeScript Â· TSX
+                       Â· Terraform Â· TypeScript Â· TSX
                           *** Beta & experimental ***
                 See supported_languages for the complete list.
 ### Getting started To install Semgrep use Homebrew or pip, or run without
 installation via Docker: ```sh # For macOS $ brew install semgrep # For Ubuntu/
 WSL/Linux/macOS $ python3 -m pip install semgrep # To try Semgrep without
 installation run via Docker $ docker run --rm -v "${PWD}:/src" returntocorp/
 semgrep semgrep ``` Once installed, Semgrep can run with single rules or entire
```

### Comparing `semgrep-1.8.0/src/semgrep.egg-info/SOURCES.txt` & `semgrep-1.9.0/src/semgrep.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 LICENSE
 MANIFEST.in
 setup.py
 src/semdep/__init__.py
 src/semdep/find_lockfiles.py
 src/semdep/package_restrictions.py
 src/semdep/parse_lockfile.py
+src/semdep/external/__init__.py
+src/semdep/external/packaging/__about__.py
+src/semdep/external/packaging/__init__.py
+src/semdep/external/packaging/_manylinux.py
+src/semdep/external/packaging/_musllinux.py
+src/semdep/external/packaging/_structures.py
+src/semdep/external/packaging/specifiers.py
+src/semdep/external/packaging/tags.py
+src/semdep/external/packaging/utils.py
+src/semdep/external/packaging/version.py
 src/semdep/parsers/__init__.py
 src/semdep/parsers/gem.py
 src/semdep/parsers/go_sum.py
 src/semdep/parsers/gradle.py
 src/semdep/parsers/package_lock.py
 src/semdep/parsers/pipfile.py
 src/semdep/parsers/poetry.py
```

