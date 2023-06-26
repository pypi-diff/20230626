# Comparing `tmp/configuraptor-1.8.0.tar.gz` & `tmp/configuraptor-1.9.2.tar.gz`

## Comparing `configuraptor-1.8.0.tar` & `configuraptor-1.9.2.tar`

### file list

```diff
@@ -1,93 +1,94 @@
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 configuraptor-1.8.0/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.8.0/coverage.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.8.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.8.0/_static/configuraptor_circle.png
--rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.8.0/_static/configuraptor_original.jpeg
--rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.8.0/_static/configuraptor_round.png
--rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.8.0/_static/configuraptor_transparent.png
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/ages.toml
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/dataclass.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/dumping.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/dumping.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/example_from_readme.json
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/example_from_readme.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/example_from_readme.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/example_from_readme.yaml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/existing_instance.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/main.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/postponed.py
--rw-r--r--   0        0        0     9464 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/readme.md
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/singleton.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/typedconfig_class.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870___init___py.html
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e___about___py.html
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e___init___py.html
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_cls_py.html
--rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_core_py.html
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_errors_py.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_helpers_py.html
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_main_py.html
--rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_singleton_py.html
--rw-r--r--   0        0        0    12019 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97___init___py.html
--rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97__types_py.html
--rw-r--r--   0        0        0     9120 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
--rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
--rw-r--r--   0        0        0    12225 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html
--rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html
--rw-r--r--   0        0        0    26392 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
--rw-r--r--   0        0        0   131736 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html
--rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_dump_py.html
--rw-r--r--   0        0        0    30314 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html
--rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/empty.toml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/example.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/example.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/example.yaml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/some.toml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/with_dict_of_custom.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/with_multiple_toplevel_keys.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/__about__.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/__init__.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/cls.py
--rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/core.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/dump.py
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/errors.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/helpers.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/postpone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/py.typed
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/singleton.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/loaders/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/loaders/_types.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/loaders/loaders_shared.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/loaders/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/constants.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_about.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_core.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_dumps.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_json_yaml.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_mypy.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_postponed.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_singleton.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_toml_basic.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_toml_dataclass.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_toml_existing.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_toml_typedconfig_class.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.8.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.8.0/LICENSE.txt
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 configuraptor-1.8.0/README.md
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 configuraptor-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 configuraptor-1.9.2/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.9.2/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.9.2/.github/workflows/su6.yml
+-rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.9.2/_static/configuraptor_circle.png
+-rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.9.2/_static/configuraptor_original.jpeg
+-rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.9.2/_static/configuraptor_round.png
+-rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.9.2/_static/configuraptor_transparent.png
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/ages.toml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/dataclass.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/dumping.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/dumping.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/example_from_readme.json
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/example_from_readme.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/example_from_readme.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/example_from_readme.yaml
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/example_mapping.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/existing_instance.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/main.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/postponed.py
+-rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/readme.md
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/singleton.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.9.2/examples/typedconfig_class.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_31a2a1dc9b603870___init___py.html
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e___about___py.html
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e___init___py.html
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_cls_py.html
+-rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_core_py.html
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_errors_py.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_helpers_py.html
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_main_py.html
+-rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_singleton_py.html
+-rw-r--r--   0        0        0    12019 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97___init___py.html
+-rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97__types_py.html
+-rw-r--r--   0        0        0     9120 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
+-rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
+-rw-r--r--   0        0        0    12225 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40___about___py.html
+-rw-r--r--   0        0        0    13937 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40___init___py.html
+-rw-r--r--   0        0        0    48825 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
+-rw-r--r--   0        0        0   137212 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_core_py.html
+-rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_dump_py.html
+-rw-r--r--   0        0        0    34632 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html
+-rw-r--r--   0        0        0    15776 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.9.2/htmlcov/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pytest_examples/empty.toml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pytest_examples/example.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pytest_examples/example.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pytest_examples/example.yaml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pytest_examples/some.toml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pytest_examples/with_dict_of_custom.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pytest_examples/with_multiple_toplevel_keys.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/__about__.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/__init__.py
+-rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/cls.py
+-rw-r--r--   0        0        0    16210 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/core.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/dump.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/errors.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/helpers.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/postpone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/py.typed
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/singleton.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/loaders/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/loaders/_types.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/loaders/loaders_shared.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.9.2/src/configuraptor/loaders/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/constants.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_about.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_core.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_dumps.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_json_yaml.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_mypy.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_postponed.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_singleton.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_toml_basic.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_toml_dataclass.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_toml_existing.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 configuraptor-1.9.2/tests/test_toml_typedconfig_class.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.9.2/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.9.2/LICENSE.txt
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 configuraptor-1.9.2/README.md
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 configuraptor-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 configuraptor-1.9.2/PKG-INFO
```

### Comparing `configuraptor-1.8.0/CHANGELOG.md` & `configuraptor-1.9.2/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.9.2 (2023-06-22)
+### Fix
+* Internal values (_) should be updatable without TypedConfig._update logic ([`ef24673`](https://github.com/trialandsuccess/configuraptor/commit/ef24673f4304fa58d2b51a429efe7dc62ddc84f9))
+
+## v1.9.1 (2023-06-22)
+### Fix
+* Key="" workaround no longer required ([`2c5fcaf`](https://github.com/trialandsuccess/configuraptor/commit/2c5fcaf8471176b82ebf5438d677e8db657018ab))
+* **mapping:** Made mapping immutable, so MutableMapping actually has different behavior ([`a68ef56`](https://github.com/trialandsuccess/configuraptor/commit/a68ef5651a457cc08f0125f01f00b98ceb49c544))
+
+### Documentation
+* **mapping:** Add example for TypedMapping ([`e430f40`](https://github.com/trialandsuccess/configuraptor/commit/e430f4065b5060fb2d2a4a8c134e8c42e9f66b74))
+
+## v1.9.0 (2023-06-22)
+### Feature
+* **mapping:** Add configuraptor.TypedMapping and .TypedMutableMapping to support **unpacking (but not on default TypedConfig) ([`b4c6b9d`](https://github.com/trialandsuccess/configuraptor/commit/b4c6b9dc01cfd6727187310610e750fa6ada3234))
+
 ## v1.8.0 (2023-06-21)
 ### Feature
 * **format:** Allow TypedConfig._format ([`0b46646`](https://github.com/trialandsuccess/configuraptor/commit/0b46646fec153a6bcdfea0c40b872da884aa9146))
 
 ## v1.7.2 (2023-06-20)
 ### Fix
 * **toml:** Tomlkit had own types, move to tomli ([`0b5f0a4`](https://github.com/trialandsuccess/configuraptor/commit/0b5f0a4333f5767fc2329cebb040c6cf4c78eff9))
```

### Comparing `configuraptor-1.8.0/coverage.svg` & `configuraptor-1.9.2/coverage.svg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/_static/configuraptor_circle.png` & `configuraptor-1.9.2/_static/configuraptor_circle.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/_static/configuraptor_original.jpeg` & `configuraptor-1.9.2/_static/configuraptor_original.jpeg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/_static/configuraptor_round.png` & `configuraptor-1.9.2/_static/configuraptor_round.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/_static/configuraptor_transparent.png` & `configuraptor-1.9.2/_static/configuraptor_transparent.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/examples/dataclass.py` & `configuraptor-1.9.2/examples/dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/examples/dumping.py` & `configuraptor-1.9.2/examples/dumping.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/examples/example_from_readme.py` & `configuraptor-1.9.2/examples/example_from_readme.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/examples/main.py` & `configuraptor-1.9.2/examples/main.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/examples/postponed.py` & `configuraptor-1.9.2/examples/postponed.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/examples/readme.md` & `configuraptor-1.9.2/examples/readme.md`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 (e.g. `key="tool.some-tool"`). If no key is passed, it will be guessed based on some criteria:
 
 - if there is only one top-level key, it will be used automatically (this happens in the case of `OtherConfig` in
   the `README` example);
 - otherwise, the name of the class is used to guess the key name (this happens in the case of `Config` in
   the `README` example).
 
-If you pass `key=""` (empty string), all data will be loaded from the top-level.
+If you pass `key=""` (empty string), all data will be loaded from the top-level. 
+This will be done automatically too if something goes wrong with the supplied key.
 Example:
 
 ```json
 // somedata.json
 {
   "string": "here",
   "number": 123
@@ -370,8 +371,33 @@
       },
       "second": {
         "name": "dependency 3.2"
       }
     }
   }
 }
-```
+```
+
+## Mappings
+
+To make a class unpackable with `**`, you need to inherit `TypedMapping` or `TypedMutableMapping`.
+Doing this will break compatibility with `Singleton`, so this unpacking feature is not enabled on the
+default `TypedConfig`.
+`TypedMapping` also makes updating the data illegal, whereas this is allowed in `TypedConfig` and `TypedMutableMapping`.
+
+```python
+# example_mapping.py
+import configuraptor
+
+
+class MyConfig(configuraptor.TypedMapping):
+    key: str
+
+
+my_config = MyConfig.load({"key": "something"})
+
+# not allowed, because it's not a Mutable Mapping:
+my_config.update(key="something else")
+
+# this would crash if MyConfig was a TypedConfig:
+"key is {key}".format(**my_config)  # == "key is something"
+```
```

### Comparing `configuraptor-1.8.0/examples/singleton.py` & `configuraptor-1.9.2/examples/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/examples/typedconfig_class.py` & `configuraptor-1.9.2/examples/typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/coverage_html.js` & `configuraptor-1.9.2/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870___init___py.html` & `configuraptor-1.9.2/htmlcov/d_31a2a1dc9b603870___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html` & `configuraptor-1.9.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html` & `configuraptor-1.9.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e___about___py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e___init___py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_cls_py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_core_py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_errors_py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_helpers_py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_main_py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_main_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_singleton_py.html` & `configuraptor-1.9.2/htmlcov/d_47560703719c1d9e_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97___init___py.html` & `configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97__types_py.html` & `configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97__types_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html` & `configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html` & `configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html` & `configuraptor-1.9.2/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40___about___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-20 10:44 +0200
+            created at 2023-06-22 13:49 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,23 +83,23 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">This file contains the module version.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.7.2"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.9.0"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-20 10:44 +0200
+            created at 2023-06-22 13:49 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,22 +7,22 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 1 statements   1 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-20 10:44 +0200
+at 2023-06-22 13:49 +0200
 
 
 1""" 
 2This file contains the module version. 
 3""" 
 4 
 5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 6# 
 7# SPDX-License-Identifier: MIT 
-8__version__ = "1.7.2" 
+8__version__ = "1.9.0" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-20 10:44 +0200
+at 2023-06-22 13:49 +0200
```

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-20 10:44 +0200
+            created at 2023-06-22 13:07 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,15 +83,15 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Exposes TypedConfig and load_into for this library.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">cls</span> <span class="key">import</span> <span class="nam">TypedConfig</span><span class="op">,</span> <span class="nam">update</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">cls</span> <span class="key">import</span> <span class="nam">TypedConfig</span><span class="op">,</span> <span class="nam">TypedMapping</span><span class="op">,</span> <span class="nam">TypedMutableMapping</span><span class="op">,</span> <span class="nam">update</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="nam">all_annotations</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="nam">check_and_convert_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="nam">convert_config</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="nam">ensure_types</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="nam">load_into</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="nam">load_into_class</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
@@ -100,42 +100,44 @@
     <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">dump</span> <span class="key">import</span> <span class="nam">asdict</span><span class="op">,</span> <span class="nam">asjson</span><span class="op">,</span> <span class="nam">astoml</span><span class="op">,</span> <span class="nam">asyaml</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">postpone</span> <span class="key">import</span> <span class="nam">postpone</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">singleton</span> <span class="key">import</span> <span class="nam">Singleton</span><span class="op">,</span> <span class="nam">SingletonMeta</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="nam">__all__</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="com"># cls</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="str">"TypedConfig"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="str">"update"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="com"># singleton</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="str">"Singleton"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="str">"SingletonMeta"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="com"># core</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="str">"all_annotations"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"check_and_convert_data"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="str">"convert_config"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="str">"ensure_types"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="str">"load_into"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="str">"load_into_class"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="str">"load_into_instance"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="com"># postpone</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="str">"postpone"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="com"># dump</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="str">"asdict"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="str">"astoml"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="str">"asyaml"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="str">"asjson"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t"><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="str">"TypedMapping"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"TypedMutableMapping"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="str">"update"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="com"># singleton</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="str">"Singleton"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="str">"SingletonMeta"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="com"># core</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="str">"all_annotations"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="str">"check_and_convert_data"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="str">"convert_config"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="str">"ensure_types"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="str">"load_into"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="str">"load_into_class"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="str">"load_into_instance"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="com"># postpone</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="str">"postpone"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="com"># dump</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="str">"asdict"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="str">"astoml"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="str">"asyaml"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="str">"asjson"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-20 10:44 +0200
+            created at 2023-06-22 13:07 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,26 +7,26 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 6 statements   6 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-20 10:44 +0200
+at 2023-06-22 13:07 +0200
 
 
 1""" 
 2Exposes TypedConfig and load_into for this library. 
 3""" 
 4 
 5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 6# 
 7# SPDX-License-Identifier: MIT 
-8from .cls import TypedConfig, update 
+8from .cls import TypedConfig, TypedMapping, TypedMutableMapping, update 
 9from .core import ( 
 10 all_annotations, 
 11 check_and_convert_data, 
 12 convert_config, 
 13 ensure_types, 
 14 load_into, 
 15 load_into_class, 
@@ -35,30 +35,32 @@
 18from .dump import asdict, asjson, astoml, asyaml 
 19from .postpone import postpone 
 20from .singleton import Singleton, SingletonMeta 
 21 
 22__all__ = [ 
 23 # cls 
 24 "TypedConfig", 
-25 "update", 
-26 # singleton 
-27 "Singleton", 
-28 "SingletonMeta", 
-29 # core 
-30 "all_annotations", 
-31 "check_and_convert_data", 
-32 "convert_config", 
-33 "ensure_types", 
-34 "load_into", 
-35 "load_into_class", 
-36 "load_into_instance", 
-37 # postpone 
-38 "postpone", 
-39 # dump 
-40 "asdict", 
-41 "astoml", 
-42 "asyaml", 
-43 "asjson", 
-44] 
+25 "TypedMapping", 
+26 "TypedMutableMapping", 
+27 "update", 
+28 # singleton 
+29 "Singleton", 
+30 "SingletonMeta", 
+31 # core 
+32 "all_annotations", 
+33 "check_and_convert_data", 
+34 "convert_config", 
+35 "ensure_types", 
+36 "load_into", 
+37 "load_into_class", 
+38 "load_into_instance", 
+39 # postpone 
+40 "postpone", 
+41 # dump 
+42 "asdict", 
+43 "astoml", 
+44 "asyaml", 
+45 "asjson", 
+46] 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-20 10:44 +0200
+at 2023-06-22 13:07 +0200
```

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_dump_py.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/cls.py: 100%</title>
+    <title>Coverage for src/configuraptor/dump.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/configuraptor/cls.py</b>:
+            <span class="text">Coverage for </span><b>src/configuraptor/dump.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">24 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">24<span class="text"> run</span></button>
+            <span class="text">31 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">31<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-21 15:50 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,100 +77,84 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Logic for the TypedConfig inheritable class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Method to dump classes to other formats.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">all_annotations</span><span class="op">,</span> <span class="nam">check_type</span><span class="op">,</span> <span class="nam">load_into</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">errors</span> <span class="key">import</span> <span class="nam">ConfigErrorExtraKey</span><span class="op">,</span> <span class="nam">ConfigErrorInvalidType</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="nam">C</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"C"</span><span class="op">,</span> <span class="nam">bound</span><span class="op">=</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedConfig</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">    Can be used instead of load_into.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="key">def</span> <span class="nam">load</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">        Load a class' config values from the config file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">        SomeClass.load(data, ...) = load_into(SomeClass, data, ...).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">return</span> <span class="nam">load_into</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="key">def</span> <span class="nam">_update</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">_strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">        Can be used if .update is overwritten with another value in the config.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">__class__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">values</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">            <span class="key">if</span> <span class="nam">value</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">_allow_none</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">                <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">json</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">tomli_w</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">yaml</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="nam">instance_of_custom_class</span><span class="op">,</span> <span class="nam">is_custom_class</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">camel_to_snake</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">def</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">_level</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">0</span><span class="op">,</span> <span class="op">/</span><span class="op">,</span> <span class="nam">with_top_level_key</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    Dump a config instance to a dictionary (recursively).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="nam">cls</span> <span class="op">=</span> <span class="nam">value</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">asdict</span><span class="op">(</span><span class="nam">_</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span> <span class="key">if</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">_</span><span class="op">)</span> <span class="key">else</span> <span class="nam">_</span> <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">dict</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">v</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span> <span class="key">if</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">v</span><span class="op">)</span> <span class="key">else</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">data</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="key">if</span> <span class="nam">_level</span> <span class="op">==</span> <span class="num">0</span> <span class="key">and</span> <span class="nam">with_top_level_key</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="com"># top-level: add an extra key indicating the class' name</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">cls_name</span> <span class="op">=</span> <span class="nam">camel_to_snake</span><span class="op">(</span><span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">return</span> <span class="op">{</span><span class="nam">cls_name</span><span class="op">:</span> <span class="nam">data</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">            <span class="key">if</span> <span class="nam">_strict</span> <span class="key">and</span> <span class="nam">key</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ConfigErrorExtraKey</span><span class="op">(</span><span class="nam">cls</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">__class__</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="key">if</span> <span class="nam">_strict</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span><span class="op">)</span> <span class="key">and</span> <span class="key">not</span> <span class="op">(</span><span class="nam">value</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="nam">_allow_none</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">(</span><span class="nam">expected_type</span><span class="op">=</span><span class="nam">annotations</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">            <span class="nam">setattr</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="key">def</span> <span class="nam">astoml</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">multiline_strings</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">    Dump a config instance to toml (recursively).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">return</span> <span class="nam">tomli_w</span><span class="op">.</span><span class="nam">dumps</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">multiline_strings</span><span class="op">=</span><span class="nam">multiline_strings</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="key">def</span> <span class="nam">update</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">_strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t"><span class="str">        Update values on this config.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="str">            _strict: allow wrong types?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t"><span class="str">            _allow_none: allow None or skip those entries?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t"><span class="str">            **values: key: value pairs in the right types to update.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_update</span><span class="op">(</span><span class="nam">_strict</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="key">def</span> <span class="nam">_format</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">string</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="str">        Format the config data into a string template.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="str">        Replacement for string.format(**config), which is only possible for MutableMappings.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="str">        MutableMapping does not work well with our Singleton Metaclass.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="key">return</span> <span class="nam">string</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="op">**</span><span class="nam">self</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="com"># also expose as separate function:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t"><span class="key">def</span> <span class="nam">update</span><span class="op">(</span><span class="nam">instance</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">_strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t"><span class="str">    Update values on a config.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t"><span class="str">        instance: config instance to update</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="str">        _strict: allow wrong types?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="str">        _allow_none: allow None or skip those entries?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t"><span class="str">        **values: key: value pairs in the right types to update.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedConfig</span><span class="op">.</span><span class="nam">_update</span><span class="op">(</span><span class="nam">instance</span><span class="op">,</span> <span class="nam">_strict</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="key">def</span> <span class="nam">asjson</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="str">    Dump a config instance to json (recursively).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="key">return</span> <span class="nam">json</span><span class="op">.</span><span class="nam">dumps</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="key">def</span> <span class="nam">asyaml</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">    Dump a config instance to yaml (recursively).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="nam">output</span> <span class="op">=</span> <span class="nam">yaml</span><span class="op">.</span><span class="nam">dump</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="com"># output is already a str but mypy doesn't know that</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="nam">output</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-21 15:50 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,105 +1,85 @@
 
-****** Coverage for src/configuraptor/cls.py: 100% ******
+****** Coverage for src/configuraptor/dump.py: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 24 statements   24 run 0 missing 0 excluded *****
+***** 31 statements   31 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-21 15:50 +0200
+at 2023-06-20 10:44 +0200
 
 
 1""" 
-2Logic for the TypedConfig inheritable class. 
+2Method to dump classes to other formats. 
 3""" 
 4 
-5import typing 
-6 
-7from .core import T_data, all_annotations, check_type, load_into 
-8from .errors import ConfigErrorExtraKey, ConfigErrorInvalidType 
-9 
-10C = typing.TypeVar("C", bound=typing.Any) 
-11 
-12 
-13class TypedConfig: 
-14 """ 
-15 Can be used instead of load_into. 
+5import json 
+6import typing 
+7 
+8import tomli_w 
+9import yaml 
+10 
+11from .core import instance_of_custom_class, is_custom_class 
+12from .helpers import camel_to_snake 
+13 
+14 
+15def asdict(inst: typing.Any, _level: int = 0, /, with_top_level_key: bool =
+True) -> dict[str, typing.Any]: 
 16 """ 
-17 
-18 @classmethod 
-19 def load( 
-20 cls: typing.Type[C], data: T_data, key: str = None, init: dict[str,
-typing.Any] = None, strict: bool = True 
-21 ) -> C: 
-22 """ 
-23 Load a class' config values from the config file. 
-24 
-25 SomeClass.load(data, ...) = load_into(SomeClass, data, ...). 
-26 """ 
-27 return load_into(cls, data, key=key, init=init, strict=strict) 
-28 
-29 def _update(self, _strict: bool = True, _allow_none: bool = False, **values:
-typing.Any) -> None: 
-30 """ 
-31 Can be used if .update is overwritten with another value in the config. 
-32 """ 
-33 annotations = all_annotations(self.__class__) 
-34 
-35 for key, value in values.items(): 
-36 if value is None and not _allow_none: 
-37 continue 
+17 Dump a config instance to a dictionary (recursively). 
+18 """ 
+19 data = {} 
+20 
+21 for key, value in inst.__dict__.items(): 
+22 cls = value.__class__ 
+23 if is_custom_class(cls): 
+24 value = asdict(value, _level + 1) 
+25 elif isinstance(value, list): 
+26 value = [asdict(_, _level + 1) if instance_of_custom_class(_) else _ for _
+in value] 
+27 elif isinstance(value, dict): 
+28 value = {k: asdict(v, _level + 1) if instance_of_custom_class(v) else v for
+k, v in value.items()} 
+29 
+30 data[key] = value 
+31 
+32 if _level == 0 and with_top_level_key: 
+33 # top-level: add an extra key indicating the class' name 
+34 cls_name = camel_to_snake(inst.__class__.__name__) 
+35 return {cls_name: data} 
+36 
+37 return data 
 38 
-39 if _strict and key not in annotations: 
-40 raise ConfigErrorExtraKey(cls=self.__class__, key=key, value=value) 
-41 
-42 if _strict and not check_type(value, annotations[key]) and not (value is
-None and _allow_none): 
-43 raise ConfigErrorInvalidType(expected_type=annotations[key], key=key,
-value=value) 
-44 
-45 setattr(self, key, value) 
+39 
+40def astoml(inst: typing.Any, multiline_strings: bool = False) -> str: 
+41 """ 
+42 Dump a config instance to toml (recursively). 
+43 """ 
+44 data = asdict(inst) 
+45 return tomli_w.dumps(data, multiline_strings=multiline_strings) 
 46 
-47 def update(self, _strict: bool = True, _allow_none: bool = False, **values:
-typing.Any) -> None: 
-48 """ 
-49 Update values on this config. 
-50 
-51 Args: 
-52 _strict: allow wrong types? 
-53 _allow_none: allow None or skip those entries? 
-54 **values: key: value pairs in the right types to update. 
-55 """ 
-56 return self._update(_strict, _allow_none, **values) 
-57 
-58 def _format(self, string: str) -> str: 
+47 
+48def asjson(inst: typing.Any, **kw: typing.Any) -> str: 
+49 """ 
+50 Dump a config instance to json (recursively). 
+51 """ 
+52 data = asdict(inst) 
+53 return json.dumps(data, **kw) 
+54 
+55 
+56def asyaml(inst: typing.Any, **kw: typing.Any) -> str: 
+57 """ 
+58 Dump a config instance to yaml (recursively). 
 59 """ 
-60 Format the config data into a string template. 
-61 
-62 Replacement for string.format(**config), which is only possible for
-MutableMappings. 
-63 MutableMapping does not work well with our Singleton Metaclass. 
-64 """ 
-65 return string.format(**self.__dict__) 
-66 
-67 
-68# also expose as separate function: 
-69def update(instance: typing.Any, _strict: bool = True, _allow_none: bool =
-False, **values: typing.Any) -> None: 
-70 """ 
-71 Update values on a config. 
-72 
-73 Args: 
-74 instance: config instance to update 
-75 _strict: allow wrong types? 
-76 _allow_none: allow None or skip those entries? 
-77 **values: key: value pairs in the right types to update. 
-78 """ 
-79 return TypedConfig._update(instance, _strict, _allow_none, **values) 
+60 data = asdict(inst) 
+61 output = yaml.dump(data, encoding=None, **kw) 
+62 # output is already a str but mypy doesn't know that 
+63 return typing.cast(str, output) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-21 15:50 +0200
+at 2023-06-20 10:44 +0200
```

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_core_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">156 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">156<span class="text"> run</span></button>
+            <span class="text">166 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">166<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
-            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">3<span class="text"> excluded</span></button>
+            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">5<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_dump_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-19 17:38 +0200
+            created at 2023-06-22 14:32 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -132,15 +132,15 @@
     <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">    If no key is manually defined for `load_into`, \</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="str">    the class' name is converted to snake_case to use as the default key.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">return</span> <span class="nam">camel_to_snake</span><span class="op">(</span><span class="nam">clsname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">classname</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="key">def</span> <span class="nam">__load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">classname</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    Tries to load the right data from a filename/path or dict, based on a manual key or a classname.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t"><span class="str">    E.g. class Tool will be mapped to key tool.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="str">    It also deals with nested keys (tool.extra -> {"tool": {"extra": ...}}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
@@ -157,430 +157,450 @@
     <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="com"># try to guess key by grabbing the first one or using the class name</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span> <span class="op">==</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">list</span><span class="op">(</span><span class="nam">data</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">        <span class="key">elif</span> <span class="nam">classname</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">_guess_key</span><span class="op">(</span><span class="nam">classname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="key">if</span> <span class="nam">key</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="key">return</span> <span class="nam">_data_for_nested_key</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="com"># no key found, just return all data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="nam">data</span> <span class="op">=</span> <span class="nam">_data_for_nested_key</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"No data found!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t"><span class="key">def</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">:</span> <span class="nam">T_typelike</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t"><span class="str">    Given a variable, check if it matches 'expected_type' (which can be a Union, parameterized generic etc.).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">dict</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Data is not a dict!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t"><span class="str">    Based on typeguard but this returns a boolean instead of returning the value or throwing a TypeCheckError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="nam">_check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="key">except</span> <span class="nam">TypeCheckError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t"><span class="key">def</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t"><span class="str">    Make sure all values in 'data' are in line with the ones stored in 'annotations'.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t"><span class="str">    If an annotated key in missing from data, it will be filled with None for convenience.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">classname</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t"><span class="str">    Wrapper around __load_data that retries with key="" if anything goes wrong.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="key">return</span> <span class="nam">__load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">classname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">    <span class="key">except</span> <span class="nam">Exception</span> <span class="key">as</span> <span class="nam">e</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="key">if</span> <span class="nam">key</span> <span class="op">!=</span> <span class="str">""</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">            <span class="key">return</span> <span class="nam">__load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="str">""</span><span class="op">,</span> <span class="nam">classname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">            <span class="com"># key already was "", just return data!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">            <span class="com"># (will probably not happen but fallback)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">            <span class="key">return</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="str">    TODO: python 3.11 exception groups to throw multiple errors at once!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">    <span class="com"># custom object to use instead of None, since typing.Optional can be None!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">    <span class="com"># cast to T to make mypy happy</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="nam">notfound</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">T</span><span class="op">,</span> <span class="nam">object</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">    <span class="nam">postponed</span> <span class="op">=</span> <span class="nam">Postponed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">    <span class="nam">final</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="nam">compare</span> <span class="op">=</span> <span class="nam">data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">notfound</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="key">if</span> <span class="nam">compare</span> <span class="key">is</span> <span class="nam">notfound</span><span class="op">:</span>  <span class="com"># pragma: nocover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">            <span class="nam">warnings</span><span class="op">.</span><span class="nam">warn</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">                <span class="str">"This should not happen since "</span> <span class="str">"`load_recursive` already fills `data` "</span> <span class="str">"based on `annotations`"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">            <span class="com"># skip!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="key">if</span> <span class="nam">compare</span> <span class="key">is</span> <span class="nam">postponed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">            <span class="com"># don't do anything with this item!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">=</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">        <span class="nam">final</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">compare</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">    <span class="key">return</span> <span class="nam">final</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t"><span class="key">def</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">items</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t"><span class="str">    Converts the config dict (from toml) or 'overwrites' dict in two ways.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t"><span class="str">    1. removes any items where the value is None, since in that case the default should be used;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t"><span class="str">    2. replaces '-' and '.' in keys with '_' so it can be mapped to the Config properties.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"-"</span><span class="op">,</span> <span class="str">"_"</span><span class="op">)</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"."</span><span class="op">,</span> <span class="str">"_"</span><span class="op">)</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">items</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">v</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t"><span class="nam">Type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t"><span class="nam">T_Type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T_Type"</span><span class="op">,</span> <span class="nam">bound</span><span class="op">=</span><span class="nam">Type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t"><span class="key">def</span> <span class="nam">is_builtin_type</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t"><span class="str">    Returns whether _type is one of the builtin types.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"__builtin__"</span><span class="op">,</span> <span class="str">"builtins"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t"><span class="key">def</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">:</span> <span class="nam">T_typelike</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t"><span class="str">    Given a variable, check if it matches 'expected_type' (which can be a Union, parameterized generic etc.).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t"><span class="str">    Based on typeguard but this returns a boolean instead of returning the value or throwing a TypeCheckError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="nam">_check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">    <span class="key">except</span> <span class="nam">TypeCheckError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t"><span class="key">def</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t"><span class="str">    Make sure all values in 'data' are in line with the ones stored in 'annotations'.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t"><span class="str">    If an annotated key in missing from data, it will be filled with None for convenience.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t"><span class="str">    TODO: python 3.11 exception groups to throw multiple errors at once!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">    <span class="com"># custom object to use instead of None, since typing.Optional can be None!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">    <span class="com"># cast to T to make mypy happy</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">    <span class="nam">notfound</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">T</span><span class="op">,</span> <span class="nam">object</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">    <span class="nam">postponed</span> <span class="op">=</span> <span class="nam">Postponed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="nam">final</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="nam">compare</span> <span class="op">=</span> <span class="nam">data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">notfound</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="key">if</span> <span class="nam">compare</span> <span class="key">is</span> <span class="nam">notfound</span><span class="op">:</span>  <span class="com"># pragma: nocover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">            <span class="nam">warnings</span><span class="op">.</span><span class="nam">warn</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">                <span class="str">"This should not happen since "</span> <span class="str">"`load_recursive` already fills `data` "</span> <span class="str">"based on `annotations`"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">            <span class="com"># skip!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="key">if</span> <span class="nam">compare</span> <span class="key">is</span> <span class="nam">postponed</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">            <span class="com"># don't do anything with this item!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">=</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">        <span class="nam">final</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">compare</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">    <span class="key">return</span> <span class="nam">final</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t"><span class="com"># def is_builtin_class_instance(obj: typing.Any) -> bool:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t"><span class="com">#     return is_builtin_type(obj.__class__)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t"><span class="key">def</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">items</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t"><span class="str">    Converts the config dict (from toml) or 'overwrites' dict in two ways.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t"><span class="key">def</span> <span class="nam">is_from_types_or_typing</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t"><span class="str">    Returns whether _type is one of the stlib typing/types types.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t"><span class="str">    1. removes any items where the value is None, since in that case the default should be used;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t"><span class="str">    2. replaces '-' and '.' in keys with '_' so it can be mapped to the Config properties.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"-"</span><span class="op">,</span> <span class="str">"_"</span><span class="op">)</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"."</span><span class="op">,</span> <span class="str">"_"</span><span class="op">)</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">items</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">v</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t"><span class="str">    e.g. types.UnionType or typing.Union</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"types"</span><span class="op">,</span> <span class="str">"typing"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t"><span class="nam">Type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t"><span class="nam">T_Type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T_Type"</span><span class="op">,</span> <span class="nam">bound</span><span class="op">=</span><span class="nam">Type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t"><span class="key">def</span> <span class="nam">is_from_other_toml_supported_module</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t"><span class="key">def</span> <span class="nam">is_builtin_type</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t"><span class="str">    Besides builtins, toml also supports 'datetime' and 'math' types, \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t"><span class="str">    so this returns whether _type is a type from these stdlib modules.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"datetime"</span><span class="op">,</span> <span class="str">"math"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t"><span class="str">    Returns whether _type is one of the builtin types.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"__builtin__"</span><span class="op">,</span> <span class="str">"builtins"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t"><span class="key">def</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t"><span class="str">    Returns whether _type is a parameterized type.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t"><span class="str">    Examples:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t"><span class="str">        list[str] -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t"><span class="str">        str -> False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t"><span class="com"># def is_builtin_class_instance(obj: typing.Any) -> bool:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t"><span class="com">#     return is_builtin_type(obj.__class__)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t"><span class="key">def</span> <span class="nam">is_from_types_or_typing</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t"><span class="str">    Returns whether _type is one of the stlib typing/types types.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t"><span class="str">    e.g. types.UnionType or typing.Union</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"types"</span><span class="op">,</span> <span class="str">"typing"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t"><span class="key">def</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t"><span class="str">    Tries to guess if _type is a builtin or a custom (user-defined) class.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t"><span class="str">    Other logic in this module depends on knowing that.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t"><span class="key">def</span> <span class="nam">is_from_other_toml_supported_module</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t"><span class="str">    Besides builtins, toml also supports 'datetime' and 'math' types, \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t"><span class="str">    so this returns whether _type is a type from these stdlib modules.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">    <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">        <span class="nam">type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">is</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_builtin_type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_from_other_toml_supported_module</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_from_types_or_typing</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">    <span class="key">return</span> <span class="nam">_type</span><span class="op">.</span><span class="nam">__module__</span> <span class="key">in</span> <span class="op">(</span><span class="str">"datetime"</span><span class="op">,</span> <span class="str">"math"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t"><span class="key">def</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t"><span class="str">    Returns whether _type is a parameterized type.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t"><span class="key">def</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">var</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t"><span class="str">    Calls `is_custom_class` on an instance of a (possibly custom) class.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">    <span class="key">return</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">var</span><span class="op">.</span><span class="nam">__class__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t"><span class="str">    Examples:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t"><span class="str">        list[str] -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t"><span class="str">        str -> False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t"><span class="key">def</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span> <span class="op">|</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t"><span class="str">    Tries to guess if _type could be optional.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t"><span class="str">    Examples:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t"><span class="str">        None -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t"><span class="str">        NoneType -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t"><span class="str">        typing.Union[str, None] -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t"><span class="str">        str | None -> True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="str">        list[str | None] -> False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t"><span class="str">        list[str] -> False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">    <span class="key">if</span> <span class="nam">_type</span> <span class="key">and</span> <span class="op">(</span><span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">in</span> <span class="op">(</span><span class="nam">dict</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">)</span> <span class="key">or</span> <span class="op">(</span><span class="nam">_type</span> <span class="key">is</span> <span class="nam">math</span><span class="op">.</span><span class="nam">nan</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">        <span class="com"># e.g. list[str]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">        <span class="com"># will crash issubclass to test it first here</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">        <span class="nam">_type</span> <span class="key">is</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">        <span class="key">or</span> <span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span> <span class="key">in</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>  <span class="com"># union with Nonetype</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span>  <span class="com"># no type  # Nonetype</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t"><span class="key">def</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t"><span class="str">    Tries to guess if _type is a builtin or a custom (user-defined) class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t"><span class="str">    Other logic in this module depends on knowing that.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">    <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">        <span class="nam">type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">is</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_builtin_type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_from_other_toml_supported_module</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">        <span class="key">and</span> <span class="key">not</span> <span class="nam">is_from_types_or_typing</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t"><span class="key">def</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">var</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t"><span class="str">    Calls `is_custom_class` on an instance of a (possibly custom) class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="key">return</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">var</span><span class="op">.</span><span class="nam">__class__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t"><span class="key">def</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">:</span> <span class="nam">Type</span> <span class="op">|</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t"><span class="str">    Tries to guess if _type could be optional.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t"><span class="key">def</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">dc</span><span class="op">.</span><span class="nam">Field</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="str">    Get Field info for a dataclass cls.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">    <span class="nam">fields</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__dataclass_fields__"</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">    <span class="key">return</span> <span class="nam">fields</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t"><span class="key">def</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t"><span class="str">    For all annotations (recursively gathered from parents with `all_annotations`), \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t"><span class="str">    try to resolve the tree of annotations.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t"><span class="str">    Uses `load_into_recurse`, not itself directly.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t"><span class="str">        class First:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t"><span class="str">            key: str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t"><span class="str">    Examples:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t"><span class="str">        None -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t"><span class="str">        NoneType -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="str">        typing.Union[str, None] -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t"><span class="str">        str | None -> True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t"><span class="str">        list[str | None] -> False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t"><span class="str">        list[str] -> False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">    <span class="key">if</span> <span class="nam">_type</span> <span class="key">and</span> <span class="op">(</span><span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span> <span class="key">in</span> <span class="op">(</span><span class="nam">dict</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">)</span> <span class="key">or</span> <span class="op">(</span><span class="nam">_type</span> <span class="key">is</span> <span class="nam">math</span><span class="op">.</span><span class="nam">nan</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">        <span class="com"># e.g. list[str]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">        <span class="com"># will crash issubclass to test it first here</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">    <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">        <span class="nam">_type</span> <span class="key">is</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">        <span class="key">or</span> <span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span> <span class="key">in</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>  <span class="com"># union with Nonetype</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">        <span class="key">or</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">NoneType</span><span class="op">,</span> <span class="nam">type</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span>  <span class="com"># no type  # Nonetype</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t"><span class="str">        class Second:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t"><span class="str">            other: First</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t"><span class="str">        # step 1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t"><span class="str">        cls = Second</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t"><span class="str">        data = {"second": {"other": {"key": "anything"}}}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t"><span class="key">def</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">dc</span><span class="op">.</span><span class="nam">Field</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t"><span class="str">    Get Field info for a dataclass cls.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">    <span class="nam">fields</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__dataclass_fields__"</span><span class="op">,</span> <span class="op">{</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">    <span class="key">return</span> <span class="nam">fields</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t"><span class="str">        # step 1.5</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t"><span class="str">        data = {"other": {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t"><span class="str">        # step 2</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t"><span class="str">        cls = First</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t"><span class="str">        data = {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t"><span class="str">        annotations: {"key": str}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t"><span class="str">    TODO: python 3.11 exception groups to throw multiple errors at once!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">    <span class="nam">updated</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">    <span class="key">for</span> <span class="nam">_key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">        <span class="key">if</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">            <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span> <span class="op">=</span> <span class="nam">data</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>  <span class="com"># value can change so define it as any instead of T</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">            <span class="key">if</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">                <span class="nam">origin</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">                <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">                <span class="key">if</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">list</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">                    <span class="nam">subtype</span> <span class="op">=</span> <span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">subtype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t"><span class="key">def</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t"><span class="str">    For all annotations (recursively gathered from parents with `all_annotations`), \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t"><span class="str">    try to resolve the tree of annotations.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t"><span class="str">    Uses `load_into_recurse`, not itself directly.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t"><span class="str">        class First:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t"><span class="str">            key: str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t"><span class="str">        class Second:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t"><span class="str">            other: First</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t"><span class="str">        # step 1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t"><span class="str">        cls = Second</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t"><span class="str">        data = {"second": {"other": {"key": "anything"}}}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t"><span class="str">        # step 1.5</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t"><span class="str">        data = {"other": {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t"><span class="str">        annotations: {"other": First}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">dict</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">                    <span class="com"># e.g. dict[str, Point]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">                    <span class="nam">subkeytype</span><span class="op">,</span> <span class="nam">subvaluetype</span> <span class="op">=</span> <span class="nam">arguments</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">                    <span class="com"># subkey(type) is not a custom class, so don't try to convert it:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">subkey</span><span class="op">:</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">subvaluetype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subkey</span><span class="op">,</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">                <span class="com"># elif origin is dict:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">                <span class="com"># keep data the same</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Union</span> <span class="key">and</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">                    <span class="key">for</span> <span class="nam">arg</span> <span class="key">in</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">                        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">                            <span class="nam">value</span> <span class="op">=</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">arg</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">                        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">                            <span class="com"># print(_type, arg, value)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">                            <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">                <span class="com"># todo: other parameterized/unions/typing.Optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">            <span class="key">elif</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">                <span class="com"># type must be C (custom class) at this point</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="nam">_load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">                    <span class="com"># make mypy and pycharm happy by telling it _type is of type C...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">                    <span class="com"># actually just passing _type as first arg!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">                    <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">Type_C</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">                    <span class="nam">value</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">        <span class="key">elif</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">            <span class="com"># property has default, use that instead.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">        <span class="key">elif</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">            <span class="com"># type is optional and not found in __dict__ -> default is None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">        <span class="key">elif</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span> <span class="key">and</span> <span class="op">(</span><span class="nam">field</span> <span class="op">:=</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_key</span><span class="op">)</span><span class="op">)</span> <span class="key">and</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span> <span class="key">is</span> <span class="key">not</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">MISSING</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">            <span class="com"># could have a default factory</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">            <span class="com"># todo: do something with field.default?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorMissingKey</span><span class="op">(</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">        <span class="nam">updated</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">    <span class="key">return</span> <span class="nam">updated</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t"><span class="key">def</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">ChainMap</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t"><span class="str">    Returns a dictionary-like ChainMap that includes annotations for all \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t"><span class="str">    attributes defined in cls or inherited from superclasses.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">    <span class="key">return</span> <span class="nam">ChainMap</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">c</span><span class="op">.</span><span class="nam">__annotations__</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__mro__"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">if</span> <span class="str">"__annotations__"</span> <span class="key">in</span> <span class="nam">c</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t"><span class="key">def</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t"><span class="str">    Wrapper around `_all_annotations` that filters away any keys in _except.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t"><span class="str">    It also flattens the ChainMap to a regular dict.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">    <span class="key">if</span> <span class="nam">_except</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">        <span class="nam">_except</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t"><span class="str">        # step 2</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t"><span class="str">        cls = First</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t"><span class="str">        data = {"key": "anything"}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t"><span class="str">        annotations: {"key": str}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t"><span class="str">    TODO: python 3.11 exception groups to throw multiple errors at once!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">    <span class="nam">updated</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">    <span class="key">for</span> <span class="nam">_key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">        <span class="key">if</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">            <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span> <span class="op">=</span> <span class="nam">data</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>  <span class="com"># value can change so define it as any instead of T</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">            <span class="key">if</span> <span class="nam">is_parameterized</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">                <span class="nam">origin</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">                <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">                <span class="key">if</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">list</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">                    <span class="nam">subtype</span> <span class="op">=</span> <span class="nam">arguments</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">subtype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">dict</span> <span class="key">and</span> <span class="nam">arguments</span> <span class="key">and</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arguments</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">                    <span class="com"># e.g. dict[str, Point]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">                    <span class="nam">subkeytype</span><span class="op">,</span> <span class="nam">subvaluetype</span> <span class="op">=</span> <span class="nam">arguments</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">                    <span class="com"># subkey(type) is not a custom class, so don't try to convert it:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">                    <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">subkey</span><span class="op">:</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">subvaluetype</span><span class="op">,</span> <span class="nam">subvalue</span><span class="op">)</span> <span class="key">for</span> <span class="nam">subkey</span><span class="op">,</span> <span class="nam">subvalue</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">                <span class="com"># elif origin is dict:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">                <span class="com"># keep data the same</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">                <span class="key">elif</span> <span class="nam">origin</span> <span class="key">is</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Union</span> <span class="key">and</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">                    <span class="key">for</span> <span class="nam">arg</span> <span class="key">in</span> <span class="nam">arguments</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">                        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">arg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">                            <span class="nam">value</span> <span class="op">=</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">arg</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">                        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">                            <span class="com"># print(_type, arg, value)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">                            <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">                <span class="com"># todo: other parameterized/unions/typing.Optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">            <span class="key">elif</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">                <span class="com"># type must be C (custom class) at this point</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="nam">_load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">                    <span class="com"># make mypy and pycharm happy by telling it _type is of type C...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">                    <span class="com"># actually just passing _type as first arg!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">                    <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">Type_C</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">                    <span class="nam">value</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">        <span class="key">elif</span> <span class="nam">_key</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">            <span class="com"># property has default, use that instead.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">        <span class="key">elif</span> <span class="nam">is_optional</span><span class="op">(</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">            <span class="com"># type is optional and not found in __dict__ -> default is None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">        <span class="key">elif</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span> <span class="key">and</span> <span class="op">(</span><span class="nam">field</span> <span class="op">:=</span> <span class="nam">dataclass_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_key</span><span class="op">)</span><span class="op">)</span> <span class="key">and</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span> <span class="key">is</span> <span class="key">not</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">MISSING</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">            <span class="com"># could have a default factory</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">            <span class="com"># todo: do something with field.default?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">field</span><span class="op">.</span><span class="nam">default_factory</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigErrorMissingKey</span><span class="op">(</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">        <span class="nam">updated</span><span class="op">[</span><span class="nam">_key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">    <span class="nam">_all</span> <span class="op">=</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">_all</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_except</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">    <span class="key">return</span> <span class="nam">updated</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t"><span class="key">def</span> <span class="nam">check_and_convert_data</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">    <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t"><span class="str">    Based on class annotations, this prepares the data for `load_into_recurse`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t"><span class="str">    1. convert config-keys to python compatible config_keys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t"><span class="str">    2. loads custom class type annotations with the same logic (see also `load_recursive`)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t"><span class="str">    3. ensures the annotated types match the actual types after loading the config file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t"><span class="key">def</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">ChainMap</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t"><span class="str">    Returns a dictionary-like ChainMap that includes annotations for all \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t"><span class="str">    attributes defined in cls or inherited from superclasses.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">    <span class="key">return</span> <span class="nam">ChainMap</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">c</span><span class="op">.</span><span class="nam">__annotations__</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__mro__"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">if</span> <span class="str">"__annotations__"</span> <span class="key">in</span> <span class="nam">c</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t"><span class="key">def</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">Type</span><span class="op">,</span> <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t"><span class="str">    Wrapper around `_all_annotations` that filters away any keys in _except.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t"><span class="str">    It also flattens the ChainMap to a regular dict.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">    <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">_except</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">    <span class="key">if</span> <span class="nam">strict</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">    <span class="key">if</span> <span class="nam">_except</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">        <span class="nam">_except</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">    <span class="nam">_all</span> <span class="op">=</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">_all</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_except</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">    <span class="key">return</span> <span class="nam">to_load</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t"><span class="str">    Loads an instance of `cls` filled with `data`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t"><span class="str">    Uses `load_recursive` to load any fillable annotated properties (see that method for an example).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t"><span class="str">    `init` can be used to optionally pass extra __init__ arguments. \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t"><span class="str">        NOTE: This will overwrite a config key with the same name!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">        <span class="nam">init</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">    <span class="com"># fixme: cls.__init__ can set other keys than the name is in kwargs!!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">    <span class="key">if</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">init</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">|=</span> <span class="nam">init</span>  <span class="com"># add extra init variables (should not happen for a dataclass but whatev)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">        <span class="com"># ensure mypy inst is an instance of the cls type (and not a fictuous `DataclassInstance`)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">C</span><span class="op">,</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t">        <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t"><span class="key">def</span> <span class="nam">check_and_convert_data</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">    <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t"><span class="str">    Based on class annotations, this prepares the data for `load_into_recurse`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t"><span class="str">    1. convert config-keys to python compatible config_keys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t"><span class="str">    2. loads custom class type annotations with the same logic (see also `load_recursive`)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t"><span class="str">    3. ensures the annotated types match the actual types after loading the config file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">    <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">_except</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">convert_config</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">load_recursive</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">    <span class="key">if</span> <span class="nam">strict</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">ensure_types</span><span class="op">(</span><span class="nam">to_load</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">    <span class="key">return</span> <span class="nam">to_load</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_into_recurse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t"><span class="str">    Loads an instance of `cls` filled with `data`.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t"><span class="str">    Similar to `load_into_recurse` but uses an existing instance of a class (so after __init__) \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t"><span class="str">    and thus does not support init.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Can not init an existing instance!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">    <span class="nam">existing_data</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t"><span class="str">    Uses `load_recursive` to load any fillable annotated properties (see that method for an example).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t"><span class="str">    `init` can be used to optionally pass extra __init__ arguments. \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t"><span class="str">        NOTE: This will overwrite a config key with the same name!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">        <span class="nam">init</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">    <span class="com"># fixme: cls.__init__ can set other keys than the name is in kwargs!!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">    <span class="key">if</span> <span class="nam">dc</span><span class="op">.</span><span class="nam">is_dataclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">init</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">|=</span> <span class="nam">init</span>  <span class="com"># add extra init variables (should not happen for a dataclass but whatev)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">        <span class="com"># ensure mypy inst is an instance of the cls type (and not a fictuous `DataclassInstance`)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">C</span><span class="op">,</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">        <span class="nam">inst</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">(</span><span class="op">**</span><span class="nam">init</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">        <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">        <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">existing_data</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">    <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_class</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_recurse.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t">    <span class="key">return</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t"><span class="key">def</span> <span class="nam">_load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t"><span class="str">    Similar to `load_into_recurse` but uses an existing instance of a class (so after __init__) \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t"><span class="str">    and thus does not support init.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t">    <span class="key">if</span> <span class="nam">init</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Can not init an existing instance!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t">    <span class="nam">existing_data</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">check_and_convert_data</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">_except</span><span class="op">=</span><span class="nam">existing_data</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_existing.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t">    <span class="nam">cls</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t">    <span class="key">return</span> <span class="nam">_load_into_instance</span><span class="op">(</span><span class="nam">inst</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t463" href="#t463">463</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t464" href="#t464">464</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t465" href="#t465">465</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t466" href="#t466">466</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t467" href="#t467">467</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t468" href="#t468">468</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t469" href="#t469">469</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t470" href="#t470">470</a></span><span class="t"><span class="str">    Load your config into a class (instance).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t471" href="#t471">471</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t472" href="#t472">472</a></span><span class="t"><span class="str">    Supports both a class or an instance as first argument, but that's hard to explain to mypy, so officially only</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t473" href="#t473">473</a></span><span class="t"><span class="str">    classes are supported, and if you want to `load_into` an instance, you should use `load_into_instance`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t474" href="#t474">474</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t475" href="#t475">475</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t476" href="#t476">476</a></span><span class="t"><span class="str">        cls: either a class or an existing instance of that class.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t477" href="#t477">477</a></span><span class="t"><span class="str">        data: can be a dictionary or a path to a file to load (as pathlib.Path or str)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t478" href="#t478">478</a></span><span class="t"><span class="str">        key: optional (nested) dictionary key to load data from (e.g. 'tool.su6.specific')</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t479" href="#t479">479</a></span><span class="t"><span class="str">        init: optional data to pass to your cls' __init__ method (only if cls is not an instance already)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t480" href="#t480">480</a></span><span class="t"><span class="str">        strict: enable type checks or allow anything?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t481" href="#t481">481</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t482" href="#t482">482</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t483" href="#t483">483</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t484" href="#t484">484</a></span><span class="t">        <span class="com"># would not be supported according to mypy, but you can still load_into(instance)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t485" href="#t485">485</a></span><span class="t">        <span class="key">return</span> <span class="nam">load_into_instance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t486" href="#t486">486</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t487" href="#t487">487</a></span><span class="t">    <span class="com"># make mypy and pycharm happy by telling it cls is of type C and not just 'type'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t488" href="#t488">488</a></span><span class="t">    <span class="com"># _cls = typing.cast(typing.Type[C], cls)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t489" href="#t489">489</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_class</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t">    <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="op">**</span><span class="nam">to_load</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t">    <span class="key">return</span> <span class="nam">inst</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_class</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_recurse.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t">    <span class="key">return</span> <span class="nam">_load_into_recurse</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t463" href="#t463">463</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t464" href="#t464">464</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t465" href="#t465">465</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into_instance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t466" href="#t466">466</a></span><span class="t">    <span class="nam">inst</span><span class="op">:</span> <span class="nam">C</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t467" href="#t467">467</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t468" href="#t468">468</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t469" href="#t469">469</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t470" href="#t470">470</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t471" href="#t471">471</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t472" href="#t472">472</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t473" href="#t473">473</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t474" href="#t474">474</a></span><span class="t"><span class="str">    Shortcut for _load_data + load_into_existing.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t475" href="#t475">475</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t476" href="#t476">476</a></span><span class="t">    <span class="nam">cls</span> <span class="op">=</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t477" href="#t477">477</a></span><span class="t">    <span class="nam">to_load</span> <span class="op">=</span> <span class="nam">_load_data</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t478" href="#t478">478</a></span><span class="t">    <span class="key">return</span> <span class="nam">_load_into_instance</span><span class="op">(</span><span class="nam">inst</span><span class="op">,</span> <span class="nam">cls</span><span class="op">,</span> <span class="nam">to_load</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t479" href="#t479">479</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t480" href="#t480">480</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t481" href="#t481">481</a></span><span class="t"><span class="key">def</span> <span class="nam">load_into</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t482" href="#t482">482</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t483" href="#t483">483</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t484" href="#t484">484</a></span><span class="t">    <span class="op">/</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t485" href="#t485">485</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t486" href="#t486">486</a></span><span class="t">    <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t487" href="#t487">487</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t488" href="#t488">488</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t489" href="#t489">489</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t490" href="#t490">490</a></span><span class="t"><span class="str">    Load your config into a class (instance).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t491" href="#t491">491</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t492" href="#t492">492</a></span><span class="t"><span class="str">    Supports both a class or an instance as first argument, but that's hard to explain to mypy, so officially only</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t493" href="#t493">493</a></span><span class="t"><span class="str">    classes are supported, and if you want to `load_into` an instance, you should use `load_into_instance`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t494" href="#t494">494</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t495" href="#t495">495</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t496" href="#t496">496</a></span><span class="t"><span class="str">        cls: either a class or an existing instance of that class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t497" href="#t497">497</a></span><span class="t"><span class="str">        data: can be a dictionary or a path to a file to load (as pathlib.Path or str)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t498" href="#t498">498</a></span><span class="t"><span class="str">        key: optional (nested) dictionary key to load data from (e.g. 'tool.su6.specific')</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t499" href="#t499">499</a></span><span class="t"><span class="str">        init: optional data to pass to your cls' __init__ method (only if cls is not an instance already)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t500" href="#t500">500</a></span><span class="t"><span class="str">        strict: enable type checks or allow anything?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t501" href="#t501">501</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t502" href="#t502">502</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t503" href="#t503">503</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t504" href="#t504">504</a></span><span class="t">        <span class="com"># would not be supported according to mypy, but you can still load_into(instance)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t505" href="#t505">505</a></span><span class="t">        <span class="key">return</span> <span class="nam">load_into_instance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t506" href="#t506">506</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t507" href="#t507">507</a></span><span class="t">    <span class="com"># make mypy and pycharm happy by telling it cls is of type C and not just 'type'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t508" href="#t508">508</a></span><span class="t">    <span class="com"># _cls = typing.cast(typing.Type[C], cls)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t509" href="#t509">509</a></span><span class="t">    <span class="key">return</span> <span class="nam">load_into_class</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_dump_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-19 17:38 +0200
+            created at 2023-06-22 14:32 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,17 +5,17 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 156 statements   156 run 0 missing 3 excluded *****
+***** 166 statements   166 run 0 missing 5 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-19 17:38 +0200
+at 2023-06-22 14:32 +0200
 
 
 1""" 
 2Contains most of the loading logic. 
 3""" 
 4 
 5import dataclasses as dc 
@@ -68,15 +68,15 @@
 50 """ 
 51 If no key is manually defined for `load_into`, \ 
 52 the class' name is converted to snake_case to use as the default key. 
 53 """ 
 54 return camel_to_snake(clsname) 
 55 
 56 
-57def _load_data(data: T_data, key: str = None, classname: str = None) -> dict
+57def __load_data(data: T_data, key: str = None, classname: str = None) -> dict
 [str, typing.Any]: 
 58 """ 
 59 Tries to load the right data from a filename/path or dict, based on a manual
 key or a classname. 
 60 
 61 E.g. class Tool will be mapped to key tool. 
 62 It also deals with nested keys (tool.extra -> {"tool": {"extra": ...}} 
@@ -95,452 +95,473 @@
 75 # try to guess key by grabbing the first one or using the class name 
 76 if len(data) == 1: 
 77 key = list(data.keys())[0] 
 78 elif classname is not None: 
 79 key = _guess_key(classname) 
 80 
 81 if key: 
-82 return _data_for_nested_key(key, data) 
-83 else: 
-84 # no key found, just return all data 
-85 return data 
+82 data = _data_for_nested_key(key, data) 
+83 
+84 if not data: 
+85 raise ValueError("No data found!") 
 86 
-87 
-88def check_type(value: typing.Any, expected_type: T_typelike) -> bool: 
-89 """ 
-90 Given a variable, check if it matches 'expected_type' (which can be a Union,
-parameterized generic etc.). 
+87 if not isinstance(data, dict): 
+88 raise ValueError("Data is not a dict!") 
+89 
+90 return data 
 91 
-92 Based on typeguard but this returns a boolean instead of returning the value
-or throwing a TypeCheckError 
-93 """ 
-94 try: 
-95 _check_type(value, expected_type) 
-96 return True 
-97 except TypeCheckError: 
-98 return False 
-99 
-100 
-101def ensure_types(data: dict[str, T], annotations: dict[str, type]) -> dict
+92 
+93def _load_data(data: T_data, key: str = None, classname: str = None) -> dict
+[str, typing.Any]: 
+94 """ 
+95 Wrapper around __load_data that retries with key="" if anything goes wrong. 
+96 """ 
+97 try: 
+98 return __load_data(data, key, classname) 
+99 except Exception as e: 
+100 if key != "": 
+101 return __load_data(data, "", classname) 
+102 else: # pragma: no cover 
+103 # key already was "", just return data! 
+104 # (will probably not happen but fallback) 
+105 return {} 
+106 
+107 
+108def check_type(value: typing.Any, expected_type: T_typelike) -> bool: 
+109 """ 
+110 Given a variable, check if it matches 'expected_type' (which can be a
+Union, parameterized generic etc.). 
+111 
+112 Based on typeguard but this returns a boolean instead of returning the
+value or throwing a TypeCheckError 
+113 """ 
+114 try: 
+115 _check_type(value, expected_type) 
+116 return True 
+117 except TypeCheckError: 
+118 return False 
+119 
+120 
+121def ensure_types(data: dict[str, T], annotations: dict[str, type]) -> dict
 [str, T | None]: 
-102 """ 
-103 Make sure all values in 'data' are in line with the ones stored in
+122 """ 
+123 Make sure all values in 'data' are in line with the ones stored in
 'annotations'. 
-104 
-105 If an annotated key in missing from data, it will be filled with None for
+124 
+125 If an annotated key in missing from data, it will be filled with None for
 convenience. 
-106 
-107 TODO: python 3.11 exception groups to throw multiple errors at once! 
-108 """ 
-109 # custom object to use instead of None, since typing.Optional can be None! 
-110 # cast to T to make mypy happy 
-111 notfound = typing.cast(T, object()) 
-112 postponed = Postponed() 
-113 
-114 final: dict[str, T | None] = {} 
-115 for key, _type in annotations.items(): 
-116 compare = data.get(key, notfound) 
-117 if compare is notfound: # pragma: nocover 
-118 warnings.warn( 
-119 "This should not happen since " "`load_recursive` already fills `data` "
+126 
+127 TODO: python 3.11 exception groups to throw multiple errors at once! 
+128 """ 
+129 # custom object to use instead of None, since typing.Optional can be None! 
+130 # cast to T to make mypy happy 
+131 notfound = typing.cast(T, object()) 
+132 postponed = Postponed() 
+133 
+134 final: dict[str, T | None] = {} 
+135 for key, _type in annotations.items(): 
+136 compare = data.get(key, notfound) 
+137 if compare is notfound: # pragma: nocover 
+138 warnings.warn( 
+139 "This should not happen since " "`load_recursive` already fills `data` "
 "based on `annotations`" 
-120 ) 
-121 # skip! 
-122 continue 
-123 
-124 if compare is postponed: 
-125 # don't do anything with this item! 
-126 continue 
-127 
-128 if not check_type(compare, _type): 
-129 raise ConfigErrorInvalidType(key, value=compare, expected_type=_type) 
-130 
-131 final[key] = compare 
-132 
-133 return final 
-134 
-135 
-136def convert_config(items: dict[str, T]) -> dict[str, T]: 
-137 """ 
-138 Converts the config dict (from toml) or 'overwrites' dict in two ways. 
-139 
-140 1. removes any items where the value is None, since in that case the
-default should be used; 
-141 2. replaces '-' and '.' in keys with '_' so it can be mapped to the Config
-properties. 
-142 """ 
-143 return {k.replace("-", "_").replace(".", "_"): v for k, v in items.items()
-if v is not None} 
-144 
-145 
-146Type = typing.Type[typing.Any] 
-147T_Type = typing.TypeVar("T_Type", bound=Type) 
-148 
-149 
-150def is_builtin_type(_type: Type) -> bool: 
-151 """ 
-152 Returns whether _type is one of the builtin types. 
-153 """ 
-154 return _type.__module__ in ("__builtin__", "builtins") 
+140 ) 
+141 # skip! 
+142 continue 
+143 
+144 if compare is postponed: 
+145 # don't do anything with this item! 
+146 continue 
+147 
+148 if not check_type(compare, _type): 
+149 raise ConfigErrorInvalidType(key, value=compare, expected_type=_type) 
+150 
+151 final[key] = compare 
+152 
+153 return final 
+154 
 155 
-156 
-157# def is_builtin_class_instance(obj: typing.Any) -> bool: 
-158# return is_builtin_type(obj.__class__) 
+156def convert_config(items: dict[str, T]) -> dict[str, T]: 
+157 """ 
+158 Converts the config dict (from toml) or 'overwrites' dict in two ways. 
 159 
-160 
-161def is_from_types_or_typing(_type: Type) -> bool: 
+160 1. removes any items where the value is None, since in that case the
+default should be used; 
+161 2. replaces '-' and '.' in keys with '_' so it can be mapped to the Config
+properties. 
 162 """ 
-163 Returns whether _type is one of the stlib typing/types types. 
+163 return {k.replace("-", "_").replace(".", "_"): v for k, v in items.items()
+if v is not None} 
 164 
-165 e.g. types.UnionType or typing.Union 
-166 """ 
-167 return _type.__module__ in ("types", "typing") 
+165 
+166Type = typing.Type[typing.Any] 
+167T_Type = typing.TypeVar("T_Type", bound=Type) 
 168 
 169 
-170def is_from_other_toml_supported_module(_type: Type) -> bool: 
+170def is_builtin_type(_type: Type) -> bool: 
 171 """ 
-172 Besides builtins, toml also supports 'datetime' and 'math' types, \ 
-173 so this returns whether _type is a type from these stdlib modules. 
-174 """ 
-175 return _type.__module__ in ("datetime", "math") 
+172 Returns whether _type is one of the builtin types. 
+173 """ 
+174 return _type.__module__ in ("__builtin__", "builtins") 
+175 
 176 
-177 
-178def is_parameterized(_type: Type) -> bool: 
-179 """ 
-180 Returns whether _type is a parameterized type. 
-181 
-182 Examples: 
-183 list[str] -> True 
-184 str -> False 
-185 """ 
-186 return typing.get_origin(_type) is not None 
-187 
+177# def is_builtin_class_instance(obj: typing.Any) -> bool: 
+178# return is_builtin_type(obj.__class__) 
+179 
+180 
+181def is_from_types_or_typing(_type: Type) -> bool: 
+182 """ 
+183 Returns whether _type is one of the stlib typing/types types. 
+184 
+185 e.g. types.UnionType or typing.Union 
+186 """ 
+187 return _type.__module__ in ("types", "typing") 
 188 
-189def is_custom_class(_type: Type) -> bool: 
-190 """ 
-191 Tries to guess if _type is a builtin or a custom (user-defined) class. 
-192 
-193 Other logic in this module depends on knowing that. 
+189 
+190def is_from_other_toml_supported_module(_type: Type) -> bool: 
+191 """ 
+192 Besides builtins, toml also supports 'datetime' and 'math' types, \ 
+193 so this returns whether _type is a type from these stdlib modules. 
 194 """ 
-195 return ( 
-196 type(_type) is type 
-197 and not is_builtin_type(_type) 
-198 and not is_from_other_toml_supported_module(_type) 
-199 and not is_from_types_or_typing(_type) 
-200 ) 
+195 return _type.__module__ in ("datetime", "math") 
+196 
+197 
+198def is_parameterized(_type: Type) -> bool: 
+199 """ 
+200 Returns whether _type is a parameterized type. 
 201 
-202 
-203def instance_of_custom_class(var: typing.Any) -> bool: 
-204 """ 
-205 Calls `is_custom_class` on an instance of a (possibly custom) class. 
-206 """ 
-207 return is_custom_class(var.__class__) 
+202 Examples: 
+203 list[str] -> True 
+204 str -> False 
+205 """ 
+206 return typing.get_origin(_type) is not None 
+207 
 208 
-209 
-210def is_optional(_type: Type | typing.Any) -> bool: 
-211 """ 
-212 Tries to guess if _type could be optional. 
-213 
-214 Examples: 
-215 None -> True 
-216 NoneType -> True 
-217 typing.Union[str, None] -> True 
-218 str | None -> True 
-219 list[str | None] -> False 
-220 list[str] -> False 
-221 """ 
-222 if _type and (is_parameterized(_type) and typing.get_origin(_type) in
-(dict, list)) or (_type is math.nan): 
-223 # e.g. list[str] 
-224 # will crash issubclass to test it first here 
-225 return False 
-226 
-227 return ( 
-228 _type is None 
-229 or types.NoneType in typing.get_args(_type) # union with Nonetype 
-230 or issubclass(types.NoneType, _type) 
-231 or issubclass(types.NoneType, type(_type)) # no type # Nonetype 
-232 ) 
+209def is_custom_class(_type: Type) -> bool: 
+210 """ 
+211 Tries to guess if _type is a builtin or a custom (user-defined) class. 
+212 
+213 Other logic in this module depends on knowing that. 
+214 """ 
+215 return ( 
+216 type(_type) is type 
+217 and not is_builtin_type(_type) 
+218 and not is_from_other_toml_supported_module(_type) 
+219 and not is_from_types_or_typing(_type) 
+220 ) 
+221 
+222 
+223def instance_of_custom_class(var: typing.Any) -> bool: 
+224 """ 
+225 Calls `is_custom_class` on an instance of a (possibly custom) class. 
+226 """ 
+227 return is_custom_class(var.__class__) 
+228 
+229 
+230def is_optional(_type: Type | typing.Any) -> bool: 
+231 """ 
+232 Tries to guess if _type could be optional. 
 233 
-234 
-235def dataclass_field(cls: Type, key: str) -> typing.Optional[dc.Field
+234 Examples: 
+235 None -> True 
+236 NoneType -> True 
+237 typing.Union[str, None] -> True 
+238 str | None -> True 
+239 list[str | None] -> False 
+240 list[str] -> False 
+241 """ 
+242 if _type and (is_parameterized(_type) and typing.get_origin(_type) in
+(dict, list)) or (_type is math.nan): 
+243 # e.g. list[str] 
+244 # will crash issubclass to test it first here 
+245 return False 
+246 
+247 return ( 
+248 _type is None 
+249 or types.NoneType in typing.get_args(_type) # union with Nonetype 
+250 or issubclass(types.NoneType, _type) 
+251 or issubclass(types.NoneType, type(_type)) # no type # Nonetype 
+252 ) 
+253 
+254 
+255def dataclass_field(cls: Type, key: str) -> typing.Optional[dc.Field
 [typing.Any]]: 
-236 """ 
-237 Get Field info for a dataclass cls. 
-238 """ 
-239 fields = getattr(cls, "__dataclass_fields__", {}) 
-240 return fields.get(key) 
-241 
-242 
-243def load_recursive(cls: Type, data: dict[str, T], annotations: dict[str,
+256 """ 
+257 Get Field info for a dataclass cls. 
+258 """ 
+259 fields = getattr(cls, "__dataclass_fields__", {}) 
+260 return fields.get(key) 
+261 
+262 
+263def load_recursive(cls: Type, data: dict[str, T], annotations: dict[str,
 Type]) -> dict[str, T]: 
-244 """ 
-245 For all annotations (recursively gathered from parents with
+264 """ 
+265 For all annotations (recursively gathered from parents with
 `all_annotations`), \ 
-246 try to resolve the tree of annotations. 
-247 
-248 Uses `load_into_recurse`, not itself directly. 
-249 
-250 Example: 
-251 class First: 
-252 key: str 
-253 
-254 class Second: 
-255 other: First 
-256 
-257 # step 1 
-258 cls = Second 
-259 data = {"second": {"other": {"key": "anything"}}} 
-260 annotations: {"other": First} 
-261 
-262 # step 1.5 
-263 data = {"other": {"key": "anything"} 
-264 annotations: {"other": First} 
-265 
-266 # step 2 
-267 cls = First 
-268 data = {"key": "anything"} 
-269 annotations: {"key": str} 
-270 
-271 
-272 TODO: python 3.11 exception groups to throw multiple errors at once! 
-273 """ 
-274 updated = {} 
-275 
-276 for _key, _type in annotations.items(): 
-277 if _key in data: 
-278 value: typing.Any = data[_key] # value can change so define it as any
-instead of T 
-279 if is_parameterized(_type): 
-280 origin = typing.get_origin(_type) 
-281 arguments = typing.get_args(_type) 
-282 if origin is list and arguments and is_custom_class(arguments[0]): 
-283 subtype = arguments[0] 
-284 value = [_load_into_recurse(subtype, subvalue) for subvalue in value] 
+266 try to resolve the tree of annotations. 
+267 
+268 Uses `load_into_recurse`, not itself directly. 
+269 
+270 Example: 
+271 class First: 
+272 key: str 
+273 
+274 class Second: 
+275 other: First 
+276 
+277 # step 1 
+278 cls = Second 
+279 data = {"second": {"other": {"key": "anything"}}} 
+280 annotations: {"other": First} 
+281 
+282 # step 1.5 
+283 data = {"other": {"key": "anything"} 
+284 annotations: {"other": First} 
 285 
-286 elif origin is dict and arguments and is_custom_class(arguments[1]): 
-287 # e.g. dict[str, Point] 
-288 subkeytype, subvaluetype = arguments 
-289 # subkey(type) is not a custom class, so don't try to convert it: 
-290 value = {subkey: _load_into_recurse(subvaluetype, subvalue) for subkey,
+286 # step 2 
+287 cls = First 
+288 data = {"key": "anything"} 
+289 annotations: {"key": str} 
+290 
+291 
+292 TODO: python 3.11 exception groups to throw multiple errors at once! 
+293 """ 
+294 updated = {} 
+295 
+296 for _key, _type in annotations.items(): 
+297 if _key in data: 
+298 value: typing.Any = data[_key] # value can change so define it as any
+instead of T 
+299 if is_parameterized(_type): 
+300 origin = typing.get_origin(_type) 
+301 arguments = typing.get_args(_type) 
+302 if origin is list and arguments and is_custom_class(arguments[0]): 
+303 subtype = arguments[0] 
+304 value = [_load_into_recurse(subtype, subvalue) for subvalue in value] 
+305 
+306 elif origin is dict and arguments and is_custom_class(arguments[1]): 
+307 # e.g. dict[str, Point] 
+308 subkeytype, subvaluetype = arguments 
+309 # subkey(type) is not a custom class, so don't try to convert it: 
+310 value = {subkey: _load_into_recurse(subvaluetype, subvalue) for subkey,
 subvalue in value.items()} 
-291 # elif origin is dict: 
-292 # keep data the same 
-293 elif origin is typing.Union and arguments: 
-294 for arg in arguments: 
-295 if is_custom_class(arg): 
-296 value = _load_into_recurse(arg, value) 
-297 else: 
-298 # print(_type, arg, value) 
-299 ... 
-300 
-301 # todo: other parameterized/unions/typing.Optional 
-302 
-303 elif is_custom_class(_type): 
-304 # type must be C (custom class) at this point 
-305 value = _load_into_recurse( 
-306 # make mypy and pycharm happy by telling it _type is of type C... 
-307 # actually just passing _type as first arg! 
-308 typing.cast(Type_C[typing.Any], _type), 
-309 value, 
-310 ) 
-311 
-312 elif _key in cls.__dict__: 
-313 # property has default, use that instead. 
-314 value = cls.__dict__[_key] 
-315 elif is_optional(_type): 
-316 # type is optional and not found in __dict__ -> default is None 
-317 value = None 
-318 elif dc.is_dataclass(cls) and (field := dataclass_field(cls, _key)) and
+311 # elif origin is dict: 
+312 # keep data the same 
+313 elif origin is typing.Union and arguments: 
+314 for arg in arguments: 
+315 if is_custom_class(arg): 
+316 value = _load_into_recurse(arg, value) 
+317 else: 
+318 # print(_type, arg, value) 
+319 ... 
+320 
+321 # todo: other parameterized/unions/typing.Optional 
+322 
+323 elif is_custom_class(_type): 
+324 # type must be C (custom class) at this point 
+325 value = _load_into_recurse( 
+326 # make mypy and pycharm happy by telling it _type is of type C... 
+327 # actually just passing _type as first arg! 
+328 typing.cast(Type_C[typing.Any], _type), 
+329 value, 
+330 ) 
+331 
+332 elif _key in cls.__dict__: 
+333 # property has default, use that instead. 
+334 value = cls.__dict__[_key] 
+335 elif is_optional(_type): 
+336 # type is optional and not found in __dict__ -> default is None 
+337 value = None 
+338 elif dc.is_dataclass(cls) and (field := dataclass_field(cls, _key)) and
 field.default_factory is not dc.MISSING: 
-319 # could have a default factory 
-320 # todo: do something with field.default? 
-321 value = field.default_factory() 
-322 else: 
-323 raise ConfigErrorMissingKey(_key, cls, _type) 
-324 
-325 updated[_key] = value 
-326 
-327 return updated 
-328 
-329 
-330def _all_annotations(cls: Type) -> ChainMap[str, Type]: 
-331 """ 
-332 Returns a dictionary-like ChainMap that includes annotations for all \ 
-333 attributes defined in cls or inherited from superclasses. 
-334 """ 
-335 return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if
-"__annotations__" in c.__dict__)) 
-336 
-337 
-338def all_annotations(cls: Type, _except: typing.Iterable[str] = None) -> dict
-[str, Type]: 
-339 """ 
-340 Wrapper around `_all_annotations` that filters away any keys in _except. 
-341 
-342 It also flattens the ChainMap to a regular dict. 
-343 """ 
-344 if _except is None: 
-345 _except = set() 
+339 # could have a default factory 
+340 # todo: do something with field.default? 
+341 value = field.default_factory() 
+342 else: 
+343 raise ConfigErrorMissingKey(_key, cls, _type) 
+344 
+345 updated[_key] = value 
 346 
-347 _all = _all_annotations(cls) 
-348 return {k: v for k, v in _all.items() if k not in _except} 
+347 return updated 
+348 
 349 
-350 
-351def check_and_convert_data( 
-352 cls: typing.Type[C], 
-353 data: dict[str, typing.Any], 
-354 _except: typing.Iterable[str], 
-355 strict: bool = True, 
-356) -> dict[str, typing.Any]: 
-357 """ 
-358 Based on class annotations, this prepares the data for
+350def _all_annotations(cls: Type) -> ChainMap[str, Type]: 
+351 """ 
+352 Returns a dictionary-like ChainMap that includes annotations for all \ 
+353 attributes defined in cls or inherited from superclasses. 
+354 """ 
+355 return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if
+"__annotations__" in c.__dict__)) 
+356 
+357 
+358def all_annotations(cls: Type, _except: typing.Iterable[str] = None) -> dict
+[str, Type]: 
+359 """ 
+360 Wrapper around `_all_annotations` that filters away any keys in _except. 
+361 
+362 It also flattens the ChainMap to a regular dict. 
+363 """ 
+364 if _except is None: 
+365 _except = set() 
+366 
+367 _all = _all_annotations(cls) 
+368 return {k: v for k, v in _all.items() if k not in _except} 
+369 
+370 
+371def check_and_convert_data( 
+372 cls: typing.Type[C], 
+373 data: dict[str, typing.Any], 
+374 _except: typing.Iterable[str], 
+375 strict: bool = True, 
+376) -> dict[str, typing.Any]: 
+377 """ 
+378 Based on class annotations, this prepares the data for
 `load_into_recurse`. 
-359 
-360 1. convert config-keys to python compatible config_keys 
-361 2. loads custom class type annotations with the same logic (see also
+379 
+380 1. convert config-keys to python compatible config_keys 
+381 2. loads custom class type annotations with the same logic (see also
 `load_recursive`) 
-362 3. ensures the annotated types match the actual types after loading the
+382 3. ensures the annotated types match the actual types after loading the
 config file. 
-363 """ 
-364 annotations = all_annotations(cls, _except=_except) 
-365 
-366 to_load = convert_config(data) 
-367 to_load = load_recursive(cls, to_load, annotations) 
-368 if strict: 
-369 to_load = ensure_types(to_load, annotations) 
-370 
-371 return to_load 
-372 
-373 
-374def _load_into_recurse( 
-375 cls: typing.Type[C], 
-376 data: dict[str, typing.Any], 
-377 init: dict[str, typing.Any] = None, 
-378 strict: bool = True, 
-379) -> C: 
-380 """ 
-381 Loads an instance of `cls` filled with `data`. 
-382 
-383 Uses `load_recursive` to load any fillable annotated properties (see that
+383 """ 
+384 annotations = all_annotations(cls, _except=_except) 
+385 
+386 to_load = convert_config(data) 
+387 to_load = load_recursive(cls, to_load, annotations) 
+388 if strict: 
+389 to_load = ensure_types(to_load, annotations) 
+390 
+391 return to_load 
+392 
+393 
+394def _load_into_recurse( 
+395 cls: typing.Type[C], 
+396 data: dict[str, typing.Any], 
+397 init: dict[str, typing.Any] = None, 
+398 strict: bool = True, 
+399) -> C: 
+400 """ 
+401 Loads an instance of `cls` filled with `data`. 
+402 
+403 Uses `load_recursive` to load any fillable annotated properties (see that
 method for an example). 
-384 `init` can be used to optionally pass extra __init__ arguments. \ 
-385 NOTE: This will overwrite a config key with the same name! 
-386 """ 
-387 if init is None: 
-388 init = {} 
-389 
-390 # fixme: cls.__init__ can set other keys than the name is in kwargs!! 
-391 
-392 if dc.is_dataclass(cls): 
-393 to_load = check_and_convert_data(cls, data, init.keys(), strict=strict) 
-394 to_load |= init # add extra init variables (should not happen for a
+404 `init` can be used to optionally pass extra __init__ arguments. \ 
+405 NOTE: This will overwrite a config key with the same name! 
+406 """ 
+407 if init is None: 
+408 init = {} 
+409 
+410 # fixme: cls.__init__ can set other keys than the name is in kwargs!! 
+411 
+412 if dc.is_dataclass(cls): 
+413 to_load = check_and_convert_data(cls, data, init.keys(), strict=strict) 
+414 to_load |= init # add extra init variables (should not happen for a
 dataclass but whatev) 
-395 
-396 # ensure mypy inst is an instance of the cls type (and not a fictuous
+415 
+416 # ensure mypy inst is an instance of the cls type (and not a fictuous
 `DataclassInstance`) 
-397 inst = typing.cast(C, cls(**to_load)) 
-398 else: 
-399 inst = cls(**init) 
-400 to_load = check_and_convert_data(cls, data, inst.__dict__.keys(),
+417 inst = typing.cast(C, cls(**to_load)) 
+418 else: 
+419 inst = cls(**init) 
+420 to_load = check_and_convert_data(cls, data, inst.__dict__.keys(),
 strict=strict) 
-401 inst.__dict__.update(**to_load) 
-402 
-403 return inst 
-404 
-405 
-406def _load_into_instance( 
-407 inst: C, 
-408 cls: typing.Type[C], 
-409 data: dict[str, typing.Any], 
-410 init: dict[str, typing.Any] = None, 
-411 strict: bool = True, 
-412) -> C: 
-413 """ 
-414 Similar to `load_into_recurse` but uses an existing instance of a class (so
-after __init__) \ 
-415 and thus does not support init. 
-416 
-417 """ 
-418 if init is not None: 
-419 raise ValueError("Can not init an existing instance!") 
-420 
-421 existing_data = inst.__dict__ 
+421 inst.__dict__.update(**to_load) 
 422 
-423 to_load = check_and_convert_data(cls, data, _except=existing_data.keys(),
-strict=strict) 
+423 return inst 
 424 
-425 inst.__dict__.update(**to_load) 
-426 
-427 return inst 
-428 
-429 
-430def load_into_class( 
-431 cls: typing.Type[C], 
-432 data: T_data, 
-433 /, 
-434 key: str = None, 
-435 init: dict[str, typing.Any] = None, 
-436 strict: bool = True, 
-437) -> C: 
-438 """ 
-439 Shortcut for _load_data + load_into_recurse. 
-440 """ 
-441 to_load = _load_data(data, key, cls.__name__) 
-442 return _load_into_recurse(cls, to_load, init=init, strict=strict) 
-443 
+425 
+426def _load_into_instance( 
+427 inst: C, 
+428 cls: typing.Type[C], 
+429 data: dict[str, typing.Any], 
+430 init: dict[str, typing.Any] = None, 
+431 strict: bool = True, 
+432) -> C: 
+433 """ 
+434 Similar to `load_into_recurse` but uses an existing instance of a class (so
+after __init__) \ 
+435 and thus does not support init. 
+436 
+437 """ 
+438 if init is not None: 
+439 raise ValueError("Can not init an existing instance!") 
+440 
+441 existing_data = inst.__dict__ 
+442 
+443 to_load = check_and_convert_data(cls, data, _except=existing_data.keys(),
+strict=strict) 
 444 
-445def load_into_instance( 
-446 inst: C, 
-447 data: T_data, 
-448 /, 
-449 key: str = None, 
-450 init: dict[str, typing.Any] = None, 
-451 strict: bool = True, 
-452) -> C: 
-453 """ 
-454 Shortcut for _load_data + load_into_existing. 
-455 """ 
-456 cls = inst.__class__ 
-457 to_load = _load_data(data, key, cls.__name__) 
-458 return _load_into_instance(inst, cls, to_load, init=init, strict=strict) 
-459 
-460 
-461def load_into( 
-462 cls: typing.Type[C], 
-463 data: T_data, 
-464 /, 
-465 key: str = None, 
-466 init: dict[str, typing.Any] = None, 
-467 strict: bool = True, 
-468) -> C: 
-469 """ 
-470 Load your config into a class (instance). 
-471 
-472 Supports both a class or an instance as first argument, but that's hard to
+445 inst.__dict__.update(**to_load) 
+446 
+447 return inst 
+448 
+449 
+450def load_into_class( 
+451 cls: typing.Type[C], 
+452 data: T_data, 
+453 /, 
+454 key: str = None, 
+455 init: dict[str, typing.Any] = None, 
+456 strict: bool = True, 
+457) -> C: 
+458 """ 
+459 Shortcut for _load_data + load_into_recurse. 
+460 """ 
+461 to_load = _load_data(data, key, cls.__name__) 
+462 return _load_into_recurse(cls, to_load, init=init, strict=strict) 
+463 
+464 
+465def load_into_instance( 
+466 inst: C, 
+467 data: T_data, 
+468 /, 
+469 key: str = None, 
+470 init: dict[str, typing.Any] = None, 
+471 strict: bool = True, 
+472) -> C: 
+473 """ 
+474 Shortcut for _load_data + load_into_existing. 
+475 """ 
+476 cls = inst.__class__ 
+477 to_load = _load_data(data, key, cls.__name__) 
+478 return _load_into_instance(inst, cls, to_load, init=init, strict=strict) 
+479 
+480 
+481def load_into( 
+482 cls: typing.Type[C], 
+483 data: T_data, 
+484 /, 
+485 key: str = None, 
+486 init: dict[str, typing.Any] = None, 
+487 strict: bool = True, 
+488) -> C: 
+489 """ 
+490 Load your config into a class (instance). 
+491 
+492 Supports both a class or an instance as first argument, but that's hard to
 explain to mypy, so officially only 
-473 classes are supported, and if you want to `load_into` an instance, you
+493 classes are supported, and if you want to `load_into` an instance, you
 should use `load_into_instance`. 
-474 
-475 Args: 
-476 cls: either a class or an existing instance of that class. 
-477 data: can be a dictionary or a path to a file to load (as pathlib.Path or
+494 
+495 Args: 
+496 cls: either a class or an existing instance of that class. 
+497 data: can be a dictionary or a path to a file to load (as pathlib.Path or
 str) 
-478 key: optional (nested) dictionary key to load data from (e.g.
+498 key: optional (nested) dictionary key to load data from (e.g.
 'tool.su6.specific') 
-479 init: optional data to pass to your cls' __init__ method (only if cls is
+499 init: optional data to pass to your cls' __init__ method (only if cls is
 not an instance already) 
-480 strict: enable type checks or allow anything? 
-481 
-482 """ 
-483 if not isinstance(cls, type): 
-484 # would not be supported according to mypy, but you can still load_into
+500 strict: enable type checks or allow anything? 
+501 
+502 """ 
+503 if not isinstance(cls, type): 
+504 # would not be supported according to mypy, but you can still load_into
 (instance) 
-485 return load_into_instance(cls, data, key=key, init=init, strict=strict) 
-486 
-487 # make mypy and pycharm happy by telling it cls is of type C and not just
+505 return load_into_instance(cls, data, key=key, init=init, strict=strict) 
+506 
+507 # make mypy and pycharm happy by telling it cls is of type C and not just
 'type' 
-488 # _cls = typing.cast(typing.Type[C], cls) 
-489 return load_into_class(cls, data, key=key, init=init, strict=strict) 
+508 # _cls = typing.cast(typing.Type[C], cls) 
+509 return load_into_class(cls, data, key=key, init=init, strict=strict) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-19 17:38 +0200
+at 2023-06-22 14:32 +0200
```

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_dump_py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_errors_py.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/dump.py: 100%</title>
+    <title>Coverage for src/configuraptor/errors.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/configuraptor/dump.py</b>:
+            <span class="text">Coverage for </span><b>src/configuraptor/errors.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">31 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">31<span class="text"> run</span></button>
+            <span class="text">46 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">46<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_dump_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-20 10:44 +0200
+            created at 2023-06-22 13:50 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,84 +77,163 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Method to dump classes to other formats.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Contains module-specific custom errors.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">json</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">dataclasses</span> <span class="key">import</span> <span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">tomli_w</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">yaml</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="nam">instance_of_custom_class</span><span class="op">,</span> <span class="nam">is_custom_class</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">camel_to_snake</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigError</span><span class="op">(</span><span class="nam">Exception</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="str">    Base exception class for this module.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">def</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">_level</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">0</span><span class="op">,</span> <span class="op">/</span><span class="op">,</span> <span class="nam">with_top_level_key</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    Dump a config instance to a dictionary (recursively).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="nam">cls</span> <span class="op">=</span> <span class="nam">value</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">asdict</span><span class="op">(</span><span class="nam">_</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span> <span class="key">if</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">_</span><span class="op">)</span> <span class="key">else</span> <span class="nam">_</span> <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">dict</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">v</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span> <span class="key">if</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">v</span><span class="op">)</span> <span class="key">else</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">data</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="key">if</span> <span class="nam">_level</span> <span class="op">==</span> <span class="num">0</span> <span class="key">and</span> <span class="nam">with_top_level_key</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="com"># top-level: add an extra key indicating the class' name</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">cls_name</span> <span class="op">=</span> <span class="nam">camel_to_snake</span><span class="op">(</span><span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">return</span> <span class="op">{</span><span class="nam">cls_name</span><span class="op">:</span> <span class="nam">data</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="key">def</span> <span class="nam">astoml</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">multiline_strings</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">    Dump a config instance to toml (recursively).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">return</span> <span class="nam">tomli_w</span><span class="op">.</span><span class="nam">dumps</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">multiline_strings</span><span class="op">=</span><span class="nam">multiline_strings</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="key">def</span> <span class="nam">asjson</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="str">    Dump a config instance to json (recursively).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="key">return</span> <span class="nam">json</span><span class="op">.</span><span class="nam">dumps</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="com"># class ConfigErrorGroup(ConfigError, ExceptionGroup):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="com">#     """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="com">#     Base Exception class for this module, but for exception groups (3.11+)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="com">#     """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="com">#     def __init__(self, _type: str, errors: list[Exception]):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="com">#         more = len(errors) > 1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="com">#         cnt = "Multiple" if more else "One"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="com">#         s = "s" if more else ""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="com">#         message = f"{cnt} {_type}{s} in config!"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="com">#         super().__init__(message, errors)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="com">#         if not errors:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="com">#             raise ValueError("Error group raised without any errors?")</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigErrorMissingKey</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">    Exception for when the config file is missing a required key.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="nam">annotated_type</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="str">        Automatically filles in the names of annotated type and cls for printing from __str__.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_annotated_type</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">annotated_type</span><span class="op">,</span> <span class="str">"__name__"</span><span class="op">,</span> <span class="nam">str</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">annotated_type</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_cls</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t"><span class="str">        Custom error message based on dataclass values and calculated actual type.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">            <span class="str">f"Config key '{self.key}' (type `{self._annotated_type}`) "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">            <span class="str">f"of class `{self._cls}` was not found in the config, "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">            <span class="str">f"but is required as a default value is not specified."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="key">def</span> <span class="nam">asyaml</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">    Dump a config instance to yaml (recursively).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="nam">output</span> <span class="op">=</span> <span class="nam">yaml</span><span class="op">.</span><span class="nam">dump</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="com"># output is already a str but mypy doesn't know that</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="nam">output</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigErrorExtraKey</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    Exception for when the config file is missing a required key.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="nam">value</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="str">        Automatically filles in the names of annotated type and cls for printing from __str__.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_cls</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_type</span> <span class="op">=</span> <span class="nam">type</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="str">        Custom error message based on dataclass values and calculated actual type.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">            <span class="str">f"Config key '{self.key}' (value: `{self.value}` type `{self._type}`) "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">            <span class="str">f"does not exist on class `{self._cls}`, but was attempted to be updated. "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">            <span class="str">f"Use strict = False to allow this behavior."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t"><span class="str">    Exception for when the config file contains a key with an unexpected type.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">    <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">    <span class="nam">expected_type</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t"><span class="str">        Store the actual type of the config variable.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">actual_type</span> <span class="op">=</span> <span class="nam">type</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">max_len</span> <span class="op">=</span> <span class="num">50</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_value</span> <span class="op">=</span> <span class="nam">str</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_value</span><span class="op">)</span> <span class="op">></span> <span class="nam">max_len</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">_value</span> <span class="op">=</span> <span class="str">f"{self._value[:max_len]}..."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="str">        Custom error message based on dataclass values and calculated actual type.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">            <span class="str">f"Config key '{self.key}' had a value (`{self._value}`) with a type (`{self.actual_type}`) "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">            <span class="str">f"that was not expected: `{self.expected_type}` is the required type."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigErrorImmutable</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t"><span class="str">    Raised when an immutable Mapping is attempted to be updated.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">    <span class="nam">cls</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t"><span class="str">        Store the class name.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_cls</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t"><span class="str">        Custom error message.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="key">return</span> <span class="str">f"{self._cls} is Immutable!"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t"><span class="key">class</span> <span class="nam">IsPostponedError</span><span class="op">(</span><span class="nam">ConfigError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t"><span class="str">    Error thrown when you try to access a 'postponed' property without filling its value first.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">    <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"This postponed property has not been filled yet!"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_dump_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-20 10:44 +0200
+            created at 2023-06-22 13:50 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,85 +1,166 @@
 
-****** Coverage for src/configuraptor/dump.py: 100% ******
+****** Coverage for src/configuraptor/errors.py: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 31 statements   31 run 0 missing 0 excluded *****
+***** 46 statements   46 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-20 10:44 +0200
+at 2023-06-22 13:50 +0200
 
 
 1""" 
-2Method to dump classes to other formats. 
+2Contains module-specific custom errors. 
 3""" 
-4 
-5import json 
-6import typing 
+4import typing 
+5from dataclasses import dataclass 
+6 
 7 
-8import tomli_w 
-9import yaml 
-10 
-11from .core import instance_of_custom_class, is_custom_class 
-12from .helpers import camel_to_snake 
+8class ConfigError(Exception): 
+9 """ 
+10 Base exception class for this module. 
+11 """ 
+12 
 13 
-14 
-15def asdict(inst: typing.Any, _level: int = 0, /, with_top_level_key: bool =
-True) -> dict[str, typing.Any]: 
-16 """ 
-17 Dump a config instance to a dictionary (recursively). 
-18 """ 
-19 data = {} 
-20 
-21 for key, value in inst.__dict__.items(): 
-22 cls = value.__class__ 
-23 if is_custom_class(cls): 
-24 value = asdict(value, _level + 1) 
-25 elif isinstance(value, list): 
-26 value = [asdict(_, _level + 1) if instance_of_custom_class(_) else _ for _
-in value] 
-27 elif isinstance(value, dict): 
-28 value = {k: asdict(v, _level + 1) if instance_of_custom_class(v) else v for
-k, v in value.items()} 
-29 
-30 data[key] = value 
-31 
-32 if _level == 0 and with_top_level_key: 
-33 # top-level: add an extra key indicating the class' name 
-34 cls_name = camel_to_snake(inst.__class__.__name__) 
-35 return {cls_name: data} 
-36 
-37 return data 
-38 
-39 
-40def astoml(inst: typing.Any, multiline_strings: bool = False) -> str: 
+14# class ConfigErrorGroup(ConfigError, ExceptionGroup): 
+15# """ 
+16# Base Exception class for this module, but for exception groups (3.11+) 
+17# """ 
+18# def __init__(self, _type: str, errors: list[Exception]): 
+19# more = len(errors) > 1 
+20# cnt = "Multiple" if more else "One" 
+21# s = "s" if more else "" 
+22# message = f"{cnt} {_type}{s} in config!" 
+23# super().__init__(message, errors) 
+24# if not errors: 
+25# raise ValueError("Error group raised without any errors?") 
+26 
+27 
+28@dataclass 
+29class ConfigErrorMissingKey(ConfigError): 
+30 """ 
+31 Exception for when the config file is missing a required key. 
+32 """ 
+33 
+34 key: str 
+35 cls: type 
+36 annotated_type: type 
+37 
+38 def __post_init__(self) -> None: 
+39 """ 
+40 Automatically filles in the names of annotated type and cls for printing
+from __str__. 
 41 """ 
-42 Dump a config instance to toml (recursively). 
-43 """ 
-44 data = asdict(inst) 
-45 return tomli_w.dumps(data, multiline_strings=multiline_strings) 
-46 
-47 
-48def asjson(inst: typing.Any, **kw: typing.Any) -> str: 
-49 """ 
-50 Dump a config instance to json (recursively). 
-51 """ 
-52 data = asdict(inst) 
-53 return json.dumps(data, **kw) 
+42 self._annotated_type = getattr(self.annotated_type, "__name__", str
+(self.annotated_type)) 
+43 self._cls = self.cls.__name__ 
+44 
+45 def __str__(self) -> str: 
+46 """ 
+47 Custom error message based on dataclass values and calculated actual type. 
+48 """ 
+49 return ( 
+50 f"Config key '{self.key}' (type `{self._annotated_type}`) " 
+51 f"of class `{self._cls}` was not found in the config, " 
+52 f"but is required as a default value is not specified." 
+53 ) 
 54 
 55 
-56def asyaml(inst: typing.Any, **kw: typing.Any) -> str: 
-57 """ 
-58 Dump a config instance to yaml (recursively). 
-59 """ 
-60 data = asdict(inst) 
-61 output = yaml.dump(data, encoding=None, **kw) 
-62 # output is already a str but mypy doesn't know that 
-63 return typing.cast(str, output) 
+56@dataclass 
+57class ConfigErrorExtraKey(ConfigError): 
+58 """ 
+59 Exception for when the config file is missing a required key. 
+60 """ 
+61 
+62 key: str 
+63 value: str 
+64 cls: type 
+65 
+66 def __post_init__(self) -> None: 
+67 """ 
+68 Automatically filles in the names of annotated type and cls for printing
+from __str__. 
+69 """ 
+70 self._cls = self.cls.__name__ 
+71 self._type = type(self.value) 
+72 
+73 def __str__(self) -> str: 
+74 """ 
+75 Custom error message based on dataclass values and calculated actual type. 
+76 """ 
+77 return ( 
+78 f"Config key '{self.key}' (value: `{self.value}` type `{self._type}`) " 
+79 f"does not exist on class `{self._cls}`, but was attempted to be updated. " 
+80 f"Use strict = False to allow this behavior." 
+81 ) 
+82 
+83 
+84@dataclass 
+85class ConfigErrorInvalidType(ConfigError): 
+86 """ 
+87 Exception for when the config file contains a key with an unexpected type. 
+88 """ 
+89 
+90 key: str 
+91 value: typing.Any 
+92 expected_type: type 
+93 
+94 def __post_init__(self) -> None: 
+95 """ 
+96 Store the actual type of the config variable. 
+97 """ 
+98 self.actual_type = type(self.value) 
+99 
+100 max_len = 50 
+101 self._value = str(self.value) 
+102 if len(self._value) > max_len: 
+103 self._value = f"{self._value[:max_len]}..." 
+104 
+105 def __str__(self) -> str: 
+106 """ 
+107 Custom error message based on dataclass values and calculated actual type. 
+108 """ 
+109 return ( 
+110 f"Config key '{self.key}' had a value (`{self._value}`) with a type (`
+{self.actual_type}`) " 
+111 f"that was not expected: `{self.expected_type}` is the required type." 
+112 ) 
+113 
+114 
+115@dataclass 
+116class ConfigErrorImmutable(ConfigError): 
+117 """ 
+118 Raised when an immutable Mapping is attempted to be updated. 
+119 """ 
+120 
+121 cls: type 
+122 
+123 def __post_init__(self) -> None: 
+124 """ 
+125 Store the class name. 
+126 """ 
+127 self._cls = self.cls.__name__ 
+128 
+129 def __str__(self) -> str: 
+130 """ 
+131 Custom error message. 
+132 """ 
+133 return f"{self._cls} is Immutable!" 
+134 
+135 
+136@dataclass 
+137class IsPostponedError(ConfigError): 
+138 """ 
+139 Error thrown when you try to access a 'postponed' property without filling
+its value first. 
+140 """ 
+141 
+142 message: str = "This postponed property has not been filled yet!" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-20 10:44 +0200
+at 2023-06-22 13:50 +0200
```

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html` & `configuraptor-1.9.2/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -56,20 +56,20 @@
         <h2>
             <span class="text">13 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">13<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_311_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_postpone_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:42 +0200
+            created at 2023-06-22 13:07 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -94,15 +94,15 @@
     <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="str">    Can be used as a metaclass:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">        class AbstractConfig(metaclass=Singleton):</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">    Source: https://stackoverflow.com/questions/6760685/creating-a-singleton-in-python</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">_instances</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">_instances</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">ClassVar</span><span class="op">[</span><span class="nam">dict</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="key">def</span> <span class="nam">__call__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">        When a class is instantiated (e.g. `AbstractConfig()`), __call__ is called. This overrides the default behavior.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_instances</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">_instances</span><span class="op">[</span><span class="nam">self</span><span class="op">]</span> <span class="op">=</span> <span class="nam">super</span><span class="op">(</span><span class="nam">SingletonMeta</span><span class="op">,</span> <span class="nam">self</span><span class="op">)</span><span class="op">.</span><span class="nam">__call__</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
@@ -126,18 +126,18 @@
     <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="str">    Mixin to make a class a singleton.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_311_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_postpone_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 11:42 +0200
+            created at 2023-06-22 13:07 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 13 statements   13 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 11:42 +0200
+at 2023-06-22 13:07 +0200
 
 
 1""" 
 2Singleton mixin/metaclass. 
 3""" 
 4 
 5import typing 
@@ -29,15 +29,16 @@
 13 Example: 
 14 class AbstractConfig(metaclass=Singleton): 
 15 
 16 Source: https://stackoverflow.com/questions/6760685/creating-a-singleton-in-
 python 
 17 """ 
 18 
-19 _instances: dict[typing.Type[typing.Any], typing.Type[typing.Any]] = {} 
+19 _instances: typing.ClassVar[dict[typing.Type[typing.Any], typing.Type
+[typing.Any]]] = {} 
 20 
 21 def __call__(self, *args: typing.Any, **kwargs: typing.Any) -> typing.Type
 [typing.Any]: 
 22 """ 
 23 When a class is instantiated (e.g. `AbstractConfig()`), __call__ is called.
 This overrides the default behavior. 
 24 """ 
@@ -62,8 +63,8 @@
 42 
 43class Singleton(metaclass=SingletonMeta): 
 44 """ 
 45 Mixin to make a class a singleton. 
 46 """ 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 11:42 +0200
+at 2023-06-22 13:07 +0200
```

### Comparing `configuraptor-1.8.0/htmlcov/favicon_32.png` & `configuraptor-1.9.2/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/index.html` & `configuraptor-1.9.2/htmlcov/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-21 15:50 +0200
+            created at 2023-06-22 14:32 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -73,39 +73,39 @@
                 <td>6</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="6 6">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_cls_py.html">src/configuraptor/cls.py</a></td>
-                <td>24</td>
+                <td>51</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="24 24">100%</td>
+                <td class="right" data-ratio="51 51">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_core_py.html">src/configuraptor/core.py</a></td>
-                <td>156</td>
+                <td>166</td>
                 <td>0</td>
-                <td>3</td>
-                <td class="right" data-ratio="156 156">100%</td>
+                <td>5</td>
+                <td class="right" data-ratio="166 166">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_dump_py.html">src/configuraptor/dump.py</a></td>
                 <td>31</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="31 31">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_errors_py.html">src/configuraptor/errors.py</a></td>
-                <td>39</td>
+                <td>46</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="39 39">100%</td>
+                <td class="right" data-ratio="46 46">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_helpers_py.html">src/configuraptor/helpers.py</a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
@@ -145,30 +145,30 @@
                 <td>0</td>
                 <td class="right" data-ratio="13 13">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>310</td>
+                <td>354</td>
                 <td>0</td>
-                <td>3</td>
-                <td class="right" data-ratio="310 310">100%</td>
+                <td>5</td>
+                <td class="right" data-ratio="354 354">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-21 15:50 +0200
+            created at 2023-06-22 14:32 +0200
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_singleton_py.html"/>
         <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -2,28 +2,28 @@
 ****** Coverage report: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-06-21 15:50 +0200
+coverage.py_v7.2.7, created at 2023-06-22 14:32 +0200
 
 Module                                statements missing excluded coverage
 src/configuraptor/__about__.py        1          0       0        100%
 src/configuraptor/__init__.py         6          0       0        100%
-src/configuraptor/cls.py              24         0       0        100%
-src/configuraptor/core.py             156        0       3        100%
+src/configuraptor/cls.py              51         0       0        100%
+src/configuraptor/core.py             166        0       5        100%
 src/configuraptor/dump.py             31         0       0        100%
-src/configuraptor/errors.py           39         0       0        100%
+src/configuraptor/errors.py           46         0       0        100%
 src/configuraptor/helpers.py          2          0       0        100%
 src/configuraptor/loaders/__init__.py 11         0       0        100%
 src/configuraptor/loaders/_types.py   4          0       0        100%
 src/configuraptor/loaders/            14         0       0        100%
 loaders_shared.py
 src/configuraptor/postpone.py         9          0       0        100%
 src/configuraptor/singleton.py        13         0       0        100%
-Total                                 310        0       3        100%
+Total                                 354        0       5        100%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-06-21 15:50 +0200
+coverage.py_v7.2.7, created at 2023-06-22 14:32 +0200
  ____
```

### Comparing `configuraptor-1.8.0/htmlcov/keybd_closed.png` & `configuraptor-1.9.2/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/keybd_open.png` & `configuraptor-1.9.2/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/htmlcov/status.json` & `configuraptor-1.9.2/htmlcov/status.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996162037037037%*

 * *Differences: {"'files'": "{'d_eb75b6cf8f5eab40___about___py': {'hash': 'f3d6090fee225db883989217e2a740bf'}, "*

 * *            "'d_eb75b6cf8f5eab40___init___py': {'hash': 'fcf8563f24b1586e1a72722455863f60'}, "*

 * *            "'d_eb75b6cf8f5eab40_cls_py': {'hash': '4eb0bef0088cbc7c1cd0ac424bf43b42', 'index': "*

 * *            "{'nums': {insert: [(2, 51)], delete: [2]}}}, 'd_eb75b6cf8f5eab40_core_py': {'hash': "*

 * *            "'1980a48acff8d9458e8ee05729ad82cd', 'index': {'nums': {insert: [(2, 166), (3, 5)], "*

 * *            "delete: [3,  […]*

```diff
@@ -269,15 +269,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/loaders_shared.py"
             }
         },
         "d_eb75b6cf8f5eab40___about___py": {
-            "hash": "3e93cb54154f78c6f81f6feef3376f69",
+            "hash": "f3d6090fee225db883989217e2a740bf",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40___about___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -286,15 +286,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/__about__.py"
             }
         },
         "d_eb75b6cf8f5eab40___init___py": {
-            "hash": "d5c1f5ac693aae2044dffde7eccaae57",
+            "hash": "fcf8563f24b1586e1a72722455863f60",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40___init___py.html",
                 "nums": [
                     0,
                     1,
                     6,
                     0,
@@ -303,39 +303,39 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/__init__.py"
             }
         },
         "d_eb75b6cf8f5eab40_cls_py": {
-            "hash": "b1f068469f7f94c16e9d267b087e8806",
+            "hash": "4eb0bef0088cbc7c1cd0ac424bf43b42",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_cls_py.html",
                 "nums": [
                     0,
                     1,
-                    24,
+                    51,
                     0,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/cls.py"
             }
         },
         "d_eb75b6cf8f5eab40_core_py": {
-            "hash": "000fc824ee5ffb18202f5e36ed1843ec",
+            "hash": "1980a48acff8d9458e8ee05729ad82cd",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_core_py.html",
                 "nums": [
                     0,
                     1,
-                    156,
-                    3,
+                    166,
+                    5,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/core.py"
             }
@@ -354,21 +354,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/dump.py"
             }
         },
         "d_eb75b6cf8f5eab40_errors_py": {
-            "hash": "f59126ae493adc32aa6331d7fc163d94",
+            "hash": "c246b517d164adf3fa3f9a012132c89f",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_errors_py.html",
                 "nums": [
                     0,
                     1,
-                    39,
+                    46,
                     0,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/errors.py"
@@ -405,15 +405,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/postpone.py"
             }
         },
         "d_eb75b6cf8f5eab40_singleton_py": {
-            "hash": "0e6e4db931998b4489d5c07b70fcbef5",
+            "hash": "b7f8b3ec8c29f6bec4d56f56dee1396c",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_singleton_py.html",
                 "nums": [
                     0,
                     1,
                     13,
                     0,
```

### Comparing `configuraptor-1.8.0/htmlcov/style.css` & `configuraptor-1.9.2/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/pytest_examples/some.toml` & `configuraptor-1.9.2/pytest_examples/some.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/src/configuraptor/__init__.py` & `configuraptor-1.9.2/src/configuraptor/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Exposes TypedConfig and load_into for this library.
 """
 
 # SPDX-FileCopyrightText: 2023-present Robin van der Noord <robinvandernoord@gmail.com>
 #
 # SPDX-License-Identifier: MIT
-from .cls import TypedConfig, update
+from .cls import TypedConfig, TypedMapping, TypedMutableMapping, update
 from .core import (
     all_annotations,
     check_and_convert_data,
     convert_config,
     ensure_types,
     load_into,
     load_into_class,
@@ -18,14 +18,16 @@
 from .dump import asdict, asjson, astoml, asyaml
 from .postpone import postpone
 from .singleton import Singleton, SingletonMeta
 
 __all__ = [
     # cls
     "TypedConfig",
+    "TypedMapping",
+    "TypedMutableMapping",
     "update",
     # singleton
     "Singleton",
     "SingletonMeta",
     # core
     "all_annotations",
     "check_and_convert_data",
```

### Comparing `configuraptor-1.8.0/src/configuraptor/core.py` & `configuraptor-1.9.2/src/configuraptor/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     """
     If no key is manually defined for `load_into`, \
     the class' name is converted to snake_case to use as the default key.
     """
     return camel_to_snake(clsname)
 
 
-def _load_data(data: T_data, key: str = None, classname: str = None) -> dict[str, typing.Any]:
+def __load_data(data: T_data, key: str = None, classname: str = None) -> dict[str, typing.Any]:
     """
     Tries to load the right data from a filename/path or dict, based on a manual key or a classname.
 
     E.g. class Tool will be mapped to key tool.
     It also deals with nested keys (tool.extra -> {"tool": {"extra": ...}}
     """
     if isinstance(data, str):
@@ -75,18 +75,39 @@
         # try to guess key by grabbing the first one or using the class name
         if len(data) == 1:
             key = list(data.keys())[0]
         elif classname is not None:
             key = _guess_key(classname)
 
     if key:
-        return _data_for_nested_key(key, data)
-    else:
-        # no key found, just return all data
-        return data
+        data = _data_for_nested_key(key, data)
+
+    if not data:
+        raise ValueError("No data found!")
+
+    if not isinstance(data, dict):
+        raise ValueError("Data is not a dict!")
+
+    return data
+
+
+def _load_data(data: T_data, key: str = None, classname: str = None) -> dict[str, typing.Any]:
+    """
+    Wrapper around __load_data that retries with key="" if anything goes wrong.
+    """
+    try:
+        return __load_data(data, key, classname)
+    except Exception as e:
+        if key != "":
+            return __load_data(data, "", classname)
+        else:  # pragma: no cover
+            warnings.warn(f"Data could not be loaded: {e}", source=e)
+            # key already was "", just return data!
+            # (will probably not happen but fallback)
+            return {}
 
 
 def check_type(value: typing.Any, expected_type: T_typelike) -> bool:
     """
     Given a variable, check if it matches 'expected_type' (which can be a Union, parameterized generic etc.).
 
     Based on typeguard but this returns a boolean instead of returning the value or throwing a TypeCheckError
```

### Comparing `configuraptor-1.8.0/src/configuraptor/dump.py` & `configuraptor-1.9.2/src/configuraptor/dump.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/src/configuraptor/errors.py` & `configuraptor-1.9.2/src/configuraptor/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,13 +109,34 @@
         return (
             f"Config key '{self.key}' had a value (`{self._value}`) with a type (`{self.actual_type}`) "
             f"that was not expected: `{self.expected_type}` is the required type."
         )
 
 
 @dataclass
+class ConfigErrorImmutable(ConfigError):
+    """
+    Raised when an immutable Mapping is attempted to be updated.
+    """
+
+    cls: type
+
+    def __post_init__(self) -> None:
+        """
+        Store the class name.
+        """
+        self._cls = self.cls.__name__
+
+    def __str__(self) -> str:
+        """
+        Custom error message.
+        """
+        return f"{self._cls} is Immutable!"
+
+
+@dataclass
 class IsPostponedError(ConfigError):
     """
     Error thrown when you try to access a 'postponed' property without filling its value first.
     """
 
     message: str = "This postponed property has not been filled yet!"
```

### Comparing `configuraptor-1.8.0/src/configuraptor/postpone.py` & `configuraptor-1.9.2/src/configuraptor/postpone.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/src/configuraptor/singleton.py` & `configuraptor-1.9.2/src/configuraptor/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/src/configuraptor/loaders/__init__.py` & `configuraptor-1.9.2/src/configuraptor/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/src/configuraptor/loaders/loaders_shared.py` & `configuraptor-1.9.2/src/configuraptor/loaders/loaders_shared.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/tests/test_core.py` & `configuraptor-1.9.2/tests/test_core.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,31 +5,51 @@
 
 import pytest
 
 from src.configuraptor import all_annotations
 from src.configuraptor.core import is_optional
 from tests.constants import EXAMPLE_FILE
 
+
 def test_invalid_extension():
     from src.configuraptor.loaders import get
 
     with pytest.raises(ValueError):
         get(".doesntexist")
 
 
 def test_is_optional_with_weird_inputs():
     assert is_optional(math.nan) is False
     assert is_optional(typing.Optional[dict[str, typing.Optional[str]]]) is True
 
+
 class Base:
     has: int
 
 
 class Sub(Base):
     has_also: int
 
 
 def test_all_annotations():
     # without except:
     assert set(all_annotations(Sub).keys()) == {"has", "has_also"}
     # with except:
     assert set(all_annotations(Sub, {"has_also"}).keys()) == {"has"}
+
+
+def test_no_data():
+    from src import configuraptor
+
+    # data must be a dict:
+    with pytest.raises(ValueError):
+        configuraptor.core._load_data(42, key=None)
+    with pytest.raises(ValueError):
+        configuraptor.core._load_data(["joe"], key=None)
+
+    # but other than that, it should be fine:
+    configuraptor.core._load_data({}, key="")
+    configuraptor.core._load_data({}, key=None)
+    configuraptor.core._load_data({"-": 0, "+": None}, key="joe", classname="-.+")
+    configuraptor.core._load_data({"-": 0, "+": None}, key="+", classname="-.+")
+    configuraptor.core._load_data({"-": 0, "+": None}, key="", classname="-.+")
+    configuraptor.core._load_data({"-": 0, "+": None}, key=None, classname="-.+")
```

### Comparing `configuraptor-1.8.0/tests/test_dumps.py` & `configuraptor-1.9.2/tests/test_dumps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import typing
 
 import tomli_w
 import yaml
 
 from src.configuraptor import TypedConfig
-from src.configuraptor.dump import asdict, asyaml, asjson, astoml
+from src.configuraptor.dump import asdict, asjson, astoml, asyaml
 
 
 class Simple(TypedConfig):
     key: str
     num: int
```

### Comparing `configuraptor-1.8.0/tests/test_json_yaml.py` & `configuraptor-1.9.2/tests/test_json_yaml.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/tests/test_postponed.py` & `configuraptor-1.9.2/tests/test_postponed.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import pytest
 
-from src.configuraptor import TypedConfig, Singleton, postpone
+from src.configuraptor import Singleton, TypedConfig, postpone
 from src.configuraptor.errors import IsPostponedError
 
 
 class Later(TypedConfig, Singleton):
     field: str  # instant
     other_field: str = postpone()
 
     def update(self):
         self.other_field = "usable"
 
 
-later = Later.load({"field": "instant"}, key="")
+later = Later.load({"field": "instant"})
 
 
 def test_postponed_can_be_filled_later():
     # later should be able to exist
     assert later
     assert later.field
     print(later, later.field)
```

### Comparing `configuraptor-1.8.0/tests/test_singleton.py` & `configuraptor-1.9.2/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/tests/test_toml_basic.py` & `configuraptor-1.9.2/tests/test_toml_basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     relevant = configuraptor.load_into(Relevant, file)
     assert relevant and relevant.key == "this one!"
 
 
 def test_guess_key_no_match():
     file = str(PYTEST_EXAMPLES / "with_multiple_toplevel_keys.toml")
     # no key and no match by class name:
-    relevant = configuraptor.load_into(Irrelevant, file, key="")
+    relevant = configuraptor.load_into(Irrelevant, file)
     assert relevant and relevant.key["value"] == "fallback"
 
 
 class TooLong:
     type: str
 
 
@@ -195,8 +195,8 @@
     not_required: typing.Optional[list[str]]
 
 
 def test_missing_required_parameterized():
     # should go through is_optional -> is_parameterized -> typing.get_origin(_type) in (dict, list) -> False -> Error
     data = {"not_required": ["list", "of", "string"]}
     with pytest.raises(ConfigErrorMissingKey):
-        configuraptor.load_into(ShouldHaveListOfString, data, key="")  # empty key to indicate data exists top-level
+        configuraptor.load_into(ShouldHaveListOfString, data)
```

### Comparing `configuraptor-1.8.0/tests/test_toml_dataclass.py` & `configuraptor-1.9.2/tests/test_toml_dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/tests/test_toml_existing.py` & `configuraptor-1.9.2/tests/test_toml_existing.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/LICENSE.txt` & `configuraptor-1.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/README.md` & `configuraptor-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `configuraptor-1.8.0/pyproject.toml` & `configuraptor-1.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 upload_to_release = false
 build_command = "hatch build"
 
 [tool.su6]
 directory = "src"
 include = []
 exclude = []
-stop-after-first-failure = false
+stop-after-first-failure = true
 coverage = 100
 badge = true
 
 [tool.black]
 target-version = ["py311"]
 line-length = 120
 # 'extend-exclude' excludes files or directories in addition to the defaults
```

### Comparing `configuraptor-1.8.0/PKG-INFO` & `configuraptor-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuraptor
-Version: 1.8.0
+Version: 1.9.2
 Summary: Load toml/yaml/json config files into classes for a typed config (type hinting etc.)
 Project-URL: Documentation, https://github.com/trialandsuccess/configuraptor#readme
 Project-URL: Issues, https://github.com/trialandsuccess/configuraptor/issues
 Project-URL: Source, https://github.com/trialandsuccess/configuraptor
 Author-email: Robin van der Noord <robin@trialandsuccess.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

