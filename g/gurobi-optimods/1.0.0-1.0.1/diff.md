# Comparing `tmp/gurobi_optimods-1.0.0.tar.gz` & `tmp/gurobi_optimods-1.0.1.tar.gz`

## Comparing `gurobi_optimods-1.0.0.tar` & `gurobi_optimods-1.0.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/Makefile
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tox.ini
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/pull_request_template.md
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/ISSUE_TEMPLATE/new_mod.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/code-quality.yml
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/doc-build.yml
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/doc-tests.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/python-tests.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/wheel-tests.yml
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/make.bat
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/requirements.txt
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/adding.rst
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/api.rst
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/conf.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/contact.rst
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/contributing.rst
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/dev-reference.rst
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/gallery.rst
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/index.rst
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/installation.rst
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/license.rst
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/usage.rst
--rw-r--r--   0        0        0     8668 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/bipartite-matching.rst
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/lad-regression.rst
--rw-r--r--   0        0        0     9904 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/min-cost-flow.rst
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/mwis.rst
--rw-r--r--   0        0        0    27733 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/portfolio.rst
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/qubo.rst
--rw-r--r--   0        0        0    15329 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/workforce.rst
--rw-r--r--   0        0        0    34323 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-example.png
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-figs.py
--rw-r--r--   0        0        0    34001 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-flow.png
--rw-r--r--   0        0        0    33714 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-result.png
--rw-r--r--   0        0        0    21501 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/lad-outlier-coeffs.png
--rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/lad-outlier-errors.png
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/lad-regression-coeffs.png
--rw-r--r--   0        0        0   540595 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/min-cost-flow-result.png
--rw-r--r--   0        0        0    26538 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/mvp.png
--rw-r--r--   0        0        0    38322 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/mwis.png
--rw-r--r--   0        0        0    16645 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/pie.png
--rw-r--r--   0        0        0    16684 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/qubo.png
--rw-r--r--   0        0        0   367978 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/shortest-path-result.png
--rw-r--r--   0        0        0    14540 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/icons/lad-regression.png
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/refs/graphs.bib
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/refs/portfolio.bib
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/refs/qubo.bib
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/refs/regression.bib
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/refs/workforce.bib
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/__init__.py
--rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/bipartite_matching.py
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/datasets.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/min_cost_flow.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/mwis.py
--rw-r--r--   0        0        0    15040 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/portfolio.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/qubo.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/regression.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/utils.py
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/workforce.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/data/graphs/simple_graph_edges.csv
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/data/graphs/simple_graph_nodes.csv
--rwxr-xr-x   0        0        0    41668 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/data/portfolio/portfolio.csv
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/data/workforce/preferences.csv
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/data/workforce/shift_requirements.csv
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/data/workforce/worker_limits.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0    11740 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_bipartite_matching.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_graph_utils.py
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_min_cost_flow.py
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_mwis.py
--rw-r--r--   0        0        0    32785 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_portfolio.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_qubo.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_regression.py
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_utils.py
--rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_workforce.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/utils.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/LICENSE
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/NOTICE
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/README.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/Makefile
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tox.ini
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/pull_request_template.md
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/ISSUE_TEMPLATE/new_mod.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/code-quality.yml
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/doc-build.yml
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/doc-tests.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/python-tests.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/wheel-tests.yml
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/requirements.txt
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/adding.rst
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/api.rst
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/conf.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/contact.rst
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/contributing.rst
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/dev-reference.rst
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/gallery.rst
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/index.rst
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/installation.rst
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/license.rst
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/usage.rst
+-rw-r--r--   0        0        0     8805 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/bipartite-matching.rst
+-rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/lad-regression.rst
+-rw-r--r--   0        0        0     9930 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/min-cost-flow.rst
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/mwis.rst
+-rw-r--r--   0        0        0    27741 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/portfolio.rst
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/qubo.rst
+-rw-r--r--   0        0        0    15439 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/workforce.rst
+-rw-r--r--   0        0        0    34323 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-example.png
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-figs.py
+-rw-r--r--   0        0        0    34001 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-flow.png
+-rw-r--r--   0        0        0    33714 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-result.png
+-rw-r--r--   0        0        0    21501 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/lad-outlier-coeffs.png
+-rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/lad-outlier-errors.png
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/lad-regression-coeffs.png
+-rw-r--r--   0        0        0   540595 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/min-cost-flow-result.png
+-rw-r--r--   0        0        0    26538 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/mvp.png
+-rw-r--r--   0        0        0    38322 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/mwis.png
+-rw-r--r--   0        0        0    16645 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/pie.png
+-rw-r--r--   0        0        0    16684 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/qubo.png
+-rw-r--r--   0        0        0   367978 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/shortest-path-result.png
+-rw-r--r--   0        0        0    14540 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/icons/lad-regression.png
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/refs/graphs.bib
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/refs/portfolio.bib
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/refs/qubo.bib
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/refs/regression.bib
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/refs/workforce.bib
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/__init__.py
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/bipartite_matching.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/datasets.py
+-rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/min_cost_flow.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/mwis.py
+-rw-r--r--   0        0        0    15040 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/portfolio.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/qubo.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/regression.py
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/utils.py
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/workforce.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/data/graphs/simple_graph_edges.csv
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/data/graphs/simple_graph_nodes.csv
+-rwxr-xr-x   0        0        0    41668 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/data/portfolio/portfolio.csv
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/data/workforce/preferences.csv
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/data/workforce/shift_requirements.csv
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/data/workforce/worker_limits.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0    11740 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_bipartite_matching.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_graph_utils.py
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_min_cost_flow.py
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_mwis.py
+-rw-r--r--   0        0        0    32785 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_portfolio.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_qubo.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_regression.py
+-rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_utils.py
+-rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_workforce.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/utils.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/LICENSE
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/NOTICE
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/README.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/PKG-INFO
```

### Comparing `gurobi_optimods-1.0.0/CODE_OF_CONDUCT.md` & `gurobi_optimods-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/.github/pull_request_template.md` & `gurobi_optimods-1.0.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/.github/ISSUE_TEMPLATE/new_mod.md` & `gurobi_optimods-1.0.1/.github/ISSUE_TEMPLATE/new_mod.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/.github/workflows/code-quality.yml` & `gurobi_optimods-1.0.1/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/.github/workflows/doc-build.yml` & `gurobi_optimods-1.0.1/.github/workflows/doc-build.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/.github/workflows/doc-tests.yml` & `gurobi_optimods-1.0.1/.github/workflows/doc-tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,25 @@
 jobs:
   doc-tests:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python: ["3.8"]
-        gurobipy: ["10.0.1"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
       - name: Install tooling
         run: |
           python -m pip install --upgrade pip
       - name: Install dependencies
         run: |
           python -m pip install -rdocs/requirements.txt
-          python -m pip install .[examples] gurobipy==${{ matrix.gurobipy }}
+          python -m pip install .[examples]
       - name: Run doctests
         run: |
           cd docs
           make doctest
```

### Comparing `gurobi_optimods-1.0.0/.github/workflows/publish-pypi.yml` & `gurobi_optimods-1.0.1/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/.github/workflows/python-tests.yml` & `gurobi_optimods-1.0.1/.github/workflows/python-tests.yml`

 * *Files 9% similar despite different names*

```diff
@@ -11,27 +11,26 @@
 jobs:
   python-tests:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python: ["3.8"]
-        gurobipy: ["10.0.1"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
       - name: Install tooling
         run: |
           python -m pip install --upgrade pip
       - name: Install dependencies
         run: |
-          python -m pip install . gurobipy==${{ matrix.gurobipy }}
+          python -m pip install .
       - name: Run unittest
         run: python -m unittest discover -b
       - name: Install networkx (optional dependency)
         run: python -m pip install networkx
       - name: Run additional tests
         run: python -m unittest discover -b
```

### Comparing `gurobi_optimods-1.0.0/.github/workflows/release.yml` & `gurobi_optimods-1.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/.github/workflows/wheel-tests.yml` & `gurobi_optimods-1.0.1/.github/workflows/wheel-tests.yml`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
     runs-on: ${{ matrix.os }}
 
     strategy:
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
         python: ["3.8", "3.9", "3.10", "3.11"]
-        gurobipy: ["10.0.1"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
@@ -31,15 +30,15 @@
         run: |
           python -m pip install --upgrade pip build
       - name: Build wheel
         run: |
           python -m build
       - name: Fetch dependencies for offline install
         run: |
-          pip wheel --wheel-dir=dist gurobipy==${{ matrix.gurobipy }} pandas numpy scipy gurobipy-pandas
+          pip wheel --wheel-dir=dist gurobipy pandas numpy scipy gurobipy-pandas
       - name: Install from built wheel
         run: |
           python -m pip install --find-links dist --no-index --only-binary=:all: gurobi-optimods
       - name: Test import
         run: |
           python -c "import gurobi_optimods"
       - name: Run unit tests
```

### Comparing `gurobi_optimods-1.0.0/docs/Makefile` & `gurobi_optimods-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/make.bat` & `gurobi_optimods-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/adding.rst` & `gurobi_optimods-1.0.1/docs/source/adding.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 ================
 
 The goal of the OptiMods is to create and maintain an open-source Python
 repository of implemented optimization use cases. Each use case will have clear,
 informative, and pretty documentation that explains both how to use it and the
 mathematical model behind it for interested readers.
 
-We hope to grow the collection of mods over time, and welcome your
-contributions. This page outlines what makes a good mod, and what you will need
+We hope to grow the collection of Mods over time, and welcome your
+contributions. This page outlines what makes a good Mod, and what you will need
 to consider when developing your contribution.
 
 Proposing a new Mod
 -------------------
 
-To propose a new mod, create an issue in our repository using the 'New Mod
+To propose a new Mod, create an issue in our repository using the 'New Mod
 Proposal' template to gather the required details. One of the maintainers will
 reach out to you on the issue to discuss the proposed topic and design.
 
 A good Mod:
 
 - solves well-known, well-defined problem from a non-optimization field;
-- has a simple interface which shields the user from interacting with gurobipy
+- has a simple interface that shields the user from interacting with gurobipy
   directly;
 - is self-contained, and follows a clean data-in data-out style leaning on
   standard packages from the python ecosystem (``numpy``, ``scipy``, and
   ``pandas`` are our first-class citizens);
-- is accompanied by clear documentation which provides background information
+- is accompanied by clear documentation that provides background information
   for the topic and a formal statement of the problem in the domain language of
   the target user; and
-- includes runnable examples codes and presentation of results in the
+- includes runnable example codes and presentation of results in the
   documentation so users can hit the ground running.
 
 Starting work on a Mod
 ----------------------
 
 First, carefully read :doc:`contributing` for details on coding standards, and
 how to get set up to work on the project. Set up your development environment as
@@ -45,27 +45,27 @@
 prepare your submission.
 
 Implementation and tests
 ------------------------
 
 Create ``src/gurobi_optimods/<mod>.py`` where your implementation will live, and
 ``tests/test_<mod>.py`` where your unit tests will live. A basic implementation
-of a mod takes this form::
+of a Mod takes this form::
 
     import logging
 
     import gurobipy as gp
 
     from gurobi_optimods.utils import optimod
 
     logger = logging.getLogger(__name__)
 
     @optimod()
     def my_mod(data, *, create_env):
-        """An optimod which solves an important problem
+        """An optimod that solves an important problem
 
         :param data: Description of argument
         :type data: Type of argument
 
         ... describe additional arguments ...
 
         :return: Description of returned result
@@ -81,42 +81,42 @@
             model.optimize()
 
             # ... Extract and post-process the solution ...
 
             return solution
 
 Mods should be stateless with respect to ``gurobipy`` objects. This means Gurobi
-environments and models are created within a mod function, and closed before the
+environments and models are created within a Mod function, and closed before the
 function returns using context managers. Gurobi environments should be created
-by calling ``create_env``. This function is provided to your mod by the
+by calling ``create_env``. This function is provided to your Mod by the
 ``@optimod()`` decorator and supplies some necessary parameters to Gurobi to
-handle console output and log files consistently across mods. The standard
+handle console output and log files consistently across Mods. The standard
 parameters ``verbose`` and ``logfile`` are also handled by the decorator and will
 be included automatically in the API documentation.
 
-If your mod needs to produce any output, use the in-built python logging call
+If your Mod needs to produce any output, use the built-in python logging call
 ``logger.info``.
 
-You should also include your mod in the :doc:`api` by adding appropriate
+You should also include your Mod in the :doc:`api` by adding appropriate
 `autodoc <https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html>`_
 references to ``docs/source/api.rst``.
 
 Preparing documentation
 -----------------------
 
-Create ``docs/source/mods/<mod>.rst`` as the documentation page for your mod. As
-each mod is different, there is no specific template for this, but please use
-the existing mod pages as a guide.
+Create ``docs/source/mods/<mod>.rst`` as the documentation page for your Mod. As
+each Mod is different, there is no specific template for this, but please use
+the existing Mod pages as a guide.
 
 A reference to your page must also be added to ``docs/source/gallery.rst`` to
 include it in the gallery page and toctree when the documentation is built. You
-should also add an icon to the gallery card for your mod.
+should also add an icon to the gallery card for your Mod.
 
 Your documentation page must contain example codes that new users can
-immediately used, with presentation of the results included in the documentation
+immediately use, with presentation of the results included in the documentation
 page.
 
 The implementation of the Mod (description of the mathematical model or
 algorithms used) should be hidden from the user at first glance. We use the ``..
 dropdown:`` directive for this. Any mathematical and algorithmic details should
 be placed in a dropdown and clearly indicate that this is advanced detail the
 user does not need to fully understand in order to use the Mod.
@@ -125,21 +125,21 @@
 ------------------
 
 Some of your examples may rely on datasets. These can be packaged with the
 optimods to enable users to quickly reproduce the examples in your documentation.
 
 - Any data files should live under a subdirectory
   ``src/gurobi_optimods/data/<mod-name>`` to reduce clutter.
-- The ``gurobi_optimods.datasets`` module should implement a function which
+- The ``gurobi_optimods.datasets`` module should implement a function that
   fetches the dataset.
 
 Submitting a pull request
 -------------------------
 
 You can submit your pull request at any time in draft mode so the maintainers
-are aware your mod is actively being worked on. This should be a pull request
+are aware your Mod is actively being worked on. This should be a pull request
 from a branch on your fork into ``gurobi-optimods/main``. Pull requests include
-a checklist of features to ensure your mod is correctly included in the Python
+a checklist of features to ensure your Mod is correctly included in the Python
 package and the built documentation.
 
-When your mod is ready for review, take your PR out of draft mode and request a
+When your Mod is ready for review, take your PR out of draft mode and request a
 review.
```

### Comparing `gurobi_optimods-1.0.0/docs/source/api.rst` & `gurobi_optimods-1.0.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/conf.py` & `gurobi_optimods-1.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/contributing.rst` & `gurobi_optimods-1.0.1/docs/source/contributing.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Contributing to OptiMods
 ========================
 
-We welcome contributions from the commumnity: bug fixes, doc corrections,
+We welcome contributions from the community: bug fixes, doc corrections,
 extensions to existing Mods, or development of new Mods. This page describes
 conventions to follow when contributing, and the development process we follow
 for the project, which is applicable to all contributors. For guidelines on
 proposing and implementing new Mods, see :doc:`adding`.
 
 Coding Standards
 ----------------
@@ -32,34 +32,34 @@
 snippets provided in the documentation work as expected.
 
 Documentation
 -------------
 
 Documentation is a core part of the OptiMods project. All Mods must be
 accompanied by a documentation page explaining their use and providing
-appropriate background information. If new mod features are added, the
+appropriate background information. If new Mod features are added, the
 documentation must reflect the changes.
 
 Development Environment
 -----------------------
 
 To set up your development environment:
 
 1. Create and activate a Python 3.8 virtual environment using your preferred
    tool. We maintain compatibility with Python 3.8 and above, so developing
    using 3.8 locally will ensure your contributions are compatible.
-2. Run ``make develop`` from the top-level of the repository. This command will
+2. Run ``make develop`` from the top level of the repository. This command will
    install (using ``pip``) all packages required to run the unit tests, run the
    doc tests, and build the sphinx documentation. It will also install
    pre-commit hooks to enforce coding standards.
 
 To run the tests:
 
 1. Activate your virtual environment.
-2. Run ``make test``. This command will run the unit tests of all mod
+2. Run ``make test``. This command will run the unit tests of all Mod
    implementations, and the doctests for examples in the documentation.
 
 To build and view the docs:
 
 1. Activate your virtual environment and change to the ``docs`` directory.
 2. Run ``make livehtml``. This command will build the docs and open up a browser
    window at the index page.
@@ -71,9 +71,9 @@
 ------------------
 
 We use issues and pull requests to manage and review contributions.
 
 - Minor doc fixes can be submitted directly as pull requests.
 - Bugs should first be reported as issues before submitting a pull request to
   fix them. Use the 'Bug report' issue template.
-- New Mod proposals should first be submitted as issues for discussion, see
+- New Mod proposals should first be submitted as issues for discussion; see
   :doc:`adding` for further details.
```

### Comparing `gurobi_optimods-1.0.0/docs/source/dev-reference.rst` & `gurobi_optimods-1.0.1/docs/source/dev-reference.rst`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This page contains further information on the tools/packages we use, to guide
 developers who are working on mods.
 
 The ``@optimod`` decorator
 --------------------------
 
-The ``@optimod`` decorator should be added to any Mod functions which need to
+The ``@optimod`` decorator should be added to any Mod functions that need to
 create Gurobi models. :doc:`adding` provides a template for how to apply the
 decorator. The decorator provides the following arguments automatically:
 
 * ``verbose``, enabling users to shut off output;
 * ``logfile``, enabling users to send Mod logs to a file; and
 * ``solver_params``, enabling users to pass a dictionary of parameters to the
   Gurobi Optimizer.
```

### Comparing `gurobi_optimods-1.0.0/docs/source/gallery.rst` & `gurobi_optimods-1.0.1/docs/source/gallery.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/index.rst` & `gurobi_optimods-1.0.1/docs/source/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 **Gurobi OptiMods**: nice APIs for common optimization tasks.
 
 ``gurobi-optimods`` is an open-source Python repository of implemented
 optimization use cases using Gurobi, each with clear, informative, and pretty
 documentation that explains how to use it and the mathematical model behind it.
 
 The package is a collection of independent 'Mods'. Each Mod is intended to be
-immediately applicable to real use-cases. However, we expect that for many
+immediately applicable to real use cases. However, we expect that for many
 practical applications users will need to understand and extend the
-implementation of a Mod to tailor it to their use-case. Read the :doc:`usage`
-section first for an overview of the design and use-case for the OptiMods.
+implementation of a Mod to tailor it to their use case. Read the :doc:`usage`
+section first for an overview of the design and use case for the OptiMods.
 
 Check out :doc:`gallery` for a quick overview of the current set of implemented
-Mods. We welcome contributions of new Mods based on use-cases you are interested
+Mods. We welcome contributions of new Mods based on use cases you are interested
 in, as well as fixes and improvements to existing Mods. See :doc:`contributing`
 and :doc:`adding` for more information on how to get involved in the project.
 
 **Please note**: while this project is open source, the ``gurobipy`` library
-which it depends on is commercial software and requires a license. See
+that it depends on is commercial software and requires a license. See
 :doc:`license` for further details.
 
 .. toctree::
    :maxdepth: 1
    :caption: Start
    :hidden:
```

### Comparing `gurobi_optimods-1.0.0/docs/source/installation.rst` & `gurobi_optimods-1.0.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/license.rst` & `gurobi_optimods-1.0.1/docs/source/license.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 License
 =======
 
 ``gurobi-optimods`` is distributed under the `Apache License 2.0
 <https://www.apache.org/licenses/LICENSE-2.0.txt>`_, meaning you can use, read,
 and modify the code freely within the license terms. However, it depends on a
-commercial package (gurobipy) which requires a license. When installed via pip
+commercial package (gurobipy) that requires a license. When installed via pip
 or conda, gurobipy ships with a :pypi:`limited trial license <gurobipy>` for the
-Gurobi Optimizer which handles models up to a certain size.
+Gurobi Optimizer that handles models up to a certain size.
 
 The example datasets in the documentation can all be solved using this trial
-license, however when using larger input datasets you may encounter the error
+license.  When using larger input datasets, you may encounter the error
 "Given data exceeds Gurobi trial license limits". To run the Mod successfully
 with your larger dataset, you will need a full license for Gurobi.
 
 - If you are a commercial user: please visit https://www.gurobi.com/free-trial/
   to request a full-featured Evaluation License which will allow you to use
   datasets of unrestricted size in the OptiMods.
 - If you are an academic user: Gurobi provides free licenses for faculty
```

### Comparing `gurobi_optimods-1.0.0/docs/source/usage.rst` & `gurobi_optimods-1.0.1/docs/source/usage.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Usage
 =====
 
 The best way to get started with the OptiMods is to try one out! Check out the
 :doc:`gallery` first to find a Mod that suits you. Each Mod comes complete with
-a page of explanatory documentation which provides background on the problem it
+a page of explanatory documentation that provides background on the problem it
 is intended to solve. The docs also include runnable example codes and datasets
 to help get you started.
 
 Note that you may need to install additional dependencies for some examples, as
-they use optional packages which are not direct dependencies of
-``gurobi-optimods``. The quick way to ensure you have a Python environment which
+they use optional packages that are not direct dependencies of
+``gurobi-optimods``. The quickest way to ensure you have a Python environment that
 can execute all the example snippets in the docs is to run the following::
 
    python -m pip install gurobi-optimods[examples]
 
-Each Mod is designed to be self-contained, with a clean data-in data-out API.
-Munge your data into the appropriate format using Python tools you already know,
-and run the Mod as outlined in its documentation page to get back a solution.
+Each Mod is designed to be self-contained, with a clean data-in, data-out API.
+To solve a problem, munge your data into the appropriate format using Python
+tools you already know, and run the Mod as outlined in its documentation page.
 
 The documentation pages also include details of the mathematical model
-underlying the Mod, should you be interested to learn more about the
+underlying the Mod, should you be interested in learning more about the
 implementation. These details are explained in sections marked "Background". It
 is not necessary to read and understand these sections in order to use the Mod
 effectively. You can also browse :ghsrc:`the Mod source <src/gurobi_optimods>`
 to find out how the mathematical models are implemented in code.
 
 Finally, we welcome contributions of new Mods, bug fixes and new features for
 existing Mods, and improvements to the documentation. This is intended to be a
 community project that grows over time to handle a wide range of optimization
-use-cases across many different fields. See :doc:`contributing` for more
+use cases across many different fields. See :doc:`contributing` for more
 details.
```

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/bipartite-matching.rst` & `gurobi_optimods-1.0.1/docs/source/mods/bipartite-matching.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,87 @@
 Maximum Bipartite Matching
 ==========================
 
 The maximum matching problem is a fundamental problem in graph theory. Given
-a graph, as a set of nodes connected to one another by edges, a matching
-is any subset of those edges which have no vertex in common. The goal of
-maximum matching is to find the largest possible such matching of a given
+a graph as a set of nodes connected by edges, a matching
+is any subset of those edges that have no vertex in common. The goal of
+maximum matching is to find the largest possible matching in a given
 graph.
 
-In this mod we consider the special case of maximum cardinality matching on
-bipartite graphs. This problem can be applied to solve exclusive assignment
-problems in practice, such as the assignment of workers or resources to tasks.
-To give a brief example, if we construct a bipartite graph where one of the
-bipartite sets represents tasks, and the other workers, then a matching is a
-set of edges each of which assigns one worker to one task. By the properties
-of a matching, each worker is assigned at most one task and each task is
-completed by at most one worker. The maximum cardinality matching is one which
-maximises the number of completed tasks (and workers given work).
+In this Mod we consider the special case of maximum cardinality matching on
+bipartite graphs. This theoretical problem can be used to solve practical
+problems such as the assignment of workers or resources to tasks. We
+construct a bipartite graph where one of the bipartite sets represents tasks,
+the other represents workers, and an edge exists between a given worker and task
+if the worker may complete that task. A matching then defines an allocation of
+workers to tasks, such that each worker is allocated to at most
+one task and each task is designated to be completed by at most one worker. The
+maximum cardinality matching maximizes the number of completed tasks and,
+consequently, the number of workers who are given work.
 
 .. Figure generated using networkx, see bipartite-matching-figs.py
 .. figure:: figures/bipartite-matching-example.png
     :width: 400
     :alt: Bipartite matching example
 
     A bipartite graph (left) and its maximum matching (right)
 
 Problem Specification
 ---------------------
 
 Consider a bipartite graph :math:`G(U, V, E)`, where :math:`U` and :math:`V`
 are disjoint vertex sets, and the edge set :math:`E \subseteq U \times V`
-joins only between, not within, the sets. A matching on this graph is any
-subset of edges such that no vertex is incident to more than one edge.
-Equivalently, the matching is a subgraph of :math:`G` where all vertices
+connects vertices between, but not within, the sets. A matching on this graph
+is any subset of edges such that no vertex is incident to more than one edge.
+Equivalently, a matching is a subgraph of :math:`G` where all vertices
 have degree at most one. A maximum matching is the largest possible matching
 on :math:`G`.
 
 .. dropdown:: Background: Mathematical Model
 
     The bipartite matching Mod is implemented by reducing the basic version of
     the problem to a minimum-cost flow problem. To do so, we introduce a source
     vertex as a predecessor to all vertices in :math:`U`, and a sink vertex as a
     successor to all vertices in :math:`V`. Giving every edge unit capacity, a
-    maximum matching is found by maximizing flow from the source to the sink. As
-    a min-cost flow, this is equivalent to adding an edge with a negative cost
-    from the sink to the source and assigning zero cost to all other edges. All
-    edges with non-zero flow in the min-cost flow solution are part of the
+    maximum matching is found by maximizing flow from the source to the sink. To
+    create a minimum-cost flow formulation, an edge with negative cost is added
+    from the sink and the source. All other edges are assigned zero cost. All
+    edges with non-zero flow in the minimum-cost flow solution are part of the
     matching.
 
     .. Figure generated using networkx, see bipartite-matching-figs.py
     .. figure:: figures/bipartite-matching-flow.png
         :width: 400
         :alt: Bipartite matching flow network
 
         A maximum flow network for the bipartite matching problem
 
-    We do not describe the mathematical formulation here, see :doc:`/mods/min-cost-flow`
-    for details. The important point to note is that when this continuous model is
-    solved using the simplex algorithm, we are guaranteed to get an integral solution
-    and thus the solution can be used to select a set of edges for the matching.
+    We do not describe the mathematical formulation here; for further details
+    refer to the :doc:`/mods/min-cost-flow` Mod. The important point to note
+    is that solving this continuous model with the simplex algorithm guarantees
+    an integral solution which can therefore be used to select a set of edges
+    for the matching.
 
 Interface
 ---------
 
 The ``maximum_bipartite_matching`` function supports scipy sparse arrays, pandas
 dataframes, and networkx graphs as possible inputs. The user must also provide
-the bipartite partitioning of the input graph. In all cases, the matching is
+the bipartite partitions of the input graph. In all cases, the matching is
 returned as a sub-graph of the input data structure.
 
 .. tabs::
 
     .. group-tab:: scipy.sparse
 
-        When given a scipy sparse array representing the adjacency matrix of
-        the graph, the user must also provide the two disjoint node sets as
-        numpy arrays. The mod will return the adjacency matrix of the matching
+        The bipartite input graph is provided as a scipy sparse array that captures
+        the adjacency matrix of the graph, where a 1.0 entry in row :math:`u` and
+        column :math:`v` indicates an edge :math:`(u,v)`.
+        The user must also provide the two disjoint node sets as
+        numpy arrays. The Mod will return the adjacency matrix of the matching
         as a scipy sparse array.
 
         .. testcode:: bipartite_matching_sp
 
             import numpy as np
             import scipy.sparse as sp
 
@@ -100,15 +104,15 @@
             ...
             Optimal objective  3.000000000e+00
             ...
 
     .. group-tab:: networkx
 
         When given a networkx graph as input, the user must also provide the
-        two disjoint node sets as numpy arrays. The mod will return the matching
+        two disjoint node sets as numpy arrays. The Mod will return the matching
         as a networkx graph (a subgraph of the input).
 
         .. testcode:: bipartite_matching_nx
 
             import networkx as nx
             import numpy as np
             from gurobi_optimods.bipartite_matching import maximum_bipartite_matching
@@ -126,18 +130,18 @@
 
             ...
             Optimal objective  4.000000000e+00
             ...
 
     .. group-tab:: pandas
 
-        The mod accepts pandas dataframes as input, where two columns in the
+        The Mod accepts pandas dataframes as input, where two columns in the
         dataframe describe the source and target vertices of an edge. The user
         must also provide the source and target column names as inputs to the
-        mode. The matching will be returned as a subset of the rows in the
+        Mod. The matching will be returned as a subset of the rows in the
         original dataframe, including all columns present in the original
         dataframe, but only those rows corresponding to the maximum matching.
 
         .. testcode:: bipartite_matching_pd
 
             import pandas as pd
             from gurobi_optimods.bipartite_matching import maximum_bipartite_matching
@@ -156,17 +160,16 @@
             :hide:
 
             ...
             Optimal objective  2.000000000e+00
 
 
 The ``maximum_bipartite_matching`` function formulates a linear program for the
-the network flow model corresponding to the given bipartite graph. Since the
-model is formulated as a network flow, Gurobi will in most cases solve the model
-using a network primal simplex algorithm.
+the minimum-cost network flow problem corresponding to the given bipartite graph.
+Gurobi will in most cases solve the model using a network primal simplex algorithm.
 
 Solution
 --------
 
 .. tabs::
 
     .. group-tab:: scipy.sparse
```

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/lad-regression.rst` & `gurobi_optimods-1.0.1/docs/source/mods/lad-regression.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Least Absolute Deviation Regression
 ===================================
 
 Least Absolute Deviation (LAD) regression is an alternative to the more commonly
 used Ordinary Least Squares (OLS) regression method. The distinction between the
-two comes down to the error metrix they use when fitted to training data: LAD
+two is the error metric used to fit the predictive model to training data. LAD
 minimizes the sum of absolute residuals, while OLS minimizes the sum of
 squares of residuals.
 
 Though most machine learning practitioners are probably more familiar with OLS,
 LAD was proposed around 50 years earlier :footcite:p:`birkes2011alternative`.
 OLS gained more popularity partly due to the fact that the computations required
-were simpler. In fact, it was the development of linear programming which made
+were simpler. It was the development of linear programming that made
 LAD computationally manageable :footcite:p:`bloomfield1980least`.
 
-LAD is generally more robust than OLS in that it is more resistant to outliers
-in the response variable :footcite:p:`birkes2011alternative`. A large residual
-for a single data point is amplified in its contribution to the loss function in
-OLS, since the residuals are squared. As a result, a single outlier can have a
+LAD is more robust than OLS in that it is more resistant to outliers
+in the response variable :footcite:p:`birkes2011alternative`. In OLS, a large residual
+for a single data point makes an outsized contribution to the loss function
+since the residuals are squared. As a result, a single outlier can have a
 large effect on the fitted coefficients and skew the resulting model. By
 contrast, a large deviation in an individual point has a less extreme effect on
 the linear loss function of LAD.
 
 Problem Specification
 ---------------------
 
 Scikit-learn's documentation gives a general explanation of `Linear Models
 <https://scikit-learn.org/stable/modules/linear_model.html>`_. The distinction
-between this mod and the Ordinary Least Squares regression from scikit-learn is the
+between this Mod and the Ordinary Least Squares regression algorithm from scikit-learn is the
 loss function. ``LADRegression`` chooses coefficients :math:`w` of a linear model
-:math:`y = Xw` to minimize the sum of absolute errors on a training
+:math:`y = Xw` so as to minimize the sum of absolute errors on a training
 dataset :math:`(X, y)`. In other words, it aims to minimize the
 following loss function:
 
 .. math::
 
     \min_w \lvert Xw - y \rvert
 
@@ -54,18 +54,18 @@
                           & u_i, v_i \ge 0                      \quad & \forall i \in I \\
                           & w_j \,\, \text{free}                \quad & \forall j \in J \\
         \end{alignat}
 
 Example Code
 ------------
 
-This mod implements the fit-predict API used by all predictive models in
+This Mod implements the fit-predict API used by all predictive models in
 scikit-learn (including the :code:`sklearn.linear_model.LinearRegression`
 class). The example below reads in the diabetes dataset from scikit-learn,
-performs a train-test split, fits an LAD regression model to the training data,
+performs a train-test split, fits a LAD regression model to the training data,
 and creates predictions for the testing data.
 
 .. testcode:: lad_regression
 
     from sklearn import datasets
     from sklearn.model_selection import train_test_split
 
@@ -126,16 +126,16 @@
         data={"OLS": ols.coef_, "LAD": lad.coef_},
         index=diabetes["feature_names"],
     )
 
     plt.figure(figsize=(8, 4))
     coefficients.plot.bar(ax=plt.gca())
 
-At this stage there isn't much to observe, the chosen coefficients are broadly
-similar.
+At this stage there isn't much to observe; the chosen coefficients are
+similar:
 
 .. figure:: figures/lad-regression-coeffs.png
     :width: 600
     :align: center
     :alt: Comparison of LAD and OLS coefficients
 
     Comparison of regression coefficients fitted by LAD and OLS
@@ -207,15 +207,15 @@
         Optimal objective  1.82...
 
 |
 
 The figure below compares the model coefficients trained on the original set and
 the outlier training set for each model type. We can see that the OLS model is
 much more significantly affected by the introduction of outliers. The dominant
-coefficients have approximately doubled in some cases,and some smaller
+coefficients have approximately doubled in some cases, and some smaller
 coefficients have even reversed their sign. By comparison, the LAD model is
 almost unchanged by the introduction of these few outliers.
 
 .. figure:: figures/lad-outlier-coeffs.png
     :width: 600
     :align: center
     :alt: Effect of training set outliers on LAD and OLS model coefficients
```

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/min-cost-flow.rst` & `gurobi_optimods-1.0.1/docs/source/mods/min-cost-flow.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Minimum-Cost Flow
 =================
 
-Minimum-cost flow problems are defined on a graph where the goal is to route
-a certain amount of flow in the cheapest way. It is a fundamental flow problem
-as many other graph problems can be modelled using this framework, for example,
-the shortest-path, maximum flow, or matching problems.
+The minimum-cost flow problem routes flow through a graph
+in the cheapest possible way. It is a fundamental problem in graphs;
+many other graph problems can be modelled in this form,
+including shortest path, maximum flow, matching, etc.
 
-The first algorithm to solve this problem was proposed by Dantzig
-:footcite:p:`dantzig1951application`, :footcite:p:`dantzig1963linear`, called
+The first algorithm to solve this problem, proposed by Dantzig
+:footcite:p:`dantzig1951application` :footcite:p:`dantzig1963linear`, was called
 the `network simplex` (NS) algorithm. Other methods have been proposed since
-then but NS remains one the most efficient approaches. Competitive methods on
+then, but NS remains one the most efficient approaches. Competitive methods on
 larger networks include cost-scaling methods (e.g. variants of the push-relabel
 algorithm by :footcite:t:`goldberg1990finding`). For a more detailed comparison
 see, for example, :footcite:t:`kovacs2015minimum`.
 
 Problem Specification
 ---------------------
 
 For a given graph :math:`G` with set of vertices :math:`V` and edges
-:math:`E`. Each edge :math:`(i,j)\in E` has the following attributes:
+:math:`E`. Each edge :math:`(i,j)\in E` has the following pair of attributes:
 
 - cost: :math:`c_{ij}\in \mathbb{R}`;
-- and capacity: :math:`B_{ij}\in\mathbb{R}`.
+- capacity: :math:`B_{ij}\in\mathbb{R}`.
 
-Each vertex :math:`i\in V` has a demand :math:`d_i\in\mathbb{R}` which can be
+Each vertex :math:`i\in V` has a demand :math:`d_i\in\mathbb{R}` that can be
 positive (requesting flow), negative (supplying flow), or zero (a transshipment
 node).
 
 The problem can be stated as finding the flow with minimal total cost
 such that:
 
 - the demand at each vertex is met exactly; and
-- the flow is capacity feasible.
+- the flow respects the capacity limit.
 
 .. dropdown:: Background: Optimization Model
 
     This Mod is implemented by formulating a Linear Program (LP) and solving it
     using Gurobi. Let us define a set of continuous variables :math:`x_{ij}` to
     represent the amount of non-negative (:math:`\geq 0`) flow going through an
     edge :math:`(i,j)\in E`.
@@ -61,25 +61,25 @@
     node) is equal to the demand. Clearly, in the case when the demand is 0,
     the outgoing flow must be equal to the incoming flow. When the demand is
     negative, this node can supply flow to the network (outgoing term is
     larger), and conversely when the demand is negative, this node can
     request flow from the network (incoming term is larger).
 
     The last constraints ensure non-negativity of the variables and that the
-    capacity per edge is not exceeded.
+    capacity limit on each edge is not exceeded.
 
 
 Code and Inputs
 ---------------
 
-For this mod, one can use input graphs of different types:
+For this Mod, one can use input graphs of different types:
 
 * pandas: using a ``pd.DataFrame``;
 * NetworkX: using a ``nx.DiGraph`` or ``nx.Graph``;
-* SciPy.sparse: using some ``sp.sparray`` matrices and NumPy's ``np.ndarray``.
+* SciPy.sparse: using ``sp.sparray`` matrices and NumPy's ``np.ndarray``.
 
 An example of these inputs with their respective requirements is shown below.
 
 .. tabs::
 
   .. group-tab:: scipy.sparse
 
@@ -114,16 +114,17 @@
             (2, 3)        10
             (2, 4)        6
             (3, 5)        1
             (4, 5)        1
           >>> print(demands)
           [-2  0 -1  1  0  2]
 
-      Three separate sparse matrices including the adjacency matrix, edge
-      capacity and cost, and a single array with the demands per node.
+      Three separate sparse matrices specify the adjacency matrix, the
+      capacity of each edge, and the cost of each edge.
+      A single array specifies the demand at each node.
 
   .. group-tab:: networkx
 
       .. doctest:: load_graph_networkx
           :options: +NORMALIZE_WHITESPACE
 
           >>> from gurobi_optimods import datasets
@@ -212,16 +213,16 @@
             (0, 1)        1.0
             (0, 2)        1.0
             (1, 3)        1.0
             (2, 4)        2.0
             (4, 5)        2.0
 
       The ``min_cost_flow_scipy`` function returns the cost of the solution as
-      well as a ``sp.sparray`` with the edges where the data is the amount of
-      non-zero flow in the solution.
+      well as a ``sp.sparray`` that provides the amount of flow for each
+      edge in the solution (but only for edges with non-zero flow).
 
   .. group-tab:: networkx
 
       .. doctest:: min_cost_flow_networkx
           :options: +NORMALIZE_WHITESPACE
 
           >>> from gurobi_optimods import datasets
```

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/mwis.rst` & `gurobi_optimods-1.0.1/docs/source/mods/mwis.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 Maximum Weighted Independent Set
 ================================
 The maximum independent set problem is one of the fundamental problems
 in combinatorial optimization with ubiquitous applications and connections to
 other problems. Maximum clique, minimum vertex cover, and maximum matching are
-example problems that can be reduced to a maximum independent set problem.
+a few examples of problems that can be reduced to a maximum independent set problem.
 
-In this mod, we consider the more general problem of the maximum weighted
-independent set (MWIS) which has applications in various fields such as computer
+In this Mod, we consider the more general problem of the maximum weighted
+independent set (MWIS), which has applications in various fields such as computer
 vision, pattern recognition, molecular structure matching, social network analysis,
 and genome data mapping. To better understand how a theoretical graph theory
 problem can be used to address a real-world challenge, let us review one
 application area in detail.
 
 To measure the structural similarity between two molecules, the
 molecules are first represented as labeled graphs where the vertices and the edges
 correspond to the atoms of the molecule and its chemical bonds, respectively. To
 find the largest substructure (subgraph) that appears in both molecular
 graphs, it suffices to find the maximum weighted independent set of a third graph,
 known as conflict graph. The vertices and the edges of the conflict
-graph, in respective terms, represent the possible mappings and conflicts
-between two molecules.
+graph represent possible mappings and conflicts
+between two molecules, respectively.
 
 
 Problem Specification
 ---------------------
 
 Consider an undirected graph :math:`G` with :math:`n` vertices and :math:`m`
 edges where each vertex is associated with a positive weight :math:`w`. Find a
 maximum weighted independent set, i.e., select a set of vertices in graph
-:math:`G` where there is no edge between any pair of vertices and the sum of the
-vertex weight is maximum.
+:math:`G` where there is no edge between any pair of selected vertices and the sum of the
+vertex weights for this set is maximised.
 
-Formally stated, let :math:`G = (V, E, w)` be an undirected graph where each
+More formally stated, let :math:`G = (V, E, w)` be an undirected graph where each
 vertex :math:`i \in V` has a positive weight :math:`w_i`. Find a subset :math:`S
 \subseteq V` such that:
 
 * no two vertices in :math:`S` are connected by an edge; and
 * among all such independent sets, the set :math:`S` has the maximum total
   vertex weight.
 
 .. dropdown:: Background: Optimization Model
 
-    This mod is implemented by formulating a Binary Integer Programming (BIP)
+    This Mod is implemented by formulating a Binary Integer Programming (BIP)
     model and solving it using Gurobi. For each vertex :math:`i \in V`, define a
     binary decision variable :math:`x_i` as below:
 
     .. math::
         x_i = \begin{cases}
             1 & \text{if vertex}\,i\,\text{belongs to set}\,S\,\\
             0 & \text{otherwise.} \\
@@ -56,23 +56,24 @@
     .. math::
         \begin{align}
         \max \quad        & \sum_{i \in V} w_i x_i \\
         \mbox{s.t.} \quad & x_i + x_j \leq 1 & \forall (i, j) \in E \\
                             & x_i \in \{0, 1\} & \forall i \in V
         \end{align}
 
-The input data for this mod includes a scipy sparse matrix in CSR format
-representing the graph :math:`G` adjacency matrix (upper triangular) and a
-numpy array representing the weights of the vertices.
+The input data for this Mod includes a scipy sparse matrix in CSR (Compressed
+SparseRow) format
+that captures the adjacency matrix of the graph :math:`G` (upper triangle only), plus a
+numpy array that captures the weights of the vertices.
 
 
 Code
 ----
 
-The example below finds the maximum weighted independent set for
+The example below finds a maximum weighted independent set for
 a graph with 8 vertices and 12 edges known as the cube graph.
 
 .. testcode:: mwis
 
     import scipy.sparse as sp
     import networkx as nx
     import numpy as np
```

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/portfolio.rst` & `gurobi_optimods-1.0.1/docs/source/mods/portfolio.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 The objective of portfolio optimization is to construct portfolios that strike an
 optimal balance between expected returns and risk.
 
 To achieve this, portfolio optimization can take into consideration several factors,
 including historical data, market trends, and the investor's risk tolerance.
 Expected returns and variances play a crucial role in the process. Expected returns
 estimate the potential gains an investor anticipates from holding a particular asset,
-while variances measure the volatility or fluctuation in the asset's returns.
+while variances measure the volatility or fluctuation in the assets' returns.
 
 The efficient frontier is a key concept in portfolio optimization. It represents the
 set of portfolios that offer the highest expected returns for a given level of risk.
-This mod returns portfolios on the
+This Mod returns portfolios on the
 efficient frontier given expected returns and variances.
 
 
 Problem Specification
 ---------------------
 
 We consider a single-period portfolio optimization problem where want
@@ -203,15 +203,15 @@
 Examples for this are single- or multi-factor models that divide the individual
 covariances into a general market movement, and an idiosyncratic risk component
 for each asset.  Also CAPM priors and risk factors obtained from principal
 component analysis can be phrased in this form. See `Efficient frontier(s) with
 cardinality constraints`_ for an example of a synthetic multi-factor model.
 
 Rather than computing the covariance matrix explicitly from the decomposition,
-it is adivised for performance and accuracy reasons to input the individual
+it is recommended for performance and accuracy reasons to input the individual
 factor matrices directly through the ``cov_factors`` keyword argurment as in
 the following example, which mimics a single-factor model:
 
 .. testcode:: mod
 
     import numpy as np
     from gurobi_optimods.portfolio import MeanVariancePortfolio
@@ -301,15 +301,15 @@
     ...
     Model has 55 quadratic objective terms
     ...
     Presolved: 62 rows, 70 columns, 160 nonzeros
     ...
 
 By incorporating leverage, we now obtain an optimal portfolio with three short
-positions, totaling to about 14% of the wealth:
+positions, totaling about 14% of assets:
 
 .. doctest:: mod
     :options: +NORMALIZE_WHITESPACE +ELLIPSIS
 
     >>> x
         AA    0.437482
         BB    0.020704
@@ -530,15 +530,15 @@
     Optimize a model with 83 rows, 91 columns and 210 nonzeros
     ...
     Model has 55 quadratic objective terms
     ...
     Presolved: 27 rows, 25 columns, 65 nonzeros
     ...
 
-The returned solution now suggests to trade only the assets "AA", "DD", "HH".
+The returned solution now suggests to trade only the assets "AA", "DD", and "HH".
 
 .. doctest:: mod
     :options: +NORMALIZE_WHITESPACE
 
     >>> x
         AA    0.482084
         BB    0.000000
@@ -699,15 +699,15 @@
     GG   0.00    0.000   False
     HH   0.09    0.090   False
     II   0.07    0.070   False
     JJ   0.00    0.000   False
 
 The traded positions are "AA" and "EE", resulting in one-time fees for one
 long, and one short transaction (in sum 0.3% of the total investment).  As
-explained in `One-time transaction fees`_, these fees are accounted by the
+explained in `One-time transaction fees`_, these fees are accounted for within the
 portfolio itself, reducing the total portfolio value as needed:
 
 .. doctest:: mod
     :options: +NORMALIZE_WHITESPACE
 
     >>> print(round(x.sum(), ndigits=6))
     0.997
```

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/qubo.rst` & `gurobi_optimods-1.0.1/docs/source/mods/qubo.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Quadratic Unconstrained Binary Optimization (QUBO)
 ==================================================
 
 Many :math:`\mathcal{NP}`-hard discrete optimization problems that naturally
 arise in application fields such as finance, energy, healthcare, and machine learning,
-can be mapped to a quadratically unconstrained binary optimization (QUBO) problem
-(:footcite:t:`kochenberger2014ubqp`), or equivalently to an Ising Hamiltonian
+can be mapped to quadratically unconstrained binary optimization (QUBO) problems
+(:footcite:t:`kochenberger2014ubqp`), or equivalently to Ising Hamiltonians
 (:footcite:t:`lucas2014ising`).
-Examples of such problems are max-cut, graph colouring, partitioning, and maximum
+Examples of such problems include max-cut, graph colouring, partitioning, and maximum
 independent set. A QUBO model is a mixed-integer quadratic program (MIQP) where
 the decision variables are restricted to take binary values and there are no
 explicit constraints.
 
-Since solving optimization problems typically requires significant computing resources,
-research in the development of novel computing architectures designed to solve QUBO problems
-has flourished in recent years (:footcite:t:`johnson2011quantum,matsubara2018ising,farhi2014quantum`).
-Such devices are fast, general-purpose, and power efficient. However, having to
-transform an optimization problem into a QUBO problem which is not as expressive and rich
-as MIP has significant drawbacks. It can make the problem significantly harder by
-penalizing the constraints into the objective function and expanding the solution space
-including both feasible and infeasible solutions. This remains to be an obstacle to the
-practical usage of special-purpose hardware in solving practically relevant optimization
-problems. Therefore, it is more efficient to avoid QUBO translations, if possible, and
-solve the problem as a MIP where the constraints are directly represented.
+Since solving optimization problems typically requires significant
+computing resources, research in the development of novel computing
+architectures designed to solve QUBO problems has flourished in recent
+years
+(:footcite:t:`johnson2011quantum,matsubara2018ising,farhi2014quantum`).
+Such devices are fast, general-purpose, and power efficient. However,
+QUBO is not nearly as expressive as MIP, so expressing an optimization
+problem in QUBO form can have significant drawbacks.  For example,
+constraints have to be modeled using penalties variables, which can
+greatly expand the solution space and significantly increase the
+difficulty of the problem.  While the lack of expressiveness of QUBO
+will probably be a significant barrier for solving general
+optimization problems, there are some problems that map quite nicely
+to QUBO form.  These problems may see a significant performance boost
+as special-purpose approaches improve over time.
 
 
 Problem Specification
 ---------------------
 
 We are given a set :math:`I` of :math:`n` items, weights :math:`q_i \in
 \mathbb{R}` for each single item :math:`i \in I`, and weights :math:`q_{ij} \in
@@ -60,15 +64,15 @@
             0 & \text{otherwise.} \\
         \end{cases}
 
     The BQP is then formulated as:
 
     .. math::
         \begin{align}
-        \max \quad        & x' Q x = \sum_{i \in I} \sum_{j \in I} q_{ij} x_i x_j & \\
+        \min \quad        & x' Q x = \sum_{i \in I} \sum_{j \in I} q_{ij} x_i x_j & \\
         \mbox{s.t.} \quad & x \in \{0, 1\}^n &
         \end{align}
 
     Note that weights :math:`q_i = q_{ii}` for single items :math:`i \in I` are
     correctly considered in the objective function since :math:`x_i x_i = x_i` holds
     for binary variables.
```

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/workforce.rst` & `gurobi_optimods-1.0.1/docs/source/mods/workforce.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 Workforce Scheduling
 ====================
 
 Workforce scheduling is an extremely widely-used application of optimization in
 practice. It involves balancing many competing concerns such as worker
 availability, cost, and preferences; shift coverage requirements; conditions on
-consecutive shifts or rest breaks; and so on. Implementation can become quite
+consecutive shifts and rest breaks; and so on. Implementation can become quite
 involved as worker requirements and entitlements become more complex.
 
 This Mod implements several basic variants of workforce scheduling. The initial
 example is deliberately simple, while later sections progressively add more
 complexity and enforce additional requirements on the generated schedule. If the
-initial example appears too simple for your use-case, please, read on!
+initial example appears too simple for your use case, please, read on!
 
 Problem Specification
 ---------------------
 
 This first example covers a simple case for a business developing a two-week
 roster. Each shift requires a given number of workers who have identical skills
-and productivity. In other words, any work can cover any shift, and all workers
-are considered equivalent. Workers provide their availability for shifts, and
-rest requirements and minimum work entitlements are handled through upper and
-lower limits, respectively, on the number of shifts a worker is rostered on for
+and productivity. In other words, any worker can cover any shift, and all workers
+are considered equivalent. Workers provide their availability for shifts.
+Rest requirements and minimum work entitlements are handled through upper and
+lower limits, respectively, on the number of shifts a worker is rostered on
 in the schedule. Optionally, preferences can be provided, in which case the
-scheduler aims to maximize satisfaction by finding a feasible roster which
+scheduler aims to maximize satisfaction by finding a feasible roster that
 maximizes the sum of preference scores of the assigned shifts.
 
-The workforce scheduling Mod takes the following three dataframes as input:
+The workforce scheduling Mod takes the following three pandas dataframes as input:
 
 * The ``availability`` dataframe has two columns: ``Worker`` and
-  ``Shift``. Each row in dataframe specifies that the given worker is
+  ``Shift``. A row in this dataframe indicates that the given worker is
   available to work the given shift. If the optional ``preferences`` argument
-  is provided, it must refer to an additional column in the ``availability``
-  dataframe containing preferences.
+  is provided, it refers to an additional column in the ``availability``
+  dataframe that provides numerical preference data.
 * The ``shift_requirements`` dataframe has two columns: ``Shift`` and
   ``Required``. Each row specifies the number of workers required for a given
-  shift. There must be one row for every unique shift in
+  shift. There must be one row for every unique shift mentioned in
   ``availability["Shift"]``.
 * The ``worker_limits`` dataframe has three columns: ``Worker``,
   ``MinShifts``, and ``MaxShifts``. Each row specifies the minimum and maximum
   number of shifts the given worker may be assigned in the schedule. There
-  must be one row for every unique worker in ``availability["Worker"]``.
+  must be one row for every unique worker mentioned in ``availability["Worker"]``.
 
-When ``solve_workforce_scheduling`` is called, a model is formulated and solved
-immediately using Gurobi. Workers will be assigned only to shifts they are
+When the main function ``solve_workforce_scheduling`` is called, a model is formulated
+and solved using Gurobi. Workers will be assigned only to shifts they are
 available for, in such a way that all requirements are covered, minimum and
 maximum shift numbers are respected, and the total sum of worker preference
-scores is maximised. If ``preferences=None``, preferences are omitted and any
+scores is maximized. If ``preferences=None``, preferences are not considered and any
 feasible schedule will be returned.
 
-The returned assignment dataframe is a subset of the availability dataframe,
-with the same columns. A row in the returned dataframe specifies that the given
+The returned assignment dataframe is a subset of the rows of the availability
+dataframe. The presence of a row in the returned dataframe signifies that the given
 worker has been assigned to the given shift.
 
 .. dropdown:: Background: Mathematical Model
 
-    The set of shifts :math:`S` is to be covered using the set of workers
+    A set of shifts :math:`S` is to be covered using a set of workers
     :math:`W`. Workers :math:`w \in W_{s} \subseteq W` are available to work
     a given shift `s`, and have a preference :math:`p_{ws}` for each
     assigned shift. Shift :math:`s` requires :math:`r_{s}` workers assigned.
     Each worker must be assigned between :math:`l_{w}` and :math:`u_{w}`
     shifts in total. The model is defined on binary variables :math:`x_{ws}`
-    which satisfy the condition
+    that represent shift assignments as follows:
 
     .. math::
 
         x_{ws} = \begin{cases}
             1 & \text{if worker w is given shift s} \\
             0 & \text{otherwise.} \\
         \end{cases}
@@ -76,16 +76,16 @@
         \begin{alignat}{2}
         \max \quad        & \sum_{s \in S} \sum_{w \in W_{s}} p_{ws} x_{ws} \\
         \mbox{s.t.} \quad & \sum_{w \in W_{s}} x_{ws} = r_{s} & \forall s \in S \\
                             & l_{w} \le \sum_{s \in S} x_{ws} \le u_{w} & \forall w \in W \\
                             & x_{ws} \in \lbrace 0, 1 \rbrace & \forall s \in S, w \in W_{s} \\
         \end{alignat}
 
-    The objective computes the total cost of all shift assignments based on
-    worker pay rates. The first constraint ensures that all shifts are
+    The objective computes the total preference value of all shift assignments, which
+    we seek to maximize.  The first constraint ensures that all shifts are
     assigned the required number of workers, while the second constraint
     ensures workers are assigned to an acceptable number of shifts.
 
 A Simple Example
 ----------------
 
 This section shows the simplest possible input dataset for the Mod, comprising
@@ -101,15 +101,15 @@
     pd.options.display.max_rows = 10
 
 .. tabs::
 
     .. tab:: ``availability``
 
         The following example table lists worker availability and preferences.
-        For example, Siva is available on July 2nd, 3rd, 5th, and so on, with a
+        For example, Siva is available on May 2nd, 3rd, 5th, and so on, with a
         stronger preference to be assigned the shift on the 5th. To use the
         preference data, the optional argument ``preferences="Preference"`` must
         be supplied.
 
         .. doctest:: workforce
             :options: +NORMALIZE_WHITESPACE
 
@@ -127,16 +127,17 @@
             68  Pauline 2023-05-11         5.0
             69  Pauline 2023-05-12         2.0
             70  Pauline 2023-05-13         4.0
             71  Pauline 2023-05-14         3.0
             <BLANKLINE>
             [72 rows x 3 columns]
 
-        In the mathematical model, the worker-shift pairings model the set
-        :math:`\lbrace (w, s) \mid s \in S, w \in W_s \rbrace` and the
+        In the mathematical model, the worker-shift pairings enumerate all
+        possible members of the set
+        :math:`\lbrace (w, s) \mid s \in S, w \in W_s \rbrace`, and the
         preference column provides values :math:`p_{ws}`.
 
     .. tab:: ``shift_requirements``
 
         The following example table lists the number of workers required for
         each shift.
 
@@ -162,15 +163,15 @@
             [14 rows x 2 columns]
 
         In the mathematical model, this table provides the values :math:`r_s`.
 
     .. tab:: ``worker_limits``
 
         The following example table lists the minimum and maximum number of
-        shifts in the planning period which each worker is entitled to.
+        shifts in the planning period that each worker is entitled to.
 
         .. doctest:: workforce
             :options: +NORMALIZE_WHITESPACE
 
             >>> from gurobi_optimods import datasets
             >>> data = datasets.load_workforce()
             >>> data.worker_limits
@@ -183,26 +184,25 @@
             5   Marisa          5          8
             6  Pauline          6          8
 
         In the mathematical model, this table provides the values :math:`l_w`
         and :math:`u_w`.
 
 The example code below solves the workforce scheduling problem for the above
-dataset. The dataset can be imported directly in the environment where
-``gurobi-optimods`` is installed.
+dataset. The dataset is imported from the ``gurobi-optimods.datasets`` module.
 
 .. testcode:: workforce
 
     from gurobi_optimods.datasets import load_workforce
     from gurobi_optimods.workforce import solve_workforce_scheduling
 
     # Load example data
     data = load_workforce()
 
-    # Solve the mod, get back a schedule
+    # Solve the Mod, get back a schedule
     assigned_shifts = solve_workforce_scheduling(
         availability=data.availability,
         shift_requirements=data.shift_requirements,
         worker_limits=data.worker_limits,
         preferences="Preference",
     )
 
@@ -214,15 +214,15 @@
     ...
     Best objective 1.850000000000e+02, best bound 1.850000000000e+02, gap 0.0000%
 
 Inspecting the Solution
 -----------------------
 
 The solution to this workforce scheduling problem is a selection of shift
-assignments. The returned dataframe is a subset of the original availability
+assignments. The returned dataframe is a subset of the original ``availability``
 dataframe.
 
 .. doctest:: workforce
     :options: +NORMALIZE_WHITESPACE
 
     >>> assigned_shifts
           Worker      Shift  Preference
@@ -278,19 +278,19 @@
 
 Enforcing Breaks
 ----------------
 
 The approach above is likely too simple for longer rosters, since the number of
 shifts assigned to each worker is only constrained over the entire time period
 of the roster. Realistically, this requirement may need to be enforced on a
-rolling basis, for example a worker may only be allowed to be assigned four
+rolling basis.  For example, a worker may only be allowed to be assigned four
 shifts in any given five day period (i.e. one rostered-off day). This is
 enforced using the ``limit_window`` keyword argument. If this optional
 argument is provided, the ``worker_limits`` constraint will be enforced over
-rolling window of the given time period, instead of over the entire roster
+a rolling window of the given duration, rather than over the entire roster
 duration.
 
 .. doctest:: workforce
     :options: +NORMALIZE_WHITESPACE +ELLIPSIS
 
     >>> worker_limits = pd.DataFrame(dict(
     ...     Worker=data.worker_limits["Worker"],
@@ -305,15 +305,15 @@
     2  Matsumi 5 days          0          4
     3    Femke 5 days          0          4
     4  Vincent 5 days          0          4
     5   Marisa 5 days          0          4
     6  Pauline 5 days          0          4
 
 The above data specifies that all workers have identical requirements to work at
-most four shifts in any given 5 day period, with no minimum number of shifts
+most four shifts in any given five day period, with no minimum number of shifts
 required. When solving this variant of the problem, ``rolling_limits`` must be
 set to ``True`` to enforce the new requirement.
 
 .. doctest:: workforce
     :options: +NORMALIZE_WHITESPACE +ELLIPSIS
 
     >>> assigned_shifts = solve_workforce_scheduling(
@@ -346,20 +346,20 @@
     2023-05-09     -      Y       -       -    -       Y       -
     2023-05-10     Y      -       Y       -    Y       -       -
     2023-05-11     Y      -       -       Y    -       Y       Y
     2023-05-12     Y      Y       Y       Y    Y       -       -
     2023-05-13     Y      Y       Y       Y    Y       Y       Y
     2023-05-14     -      Y       Y       Y    Y       Y       -
 
-Notice that Siva's shifts have been adjusted so as to avoid any worker working
-more than 5 consecutive days.
+Notice that Siva's shifts have been adjusted to meet the requirement that
+not worker should work five or more consecutive days.
 
 Further Requirements
 --------------------
 
 As mentioned in the introduction, this Mod implements some basic cases of
 workforce scheduling, and is limited in scope. However, similar modelling
 approaches to those described here can be applied to handle more complex
-requirements. For further information, see :footcite:t:`ERNST20043` (among many,
-many other references on the topic).
+requirements. For further information, see :footcite:t:`ERNST20043` (one
+among many references on the topic).
 
 .. footbibliography::
```

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-example.png` & `gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-example.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-figs.py` & `gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-figs.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-flow.png` & `gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-flow.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-result.png` & `gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-result.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/figures/lad-outlier-coeffs.png` & `gurobi_optimods-1.0.1/docs/source/mods/figures/lad-outlier-coeffs.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/figures/lad-outlier-errors.png` & `gurobi_optimods-1.0.1/docs/source/mods/figures/lad-outlier-errors.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/figures/lad-regression-coeffs.png` & `gurobi_optimods-1.0.1/docs/source/mods/figures/lad-regression-coeffs.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/figures/min-cost-flow-result.png` & `gurobi_optimods-1.0.1/docs/source/mods/figures/min-cost-flow-result.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/figures/mvp.png` & `gurobi_optimods-1.0.1/docs/source/mods/figures/mvp.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/figures/mwis.png` & `gurobi_optimods-1.0.1/docs/source/mods/figures/mwis.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/figures/pie.png` & `gurobi_optimods-1.0.1/docs/source/mods/figures/pie.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/figures/qubo.png` & `gurobi_optimods-1.0.1/docs/source/mods/figures/qubo.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/figures/shortest-path-result.png` & `gurobi_optimods-1.0.1/docs/source/mods/figures/shortest-path-result.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/mods/icons/lad-regression.png` & `gurobi_optimods-1.0.1/docs/source/mods/icons/lad-regression.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/refs/graphs.bib` & `gurobi_optimods-1.0.1/docs/source/refs/graphs.bib`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/docs/source/refs/qubo.bib` & `gurobi_optimods-1.0.1/docs/source/refs/qubo.bib`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/src/gurobi_optimods/bipartite_matching.py` & `gurobi_optimods-1.0.1/src/gurobi_optimods/bipartite_matching.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         graph, or pandas dataframe.
     nodes1 : ndarray or str
         Nodes in the first bipartite set. If ``graph`` is a scipy sparse matrix,
         ``nodes1`` must be a numpy array. If ``graph`` is a pandas dataframe,
         ``nodes1`` must be a column name. If ``graph`` is a networkx graph,
         ``nodes1`` must be a list.
     nodes2 : ndarray or str
-        Nodes in the first bipartite set. If ``graph`` is a scipy sparse matrix,
+        Nodes in the second bipartite set. If ``graph`` is a scipy sparse matrix,
         ``nodes2`` must be a numpy array. If ``graph`` is a pandas dataframe,
         ``nodes2`` must be a column name. If ``graph`` is a networkx graph,
         ``nodes2`` must be a list.
 
     Returns
     -------
     spmatrix or Graph or DataFrame
         A subgraph of the original ``graph`` (with the same data type) specifying
         the maximum matching
     """
-    if isinstance(graph, sp.spmatrix):
+    if sp.issparse(graph):
         return _maximum_bipartite_matching_scipy(graph, nodes1, nodes2, create_env)
     elif isinstance(graph, pd.DataFrame):
         return _maximum_bipartite_matching_pandas(graph, nodes1, nodes2, create_env)
     elif nx is not None and isinstance(graph, nx.Graph):
         return _maximum_bipartite_matching_networkx(graph, nodes1, nodes2, create_env)
     else:
         raise ValueError(f"Unknown graph type: {type(graph)}")
@@ -190,15 +190,15 @@
     # Solve min-cost flow problem (in this case, it's actually max-profit)
     with create_env() as env, gp.Model(env=env) as model:
         # Create incidence matrix from edge lists.
         indices = np.column_stack((from_arc, to_arc)).reshape(-1, order="C")
         indptr = np.arange(0, 2 * from_arc.shape[0] + 2, 2)
         ones = np.ones(from_arc.shape)
         data = np.column_stack((ones * -1.0, ones)).reshape(-1, order="C")
-        A = sp.csc_array((data, indices, indptr))
+        A = sp.csc_matrix((data, indices, indptr))
 
         # Solve model with gurobi, return cost and flows
         x = model.addMVar(A.shape[1], lb=0, ub=capacity)
         model.setObjective(x[-1], sense=GRB.MAXIMIZE)
         model.addMConstr(A, x, GRB.EQUAL, balance)
         model.optimize()
         if model.Status == GRB.INFEASIBLE:
```

### Comparing `gurobi_optimods-1.0.0/src/gurobi_optimods/datasets.py` & `gurobi_optimods-1.0.1/src/gurobi_optimods/datasets.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/src/gurobi_optimods/min_cost_flow.py` & `gurobi_optimods-1.0.1/src/gurobi_optimods/min_cost_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
     # Create incidence matrix from edge lists.
     indices = np.column_stack((edge_source, edge_target)).reshape(-1, order="C")
     indptr = np.arange(0, 2 * edge_source.shape[0] + 2, 2)
     ones = np.ones(edge_source.shape)
     data = np.column_stack((ones * -1.0, ones)).reshape(-1, order="C")
 
-    A = sp.csc_array((data, indices, indptr))
+    A = sp.csc_matrix((data, indices, indptr))
 
     logger.info("Solving min-cost flow with {0} nodes and {1} edges".format(*A.shape))
 
     # Solve model with gurobi, return cost and flows
     with create_env() as env, gp.Model(env=env) as model:
         x = model.addMVar(A.shape[1], lb=0, obj=costs, name="x")
         model.addConstr(x <= capacities, name="capacity")
@@ -161,16 +161,16 @@
     G : DiGraph
         Graph with edge attributes ``capacity`` and ``cost``, as well as node
         attributes ``demand``.
 
     Returns
     -------
     tuple
-        Cost of the minimum cost flow (float), dictionary indexed by edges with
-        non-zero flow in the solution (dict)
+        Cost of the minimum cost flow (float), a subgraph of the original graph
+        specifying the flow
     """
     logger.info(
         f"Solving min-cost flow with {len(G.nodes)} nodes and {len(G.edges)} edges"
     )
 
     with create_env() as env, gp.Model(env=env) as model:
         edges, capacities, costs = gp.multidict(
```

### Comparing `gurobi_optimods-1.0.0/src/gurobi_optimods/mwis.py` & `gurobi_optimods-1.0.1/src/gurobi_optimods/mwis.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/src/gurobi_optimods/portfolio.py` & `gurobi_optimods-1.0.1/src/gurobi_optimods/portfolio.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/src/gurobi_optimods/qubo.py` & `gurobi_optimods-1.0.1/src/gurobi_optimods/qubo.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/src/gurobi_optimods/regression.py` & `gurobi_optimods-1.0.1/src/gurobi_optimods/regression.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/src/gurobi_optimods/utils.py` & `gurobi_optimods-1.0.1/src/gurobi_optimods/utils.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/src/gurobi_optimods/workforce.py` & `gurobi_optimods-1.0.1/src/gurobi_optimods/workforce.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/src/gurobi_optimods/data/portfolio/portfolio.csv` & `gurobi_optimods-1.0.1/src/gurobi_optimods/data/portfolio/portfolio.csv`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/src/gurobi_optimods/data/workforce/preferences.csv` & `gurobi_optimods-1.0.1/src/gurobi_optimods/data/workforce/preferences.csv`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/tests/test_bipartite_matching.py` & `gurobi_optimods-1.0.1/tests/test_bipartite_matching.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/tests/test_graph_utils.py` & `gurobi_optimods-1.0.1/tests/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/tests/test_min_cost_flow.py` & `gurobi_optimods-1.0.1/tests/test_min_cost_flow.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/tests/test_mwis.py` & `gurobi_optimods-1.0.1/tests/test_mwis.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/tests/test_portfolio.py` & `gurobi_optimods-1.0.1/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/tests/test_qubo.py` & `gurobi_optimods-1.0.1/tests/test_qubo.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/tests/test_regression.py` & `gurobi_optimods-1.0.1/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/tests/test_utils.py` & `gurobi_optimods-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/tests/test_workforce.py` & `gurobi_optimods-1.0.1/tests/test_workforce.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/tests/utils.py` & `gurobi_optimods-1.0.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/.gitignore` & `gurobi_optimods-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/LICENSE` & `gurobi_optimods-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/NOTICE` & `gurobi_optimods-1.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/README.md` & `gurobi_optimods-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/gurobi-optimods.svg)](https://pypi.org/project/gurobi-optimods)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gurobi-optimods.svg)](https://pypi.org/project/gurobi-optimods)
 [![Tests](https://github.com/Gurobi/gurobi-optimods/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/Gurobi/gurobi-optimods/actions/workflows/test.yml?query=branch%3Amain++)
-[![Docs](https://readthedocs.com/projects/gurobi-optimization-gurobi-optimods/badge/?version=latest)](https://gurobi-optimization-gurobi-optimods.readthedocs-hosted.com/en/latest)
+[![Docs](https://readthedocs.com/projects/gurobi-optimization-gurobi-optimods/badge/?version=stable)](https://gurobi-optimization-gurobi-optimods.readthedocs-hosted.com/en/stable)
 
 # gurobi-optimods: nice APIs for common optimization tasks
 
 ``gurobi-optimods`` is an open-source Python repository of implemented
 optimization use cases, each with clear, informative, and pretty documentation
 that explains how to use it and the mathematical model behind it.
 
@@ -31,15 +31,15 @@
 - [numpy: The fundamental package for scientific computing with Python](https://pypi.org/project/numpy/)
 - [scipy: Fundamental algorithms for scientific computing in Python](https://pypi.org/project/scipy/)
 - [pandas: powerful Python data analysis toolkit](https://pypi.org/project/pandas/)
 - [gurobipy-pandas: Convenience wrapper for building optimization models from pandas data](https://pypi.org/project/gurobipy-pandas/)
 
 ## Documentation
 
-Full documentation for `gurobi-optimods` is hosted on [readthedocs](https://gurobi-optimization-gurobi-optimods.readthedocs-hosted.com/en/latest).
+Full documentation for `gurobi-optimods` is hosted on [readthedocs](https://gurobi-optimization-gurobi-optimods.readthedocs-hosted.com/en/stable).
 
 ## License
 
 `gurobi-optimods` is distributed under the terms of the [Apache License 2.0](https://spdx.org/licenses/Apache-2.0.html).
 
 ## Contact Us
```

### Comparing `gurobi_optimods-1.0.0/pyproject.toml` & `gurobi_optimods-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.0/PKG-INFO` & `gurobi_optimods-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-optimods
-Version: 1.0.0
+Version: 1.0.1
 Summary: Nice APIs for common optimization tasks
 Author-email: Simon Bowly <bowly@gurobi.com>, Robert Luce <luce@gurobi.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
 Keywords: gurobipy,optimization,pandas,scipy
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 Requires-Dist: networkx; extra == 'examples'
 Requires-Dist: scikit-learn; extra == 'examples'
 Description-Content-Type: text/markdown
 
 [![PyPI - Version](https://img.shields.io/pypi/v/gurobi-optimods.svg)](https://pypi.org/project/gurobi-optimods)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gurobi-optimods.svg)](https://pypi.org/project/gurobi-optimods)
 [![Tests](https://github.com/Gurobi/gurobi-optimods/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/Gurobi/gurobi-optimods/actions/workflows/test.yml?query=branch%3Amain++)
-[![Docs](https://readthedocs.com/projects/gurobi-optimization-gurobi-optimods/badge/?version=latest)](https://gurobi-optimization-gurobi-optimods.readthedocs-hosted.com/en/latest)
+[![Docs](https://readthedocs.com/projects/gurobi-optimization-gurobi-optimods/badge/?version=stable)](https://gurobi-optimization-gurobi-optimods.readthedocs-hosted.com/en/stable)
 
 # gurobi-optimods: nice APIs for common optimization tasks
 
 ``gurobi-optimods`` is an open-source Python repository of implemented
 optimization use cases, each with clear, informative, and pretty documentation
 that explains how to use it and the mathematical model behind it.
 
@@ -59,15 +59,15 @@
 - [numpy: The fundamental package for scientific computing with Python](https://pypi.org/project/numpy/)
 - [scipy: Fundamental algorithms for scientific computing in Python](https://pypi.org/project/scipy/)
 - [pandas: powerful Python data analysis toolkit](https://pypi.org/project/pandas/)
 - [gurobipy-pandas: Convenience wrapper for building optimization models from pandas data](https://pypi.org/project/gurobipy-pandas/)
 
 ## Documentation
 
-Full documentation for `gurobi-optimods` is hosted on [readthedocs](https://gurobi-optimization-gurobi-optimods.readthedocs-hosted.com/en/latest).
+Full documentation for `gurobi-optimods` is hosted on [readthedocs](https://gurobi-optimization-gurobi-optimods.readthedocs-hosted.com/en/stable).
 
 ## License
 
 `gurobi-optimods` is distributed under the terms of the [Apache License 2.0](https://spdx.org/licenses/Apache-2.0.html).
 
 ## Contact Us
```

