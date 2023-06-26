# Comparing `tmp/dev-gpt-0.18.44.dev3.tar.gz` & `tmp/dev-gpt-0.18.45.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-gpt-0.18.44.dev3.tar", last modified: Mon Jun 26 13:16:19 2023, max compression
+gzip compressed data, was "dev-gpt-0.18.45.dev1.tar", last modified: Mon Jun 26 13:17:02 2023, max compression
```

## Comparing `dev-gpt-0.18.44.dev3.tar` & `dev-gpt-0.18.45.dev1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.218276 dev-gpt-0.18.44.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21577 2023-06-26 13:16:19.218276 dev-gpt-0.18.44.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20820 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.206276 dev-gpt-0.18.44.dev3/dev_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 13:16:18.000000 dev-gpt-0.18.44.dev3/dev_gpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.206276 dev-gpt-0.18.44.dev3/dev_gpt/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/apis/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/apis/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/apis/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.206276 dev-gpt-0.18.44.dev3/dev_gpt/options/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.206276 dev-gpt-0.18.44.dev3/dev_gpt/options/configure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/configure/key_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.210276 dev-gpt-0.18.44.dev3/dev_gpt/options/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/deploy/deployer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.210276 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.210276 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/auto_refine_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/extract_information.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/fix_based_on_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/get_user_input_if_needed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/question_answering.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/conversation_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    32269 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.210276 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/pm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/pm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/pm/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/pm/task_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/prompt_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.202276 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.210276 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/base_image/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/base_image/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.214276 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/gateway/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/gateway/app_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/gateway/app_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/gateway/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/gateway/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.214276 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/microservice/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/microservice/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/microservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/microservice/google_custom_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/microservice/gpt_3_5_turbo.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/templates_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    20692 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/templates_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.214276 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/tools/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/generate/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.214276 dev-gpt-0.18.44.dev3/dev_gpt/options/run/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/options/run/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.214276 dev-gpt-0.18.44.dev3/dev_gpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/dev_gpt/utils/string_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.206276 dev-gpt-0.18.44.dev3/dev_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21577 2023-06-26 13:16:19.000000 dev-gpt-0.18.44.dev3/dev_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-26 13:16:19.000000 dev-gpt-0.18.44.dev3/dev_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:16:19.000000 dev-gpt-0.18.44.dev3/dev_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 13:16:19.000000 dev-gpt-0.18.44.dev3/dev_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-26 13:16:19.000000 dev-gpt-0.18.44.dev3/dev_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 13:16:19.000000 dev-gpt-0.18.44.dev3/dev_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 13:16:19.218276 dev-gpt-0.18.44.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.214276 dev-gpt-0.18.44.dev3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.218276 dev-gpt-0.18.44.dev3/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/integration/test_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:19.218276 dev-gpt-0.18.44.dev3/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/unit/test_construct_sub_task_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/unit/test_error_summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/unit/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/unit/test_response_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/unit/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/unit/test_self_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/unit/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/unit/test_sub_fn_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/unit/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-26 13:16:14.000000 dev-gpt-0.18.44.dev3/test/unit/test_yes_no_question.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.645341 dev-gpt-0.18.45.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21577 2023-06-26 13:17:02.645341 dev-gpt-0.18.45.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20820 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.637341 dev-gpt-0.18.45.dev1/dev_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 13:17:02.000000 dev-gpt-0.18.45.dev1/dev_gpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.637341 dev-gpt-0.18.45.dev1/dev_gpt/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/apis/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/apis/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/apis/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.637341 dev-gpt-0.18.45.dev1/dev_gpt/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.637341 dev-gpt-0.18.45.dev1/dev_gpt/options/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/configure/key_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.637341 dev-gpt-0.18.45.dev1/dev_gpt/options/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/deploy/deployer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.641341 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.641341 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/auto_refine_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/extract_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/fix_based_on_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/get_user_input_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/conversation_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32269 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.641341 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/pm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/pm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/pm/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/pm/task_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/prompt_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.637341 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.641341 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/base_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/base_image/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.641341 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/gateway/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/gateway/app_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/gateway/app_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/gateway/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/gateway/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.641341 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/microservice/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/microservice/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/microservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/microservice/google_custom_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/microservice/gpt_3_5_turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/templates_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20692 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/templates_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.641341 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/tools/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/generate/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.641341 dev-gpt-0.18.45.dev1/dev_gpt/options/run/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/options/run/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.641341 dev-gpt-0.18.45.dev1/dev_gpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/dev_gpt/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.637341 dev-gpt-0.18.45.dev1/dev_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21577 2023-06-26 13:17:02.000000 dev-gpt-0.18.45.dev1/dev_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-26 13:17:02.000000 dev-gpt-0.18.45.dev1/dev_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:17:02.000000 dev-gpt-0.18.45.dev1/dev_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 13:17:02.000000 dev-gpt-0.18.45.dev1/dev_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-26 13:17:02.000000 dev-gpt-0.18.45.dev1/dev_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 13:17:02.000000 dev-gpt-0.18.45.dev1/dev_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 13:17:02.645341 dev-gpt-0.18.45.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.641341 dev-gpt-0.18.45.dev1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.641341 dev-gpt-0.18.45.dev1/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/integration/test_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:17:02.645341 dev-gpt-0.18.45.dev1/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/unit/test_construct_sub_task_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/unit/test_error_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/unit/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/unit/test_response_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/unit/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/unit/test_self_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/unit/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/unit/test_sub_fn_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/unit/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-26 13:16:54.000000 dev-gpt-0.18.45.dev1/test/unit/test_yes_no_question.py
```

### Comparing `dev-gpt-0.18.44.dev3/LICENSE` & `dev-gpt-0.18.45.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/PKG-INFO` & `dev-gpt-0.18.45.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.44.dev3
+Version: 0.18.45.dev1
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.44.dev3 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.45.dev1 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Jina AI
 Author-email: hello@jina.ai License: Apache 2.0 Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `dev-gpt-0.18.44.dev3/README.md` & `dev-gpt-0.18.45.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/apis/gpt.py` & `dev-gpt-0.18.45.dev1/dev_gpt/apis/gpt.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/apis/jina_cloud.py` & `dev-gpt-0.18.45.dev1/dev_gpt/apis/jina_cloud.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/apis/pypi.py` & `dev-gpt-0.18.45.dev1/dev_gpt/apis/pypi.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/cli.py` & `dev-gpt-0.18.45.dev1/dev_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/constants.py` & `dev-gpt-0.18.45.dev1/dev_gpt/constants.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/__init__.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/__init__.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/configure/key_handling.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/configure/key_handling.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/auto_refine_description.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/auto_refine_description.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/extract_information.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/extract_information.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/fix_based_on_error.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/fix_based_on_error.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/get_user_input_if_needed.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/get_user_input_if_needed.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/question_answering.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/question_answering.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/translation.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/translation.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/conversation_logger.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/conversation_logger.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/generator.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/generator.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/parser.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/parser.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/pm/pm.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/pm/pm.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/pm/task_tree_schema.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/pm/task_tree_schema.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/gateway/app_template.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/gateway/app_template.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/gateway/custom_gateway.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/gateway/custom_gateway.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/gateway/nginx.conf` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/gateway/nginx.conf`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/microservice/google_custom_search.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/microservice/google_custom_search.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/static_files/microservice/gpt_3_5_turbo.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/static_files/microservice/gpt_3_5_turbo.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/templates_system.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/templates_system.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/templates_user.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/templates_user.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/options/generate/ui.py` & `dev-gpt-0.18.45.dev1/dev_gpt/options/generate/ui.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/utils/io.py` & `dev-gpt-0.18.45.dev1/dev_gpt/utils/io.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt/utils/string_tools.py` & `dev-gpt-0.18.45.dev1/dev_gpt/utils/string_tools.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt.egg-info/PKG-INFO` & `dev-gpt-0.18.45.dev1/dev_gpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.44.dev3
+Version: 0.18.45.dev1
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.44.dev3 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.45.dev1 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Jina AI
 Author-email: hello@jina.ai License: Apache 2.0 Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `dev-gpt-0.18.44.dev3/dev_gpt.egg-info/SOURCES.txt` & `dev-gpt-0.18.45.dev1/dev_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/setup.py` & `dev-gpt-0.18.45.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/test/conftest.py` & `dev-gpt-0.18.45.dev1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/test/integration/test_generator.py` & `dev-gpt-0.18.45.dev1/test/integration/test_generator.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/test/unit/test_api.py` & `dev-gpt-0.18.45.dev1/test/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/test/unit/test_error_summarization.py` & `dev-gpt-0.18.45.dev1/test/unit/test_error_summarization.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/test/unit/test_packages.py` & `dev-gpt-0.18.45.dev1/test/unit/test_packages.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/test/unit/test_response_parsing.py` & `dev-gpt-0.18.45.dev1/test/unit/test_response_parsing.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/test/unit/test_self_refinement.py` & `dev-gpt-0.18.45.dev1/test/unit/test_self_refinement.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/test/unit/test_strings.py` & `dev-gpt-0.18.45.dev1/test/unit/test_strings.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/test/unit/test_sub_fn_tree.py` & `dev-gpt-0.18.45.dev1/test/unit/test_sub_fn_tree.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/test/unit/test_tools.py` & `dev-gpt-0.18.45.dev1/test/unit/test_tools.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.44.dev3/test/unit/test_yes_no_question.py` & `dev-gpt-0.18.45.dev1/test/unit/test_yes_no_question.py`

 * *Files identical despite different names*

