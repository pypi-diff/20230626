# Comparing `tmp/khoj_assistant-0.6.3.dev96.tar.gz` & `tmp/khoj_assistant-0.6.3.dev97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Jun 25 18:41:47 2023, max compression
+gzip compressed data, last modified: Mon Jun 26 18:37:34 2023, max compression
```

## Comparing `khoj_assistant-0.6.3.dev96.tar` & `khoj_assistant-0.6.3.dev97.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0        0 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/__init__.py
--rw-r--r--   0        0        0    10848 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/configure.py
--rw-r--r--   0        0        0     4929 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      987 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    17819 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     3435 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0     9894 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0     5981 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     4419 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     6647 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    12798 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3492 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1828 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58507 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0   205167 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     7946 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6053 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0     6985 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5708 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     6891 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     6533 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16789 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5160 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    13690 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     3986 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      463 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7470 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2713 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3690 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    10930 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2494 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/utils/config.py
--rw-r--r--   0        0        0     3070 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6779 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4158 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1047 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/.gitignore
--rw-r--r--   0        0        0    32472 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/LICENSE
--rw-r--r--   0        0        0    22944 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/README.md
--rw-r--r--   0        0        0     2801 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/pyproject.toml
--rw-r--r--   0        0        0    25306 2023-06-25 18:41:47.000000 khoj_assistant-0.6.3.dev96/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10868 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/configure.py
+-rw-r--r--   0        0        0     4929 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/desktop/file_browser.py
+-rw-r--r--   0        0        0      987 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/desktop/labelled_text_field.py
+-rw-r--r--   0        0        0    17819 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1316 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     3435 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0     9894 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0     5981 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     4419 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     6647 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    12798 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3492 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1828 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58507 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0   205167 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     7946 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6053 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0     6985 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5708 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     6891 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     6533 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16789 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5160 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    13690 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     4001 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7470 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2713 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3690 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    10930 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2012 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2494 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     3070 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6779 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4158 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1047 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/.gitignore
+-rw-r--r--   0        0        0    32472 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/LICENSE
+-rw-r--r--   0        0        0    22944 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/README.md
+-rw-r--r--   0        0        0     2801 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/pyproject.toml
+-rw-r--r--   0        0        0    25306 2023-06-26 18:37:34.000000 khoj_assistant-0.6.3.dev97/PKG-INFO
```

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/configure.py` & `khoj_assistant-0.6.3.dev97/src/khoj/configure.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
 
     state.processor_config.conversation.chat_session = None
     logger.info("📩 Saved current chat session to conversation logs")
 
 
 @schedule.repeat(schedule.every(59).minutes)
 def upload_telemetry():
-    if not state.config.app.should_log_telemetry or not state.telemetry:
+    if not state.config or not state.config.app.should_log_telemetry or not state.telemetry:
         message = "📡 No telemetry to upload" if not state.telemetry else "📡 Telemetry logging disabled"
         logger.debug(message)
         return
 
     try:
         logger.debug(f"📡 Upload usage telemetry to {constants.telemetry_server}:\n{state.telemetry}")
         requests.post(constants.telemetry_server, json=state.telemetry)
```

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/main.py` & `khoj_assistant-0.6.3.dev97/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/desktop/file_browser.py` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/desktop/file_browser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/desktop/labelled_text_field.py` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/desktop/labelled_text_field.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/404.html` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/chat.html` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/config.html` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/index.html` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.6.3.dev97/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.6.3.dev97/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.6.3.dev97/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.6.3.dev97/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.6.3.dev97/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.6.3.dev97/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.6.3.dev97/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.6.3.dev97/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.6.3.dev97/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.6.3.dev97/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.6.3.dev97/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.6.3.dev97/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/routers/api.py` & `khoj_assistant-0.6.3.dev97/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/routers/api_beta.py` & `khoj_assistant-0.6.3.dev97/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/routers/web_client.py` & `khoj_assistant-0.6.3.dev97/src/khoj/routers/web_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,17 +61,18 @@
     default_copy = constants.default_config.copy()
     default_content_type = default_copy["content-type"][content_type]  # type: ignore
 
     default_config = TextContentConfig(
         compressed_jsonl=default_content_type["compressed-jsonl"],
         embeddings_file=default_content_type["embeddings-file"],
     )
+
     current_config = (
         state.config.content_type[content_type]
-        if state.config and state.config.content_type and content_type in state.config.content_type
+        if state.config and state.config.content_type and state.config.content_type[content_type]  # type: ignore
         else default_config
     )
     current_config = json.loads(current_config.json())
 
     return templates.TemplateResponse(
         "content_type_input.html",
         context={
```

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.6.3.dev97/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.6.3.dev97/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.6.3.dev97/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/search_type/image_search.py` & `khoj_assistant-0.6.3.dev97/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/search_type/text_search.py` & `khoj_assistant-0.6.3.dev97/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/utils/cli.py` & `khoj_assistant-0.6.3.dev97/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/utils/config.py` & `khoj_assistant-0.6.3.dev97/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/utils/constants.py` & `khoj_assistant-0.6.3.dev97/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/utils/helpers.py` & `khoj_assistant-0.6.3.dev97/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/utils/jsonl.py` & `khoj_assistant-0.6.3.dev97/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/utils/models.py` & `khoj_assistant-0.6.3.dev97/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.6.3.dev97/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/utils/state.py` & `khoj_assistant-0.6.3.dev97/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/src/khoj/utils/yaml.py` & `khoj_assistant-0.6.3.dev97/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/.gitignore` & `khoj_assistant-0.6.3.dev97/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/LICENSE` & `khoj_assistant-0.6.3.dev97/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/README.md` & `khoj_assistant-0.6.3.dev97/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/pyproject.toml` & `khoj_assistant-0.6.3.dev97/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev96/PKG-INFO` & `khoj_assistant-0.6.3.dev97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.6.3.dev96
+Version: 0.6.3.dev97
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

