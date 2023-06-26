# Comparing `tmp/thipster-0.19.4.tar.gz` & `tmp/thipster-0.19.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.19.4.tar", last modified: Mon Jun 26 09:01:29 2023, max compression
+gzip compressed data, was "thipster-0.19.5.tar", last modified: Mon Jun 26 09:32:10 2023, max compression
```

## Comparing `thipster-0.19.4.tar` & `thipster-0.19.5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:01:29.432322 thipster-0.19.4/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-26 09:01:25.000000 thipster-0.19.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-26 09:01:25.000000 thipster-0.19.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5376 2023-06-26 09:01:29.432322 thipster-0.19.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4544 2023-06-26 09:01:25.000000 thipster-0.19.4/README.md
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-26 09:01:25.000000 thipster-0.19.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-26 09:01:25.000000 thipster-0.19.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 09:01:29.432322 thipster-0.19.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1848 2023-06-26 09:01:26.000000 thipster-0.19.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:01:29.424322 thipster-0.19.4/tests/
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:01:29.424322 thipster-0.19.4/tests/engine/
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     6190 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:01:29.424322 thipster-0.19.4/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:01:29.424322 thipster-0.19.4/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    16811 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 root         (0) root         (0)    15104 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3748 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     5314 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/parser/test_parserfactory.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/parser/test_yamlparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:01:29.424322 thipster-0.19.4/tests/repository/
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/repository/test_github_repository.py
--rw-r--r--   0 root         (0) root         (0)     6375 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/repository/test_local_repository.py
--rw-r--r--   0 root         (0) root         (0)     6201 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/repository/test_resourcemodel.py
--rw-r--r--   0 root         (0) root         (0)     3577 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     6483 2023-06-26 09:01:25.000000 thipster-0.19.4/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:01:29.424322 thipster-0.19.4/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:01:29.428322 thipster-0.19.4/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:01:29.428322 thipster-0.19.4/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5610 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      456 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     2166 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     5081 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4646 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:01:29.428322 thipster-0.19.4/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:01:29.428322 thipster-0.19.4/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12599 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     5311 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13732 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    16910 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     3223 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     2127 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2450 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    21596 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2631 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6866 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:01:29.432322 thipster-0.19.4/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4821 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:01:29.432322 thipster-0.19.4/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24574 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     3350 2023-06-26 09:01:25.000000 thipster-0.19.4/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:01:29.428322 thipster-0.19.4/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5376 2023-06-26 09:01:29.000000 thipster-0.19.4/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1957 2023-06-26 09:01:29.000000 thipster-0.19.4/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 09:01:29.000000 thipster-0.19.4/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      388 2023-06-26 09:01:29.000000 thipster-0.19.4/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-26 09:01:29.000000 thipster-0.19.4/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:32:10.872453 thipster-0.19.5/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-26 09:32:05.000000 thipster-0.19.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-26 09:32:05.000000 thipster-0.19.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-06-26 09:32:10.872453 thipster-0.19.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4544 2023-06-26 09:32:05.000000 thipster-0.19.5/README.md
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-26 09:32:05.000000 thipster-0.19.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-26 09:32:05.000000 thipster-0.19.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 09:32:10.872453 thipster-0.19.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-06-26 09:32:06.000000 thipster-0.19.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:32:10.860452 thipster-0.19.5/tests/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:32:10.860452 thipster-0.19.5/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6190 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:32:10.860452 thipster-0.19.5/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:32:10.860452 thipster-0.19.5/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    16811 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 root         (0) root         (0)    15104 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3748 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     5314 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/parser/test_parserfactory.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/parser/test_yamlparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:32:10.864452 thipster-0.19.5/tests/repository/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/repository/test_github_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6375 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/repository/test_local_repository.py
+-rw-r--r--   0 root         (0) root         (0)     6201 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/repository/test_resourcemodel.py
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     6483 2023-06-26 09:32:05.000000 thipster-0.19.5/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:32:10.864452 thipster-0.19.5/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:32:10.864452 thipster-0.19.5/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:32:10.864452 thipster-0.19.5/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5610 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     5081 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4646 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:32:10.868452 thipster-0.19.5/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:32:10.868452 thipster-0.19.5/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12599 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     5311 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13732 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    16910 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    21596 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6866 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:32:10.872453 thipster-0.19.5/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/repository/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4821 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:32:10.872453 thipster-0.19.5/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24680 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     3350 2023-06-26 09:32:05.000000 thipster-0.19.5/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:32:10.864452 thipster-0.19.5/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-06-26 09:32:10.000000 thipster-0.19.5/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-26 09:32:10.000000 thipster-0.19.5/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 09:32:10.000000 thipster-0.19.5/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      388 2023-06-26 09:32:10.000000 thipster-0.19.5/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-26 09:32:10.000000 thipster-0.19.5/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.19.4/LICENSE` & `thipster-0.19.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/PKG-INFO` & `thipster-0.19.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.19.4
+Version: 0.19.5
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.19.4 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.19.5 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.19.4/README.md` & `thipster-0.19.5/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/pyproject.toml` & `thipster-0.19.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/setup.py` & `thipster-0.19.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('requirements').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.19.4'
+__version__ = '0.19.5'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as rm:
     readme = rm.read()
```

### Comparing `thipster-0.19.4/tests/engine/test_engine.py` & `thipster-0.19.5/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/tests/engine/test_generation.py` & `thipster-0.19.5/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/tests/parser/dsl_parser/test_ast.py` & `thipster-0.19.5/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.19.5/tests/parser/dsl_parser/test_dslparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.19.5/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/tests/parser/dsl_parser/test_token.py` & `thipster-0.19.5/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.19.5/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/tests/parser/test_parsedfile.py` & `thipster-0.19.5/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/tests/parser/test_parserfactory.py` & `thipster-0.19.5/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/tests/parser/test_yamlparser.py` & `thipster-0.19.5/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/tests/repository/test_github_repository.py` & `thipster-0.19.5/tests/repository/test_github_repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 import pytest
 
 from thipster.engine.resource_model import ResourceModel
 from thipster.repository import GithubRepo
 from thipster.repository.exceptions import ModelNotFoundError
 
 repository = 'THipster/models'
+branch = 'main'
 
 
 def test_get_bucket():
     """Test get bucket model."""
-    gcp_bucket = 'gcp/bucket'
+    gcp_bucket = 'bucket'
     resources = [gcp_bucket]
 
-    repo = GithubRepo(repository)
+    repo = GithubRepo(repository, branch)
 
     models = repo.get(resources)
     assert isinstance(models, dict)
     assert len(models) == 2
 
     assert gcp_bucket in models
     assert isinstance(models[gcp_bucket], ResourceModel)
@@ -27,19 +28,19 @@
     assert len(bucket.attributes) == 1
     assert len(bucket.dependencies) == 0
     assert bucket.resource_type == gcp_bucket
 
 
 def test_get_vm():
     """Test get vm model and its dependencies."""
-    gcp_network = 'gcp/network'
-    gcp_vm = 'gcp/vm'
+    gcp_network = 'network'
+    gcp_vm = 'vm'
     resources = [gcp_vm]
 
-    repo = GithubRepo(repository)
+    repo = GithubRepo(repository, branch)
 
     models = repo.get(resources)
     assert isinstance(models, dict)
     assert len(models) == 2
 
     assert gcp_vm in models
     assert isinstance(models[gcp_vm], ResourceModel)
```

### Comparing `thipster-0.19.4/tests/repository/test_local_repository.py` & `thipster-0.19.5/tests/repository/test_local_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/tests/repository/test_resourcemodel.py` & `thipster-0.19.5/tests/repository/test_resourcemodel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/tests/test_e2e.py` & `thipster-0.19.5/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/tests/test_tools.py` & `thipster-0.19.5/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/auth/google.py` & `thipster-0.19.5/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/engine/engine.py` & `thipster-0.19.5/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/engine/i_parser.py` & `thipster-0.19.5/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/engine/i_repository.py` & `thipster-0.19.5/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/engine/i_terraform.py` & `thipster-0.19.5/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/engine/parsed_file.py` & `thipster-0.19.5/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/engine/resource_model.py` & `thipster-0.19.5/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/helpers.py` & `thipster-0.19.5/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/parser/dsl_parser/ast.py` & `thipster-0.19.5/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.19.5/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.19.5/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/parser/dsl_parser/lexer.py` & `thipster-0.19.5/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.19.5/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/parser/dsl_parser/parser.py` & `thipster-0.19.5/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/parser/dsl_parser/token.py` & `thipster-0.19.5/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.19.5/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/parser/exceptions.py` & `thipster-0.19.5/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/parser/parser_factory.py` & `thipster-0.19.5/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/parser/yaml_parser.py` & `thipster-0.19.5/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/repository/exceptions.py` & `thipster-0.19.5/thipster/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/repository/github.py` & `thipster-0.19.5/thipster/repository/github.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """GithubRepo.py module."""
 
+import json
+
 import requests
 
 from .exceptions import ModelNotFoundError
 from .json import JSONRepo
 
 
 class GithubRepo(JSONRepo):
@@ -41,15 +43,25 @@
             Name of the desired resource
 
         Returns
         -------
         str | bytes | bytearray
             Content of the JSON file defining the desired resource
         """
+        config_response = requests.get(
+            f'https://raw.githubusercontent.com/{self.__repo}/{self.__branch}/thipster-config.json',
+        )
+
+        if not config_response.ok:
+            raise ModelNotFoundError(name)
+
+        config_file: dict = json.loads(config_response.content)
+        repo_directory = config_file.get('model_folder')
+
         response = requests.get(
-            f'https://raw.githubusercontent.com/{self.__repo}/{self.__branch}/{name}.json',
+            f'https://raw.githubusercontent.com/{self.__repo}/{self.__branch}/{repo_directory}/{name}.json',
         )
 
         if not response.ok:
             raise ModelNotFoundError(name)
 
         return response.content
```

### Comparing `thipster-0.19.4/thipster/repository/json.py` & `thipster-0.19.5/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/repository/local.py` & `thipster-0.19.5/thipster/repository/local.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster/terraform/cdk.py` & `thipster-0.19.5/thipster/terraform/cdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -644,16 +644,19 @@
         if 'var_type' in internal_object_model else 'Unknown'
 
     if internal_object_type.startswith('list') or internal_object_model['is_list']:
         if internal_object_name not in ctx.resource_args\
                 and not internal_object_base_ctx.arg_to_complete:
             ctx.resource_args[internal_object_name] = []
 
-        if isinstance(internal_object_args, list)\
-                and not isinstance(internal_object_args[0], pf.ParsedAttribute):
+        if (
+            isinstance(internal_object_args, list)
+            and len(internal_object_args) > 0
+            and not isinstance(internal_object_args[0], pf.ParsedAttribute)
+        ):
             for internal_object in internal_object_args:
                 internal_object_ctx = copy.deepcopy(internal_object_base_ctx)
                 internal_object_ctx.regenerate()
 
                 if isinstance(internal_object, pf.ParsedDict):
                     res = _create_resource(
                         internal_object_ctx,
@@ -766,14 +769,15 @@
             ctx,
             resource_type=dependency_type,
         )
 
         # Creates explicit dependency
         if (
             isinstance(attribute_value, list)
+            and len(attribute_value) > 0
             and isinstance(attribute_value[0], pf.ParsedDict)
         ):
             ctx.resource_args[attribute_name] = []
             for dict_value in attribute_value:
                 dep_ctx.regenerate()
                 ctx.resource_args[attribute_name].append(
                     _create_dependency(
```

### Comparing `thipster-0.19.4/thipster/terraform/exceptions.py` & `thipster-0.19.5/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.19.4/thipster.egg-info/PKG-INFO` & `thipster-0.19.5/thipster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.19.4
+Version: 0.19.5
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.19.4 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.19.5 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.19.4/thipster.egg-info/SOURCES.txt` & `thipster-0.19.5/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

