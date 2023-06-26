# Comparing `tmp/formulaic-0.6.2.tar.gz` & `tmp/formulaic-0.6.3.tar.gz`

## Comparing `formulaic-0.6.2.tar` & `formulaic-0.6.3.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 formulaic-0.6.2/benchmarks/README.md
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 formulaic-0.6.2/benchmarks/benchmark.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 formulaic-0.6.2/benchmarks/benchmarks.csv
--rw-r--r--   0        0        0    34436 2020-02-02 00:00:00.000000 formulaic-0.6.2/benchmarks/benchmarks.png
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 formulaic-0.6.2/benchmarks/plot.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 formulaic-0.6.2/benchmarks/requirements.txt
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/mkdocs.yml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/requirements.in
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/requirements.txt
--rw-r--r--   0        0        0    16859 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/changelog.md
--rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/formulas.md
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/index.md
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/installation.md
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/migration.md
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/assets/images/favicon.png
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/assets/images/logo.png
--rw-r--r--   0        0        0    42441 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/assets/images/logo.svg
--rw-r--r--   0        0        0    43761 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/assets/images/logo_with_text.png
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/concepts/index.md
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/dev/index.md
--rw-r--r--   0        0        0    46448 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/contrasts.ipynb
--rw-r--r--   0        0        0    29663 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/formulae.ipynb
--rw-r--r--   0        0        0     9850 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/grammar.md
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/index.md
--rw-r--r--   0        0        0    14831 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/integration.ipynb
--rw-r--r--   0        0        0    27554 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/model_specs.ipynb
--rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/quickstart.ipynb
--rw-r--r--   0        0        0   162005 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/splines.ipynb
--rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 formulaic-0.6.2/docsite/docs/guides/transforms.ipynb
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/_version.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/errors.py
--rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/formula.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/model_matrix.py
--rw-r--r--   0        0        0    15924 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/model_spec.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/sugar.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/__init__.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/arrow.py
--rw-r--r--   0        0        0    32051 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/base.py
--rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/pandas.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/types/__init__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/types/enums.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/types/evaluated_factor.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/types/factor_values.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/types/scoped_factor.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/materializers/types/scoped_term.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/__init__.py
--rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/parser.py
--rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/utils.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/algos/__init__.py
--rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/algos/tokenize.py
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/algos/tokens_to_ast.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/__init__.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/ast_node.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/factor.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/formula_parser.py
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/operator.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/operator_resolver.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/ordered_set.py
--rw-r--r--   0        0        0    17126 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/structured.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/term.py
--rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/parser/types/token.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/transforms/__init__.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/transforms/basis_spline.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/transforms/contrasts.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/transforms/identity.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/transforms/patsy_compat.py
--rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/transforms/poly.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/transforms/scale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/__init__.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/calculus.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/cast.py
--rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/constraints.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/context.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/iterators.py
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/layered_mapping.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/sentinels.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/sparse.py
--rw-r--r--   0        0        0    10122 2020-02-02 00:00:00.000000 formulaic-0.6.2/formulaic/utils/stateful_transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/__init__.py
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/test_formula.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/test_model_matrix.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/test_model_spec.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/test_sugar.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/__init__.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/test_arrow.py
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/test_base.py
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/test_pandas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/types/__init__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/types/test_evaluated_factor.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/types/test_factor_values.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/types/test_scoped_factor.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/materializers/types/test_scoped_term.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/__init__.py
--rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/test_parser.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/algos/__init__.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/algos/test_tokenize.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/algos/test_tokens_to_ast.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/__init__.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_ast_node.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_factor.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_formula_parser.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_operator.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_operator_resolver.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_ordered_set.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_structured.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_term.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/parser/types/test_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/transforms/__init__.py
--rw-r--r--   0        0        0    12756 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/transforms/test_basis_spline.py
--rw-r--r--   0        0        0    29890 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/transforms/test_contrasts.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/transforms/test_identity.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/transforms/test_patsy_compat.py
--rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/transforms/test_poly.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/transforms/test_scale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/__init__.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_calculus.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_capture_context.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_cast.py
--rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_constraints.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_iterators.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_layered_mapping.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_sentinels.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_sparse.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 formulaic-0.6.2/tests/utils/test_stateful_transforms.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 formulaic-0.6.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 formulaic-0.6.2/LICENSE
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 formulaic-0.6.2/README.md
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 formulaic-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 formulaic-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 formulaic-0.6.3/benchmarks/README.md
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 formulaic-0.6.3/benchmarks/benchmark.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 formulaic-0.6.3/benchmarks/benchmarks.csv
+-rw-r--r--   0        0        0    34436 2020-02-02 00:00:00.000000 formulaic-0.6.3/benchmarks/benchmarks.png
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 formulaic-0.6.3/benchmarks/plot.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 formulaic-0.6.3/benchmarks/requirements.txt
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/mkdocs.yml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/requirements.in
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/requirements.txt
+-rw-r--r--   0        0        0    17079 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/changelog.md
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/formulas.md
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/index.md
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/installation.md
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/migration.md
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/assets/images/logo.png
+-rw-r--r--   0        0        0    42441 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0    43761 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/assets/images/logo_with_text.png
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/concepts/index.md
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/dev/index.md
+-rw-r--r--   0        0        0    46448 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/contrasts.ipynb
+-rw-r--r--   0        0        0    29663 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/formulae.ipynb
+-rw-r--r--   0        0        0     9850 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/grammar.md
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/index.md
+-rw-r--r--   0        0        0    14831 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/integration.ipynb
+-rw-r--r--   0        0        0    27554 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/model_specs.ipynb
+-rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/quickstart.ipynb
+-rw-r--r--   0        0        0   162005 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/splines.ipynb
+-rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 formulaic-0.6.3/docsite/docs/guides/transforms.ipynb
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/_version.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/errors.py
+-rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/formula.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/model_matrix.py
+-rw-r--r--   0        0        0    15924 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/model_spec.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/sugar.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/__init__.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/arrow.py
+-rw-r--r--   0        0        0    32051 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/base.py
+-rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/pandas.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/types/__init__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/types/enums.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/types/evaluated_factor.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/types/factor_values.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/types/scoped_factor.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/materializers/types/scoped_term.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/__init__.py
+-rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/parser.py
+-rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/utils.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/algos/__init__.py
+-rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/algos/tokenize.py
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/algos/tokens_to_ast.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/__init__.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/ast_node.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/factor.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/formula_parser.py
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/operator.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/operator_resolver.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/ordered_set.py
+-rw-r--r--   0        0        0    17126 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/structured.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/term.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/parser/types/token.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/transforms/__init__.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/transforms/basis_spline.py
+-rw-r--r--   0        0        0    26786 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/transforms/contrasts.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/transforms/identity.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/transforms/patsy_compat.py
+-rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/transforms/poly.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/transforms/scale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/__init__.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/calculus.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/cast.py
+-rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/constraints.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/context.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/iterators.py
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/layered_mapping.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/sentinels.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/sparse.py
+-rw-r--r--   0        0        0    10122 2020-02-02 00:00:00.000000 formulaic-0.6.3/formulaic/utils/stateful_transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/__init__.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/test_formula.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/test_model_matrix.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/test_model_spec.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/test_sugar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/__init__.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/test_arrow.py
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/test_base.py
+-rw-r--r--   0        0        0    15530 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/test_pandas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/types/__init__.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/types/test_evaluated_factor.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/types/test_factor_values.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/types/test_scoped_factor.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/materializers/types/test_scoped_term.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/__init__.py
+-rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/test_parser.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/algos/__init__.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/algos/test_tokenize.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/algos/test_tokens_to_ast.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/__init__.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_ast_node.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_factor.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_formula_parser.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_operator.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_operator_resolver.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_ordered_set.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_structured.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_term.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/parser/types/test_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/transforms/__init__.py
+-rw-r--r--   0        0        0    12756 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/transforms/test_basis_spline.py
+-rw-r--r--   0        0        0    29890 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/transforms/test_contrasts.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/transforms/test_identity.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/transforms/test_patsy_compat.py
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/transforms/test_poly.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/transforms/test_scale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/__init__.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_calculus.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_capture_context.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_cast.py
+-rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_constraints.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_iterators.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_layered_mapping.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_sentinels.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_sparse.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 formulaic-0.6.3/tests/utils/test_stateful_transforms.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 formulaic-0.6.3/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 formulaic-0.6.3/LICENSE
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 formulaic-0.6.3/README.md
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 formulaic-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 formulaic-0.6.3/PKG-INFO
```

### Comparing `formulaic-0.6.2/benchmarks/README.md` & `formulaic-0.6.3/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/benchmarks/benchmark.py` & `formulaic-0.6.3/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/benchmarks/benchmarks.csv` & `formulaic-0.6.3/benchmarks/benchmarks.csv`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/benchmarks/benchmarks.png` & `formulaic-0.6.3/benchmarks/benchmarks.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/benchmarks/plot.py` & `formulaic-0.6.3/benchmarks/plot.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/mkdocs.yml` & `formulaic-0.6.3/docsite/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/requirements.txt` & `formulaic-0.6.3/docsite/requirements.txt`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/changelog.md` & `formulaic-0.6.3/docsite/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 For changes since the latest tagged release, please refer to the
 [git commit log](https://github.com/matthewwardrop/formulaic/commits/main).
 
 ---
 
+## 0.6.3 (26 June 2023)
+
+This is a minor release with a bugfix.
+
+**Bugfixes and cleanups:**
+
+* Fixed a regression introduced in the previous release when materializing
+  categorical encodings of variables with no levels.
+
 ## 0.6.2 (22 June 2023)
 
 This is a minor release with several bugfixes.
 
 **Bugfixes and cleanups:**
 
 * Fixed issues handling empty data sets in formulae that used categorical
   encoding.
-* Added the MIT license to distribution classifiers.ss
+* Added the MIT license to distribution classifiers.
 
 ## 0.6.1 (2 May 2023)
 
 This is a minor release with one new feature.
 
 **New features and enhancements:**
```

### Comparing `formulaic-0.6.2/docsite/docs/formulas.md` & `formulaic-0.6.3/docsite/docs/formulas.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/index.md` & `formulaic-0.6.3/docsite/docs/index.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/installation.md` & `formulaic-0.6.3/docsite/docs/installation.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/migration.md` & `formulaic-0.6.3/docsite/docs/migration.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/assets/images/favicon.png` & `formulaic-0.6.3/docsite/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/assets/images/logo.png` & `formulaic-0.6.3/docsite/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/assets/images/logo.svg` & `formulaic-0.6.3/docsite/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/assets/images/logo_with_text.png` & `formulaic-0.6.3/docsite/docs/assets/images/logo_with_text.png`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/concepts/index.md` & `formulaic-0.6.3/docsite/docs/concepts/index.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/guides/contrasts.ipynb` & `formulaic-0.6.3/docsite/docs/guides/contrasts.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/guides/formulae.ipynb` & `formulaic-0.6.3/docsite/docs/guides/formulae.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/guides/grammar.md` & `formulaic-0.6.3/docsite/docs/guides/grammar.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/guides/integration.ipynb` & `formulaic-0.6.3/docsite/docs/guides/integration.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/guides/model_specs.ipynb` & `formulaic-0.6.3/docsite/docs/guides/model_specs.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/guides/quickstart.ipynb` & `formulaic-0.6.3/docsite/docs/guides/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/guides/splines.ipynb` & `formulaic-0.6.3/docsite/docs/guides/splines.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/docsite/docs/guides/transforms.ipynb` & `formulaic-0.6.3/docsite/docs/guides/transforms.ipynb`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/__init__.py` & `formulaic-0.6.3/formulaic/__init__.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/errors.py` & `formulaic-0.6.3/formulaic/errors.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/formula.py` & `formulaic-0.6.3/formulaic/formula.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/model_matrix.py` & `formulaic-0.6.3/formulaic/model_matrix.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/model_spec.py` & `formulaic-0.6.3/formulaic/model_spec.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/sugar.py` & `formulaic-0.6.3/formulaic/sugar.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/materializers/arrow.py` & `formulaic-0.6.3/formulaic/materializers/arrow.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/materializers/base.py` & `formulaic-0.6.3/formulaic/materializers/base.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/materializers/pandas.py` & `formulaic-0.6.3/formulaic/materializers/pandas.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/materializers/types/evaluated_factor.py` & `formulaic-0.6.3/formulaic/materializers/types/evaluated_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/materializers/types/factor_values.py` & `formulaic-0.6.3/formulaic/materializers/types/factor_values.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/materializers/types/scoped_factor.py` & `formulaic-0.6.3/formulaic/materializers/types/scoped_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/materializers/types/scoped_term.py` & `formulaic-0.6.3/formulaic/materializers/types/scoped_term.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/parser/parser.py` & `formulaic-0.6.3/formulaic/parser/parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/parser/utils.py` & `formulaic-0.6.3/formulaic/parser/utils.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/parser/algos/tokenize.py` & `formulaic-0.6.3/formulaic/parser/algos/tokenize.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/parser/algos/tokens_to_ast.py` & `formulaic-0.6.3/formulaic/parser/algos/tokens_to_ast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/parser/types/ast_node.py` & `formulaic-0.6.3/formulaic/parser/types/ast_node.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/parser/types/factor.py` & `formulaic-0.6.3/formulaic/parser/types/factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/parser/types/formula_parser.py` & `formulaic-0.6.3/formulaic/parser/types/formula_parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/parser/types/operator.py` & `formulaic-0.6.3/formulaic/parser/types/operator.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/parser/types/operator_resolver.py` & `formulaic-0.6.3/formulaic/parser/types/operator_resolver.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/parser/types/ordered_set.py` & `formulaic-0.6.3/formulaic/parser/types/ordered_set.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/parser/types/structured.py` & `formulaic-0.6.3/formulaic/parser/types/structured.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/parser/types/term.py` & `formulaic-0.6.3/formulaic/parser/types/term.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/parser/types/token.py` & `formulaic-0.6.3/formulaic/parser/types/token.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/transforms/__init__.py` & `formulaic-0.6.3/formulaic/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/transforms/basis_spline.py` & `formulaic-0.6.3/formulaic/transforms/basis_spline.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/transforms/contrasts.py` & `formulaic-0.6.3/formulaic/transforms/contrasts.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,19 +202,35 @@
             raise ValueError(
                 "Output type for contrasts must be one of: 'pandas', 'numpy' or 'sparse'."
             )
 
         # Short-circuit when we know the output encoding will be empty
         if not levels or len(levels) == 1 and reduced_rank:
             if output == "pandas":
-                return pandas.DataFrame()
-            if output == "numpy":
-                return numpy.ones((dummies.shape[0], 0))
-            if output == "sparse":
-                return spsparse.csc_matrix((dummies.shape[0], 0))
+                encoded = pandas.DataFrame(
+                    index=dummies.index
+                    if isinstance(dummies, pandas.DataFrame)
+                    else range(dummies.shape[0])
+                )
+            elif output == "numpy":
+                encoded = numpy.ones((dummies.shape[0], 0))
+            elif output == "sparse":
+                encoded = spsparse.csc_matrix((dummies.shape[0], 0))
+            else:  # pragma: no cover
+                raise ValueError(
+                    "Short-circuiting is only implemented for output types: 'pandas', 'numpy' or 'sparse'."
+                )
+            return FactorValues(
+                encoded,
+                kind="categorical",
+                column_names=[],
+                spans_intercept=False,
+                format=self.get_factor_format(levels, reduced_rank=reduced_rank),
+                encoded=True,
+            )
 
         sparse = output == "sparse"
         encoded = self._apply(
             dummies, levels=levels, reduced_rank=reduced_rank, sparse=sparse
         )
         coding_column_names = self.get_coding_column_names(
             levels, reduced_rank=reduced_rank
@@ -354,15 +370,15 @@
         """
         Determine whether the encoded contrasts span the intercept.
 
         Args:
             levels: The names of the levels/categories in the data.
             reduced_rank: Whether the contrast encoding used had reduced rank.
         """
-        return not reduced_rank
+        return len(levels) > 0 and not reduced_rank
 
     def get_drop_field(self, levels, reduced_rank=True) -> Union[int, str]:
         """
         Determine which column to drop to be full rank after this encoding.
         If this contrast encoding is already reduced in rank, then this method
         should return `None`.
```

### Comparing `formulaic-0.6.2/formulaic/transforms/patsy_compat.py` & `formulaic-0.6.3/formulaic/transforms/patsy_compat.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/transforms/poly.py` & `formulaic-0.6.3/formulaic/transforms/poly.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/transforms/scale.py` & `formulaic-0.6.3/formulaic/transforms/scale.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/utils/calculus.py` & `formulaic-0.6.3/formulaic/utils/calculus.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/utils/cast.py` & `formulaic-0.6.3/formulaic/utils/cast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/utils/constraints.py` & `formulaic-0.6.3/formulaic/utils/constraints.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/utils/context.py` & `formulaic-0.6.3/formulaic/utils/context.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/utils/iterators.py` & `formulaic-0.6.3/formulaic/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/utils/layered_mapping.py` & `formulaic-0.6.3/formulaic/utils/layered_mapping.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/utils/sparse.py` & `formulaic-0.6.3/formulaic/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/formulaic/utils/stateful_transforms.py` & `formulaic-0.6.3/formulaic/utils/stateful_transforms.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/test_formula.py` & `formulaic-0.6.3/tests/test_formula.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/test_model_matrix.py` & `formulaic-0.6.3/tests/test_model_matrix.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/test_model_spec.py` & `formulaic-0.6.3/tests/test_model_spec.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/test_sugar.py` & `formulaic-0.6.3/tests/test_sugar.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/materializers/test_arrow.py` & `formulaic-0.6.3/tests/materializers/test_arrow.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/materializers/test_base.py` & `formulaic-0.6.3/tests/materializers/test_base.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/materializers/test_pandas.py` & `formulaic-0.6.3/tests/materializers/test_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,21 @@
 }
 
 
 class TestPandasMaterializer:
     @pytest.fixture
     def data(self):
         return pandas.DataFrame(
-            {"a": [1, 2, 3], "b": [1, 2, 3], "A": ["a", "b", "c"], "B": ["a", "b", "c"]}
+            {
+                "a": [1, 2, 3],
+                "b": [1, 2, 3],
+                "A": ["a", "b", "c"],
+                "B": ["a", "b", "c"],
+                "D": ["a", "a", "a"],
+            }
         )
 
     @pytest.fixture
     def data_with_nulls(self):
         return pandas.DataFrame(
             {"a": [1, 2, None], "A": ["a", None, "c"], "B": ["a", "b", None]}
         )
@@ -401,7 +407,25 @@
         o = BytesIO()
         ms = materializer.get_model_matrix("a ~ a:A")
         pickle.dump(ms.model_spec, o)
         o.seek(0)
         ms2 = pickle.load(o)
         assert isinstance(ms, Structured)
         assert ms2.lhs.formula.root == ["a"]
+
+    def test_no_levels_encoding(self, data):
+        mm = PandasMaterializer(data, output="pandas").get_model_matrix("a + D")
+
+        assert mm.model_spec.column_names == ("Intercept", "a")
+        assert mm.shape == (3, 2)
+
+        print(mm)
+
+        mm = PandasMaterializer(data, output="sparse").get_model_matrix("a + D")
+
+        assert mm.model_spec.column_names == ("Intercept", "a")
+        assert mm.shape == (3, 2)
+
+        mm = PandasMaterializer(data, output="numpy").get_model_matrix("a + D")
+
+        assert mm.model_spec.column_names == ("Intercept", "a")
+        assert mm.shape == (3, 2)
```

### Comparing `formulaic-0.6.2/tests/materializers/types/test_evaluated_factor.py` & `formulaic-0.6.3/tests/materializers/types/test_evaluated_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/materializers/types/test_scoped_factor.py` & `formulaic-0.6.3/tests/materializers/types/test_scoped_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/materializers/types/test_scoped_term.py` & `formulaic-0.6.3/tests/materializers/types/test_scoped_term.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/parser/test_parser.py` & `formulaic-0.6.3/tests/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/parser/test_utils.py` & `formulaic-0.6.3/tests/parser/test_utils.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/parser/algos/test_tokenize.py` & `formulaic-0.6.3/tests/parser/algos/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/parser/algos/test_tokens_to_ast.py` & `formulaic-0.6.3/tests/parser/algos/test_tokens_to_ast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/parser/types/test_ast_node.py` & `formulaic-0.6.3/tests/parser/types/test_ast_node.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/parser/types/test_factor.py` & `formulaic-0.6.3/tests/parser/types/test_factor.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/parser/types/test_formula_parser.py` & `formulaic-0.6.3/tests/parser/types/test_formula_parser.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/parser/types/test_operator.py` & `formulaic-0.6.3/tests/parser/types/test_operator.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/parser/types/test_operator_resolver.py` & `formulaic-0.6.3/tests/parser/types/test_operator_resolver.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/parser/types/test_structured.py` & `formulaic-0.6.3/tests/parser/types/test_structured.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/parser/types/test_term.py` & `formulaic-0.6.3/tests/parser/types/test_term.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/parser/types/test_token.py` & `formulaic-0.6.3/tests/parser/types/test_token.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/transforms/test_basis_spline.py` & `formulaic-0.6.3/tests/transforms/test_basis_spline.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/transforms/test_contrasts.py` & `formulaic-0.6.3/tests/transforms/test_contrasts.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
             reduced_rank=True,
         )
         assert empty_numpy_reduced.shape == (6, 0)
 
         empty_pandas = encode_contrasts(
             data=["a", "b", "c", "a", "b", "c"], levels=[], output="pandas"
         )
-        assert empty_pandas.shape == (0, 0)
+        assert empty_pandas.shape == (6, 0)
 
         empty_sparse = encode_contrasts(
             data=["a", "b", "c", "a", "b", "c"], levels=[], output="sparse"
         )
         assert empty_sparse.shape == (6, 0)
```

### Comparing `formulaic-0.6.2/tests/transforms/test_patsy_compat.py` & `formulaic-0.6.3/tests/transforms/test_patsy_compat.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/transforms/test_poly.py` & `formulaic-0.6.3/tests/transforms/test_poly.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/transforms/test_scale.py` & `formulaic-0.6.3/tests/transforms/test_scale.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/utils/test_calculus.py` & `formulaic-0.6.3/tests/utils/test_calculus.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/utils/test_cast.py` & `formulaic-0.6.3/tests/utils/test_cast.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/utils/test_constraints.py` & `formulaic-0.6.3/tests/utils/test_constraints.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/utils/test_layered_mapping.py` & `formulaic-0.6.3/tests/utils/test_layered_mapping.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/utils/test_sparse.py` & `formulaic-0.6.3/tests/utils/test_sparse.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/tests/utils/test_stateful_transforms.py` & `formulaic-0.6.3/tests/utils/test_stateful_transforms.py`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/.gitignore` & `formulaic-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/LICENSE` & `formulaic-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/README.md` & `formulaic-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/pyproject.toml` & `formulaic-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `formulaic-0.6.2/PKG-INFO` & `formulaic-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formulaic
-Version: 0.6.2
+Version: 0.6.3
 Summary: An implementation of Wilkinson formulas.
 Project-URL: repository, https://github.com/matthewwardrop/formulaic
 Project-URL: documentation, https://matthewwardrop.github.io/formulaic
 Author-email: Matthew Wardrop <mpwardrop@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

