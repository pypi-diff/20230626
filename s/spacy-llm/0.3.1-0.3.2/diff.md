# Comparing `tmp/spacy-llm-0.3.1.tar.gz` & `tmp/spacy-llm-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-llm-0.3.1.tar", last modified: Fri Jun 23 13:19:00 2023, max compression
+gzip compressed data, was "spacy-llm-0.3.2.tar", last modified: Mon Jun 26 12:21:30 2023, max compression
```

## Comparing `spacy-llm-0.3.1.tar` & `spacy-llm-0.3.2.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/
--rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    62605 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    61361 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      736 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1810 2023-06-23 13:19:00.737381 spacy-llm-0.3.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.721382 spacy-llm-0.3.1/spacy_llm/
--rw-r--r--   0 vsts      (1001) docker     (122)      234 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.721382 spacy-llm-0.3.1/spacy_llm/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)      348 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.721382 spacy-llm-0.3.1/spacy_llm/backends/integration/
--rw-r--r--   0 vsts      (1001) docker     (122)      502 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.725381 spacy-llm-0.3.1/spacy_llm/backends/integration/hf/
--rw-r--r--   0 vsts      (1001) docker     (122)      279 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/hf/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4712 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/hf/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2583 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/hf/dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3435 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/hf/openllama.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4715 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/hf/stablelm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.725381 spacy-llm-0.3.1/spacy_llm/backends/integration/remote/
--rw-r--r--   0 vsts      (1001) docker     (122)      280 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/remote/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1256 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/remote/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2807 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/remote/langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2592 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/integration/remote/minichain.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.725381 spacy-llm-0.3.1/spacy_llm/backends/rest/
--rw-r--r--   0 vsts      (1001) docker     (122)      229 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/rest/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4784 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/rest/anthropic.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6223 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/rest/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4157 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/rest/cohere.py
--rw-r--r--   0 vsts      (1001) docker     (122)      571 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/rest/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6601 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/rest/openai.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1901 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/backends/rest/registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7765 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1033 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.725381 spacy-llm-0.3.1/spacy_llm/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11318 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/pipeline/llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.725381 spacy-llm-0.3.1/spacy_llm/registry/
--rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/registry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/registry/normalizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1702 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/registry/reader.py
--rw-r--r--   0 vsts      (1001) docker     (122)      454 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/registry/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.725381 spacy-llm-0.3.1/spacy_llm/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3959 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/lemma.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7947 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)      512 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7901 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8724 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/spancat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.725381 spacy-llm-0.3.1/spacy_llm/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1003 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/lemma.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/ner.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/ner.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/rel.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/spancat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/spancat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/textcat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/textcat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/templates/textcat.v3.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)    15128 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/textcat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.729381 spacy-llm-0.3.1/spacy_llm/tasks/util/
--rw-r--r--   0 vsts      (1001) docker     (122)      220 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      223 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/util/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/util/parsing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4009 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/util/serialization.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4826 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tasks/util/span.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.729381 spacy-llm-0.3.1/spacy_llm/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.729381 spacy-llm-0.3.1/spacy_llm/tests/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2294 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_anthropic.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2960 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_cohere.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1682 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_minichain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1869 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_openllama.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3307 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_rest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2092 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/backends/test_stablelm.py
--rw-r--r--   0 vsts      (1001) docker     (122)      315 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1111 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.729381 spacy-llm-0.3.1/spacy_llm/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8027 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/pipeline/test_llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.729381 spacy-llm-0.3.1/spacy_llm/tests/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/
--rw-r--r--   0 vsts      (1001) docker     (122)     1115 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/lemma_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/lemma_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/lemma_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/ner_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/ner_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/ner_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/rel_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/spacy_llm/tests/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/templates/lemma_template.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/templates/ner_template.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/templates/textcat_template.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)     7949 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/test_lemma.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22403 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/test_ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5704 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/test_rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17202 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/test_spancat.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23835 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/tasks/test_textcat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5934 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/test_cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2001 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/test_combinations.py
--rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/tests/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8941 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/ty.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1764 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/spacy_llm/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.721382 spacy-llm-0.3.1/spacy_llm.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    62605 2023-06-23 13:19:00.000000 spacy-llm-0.3.1/spacy_llm.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     4685 2023-06-23 13:19:00.000000 spacy-llm-0.3.1/spacy_llm.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-23 13:19:00.000000 spacy-llm-0.3.1/spacy_llm.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-06-23 13:19:00.000000 spacy-llm-0.3.1/spacy_llm.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-23 13:19:00.000000 spacy-llm-0.3.1/spacy_llm.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      149 2023-06-23 13:19:00.000000 spacy-llm-0.3.1/spacy_llm.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-06-23 13:19:00.000000 spacy-llm-0.3.1/spacy_llm.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/multitask_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/multitask_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/multitask_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/ner_dolly/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/ner_dolly/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/ner_dolly/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/ner_langchain_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/ner_langchain_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/ner_langchain_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/ner_minichain_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/ner_minichain_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/ner_minichain_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/rel_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/rel_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/rel_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3509 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/tests/test_readme_examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2843 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/tests/test_usage_examples.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 13:19:00.733381 spacy-llm-0.3.1/usage_examples/textcat_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/textcat_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-06-23 13:18:50.000000 spacy-llm-0.3.1/usage_examples/textcat_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.404330 spacy-llm-0.3.2/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    63200 2023-06-26 12:21:30.404330 spacy-llm-0.3.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    61956 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      736 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1810 2023-06-26 12:21:30.404330 spacy-llm-0.3.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.388330 spacy-llm-0.3.2/spacy_llm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      234 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.388330 spacy-llm-0.3.2/spacy_llm/backends/
+-rw-r--r--   0 vsts      (1001) docker     (122)      348 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.388330 spacy-llm-0.3.2/spacy_llm/backends/integration/
+-rw-r--r--   0 vsts      (1001) docker     (122)      502 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.392330 spacy-llm-0.3.2/spacy_llm/backends/integration/hf/
+-rw-r--r--   0 vsts      (1001) docker     (122)      279 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/hf/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4712 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/hf/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2583 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/hf/dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3435 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/hf/openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4715 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/hf/stablelm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.392330 spacy-llm-0.3.2/spacy_llm/backends/integration/remote/
+-rw-r--r--   0 vsts      (1001) docker     (122)      280 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/remote/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1256 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/remote/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2807 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/remote/langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2592 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/integration/remote/minichain.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.392330 spacy-llm-0.3.2/spacy_llm/backends/rest/
+-rw-r--r--   0 vsts      (1001) docker     (122)      229 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/rest/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4784 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/rest/anthropic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6223 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/rest/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4157 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/rest/cohere.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      571 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/rest/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6601 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/rest/openai.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1901 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/backends/rest/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7765 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1033 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.392330 spacy-llm-0.3.2/spacy_llm/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11370 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/pipeline/llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.392330 spacy-llm-0.3.2/spacy_llm/registry/
+-rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/registry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/registry/normalizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1702 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/registry/reader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      454 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/registry/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.392330 spacy-llm-0.3.2/spacy_llm/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3959 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7947 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      512 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7901 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8724 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/spancat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.396330 spacy-llm-0.3.2/spacy_llm/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1003 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/lemma.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/ner.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/ner.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/rel.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/spancat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/spancat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/textcat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/textcat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/templates/textcat.v3.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)    15128 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/textcat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.396330 spacy-llm-0.3.2/spacy_llm/tasks/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)      220 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      223 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/util/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/util/parsing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4009 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/util/serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4826 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tasks/util/span.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.396330 spacy-llm-0.3.2/spacy_llm/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.396330 spacy-llm-0.3.2/spacy_llm/tests/backends/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2294 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_anthropic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2960 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_cohere.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1682 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_minichain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1869 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3307 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_rest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2092 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/backends/test_stablelm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      315 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1111 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.396330 spacy-llm-0.3.2/spacy_llm/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8288 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/pipeline/test_llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.400330 spacy-llm-0.3.2/spacy_llm/tests/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.400330 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1115 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/lemma_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/lemma_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/lemma_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/ner_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/ner_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/ner_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/rel_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_binary_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.400330 spacy-llm-0.3.2/spacy_llm/tests/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/templates/lemma_template.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/templates/ner_template.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/templates/textcat_template.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)     7949 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/test_lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22403 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/test_ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5704 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/test_rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17202 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/test_spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23835 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/tasks/test_textcat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7253 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/test_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2001 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/test_combinations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8941 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/ty.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1764 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/spacy_llm/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.388330 spacy-llm-0.3.2/spacy_llm.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    63200 2023-06-26 12:21:30.000000 spacy-llm-0.3.2/spacy_llm.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4685 2023-06-26 12:21:30.000000 spacy-llm-0.3.2/spacy_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-26 12:21:30.000000 spacy-llm-0.3.2/spacy_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-06-26 12:21:30.000000 spacy-llm-0.3.2/spacy_llm.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-26 12:21:30.000000 spacy-llm-0.3.2/spacy_llm.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      149 2023-06-26 12:21:30.000000 spacy-llm-0.3.2/spacy_llm.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-06-26 12:21:30.000000 spacy-llm-0.3.2/spacy_llm.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.400330 spacy-llm-0.3.2/usage_examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.400330 spacy-llm-0.3.2/usage_examples/multitask_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/multitask_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/multitask_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.400330 spacy-llm-0.3.2/usage_examples/ner_dolly/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/ner_dolly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/ner_dolly/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.400330 spacy-llm-0.3.2/usage_examples/ner_langchain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/ner_langchain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/ner_langchain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.404330 spacy-llm-0.3.2/usage_examples/ner_minichain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/ner_minichain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/ner_minichain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.404330 spacy-llm-0.3.2/usage_examples/rel_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/rel_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/rel_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.404330 spacy-llm-0.3.2/usage_examples/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3509 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/tests/test_readme_examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2843 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/tests/test_usage_examples.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-26 12:21:30.404330 spacy-llm-0.3.2/usage_examples/textcat_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/textcat_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-06-26 12:21:18.000000 spacy-llm-0.3.2/usage_examples/textcat_openai/run_pipeline.py
```

### Comparing `spacy-llm-0.3.1/LICENSE` & `spacy-llm-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/PKG-INFO` & `spacy-llm-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.3.1
+Version: 0.3.2
 Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
 Classifier: Development Status :: 4 - Beta
@@ -1022,31 +1022,35 @@
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
 
 ### Cache
 
 Interacting with LLMs, either through an external API or a local instance, is costly.
 Since developing an NLP pipeline generally means a lot of exploration and prototyping,
-`spacy-llm` implements a built-in cache to avoid reprocessing the same documents at each run.
+`spacy-llm` implements a built-in cache to avoid reprocessing the same documents at each run
+that keeps batches of documents stored on disk.
 
 Example config block:
 
 ```ini
 [components.llm.cache]
-@llm_misc = "spacy.BatchCache.v1",
+@llm_misc = "spacy.BatchCache.v1"
 path = "path/to/cache"
 batch_size = 64
 max_batches_in_mem = 4
 ```
 
-| Argument             | Type                         | Default | Description                                          |
-| -------------------- | ---------------------------- | ------- | ---------------------------------------------------- |
-| `path`               | `Optional[Union[str, Path]]` | `None`  | Cache directory. If `None`, no caching is performed. |
-| `batch_size`         | `int`                        | 64      | Number of docs in one batch (file).                  |
-| `max_batches_in_mem` | `int`                        | 4       | Max. number of batches to hold in memory.            |
+| Argument             | Type                         | Default | Description                                                                                                               |
+| -------------------- | ---------------------------- | ------- | ------------------------------------------------------------------------------------------------------------------------- |
+| `path`               | `Optional[Union[str, Path]]` | `None`  | Cache directory. If `None`, no caching is performed, and this component will act as a NoOp.                               |
+| `batch_size`         | `int`                        | 64      | Number of docs in one batch (file). Once a batch is full, it will be peristed to disk.                                    |
+| `max_batches_in_mem` | `int`                        | 4       | Max. number of batches to hold in memory. Allows you to limit the effect on your memory if you're handling a lot of docs. |
+
+When retrieving a document, the `BatchCache` will first figure out what batch the document belongs to. If the batch
+isn't in memory it will try to load the batch from disk and then move it into memory. 
 
 Note that since the cache is generated by a registered function, you can also provide your own registered function
 returning your own cache implementation. If you wish to do so, ensure that your cache object adheres to the
 `Protocol` defined in `spacy_llm.ty.Cache`.
 
 ### Various functions
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.3.1 Summary: Integrating LLMs
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.3.2 Summary: Integrating LLMs
 into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
 github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
@@ -633,23 +633,29 @@
 open_llama_7b_700bt_preview"` Note that Hugging Face will download this model
 the first time you use it - you can [define the cached directory](https://
 huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting the
 environmental variable `HF_HOME`. ### Cache Interacting with LLMs, either
 through an external API or a local instance, is costly. Since developing an NLP
 pipeline generally means a lot of exploration and prototyping, `spacy-llm`
 implements a built-in cache to avoid reprocessing the same documents at each
-run. Example config block: ```ini [components.llm.cache] @llm_misc =
-"spacy.BatchCache.v1", path = "path/to/cache" batch_size = 64
-max_batches_in_mem = 4 ``` | Argument | Type | Default | Description | | ------
--------------- | ---------------------------- | ------- | ---------------------
-------------------------------- | | `path` | `Optional[Union[str, Path]]` |
-`None` | Cache directory. If `None`, no caching is performed. | | `batch_size`
-| `int` | 64 | Number of docs in one batch (file). | | `max_batches_in_mem` |
-`int` | 4 | Max. number of batches to hold in memory. | Note that since the
-cache is generated by a registered function, you can also provide your own
+run that keeps batches of documents stored on disk. Example config block:
+```ini [components.llm.cache] @llm_misc = "spacy.BatchCache.v1" path = "path/
+to/cache" batch_size = 64 max_batches_in_mem = 4 ``` | Argument | Type |
+Default | Description | | -------------------- | ---------------------------- |
+------- | ---------------------------------------------------------------------
+---------------------------------------------------- | | `path` | `Optional
+[Union[str, Path]]` | `None` | Cache directory. If `None`, no caching is
+performed, and this component will act as a NoOp. | | `batch_size` | `int` | 64
+| Number of docs in one batch (file). Once a batch is full, it will be peristed
+to disk. | | `max_batches_in_mem` | `int` | 4 | Max. number of batches to hold
+in memory. Allows you to limit the effect on your memory if you're handling a
+lot of docs. | When retrieving a document, the `BatchCache` will first figure
+out what batch the document belongs to. If the batch isn't in memory it will
+try to load the batch from disk and then move it into memory. Note that since
+the cache is generated by a registered function, you can also provide your own
 registered function returning your own cache implementation. If you wish to do
 so, ensure that your cache object adheres to the `Protocol` defined in
 `spacy_llm.ty.Cache`. ### Various functions #### spacy.FewShotReader.v1 This
 function is registered in spaCy's `misc` registry, and reads in examples from a
 `.yml`, `.yaml`, `.json` or `.jsonl` file. It uses [`srsly`](https://
 github.com/explosion/srsly) to read in these files and parses them depending on
 the file extension. ```ini [components.llm.task.examples] @misc =
```

### Comparing `spacy-llm-0.3.1/README.md` & `spacy-llm-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -990,31 +990,35 @@
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
 
 ### Cache
 
 Interacting with LLMs, either through an external API or a local instance, is costly.
 Since developing an NLP pipeline generally means a lot of exploration and prototyping,
-`spacy-llm` implements a built-in cache to avoid reprocessing the same documents at each run.
+`spacy-llm` implements a built-in cache to avoid reprocessing the same documents at each run
+that keeps batches of documents stored on disk.
 
 Example config block:
 
 ```ini
 [components.llm.cache]
-@llm_misc = "spacy.BatchCache.v1",
+@llm_misc = "spacy.BatchCache.v1"
 path = "path/to/cache"
 batch_size = 64
 max_batches_in_mem = 4
 ```
 
-| Argument             | Type                         | Default | Description                                          |
-| -------------------- | ---------------------------- | ------- | ---------------------------------------------------- |
-| `path`               | `Optional[Union[str, Path]]` | `None`  | Cache directory. If `None`, no caching is performed. |
-| `batch_size`         | `int`                        | 64      | Number of docs in one batch (file).                  |
-| `max_batches_in_mem` | `int`                        | 4       | Max. number of batches to hold in memory.            |
+| Argument             | Type                         | Default | Description                                                                                                               |
+| -------------------- | ---------------------------- | ------- | ------------------------------------------------------------------------------------------------------------------------- |
+| `path`               | `Optional[Union[str, Path]]` | `None`  | Cache directory. If `None`, no caching is performed, and this component will act as a NoOp.                               |
+| `batch_size`         | `int`                        | 64      | Number of docs in one batch (file). Once a batch is full, it will be peristed to disk.                                    |
+| `max_batches_in_mem` | `int`                        | 4       | Max. number of batches to hold in memory. Allows you to limit the effect on your memory if you're handling a lot of docs. |
+
+When retrieving a document, the `BatchCache` will first figure out what batch the document belongs to. If the batch
+isn't in memory it will try to load the batch from disk and then move it into memory. 
 
 Note that since the cache is generated by a registered function, you can also provide your own registered function
 returning your own cache implementation. If you wish to do so, ensure that your cache object adheres to the
 `Protocol` defined in `spacy_llm.ty.Cache`.
 
 ### Various functions
```

#### html2text {}

```diff
@@ -616,23 +616,29 @@
 open_llama_7b_700bt_preview"` Note that Hugging Face will download this model
 the first time you use it - you can [define the cached directory](https://
 huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting the
 environmental variable `HF_HOME`. ### Cache Interacting with LLMs, either
 through an external API or a local instance, is costly. Since developing an NLP
 pipeline generally means a lot of exploration and prototyping, `spacy-llm`
 implements a built-in cache to avoid reprocessing the same documents at each
-run. Example config block: ```ini [components.llm.cache] @llm_misc =
-"spacy.BatchCache.v1", path = "path/to/cache" batch_size = 64
-max_batches_in_mem = 4 ``` | Argument | Type | Default | Description | | ------
--------------- | ---------------------------- | ------- | ---------------------
-------------------------------- | | `path` | `Optional[Union[str, Path]]` |
-`None` | Cache directory. If `None`, no caching is performed. | | `batch_size`
-| `int` | 64 | Number of docs in one batch (file). | | `max_batches_in_mem` |
-`int` | 4 | Max. number of batches to hold in memory. | Note that since the
-cache is generated by a registered function, you can also provide your own
+run that keeps batches of documents stored on disk. Example config block:
+```ini [components.llm.cache] @llm_misc = "spacy.BatchCache.v1" path = "path/
+to/cache" batch_size = 64 max_batches_in_mem = 4 ``` | Argument | Type |
+Default | Description | | -------------------- | ---------------------------- |
+------- | ---------------------------------------------------------------------
+---------------------------------------------------- | | `path` | `Optional
+[Union[str, Path]]` | `None` | Cache directory. If `None`, no caching is
+performed, and this component will act as a NoOp. | | `batch_size` | `int` | 64
+| Number of docs in one batch (file). Once a batch is full, it will be peristed
+to disk. | | `max_batches_in_mem` | `int` | 4 | Max. number of batches to hold
+in memory. Allows you to limit the effect on your memory if you're handling a
+lot of docs. | When retrieving a document, the `BatchCache` will first figure
+out what batch the document belongs to. If the batch isn't in memory it will
+try to load the batch from disk and then move it into memory. Note that since
+the cache is generated by a registered function, you can also provide your own
 registered function returning your own cache implementation. If you wish to do
 so, ensure that your cache object adheres to the `Protocol` defined in
 `spacy_llm.ty.Cache`. ### Various functions #### spacy.FewShotReader.v1 This
 function is registered in spaCy's `misc` registry, and reads in examples from a
 `.yml`, `.yaml`, `.json` or `.jsonl` file. It uses [`srsly`](https://
 github.com/explosion/srsly) to read in these files and parses them depending on
 the file extension. ```ini [components.llm.task.examples] @misc =
```

### Comparing `spacy-llm-0.3.1/pyproject.toml` & `spacy-llm-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/setup.cfg` & `spacy-llm-0.3.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.3.1
+version = 0.3.2
 description = Integrating LLMs into structured NLP pipelines
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `spacy-llm-0.3.1/spacy_llm/backends/integration/hf/base.py` & `spacy-llm-0.3.2/spacy_llm/backends/integration/hf/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/backends/integration/hf/dolly.py` & `spacy-llm-0.3.2/spacy_llm/backends/integration/hf/dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/backends/integration/hf/openllama.py` & `spacy-llm-0.3.2/spacy_llm/backends/integration/hf/openllama.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/backends/integration/hf/stablelm.py` & `spacy-llm-0.3.2/spacy_llm/backends/integration/hf/stablelm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/backends/integration/remote/base.py` & `spacy-llm-0.3.2/spacy_llm/backends/integration/remote/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/backends/integration/remote/langchain.py` & `spacy-llm-0.3.2/spacy_llm/backends/integration/remote/langchain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/backends/integration/remote/minichain.py` & `spacy-llm-0.3.2/spacy_llm/backends/integration/remote/minichain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/backends/rest/anthropic.py` & `spacy-llm-0.3.2/spacy_llm/backends/rest/anthropic.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/backends/rest/base.py` & `spacy-llm-0.3.2/spacy_llm/backends/rest/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/backends/rest/cohere.py` & `spacy-llm-0.3.2/spacy_llm/backends/rest/cohere.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/backends/rest/noop.py` & `spacy-llm-0.3.2/spacy_llm/backends/rest/noop.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/backends/rest/openai.py` & `spacy-llm-0.3.2/spacy_llm/backends/rest/openai.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/backends/rest/registry.py` & `spacy-llm-0.3.2/spacy_llm/backends/rest/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/cache.py` & `spacy-llm-0.3.2/spacy_llm/cache.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/compat.py` & `spacy-llm-0.3.2/spacy_llm/compat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/pipeline/llm.py` & `spacy-llm-0.3.2/spacy_llm/pipeline/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,29 +210,31 @@
             )
 
         final_docs = []
         for i, doc in enumerate(docs):
             if is_cached[i]:
                 cached_doc = self._cache[doc]
                 assert cached_doc is not None
+                cached_doc._context = doc._context
                 final_docs.append(cached_doc)
             else:
                 doc = next(modified_docs)
-                self._cache.add(doc)
-                final_docs.append(doc)
 
                 if self._save_io:
                     # Make sure the `llm_io` field is set
                     doc.user_data["llm_io"] = doc.user_data.get(
                         "llm_io", defaultdict(dict)
                     )
                     llm_io = doc.user_data["llm_io"][self._name]
                     llm_io["prompt"] = str(next(prompts_iters[2]))
                     llm_io["response"] = str(next(responses_iters[2]))
 
+                self._cache.add(doc)
+                final_docs.append(doc)
+
         return final_docs
 
     def to_bytes(
         self,
         *,
         exclude: Tuple[str] = cast(Tuple[str], tuple()),
     ) -> bytes:
```

### Comparing `spacy-llm-0.3.1/spacy_llm/registry/normalizer.py` & `spacy-llm-0.3.2/spacy_llm/registry/normalizer.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/registry/reader.py` & `spacy-llm-0.3.2/spacy_llm/registry/reader.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/__init__.py` & `spacy-llm-0.3.2/spacy_llm/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/lemma.py` & `spacy-llm-0.3.2/spacy_llm/tasks/lemma.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/ner.py` & `spacy-llm-0.3.2/spacy_llm/tasks/ner.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/noop.py` & `spacy-llm-0.3.2/spacy_llm/tasks/noop.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/rel.py` & `spacy-llm-0.3.2/spacy_llm/tasks/rel.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/spancat.py` & `spacy-llm-0.3.2/spacy_llm/tasks/spancat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/templates/lemma.jinja` & `spacy-llm-0.3.2/spacy_llm/tasks/templates/lemma.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/templates/ner.jinja` & `spacy-llm-0.3.2/spacy_llm/tasks/templates/ner.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/templates/ner.v2.jinja` & `spacy-llm-0.3.2/spacy_llm/tasks/templates/ner.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/templates/rel.jinja` & `spacy-llm-0.3.2/spacy_llm/tasks/templates/rel.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/templates/spancat.jinja` & `spacy-llm-0.3.2/spacy_llm/tasks/templates/spancat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/templates/spancat.v2.jinja` & `spacy-llm-0.3.2/spacy_llm/tasks/templates/spancat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/templates/textcat.jinja` & `spacy-llm-0.3.2/spacy_llm/tasks/templates/textcat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/templates/textcat.v2.jinja` & `spacy-llm-0.3.2/spacy_llm/tasks/templates/textcat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/templates/textcat.v3.jinja` & `spacy-llm-0.3.2/spacy_llm/tasks/templates/textcat.v3.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/textcat.py` & `spacy-llm-0.3.2/spacy_llm/tasks/textcat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/util/parsing.py` & `spacy-llm-0.3.2/spacy_llm/tasks/util/parsing.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/util/serialization.py` & `spacy-llm-0.3.2/spacy_llm/tasks/util/serialization.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tasks/util/span.py` & `spacy-llm-0.3.2/spacy_llm/tasks/util/span.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/backends/test_anthropic.py` & `spacy-llm-0.3.2/spacy_llm/tests/backends/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/backends/test_cohere.py` & `spacy-llm-0.3.2/spacy_llm/tests/backends/test_cohere.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/backends/test_dolly.py` & `spacy-llm-0.3.2/spacy_llm/tests/backends/test_dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/backends/test_langchain.py` & `spacy-llm-0.3.2/spacy_llm/tests/backends/test_langchain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/backends/test_minichain.py` & `spacy-llm-0.3.2/spacy_llm/tests/backends/test_minichain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/backends/test_openllama.py` & `spacy-llm-0.3.2/spacy_llm/tests/backends/test_openllama.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/backends/test_rest.py` & `spacy-llm-0.3.2/spacy_llm/tests/backends/test_rest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/backends/test_stablelm.py` & `spacy-llm-0.3.2/spacy_llm/tests/backends/test_stablelm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/conftest.py` & `spacy-llm-0.3.2/spacy_llm/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/pipeline/test_llm.py` & `spacy-llm-0.3.2/spacy_llm/tests/pipeline/test_llm.py`

 * *Files 11% similar despite different names*

```diff
@@ -94,14 +94,19 @@
 
     texts = [cached_text, "This is a test", "This is another test"]
 
     # Run it again, along with other documents
     docs = list(nlp.pipe(texts=texts, n_process=n_process))
     assert [doc.text for doc in docs] == texts
 
+    egs = [(text, i) for i, text in enumerate(texts)]
+    egs_processed = list(nlp.pipe(egs, as_tuples=True, n_process=n_process))
+    assert [doc.text for doc, _ in egs_processed] == texts
+    assert [eg for _, eg in egs_processed] == list(range(len(texts)))
+
 
 def test_llm_pipe_empty(nlp):
     """Test call .pipe() with empty batch."""
     assert list(nlp.pipe(texts=[])) == []
 
 
 def test_llm_serialize_bytes():
```

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/lemma_examples.json` & `spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/lemma_examples.json`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/lemma_examples.jsonl` & `spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/lemma_examples.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/lemma_examples.yml` & `spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/lemma_examples.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/tasks/examples/rel_examples.jsonl` & `spacy-llm-0.3.2/spacy_llm/tests/tasks/examples/rel_examples.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/tasks/test_lemma.py` & `spacy-llm-0.3.2/spacy_llm/tests/tasks/test_lemma.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/tasks/test_ner.py` & `spacy-llm-0.3.2/spacy_llm/tests/tasks/test_ner.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/tasks/test_rel.py` & `spacy-llm-0.3.2/spacy_llm/tests/tasks/test_rel.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/tasks/test_spancat.py` & `spacy-llm-0.3.2/spacy_llm/tests/tasks/test_spancat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/tasks/test_textcat.py` & `spacy-llm-0.3.2/spacy_llm/tests/tasks/test_textcat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/test_cache.py` & `spacy-llm-0.3.2/spacy_llm/tests/test_cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import copy
+import os
 import time
 from pathlib import Path
 from typing import Dict
 
 import pytest
 import spacy
 import srsly  # type: ignore[import]
 from spacy.language import Language
 from spacy.tokens import DocBin
 
 from ..cache import BatchCache
+from .compat import has_openai_key
 
 _DEFAULT_CFG = {
     "backend": {"api": "NoOp", "config": {"model": "NoOp"}},
     "task": {"@llm_tasks": "spacy.NoOp.v1"},
     "cache": {
         "batch_size": 2,
         "max_batches_in_mem": 3,
@@ -149,7 +151,36 @@
     with spacy.util.make_tempdir() as tmpdir:
         # Non-existing cache directory should be created.
         config = copy.deepcopy(_DEFAULT_CFG)
         assert not (tmpdir / "new_dir").exists()
         config["cache"]["path"] = str(tmpdir / "new_dir")
         spacy.blank("en").add_pipe("llm", config=config)
         assert (tmpdir / "new_dir").exists()
+
+
+@pytest.mark.external
+@pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
+def test_caching_llm_io() -> None:
+    """Test availability of LLM IO after caching."""
+    with spacy.util.make_tempdir() as tmpdir:
+        config = copy.deepcopy(_DEFAULT_CFG)
+        config["backend"]["api"] = "OpenAI"  # type: ignore[index]
+        config["backend"]["config"] = {"model": "gpt-3.5-turbo"}  # type: ignore[index]
+        config["cache"]["path"] = str(tmpdir)  # type: ignore[index]
+        config["cache"]["batch_size"] = 3  # type: ignore[index]
+        config["save_io"] = True
+        nlp = spacy.blank("en")
+        nlp.add_pipe("llm", config=config)
+        docs = [nlp(txt) for txt in ("What's 1+1?", "What's 2+2?", "What's 3+3?")]
+
+        assert all([doc.user_data["llm_io"]["llm"]] for doc in docs)
+        cached_file_names = [
+            f
+            for f in os.listdir(tmpdir)
+            if os.path.isfile(tmpdir / f) and f.endswith(".spacy")
+        ]
+        assert len(cached_file_names) == 1
+        cached_docs = list(
+            DocBin().from_disk(tmpdir / cached_file_names[0]).get_docs(nlp.vocab)
+        )
+        assert len(cached_docs) == 3
+        assert all([doc.user_data["llm_io"]["llm"]] for doc in cached_docs)
```

### Comparing `spacy-llm-0.3.1/spacy_llm/tests/test_combinations.py` & `spacy-llm-0.3.2/spacy_llm/tests/test_combinations.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/ty.py` & `spacy-llm-0.3.2/spacy_llm/ty.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm/util.py` & `spacy-llm-0.3.2/spacy_llm/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/spacy_llm.egg-info/PKG-INFO` & `spacy-llm-0.3.2/spacy_llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.3.1
+Version: 0.3.2
 Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
 Classifier: Development Status :: 4 - Beta
@@ -1022,31 +1022,35 @@
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
 
 ### Cache
 
 Interacting with LLMs, either through an external API or a local instance, is costly.
 Since developing an NLP pipeline generally means a lot of exploration and prototyping,
-`spacy-llm` implements a built-in cache to avoid reprocessing the same documents at each run.
+`spacy-llm` implements a built-in cache to avoid reprocessing the same documents at each run
+that keeps batches of documents stored on disk.
 
 Example config block:
 
 ```ini
 [components.llm.cache]
-@llm_misc = "spacy.BatchCache.v1",
+@llm_misc = "spacy.BatchCache.v1"
 path = "path/to/cache"
 batch_size = 64
 max_batches_in_mem = 4
 ```
 
-| Argument             | Type                         | Default | Description                                          |
-| -------------------- | ---------------------------- | ------- | ---------------------------------------------------- |
-| `path`               | `Optional[Union[str, Path]]` | `None`  | Cache directory. If `None`, no caching is performed. |
-| `batch_size`         | `int`                        | 64      | Number of docs in one batch (file).                  |
-| `max_batches_in_mem` | `int`                        | 4       | Max. number of batches to hold in memory.            |
+| Argument             | Type                         | Default | Description                                                                                                               |
+| -------------------- | ---------------------------- | ------- | ------------------------------------------------------------------------------------------------------------------------- |
+| `path`               | `Optional[Union[str, Path]]` | `None`  | Cache directory. If `None`, no caching is performed, and this component will act as a NoOp.                               |
+| `batch_size`         | `int`                        | 64      | Number of docs in one batch (file). Once a batch is full, it will be peristed to disk.                                    |
+| `max_batches_in_mem` | `int`                        | 4       | Max. number of batches to hold in memory. Allows you to limit the effect on your memory if you're handling a lot of docs. |
+
+When retrieving a document, the `BatchCache` will first figure out what batch the document belongs to. If the batch
+isn't in memory it will try to load the batch from disk and then move it into memory. 
 
 Note that since the cache is generated by a registered function, you can also provide your own registered function
 returning your own cache implementation. If you wish to do so, ensure that your cache object adheres to the
 `Protocol` defined in `spacy_llm.ty.Cache`.
 
 ### Various functions
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.3.1 Summary: Integrating LLMs
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.3.2 Summary: Integrating LLMs
 into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
 github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
@@ -633,23 +633,29 @@
 open_llama_7b_700bt_preview"` Note that Hugging Face will download this model
 the first time you use it - you can [define the cached directory](https://
 huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting the
 environmental variable `HF_HOME`. ### Cache Interacting with LLMs, either
 through an external API or a local instance, is costly. Since developing an NLP
 pipeline generally means a lot of exploration and prototyping, `spacy-llm`
 implements a built-in cache to avoid reprocessing the same documents at each
-run. Example config block: ```ini [components.llm.cache] @llm_misc =
-"spacy.BatchCache.v1", path = "path/to/cache" batch_size = 64
-max_batches_in_mem = 4 ``` | Argument | Type | Default | Description | | ------
--------------- | ---------------------------- | ------- | ---------------------
-------------------------------- | | `path` | `Optional[Union[str, Path]]` |
-`None` | Cache directory. If `None`, no caching is performed. | | `batch_size`
-| `int` | 64 | Number of docs in one batch (file). | | `max_batches_in_mem` |
-`int` | 4 | Max. number of batches to hold in memory. | Note that since the
-cache is generated by a registered function, you can also provide your own
+run that keeps batches of documents stored on disk. Example config block:
+```ini [components.llm.cache] @llm_misc = "spacy.BatchCache.v1" path = "path/
+to/cache" batch_size = 64 max_batches_in_mem = 4 ``` | Argument | Type |
+Default | Description | | -------------------- | ---------------------------- |
+------- | ---------------------------------------------------------------------
+---------------------------------------------------- | | `path` | `Optional
+[Union[str, Path]]` | `None` | Cache directory. If `None`, no caching is
+performed, and this component will act as a NoOp. | | `batch_size` | `int` | 64
+| Number of docs in one batch (file). Once a batch is full, it will be peristed
+to disk. | | `max_batches_in_mem` | `int` | 4 | Max. number of batches to hold
+in memory. Allows you to limit the effect on your memory if you're handling a
+lot of docs. | When retrieving a document, the `BatchCache` will first figure
+out what batch the document belongs to. If the batch isn't in memory it will
+try to load the batch from disk and then move it into memory. Note that since
+the cache is generated by a registered function, you can also provide your own
 registered function returning your own cache implementation. If you wish to do
 so, ensure that your cache object adheres to the `Protocol` defined in
 `spacy_llm.ty.Cache`. ### Various functions #### spacy.FewShotReader.v1 This
 function is registered in spaCy's `misc` registry, and reads in examples from a
 `.yml`, `.yaml`, `.json` or `.jsonl` file. It uses [`srsly`](https://
 github.com/explosion/srsly) to read in these files and parses them depending on
 the file extension. ```ini [components.llm.task.examples] @misc =
```

### Comparing `spacy-llm-0.3.1/spacy_llm.egg-info/SOURCES.txt` & `spacy-llm-0.3.2/spacy_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/usage_examples/multitask_openai/run_pipeline.py` & `spacy-llm-0.3.2/usage_examples/multitask_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/usage_examples/ner_dolly/run_pipeline.py` & `spacy-llm-0.3.2/usage_examples/ner_dolly/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/usage_examples/ner_langchain_openai/run_pipeline.py` & `spacy-llm-0.3.2/usage_examples/ner_langchain_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/usage_examples/ner_minichain_openai/run_pipeline.py` & `spacy-llm-0.3.2/usage_examples/ner_minichain_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/usage_examples/rel_openai/run_pipeline.py` & `spacy-llm-0.3.2/usage_examples/rel_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/usage_examples/tests/test_readme_examples.py` & `spacy-llm-0.3.2/usage_examples/tests/test_readme_examples.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/usage_examples/tests/test_usage_examples.py` & `spacy-llm-0.3.2/usage_examples/tests/test_usage_examples.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.3.1/usage_examples/textcat_openai/run_pipeline.py` & `spacy-llm-0.3.2/usage_examples/textcat_openai/run_pipeline.py`

 * *Files identical despite different names*

